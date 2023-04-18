# Comparing `tmp/fatld-0.1.5.tar.gz` & `tmp/fatld-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fatld-0.1.5.tar", max compression
+gzip compressed data, was "fatld-0.1.6.tar", max compression
```

## Comparing `fatld-0.1.5.tar` & `fatld-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rwxr-xr-x   0        0        0     3239 2023-03-10 20:43:01.274937 fatld-0.1.5/README.md
--rwxr-xr-x   0        0        0      147 2023-03-10 14:52:46.609143 fatld-0.1.5/fatld/__init__.py
--rwxr-xr-x   0        0        0    32820 2023-04-07 14:18:24.270482 fatld-0.1.5/fatld/design.py
--rwxr-xr-x   0        0        0     6794 2023-03-10 14:53:29.404853 fatld-0.1.5/fatld/main.py
--rwxr-xr-x   0        0        0     8448 2023-03-10 14:53:29.419886 fatld-0.1.5/fatld/relation.py
--rwxr-xr-x   0        0        0     1040 2023-04-07 14:24:08.747177 fatld-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4027 1970-01-01 00:00:00.000000 fatld-0.1.5/setup.py
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 fatld-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     3239 2023-03-10 20:43:01.274937 fatld-0.1.6/README.md
+-rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.6/fatld/__init__.py
+-rwxr-xr-x   0        0        0    33809 2023-04-18 13:22:16.768689 fatld-0.1.6/fatld/design.py
+-rwxr-xr-x   0        0        0     6794 2023-03-10 14:53:29.404853 fatld-0.1.6/fatld/main.py
+-rwxr-xr-x   0        0        0     8448 2023-03-10 14:53:29.419886 fatld-0.1.6/fatld/relation.py
+-rwxr-xr-x   0        0        0     1040 2023-04-18 13:22:46.910889 fatld-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 fatld-0.1.6/PKG-INFO
```

### Comparing `fatld-0.1.5/README.md` & `fatld-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fatld-0.1.5/fatld/design.py` & `fatld-0.1.6/fatld/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,36 +224,42 @@
         best_wlp, permutations : tuple[list[float], list[int]]
             Returns the minimal qWLP and the corresponding permutations of the
             factor levels. The qWLP starts with words of length 3.
         """
         # Declare global variables
         global scaled_contrast_matrix
 
-        # Compute the 12 permutations of the four levels
+        # Compute the 12 basic permutations of the four levels
         perms = []
         for p in permutations(range(3)):
             for i in range(4):
                 ordering = list(p)
                 ordering.insert(i, 3)
                 perms.append(ordering)
         perms = perms[:12]
 
-        # Initialize list for best beta_vectors
-        best_perm = []
-        best_vector = []
-
-        # Compute the beta-vector for each permutation
-        for i, p in enumerate(product(range(12), repeat=self.m)):
-            perm_list = [perms[i] for i in p]
-            beta_vector = beta_wlp(
-                self, permutation_list=perm_list, max_length=max_length
-            )
-            if i == 0 or best_vector > beta_vector:
-                best_perm = perm_list
-                best_vector = beta_vector
+        # Compute all possible permutations for m factors
+        all_perms = []
+        for _, p in enumerate(product(range(12), repeat=self.m)):
+            all_perms.append([perms[i] for i in p])
+
+        # Compute beta wlp for all permutations
+        a_vector_list = beta_wlp(
+            design=self, permutation_list=all_perms, max_length=max_length
+        )
+
+        # Find the best Beta vector and the corresponding permutation
+        best_vector = a_vector_list[0]
+        best_perm = all_perms[0]
+
+        for i, v in enumerate(a_vector_list[1:]):
+            if best_vector > v:
+                best_vector = v
+                best_perm = all_perms[i]
+
         return best_vector, best_perm
 
     def resolution(self) -> int | None:
         """
         Compute the resolution of the design.
         """
         wlp = self.wlp()
@@ -656,56 +662,57 @@
     cols_num = [gen2num(i) for i in cols_gen]
     added_cols = [i for i in cols_num if np.log2(i) % 1 != 0]
     return Design(run_size, n_flvl, added_cols)
 
 
 def beta_wlp(
     design: Design,
-    permutation_list: list[list[int]],
+    permutation_list: list[list[list[int]]],
     max_length: None | int = None,
-) -> list[float]:
+) -> list[list[float]]:
     """
     Compute the beta WLP of the design.
 
     Parameters
     ----------
     design : fatld.Design
         Four-and-two-level design
-    permutation_list : list[list[int]]
-        List of sublists, where each sublist corresponds to the ordering of the levels
-        a four-level factor (of the form [0,1,2,3]).
+    permutation_list : list[list[list[int]]]
+        List of permutations for the m four-level factors.
+        Each permutation is a list of m sublists, where each sublist corresponds to the
+        ordering of the levels of a four-level factor (of the form [0,1,2,3]).
     max_length : None | int, optional
         Maximum length of words considered in the beta WLP, by default None so that all
         the word lengths are considered.
 
     Returns
     -------
-    beta_wlp : list[float]
-        Vector of the Aq values starting with words of length 3.
+    beta_wlp : list[list[float]]
+        List of vectors of the Aq values starting with words of length 3.
+        Each vector in the list corresponds to the beta wlp for the corresponding
+        permutation in `permutation_list`.
     """
     # Declare global variables
     global scaled_contrast_matrix
 
     design_matrix = design.array
     m = design.m
     n = design.n
     N = design.runsize
 
-    # Permutations have to contain only 0,1,2,3
-    if any([len(i) != 4 for i in permutation_list]):
-        raise ValueError("Each permutation must contain four elements")
-
-    if any([i not in [0, 1, 2, 3] for p in permutation_list for i in p]):
-        raise ValueError("Permutations can only contain 0, 1, 2, or 3")
-    # There must be one permutation per four-level factor
-    if len(permutation_list) != design.m:
-        raise ValueError(
-            "There must be one permutation per four-level factor, only %i given"
-            % len(permutation_list)
-        )
+    # Each permutation must contain m sublists
+    if any([len(i) != m for i in permutation_list]):
+        raise ValueError("Each permutation must contain m sublists")
+    # Each sublist in a permutation has to contain only 0,1,2,3
+    for p in permutation_list:
+        if any([len(i) != 4 for i in p]):
+            raise ValueError("Each sublist in a permutation must contain four elements")
+
+        if any([i not in [0, 1, 2, 3] for x in p for i in x]):
+            raise ValueError("Sublists in permutations can only contain 0, 1, 2, or 3")
 
     # Isolate four-level and two-level part of the design
     fl_matrix = design_matrix[:, :m]
     tl_matrix = design_matrix[:, m:]
 
     # Build all interactions between all two-level factors
     if max_length is None:
@@ -713,105 +720,113 @@
     else:
         max_n_value = max_length - 1
     tfi_model_matrix = build_tfi_model_matrix(n=n, max_length=max_n_value)
     tl_interaction_matrix = np.matmul(tl_matrix, tfi_model_matrix) % 2
     tl_interaction_matrix = (2 * tl_interaction_matrix) - 1
     tl_interaction_length = np.sum(tfi_model_matrix, axis=0).tolist()
 
-    # Unfold the four-level factors into L, Q, C matrices
-    fl_contrast_list = []
-    for x in range(m):
-        permutation = permutation_list[x]
-        mix_contrast_matrix = scaled_contrast_matrix[permutation, :]
-        single_fl_contrast_matrix = np.zeros((N, 3))
-        for i in range(4):
-            single_fl_contrast_matrix[
-                fl_matrix[:, x] == i, :
-            ] = mix_contrast_matrix[  # noqa: E201
-                i, :
-            ]
-        fl_contrast_list.append(single_fl_contrast_matrix)
-    fl_contrast_matrix = np.hstack(fl_contrast_list)
+    # Empty list to hold the Beta vectors for all the permutations
+    a_vectors_list = []
+    for single_permutation in permutation_list:
+        # Unfold the four-level factors into L, Q, C matrices
+        fl_contrast_list = []
+        for x in range(m):
+            permutation = single_permutation[x]
+            mix_contrast_matrix = scaled_contrast_matrix[permutation, :]
+            single_fl_contrast_matrix = np.zeros((N, 3))
+            for i in range(4):
+                single_fl_contrast_matrix[
+                    fl_matrix[:, x] == i, :
+                ] = mix_contrast_matrix[  # noqa: E201
+                    i, :
+                ]
+            fl_contrast_list.append(single_fl_contrast_matrix)
+        fl_contrast_matrix = np.hstack(fl_contrast_list)
 
-    # Initialize the length and type vectors
-    fl_contrast_length = [i + 1 for _ in range(m) for i in range(3)]
+        # Initialize the length and type vectors
+        fl_contrast_length = [i + 1 for _ in range(m) for i in range(3)]
 
-    # No interaction can be created
-    if m == 1:
-        fl_full_contrast_matrix = fl_contrast_matrix
-    # Main effects for the two four-level factors and the 3^2 interactions between the
-    # 6 terms.
-    elif m == 2:
-        fl_contrast_interaction_list = []
-        for p in product(range(3), repeat=2):
-            new_p = [x + (3 * i) for i, x in enumerate(p)]
-            single_fl_contrast_interaction_vector = np.prod(
-                fl_contrast_matrix[:, new_p], axis=1
-            )[:, None]
-            fl_contrast_interaction_list.append(single_fl_contrast_interaction_vector)
-            fl_contrast_length.append(sum(p) + 2)
-        fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
-        fl_full_contrast_matrix = np.concatenate(
-            (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
-        )
-    # Three different terms:
-    # - Main effects for the 3 four-level factors (3*3=9 terms)
-    # - Interactions between 2 of the 3 four-level factors (3 ways of creating 9 terms)
-    # - Interactions between the 3 four-level factors (27 terms)
-    elif m == 3:
-        # Interactions between 2 of the 3 four-level factors
-        fl_contrast_interaction_list = []
-        for c in combinations(range(3), 2):
+        # No interaction can be created
+        if m == 1:
+            fl_full_contrast_matrix = fl_contrast_matrix
+        # Main effects for the two four-level factors and the 3^2 interactions between
+        # the 6 terms.
+        elif m == 2:
+            fl_contrast_interaction_list = []
             for p in product(range(3), repeat=2):
-                new_p = [3 * c[i] + x for i, x in enumerate(p)]
+                new_p = [x + (3 * i) for i, x in enumerate(p)]
                 single_fl_contrast_interaction_vector = np.prod(
                     fl_contrast_matrix[:, new_p], axis=1
                 )[:, None]
                 fl_contrast_interaction_list.append(
                     single_fl_contrast_interaction_vector
                 )
                 fl_contrast_length.append(sum(p) + 2)
+            fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
+            fl_full_contrast_matrix = np.concatenate(
+                (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
+            )
+        # Three different terms:
+        # - Main effects for the 3 four-level factors (3*3=9 terms)
+        # - Interactions between 2 of the 3 four-level factors (3 ways of creating 9)
+        # - Interactions between the 3 four-level factors (27 terms)
+        elif m == 3:
+            # Interactions between 2 of the 3 four-level factors
+            fl_contrast_interaction_list = []
+            for c in combinations(range(3), 2):
+                for p in product(range(3), repeat=2):
+                    new_p = [3 * c[i] + x for i, x in enumerate(p)]
+                    single_fl_contrast_interaction_vector = np.prod(
+                        fl_contrast_matrix[:, new_p], axis=1
+                    )[:, None]
+                    fl_contrast_interaction_list.append(
+                        single_fl_contrast_interaction_vector
+                    )
+                    fl_contrast_length.append(sum(p) + 2)
+
+            # Interactions between 3 four-level factors
+            for p in product(range(3), repeat=3):
+                # p is a tuple with two numbers corresponding with the polynomial
+                # contrasts chosen for the product
+                new_p = [3 * i + x for i, x in enumerate(p)]
+                single_fl_contrast_interaction_vector = np.prod(
+                    fl_contrast_matrix[:, new_p], axis=1
+                )[:, None]
+                fl_contrast_interaction_list.append(
+                    single_fl_contrast_interaction_vector
+                )
+                fl_contrast_length.append(sum(p) + 3)
+            fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
+            fl_full_contrast_matrix = np.concatenate(
+                (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
+            )
+        else:
+            raise ValueError("Unknown m value: %i" % m)
 
-        # Interactions between 3 four-level factors
-        for p in product(range(3), repeat=3):
-            # p is a tuple with two numbers corresponding with the polynomial contrasts
-            # chosen for the product
-            new_p = [3 * i + x for i, x in enumerate(p)]
-            single_fl_contrast_interaction_vector = np.prod(
-                fl_contrast_matrix[:, new_p], axis=1
-            )[:, None]
-            fl_contrast_interaction_list.append(single_fl_contrast_interaction_vector)
-            fl_contrast_length.append(sum(p) + 3)
-        fl_contrast_interaction_matrix = np.hstack(fl_contrast_interaction_list)
-        fl_full_contrast_matrix = np.concatenate(
-            (fl_contrast_matrix, fl_contrast_interaction_matrix), axis=1
+        # Build word length vector
+        word_length = (
+            np.array(fl_contrast_length)[:, None].T
+            + np.array(tl_interaction_length)[:, None]  # noqa: W503
         )
-    else:
-        raise ValueError("Unknown m value")
-
-    # Build word length vector
-    word_length = (
-        np.array(fl_contrast_length)[:, None].T
-        + np.array(tl_interaction_length)[:, None]  # noqa: W503
-    )
-
-    # Compute squared correlations
-    correlation = (tl_interaction_matrix.T @ fl_full_contrast_matrix) / N
-    correlation_sq = np.round(correlation**2, 2)
 
-    # Compute Beta values
-    if max_length is None:
-        max_Aq_length = int(np.amax(word_length)) + 1
-    else:
-        max_Aq_length = max_length + 1
-    a_vector = []
-    for length in range(3, max_Aq_length):
-        a_value = np.round(np.sum(correlation_sq[word_length == length]), 2)
-        a_vector.append(a_value)
-    return a_vector
+        # Compute squared correlations
+        correlation = (tl_interaction_matrix.T @ fl_full_contrast_matrix) / N
+        correlation_sq = np.round(correlation**2, 2)
+
+        # Compute Beta values
+        if max_length is None:
+            max_Aq_length = int(np.amax(word_length)) + 1
+        else:
+            max_Aq_length = max_length + 1
+        a_vector = []
+        for length in range(3, max_Aq_length):
+            a_value = np.round(np.sum(correlation_sq[word_length == length]), 2)
+            a_vector.append(a_value)
+        a_vectors_list.append(a_vector)
+    return a_vectors_list
 
 
 def nbr_interactions(n: int, max_length: int) -> int:
     """
     Compute the total number of interactions between i factors among n, where i
     ranges between 1 and max_length.
     """
```

### Comparing `fatld-0.1.5/fatld/main.py` & `fatld-0.1.6/fatld/main.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.5/fatld/relation.py` & `fatld-0.1.6/fatld/relation.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.5/pyproject.toml` & `fatld-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fatld"
-version = "0.1.5"
+version = "0.1.6"
 description = "Generate and characterize designs with four-and-two-level (FATL) factors"
 authors = ["Alexandre Bohyn <alexandre.bohyn@kuleuven.be>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://abohyndoe.github.io/fatld/"
 repository = "https://github.com/ABohynDOE/fatld"
 keywords = ["design", "doe"]
```

### Comparing `fatld-0.1.5/setup.py` & `fatld-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fatld
+Version: 0.1.6
+Summary: Generate and characterize designs with four-and-two-level (FATL) factors
+Home-page: https://abohyndoe.github.io/fatld/
+License: MIT
+Keywords: design,doe
+Author: Alexandre Bohyn
+Author-email: alexandre.bohyn@kuleuven.be
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: oapackage (>=2.7.6,<3.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Project-URL: Repository, https://github.com/ABohynDOE/fatld
+Description-Content-Type: text/markdown
 
-packages = \
-['fatld']
+# Four And Two Level Designs
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/fatld.svg)](https://badge.fury.io/py/fatld)
+[![CI](https://github.com/ABohynDOE/fatld/actions/workflows/CI.yml/badge.svg)](https://github.com/ABohynDOE/fatld/actions/workflows/CI.yml)
 
-install_requires = \
-['matplotlib>=3.6.3,<4.0.0',
- 'numpy>=1.24.2,<2.0.0',
- 'oapackage>=2.7.6,<3.0.0',
- 'pandas>=1.5.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'fatld',
-    'version': '0.1.5',
-    'description': 'Generate and characterize designs with four-and-two-level (FATL) factors',
-    'long_description': '# Four And Two Level Designs\n\n[![PyPI version](https://badge.fury.io/py/fatld.svg)](https://badge.fury.io/py/fatld)\n[![CI](https://github.com/ABohynDOE/fatld/actions/workflows/CI.yml/badge.svg)](https://github.com/ABohynDOE/fatld/actions/workflows/CI.yml)\n\nThe `fatld` package contains functionality to generate and characterize designs with four-and-two-level (FATL) factors.\nDesign characteristics include word length pattern, defining relation, and number of clear interactions.\nFor more information about the package see the documentation at [https://abohyndoe.github.io/fatld/](https://abohyndoe.github.io/fatld/).\nA large collection of FATL designs can be explored interactively using a web app at [https://abohyndoe.shinyapps.io/fatldesign-selection-tool/](https://abohyndoe.shinyapps.io/fatldesign-selection-tool/).\n\n## Usage\n\nThe package can be used from Python:\n\n```python\n>>> import fatld\n>>> D = fatld.Design(runsize=32, m=1, cols=[21, 27, 29])\n>>> D.wlp()\n[1, 3, 3, 0, 0]\n>>> D.defining_relation()\n[\'A1cef\', \'A3deg\', \'A1cdeh\']\n>>> print("There are %s 2-2 interactions totally clear from any main effect or other interaction." % D.clear(\'2-2\', \'all\'))\nThere are 6 2-2 interactions totally clear from any main effect or other interaction.\n>>> print("The design contains %s four-level factors and %s two-level factors" % (D.m, D.n))\nThe design contains 1 four-level factors and 6 two-level factors\n```\n\nFor more examples see the documentation.\n\n## Installation\n\nThe Python interface to the package is available on pypi. Installation can be done using the following command:\n\n```bash\npip install fatld\n```\n\n## Development\n\nAll development is done in a virtual environment based on `poetry`, activate it using:\n\n```shell\npoetry shell\n```\n\n### Code style\n\n* Try to follow the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide. A usefull tool for automated formatting is [black](https://pypi.python.org/pypi/black). We do allow lines upto 120 characters.\n* Document functions using the [Numpy docstring](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html#example-numpy) convention\n\n* Linting is based on `ruff`, configuration is found in the [pyproject.toml](pyproject.toml) file.\n\n* Tests are ran using `pytest` and a coverage report can be generated using `coverage` inside the virtual environment:\n\n    ```shell\n    coverage run -m pytest tests\n    coverage report -m\n    ```\n\n### Submitting code\n\nIf you would like to contribute, please submit a pull request. (See the [Github Hello World](https://guides.github.com/activities/hello-world/) example, if you are new to Github).\n\nBy contributing to the repository you state you own the copyright to those contributions and agree to include your contributions as part of this project under the BSD license.\n\n### Bugs reports and feature requests\n\nTo submit a bug report or feature request use the [Github issue tracker](https://github.com/ABohynDOE/fatld/issues).\nSearch for existing and closed issues first. If your problem or idea is not yet addressed, please open a new issue.\n\n### Contact\n\nFor further information please contact alexandre dot bohyn at kuleuven dot be\n',
-    'author': 'Alexandre Bohyn',
-    'author_email': 'alexandre.bohyn@kuleuven.be',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://abohyndoe.github.io/fatld/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+The `fatld` package contains functionality to generate and characterize designs with four-and-two-level (FATL) factors.
+Design characteristics include word length pattern, defining relation, and number of clear interactions.
+For more information about the package see the documentation at [https://abohyndoe.github.io/fatld/](https://abohyndoe.github.io/fatld/).
+A large collection of FATL designs can be explored interactively using a web app at [https://abohyndoe.shinyapps.io/fatldesign-selection-tool/](https://abohyndoe.shinyapps.io/fatldesign-selection-tool/).
 
+## Usage
+
+The package can be used from Python:
+
+```python
+>>> import fatld
+>>> D = fatld.Design(runsize=32, m=1, cols=[21, 27, 29])
+>>> D.wlp()
+[1, 3, 3, 0, 0]
+>>> D.defining_relation()
+['A1cef', 'A3deg', 'A1cdeh']
+>>> print("There are %s 2-2 interactions totally clear from any main effect or other interaction." % D.clear('2-2', 'all'))
+There are 6 2-2 interactions totally clear from any main effect or other interaction.
+>>> print("The design contains %s four-level factors and %s two-level factors" % (D.m, D.n))
+The design contains 1 four-level factors and 6 two-level factors
+```
+
+For more examples see the documentation.
+
+## Installation
+
+The Python interface to the package is available on pypi. Installation can be done using the following command:
+
+```bash
+pip install fatld
+```
+
+## Development
+
+All development is done in a virtual environment based on `poetry`, activate it using:
+
+```shell
+poetry shell
+```
+
+### Code style
+
+* Try to follow the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide. A usefull tool for automated formatting is [black](https://pypi.python.org/pypi/black). We do allow lines upto 120 characters.
+* Document functions using the [Numpy docstring](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html#example-numpy) convention
+
+* Linting is based on `ruff`, configuration is found in the [pyproject.toml](pyproject.toml) file.
+
+* Tests are ran using `pytest` and a coverage report can be generated using `coverage` inside the virtual environment:
+
+    ```shell
+    coverage run -m pytest tests
+    coverage report -m
+    ```
+
+### Submitting code
+
+If you would like to contribute, please submit a pull request. (See the [Github Hello World](https://guides.github.com/activities/hello-world/) example, if you are new to Github).
+
+By contributing to the repository you state you own the copyright to those contributions and agree to include your contributions as part of this project under the BSD license.
+
+### Bugs reports and feature requests
+
+To submit a bug report or feature request use the [Github issue tracker](https://github.com/ABohynDOE/fatld/issues).
+Search for existing and closed issues first. If your problem or idea is not yet addressed, please open a new issue.
+
+### Contact
+
+For further information please contact alexandre dot bohyn at kuleuven dot be
 
-setup(**setup_kwargs)
```

