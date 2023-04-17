# Comparing `tmp/alpineer-0.1.5.tar.gz` & `tmp/alpineer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpineer-0.1.5.tar", max compression
+gzip compressed data, was "alpineer-0.1.6.tar", max compression
```

## Comparing `alpineer-0.1.5.tar` & `alpineer-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11845 2023-02-13 19:15:11.174245 alpineer-0.1.5/LICENSE
--rw-r--r--   0        0        0     4069 2023-02-13 19:15:11.174245 alpineer-0.1.5/README.md
--rw-r--r--   0        0        0     2847 2023-02-13 19:16:26.531626 alpineer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/__init__.py
--rw-r--r--   0        0        0     1398 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/data_utils.py
--rw-r--r--   0        0        0      939 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/image_utils.py
--rw-r--r--   0        0        0     7760 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/io_utils.py
--rw-r--r--   0        0        0    23288 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/load_utils.py
--rw-r--r--   0        0        0     7598 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/misc_utils.py
--rw-r--r--   0        0        0        0 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/py.typed
--rw-r--r--   0        0        0      223 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/settings.py
--rw-r--r--   0        0        0    20206 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/test_utils.py
--rw-r--r--   0        0        0     5109 2023-02-13 19:15:11.178245 alpineer-0.1.5/src/alpineer/tiff_utils.py
--rw-r--r--   0        0        0     5145 1970-01-01 00:00:00.000000 alpineer-0.1.5/setup.py
--rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 alpineer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11845 2023-04-17 22:10:21.890788 alpineer-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4069 2023-04-17 22:10:21.890788 alpineer-0.1.6/README.md
+-rw-r--r--   0        0        0     2847 2023-04-17 22:11:36.131760 alpineer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/__init__.py
+-rw-r--r--   0        0        0     1398 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/data_utils.py
+-rw-r--r--   0        0        0      939 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/image_utils.py
+-rw-r--r--   0        0        0     7760 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/io_utils.py
+-rw-r--r--   0        0        0    22804 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/load_utils.py
+-rw-r--r--   0        0        0     8209 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/misc_utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/py.typed
+-rw-r--r--   0        0        0      223 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/settings.py
+-rw-r--r--   0        0        0    20206 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/test_utils.py
+-rw-r--r--   0        0        0     5109 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/tiff_utils.py
+-rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 alpineer-0.1.6/PKG-INFO
```

### Comparing `alpineer-0.1.5/LICENSE` & `alpineer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/README.md` & `alpineer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/pyproject.toml` & `alpineer-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpineer"
-version = "0.1.5"
+version = "0.1.6"
 description = "Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy."
 authors = [
     "Noah Frey Greenwald <nfgreen@stanford.edu>",
     "Adam Kagel <ackagel@stanford.edu>",
     "Alex Kong <alkong@stanford.edu>",
     "Cami Laura Sowers <csowers@stanford.edu>",
     "Sricharan Reddy Varra <srivarra@stanford.edu>",
```

### Comparing `alpineer-0.1.5/src/alpineer/data_utils.py` & `alpineer-0.1.6/src/alpineer/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/src/alpineer/image_utils.py` & `alpineer-0.1.6/src/alpineer/image_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/src/alpineer/io_utils.py` & `alpineer-0.1.6/src/alpineer/io_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/src/alpineer/load_utils.py` & `alpineer-0.1.6/src/alpineer/load_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,82 +340,82 @@
         dims=["fovs", "rows", "cols", xr_dim_name],
     )
 
     return img_xr
 
 
 def check_fov_name_prefix(fov_list):
-    """Checks for a prefix (usually detailing a run name) in any of the provided FOV names
+    """Checks for a prefix (usually detailing a run/tile name) in any of the provided FOV names
 
     Args:
         fov_list (list): list of fov name
     Returns:
-        tuple: (bool) whether at least one fov names has a prefix,
-               (list / dict) if prefix, dictionary with fov name as keys and prefixes as values
-                otherwise return a simple list of the fov names
+        (dict): dictionary with prefixes as the keys and fov names as values
     """
 
-    # check for prefix in any of the fov names
-    prefix = False
+    # dict containing fov name and run name
+    fov_names = {}
     for folder in fov_list:
-        if re.search("R.{1,3}C.{1,3}", folder).start() != 0:
-            prefix = True
-
-    if prefix:
-        # dict containing fov name and run name
-        fov_names = {}
-        for folder in fov_list:
-            fov = "".join(folder.split("_")[-1:])
-            prefix_name = "_".join(folder.split("_")[:-1])
-            fov_names[fov] = prefix_name
-    else:
-        # original list of fov names
-        fov_names = fov_list
+        fov = "".join(folder.split("_")[-1:])
+        prefix_name = "_".join(folder.split("_")[:-1])
+        if prefix_name in fov_names.keys():
+            fov_names[prefix_name].append(fov)
+        else:
+            fov_names[prefix_name] = [fov]
 
-    return prefix, fov_names
+    return fov_names
 
 
 def get_tiled_fov_names(fov_list, return_dims=False):
     """Generates the complete tiled fov list when given a list of fov names
 
     Args:
         fov_list (list):
-            list of fov names
+            list of fov names with are suffixed with RnCm, where n and m are any integer.
         return_dims (bool):
             whether to also return row and col dimensions
     Returns:
-        tuple: names of all fovs expected for tiled image shape, and dimensions if return_dims
+        list: list of tuples the fov prefix, all fovs expected for tiled image shape,
+        row_num and col_num
     """
 
-    rows, cols, expected_fovs = [], [], []
+    expected_tiles = []
 
-    # check for run name prefix
-    prefix, fov_names = check_fov_name_prefix(fov_list)
+    # check for run name prefixes
+    tiled_fov_names = check_fov_name_prefix(fov_list)
+    prefixes = tiled_fov_names.keys()
+    search_term: re.Pattern = re.compile(r"R\+?(\d+)C\+?(\d+)")
+
+    # get expected names for each tile
+    for tile in prefixes:
+        rows, cols, expected_fovs = [], [], []
+        fov_names = tiled_fov_names[tile]
+        # get tiled image dimensions
+        for fov in fov_names:
+            R, C = re.search(search_term, fov).group(1, 2)
+            rows.append(int(R))
+            cols.append(int(C))
+        row_num, col_num = max(rows), max(cols)
+
+        # fill list of expected fov names
+        for n in range(row_num):
+            for m in range(col_num):
+                fov = f"R{n + 1}C{m + 1}"
+                # prepend run names
+                if tile == "":
+                    expected_fovs.append(fov)
+                else:
+                    expected_fovs.append(f"{tile}_" + fov)
 
-    # get tiled image dimensions
-    for fov in fov_names:
-        fov_digits = re.findall(r"\d+", fov)
-        rows.append(int(fov_digits[0]))
-        cols.append(int(fov_digits[1]))
-    row_num, col_num = max(rows), max(cols)
-
-    # fill list of expected fov names
-    for n in range(row_num):
-        for m in range(col_num):
-            fov = f"R{n + 1}C{m + 1}"
-            # prepend run names
-            if prefix and fov in list(fov_names.keys()):
-                expected_fovs.append(f"{fov_names[fov]}_" + fov)
-            else:
-                expected_fovs.append(fov)
+        if return_dims:
+            expected_tiles.append((tile, expected_fovs, row_num, col_num))
+        else:
+            expected_tiles.append(expected_fovs)
 
-    if return_dims:
-        return expected_fovs, row_num, col_num
-    else:
-        return expected_fovs
+    return expected_tiles
 
 
 def load_tiled_img_data(
     data_dir, fovs, expected_fovs, channel, single_dir, file_ext="tiff", img_sub_folder=""
 ):
     """Takes a set of images from a directory structure and loads them into a tiled xarray.
 
@@ -446,30 +446,14 @@
     if type(fovs) is dict:
         fov_list = list(fovs.values())
         tiled_names = list(fovs.keys())
     else:
         fov_list = fovs
         tiled_names = []
 
-    # no missing fov images, load data normally and return array
-    if len(fov_list) == len(expected_fovs):
-        if single_dir:
-            img_xr = load_imgs_from_dir(
-                data_dir,
-                match_substring=channel,
-                xr_dim_name="channels",
-                trim_suffix="_" + channel,
-                xr_channel_names=[channel],
-            )
-        else:
-            img_xr = load_imgs_from_tree(
-                data_dir, img_sub_folder, fovs=fov_list, channels=[channel]
-            )
-        return img_xr
-
     # missing fov directories, read in a test image to get data type
     if single_dir:
         test_path = os.path.join(data_dir, expected_fovs[0] + "_" + channel + "." + file_ext)
     else:
         test_path = os.path.join(
             os.path.join(data_dir, fov_list[0], img_sub_folder, channel + "." + file_ext)
         )
```

### Comparing `alpineer-0.1.5/src/alpineer/misc_utils.py` & `alpineer-0.1.6/src/alpineer/misc_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         a
         if isinstance(a, Iterable)
         and not ((isinstance(a, str) and ignore_str) or isinstance(a, type))
         else [a]
     )
 
 
-def verify_in_list(warn=False, **kwargs):
+def verify_in_list(warn: bool = False, **kwargs) -> bool:
     """Verify at least whether the values in the first list exist in the second
 
     Args:
         warn (bool):
             Whether to issue warning instead of error, defaults to False
         **kwargs (list, list):
             Two lists, but will work for single elements as well.
@@ -95,51 +95,55 @@
         Warning:
             if not all values are found and warn is True
     """
 
     if len(kwargs) != 2:
         raise ValueError("You must provide 2 arguments to verify_in_list")
 
-    test_list, good_values = kwargs.values()
-    test_list = list(make_iterable(test_list))
-    good_values = list(make_iterable(good_values))
-
-    for v in [test_list, good_values]:
-        if len(v) == 0:
-            raise ValueError("List arguments cannot be empty")
-
-    if not np.isin(test_list, good_values).all():
-        test_list_name, good_values_name = kwargs.keys()
-        test_list_name = test_list_name.replace("_", " ")
-        good_values_name = good_values_name.replace("_", " ")
+    rhs_name, lhs_name = map(lambda s: s.replace("_", " "), kwargs.keys())
 
-        # Calculate the difference between the `test_list` and the `good_values`
-        difference = [str(val) for val in test_list if val not in good_values]
+    lhs_list, rhs_list = map(lambda l: list(make_iterable(l)), kwargs.values())
+
+    # Check if either list inputs are `None` (or both)
+    if any(v == [None] for v in (lhs_list, rhs_list)):
+        return True
+    # If the Left Hand List is empty, the Right Hand List will always be contained in it.
+    if len(lhs_list) == 0:
+        return True
+    # If the Right Hand List is empty, the Left Hand List will never be contained in it.
+    # Throw a ValueError
+    if len(rhs_list) == 0:
+        raise ValueError(f"The list {lhs_name} is empty.")
+
+    if not np.isin(lhs_list, rhs_list).all():
+        # Calculate the difference between the `lhs_list` and the `rhs_list`
+        difference = [str(val) for val in lhs_list if val not in rhs_list]
 
         # Only printing up to the first 10 invalid values.
         err_str = (
             "Not all values given in list {0:^} were found in list {1:^}.\n "
             "Displaying {2} of {3} invalid value(s) for list {4:^}\n"
         ).format(
-            test_list_name,
-            good_values_name,
+            rhs_name,
+            lhs_name,
             min(len(difference), 10),
             len(difference),
-            test_list_name,
+            rhs_name,
         )
 
         err_str += create_invalid_data_str(difference)
 
         if warn:
             warnings.warn(err_str)
         else:
             raise ValueError(err_str)
+    return True
 
 
-def verify_same_elements(enforce_order=False, warn=False, **kwargs):
+def verify_same_elements(enforce_order=False, warn=False, **kwargs) -> bool:
     """Verify if two lists contain the same elements regardless of count
 
     Args:
         enforce_order (bool):
             Whether to also check for the same ordering between the two lists
         warn (bool):
             Whether to issue warning instead of error, defaults to False
@@ -158,14 +162,24 @@
 
     try:
         list_one_cast = list(list_one)
         list_two_cast = list(list_two)
     except TypeError:
         raise ValueError("Both arguments provided must be lists or list types")
 
+    # Check if either list inputs are `None` (or both)
+    if any(v == [None] for v in [list_one_cast, list_two_cast]):
+        return True
+    # If both lists are empty
+    if all(len(v) == 0 for v in [list_one_cast, list_two_cast]):
+        return True
+    # If either list one, or two have a length of 0, but not both.
+    if (len(list_one_cast) == 0) is not (len(list_two_cast) == 0):
+        return False
+
     list_one_name, list_two_name = kwargs.keys()
     list_one_name = list_one_name.replace("_", " ")
     list_two_name = list_two_name.replace("_", " ")
 
     if not np.all(set(list_one_cast) == set(list_two_cast)):
         # Values in list one that are not in list two
         missing_vals_1 = [str(val) for val in (set(list_one_cast) - set(list_two_cast))]
@@ -225,7 +239,8 @@
                     list_one_name,
                     list_two_name,
                     list_one_cast[first_bad_index],
                     list_two_cast[first_bad_index],
                     first_bad_index,
                 )
             )
+    return True
```

### Comparing `alpineer-0.1.5/src/alpineer/test_utils.py` & `alpineer-0.1.6/src/alpineer/test_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/src/alpineer/tiff_utils.py` & `alpineer-0.1.6/src/alpineer/tiff_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.5/setup.py` & `alpineer-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: alpineer
+Version: 0.1.6
+Summary: Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy.
+Home-page: https://github.com/angelolab/tmi
+License: Modified Apache 2.0
+Author: Noah Frey Greenwald
+Author-email: nfgreen@stanford.edu
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: charset-normalizer (>=2.1.1,<3.0.0)
+Requires-Dist: matplotlib (>=3,<4)
+Requires-Dist: natsort (>=8,<9)
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Requires-Dist: pillow (>=9,<10)
+Requires-Dist: scikit-image (<1.0.0)
+Requires-Dist: tifffile
+Requires-Dist: xarray
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Project-URL: Documentation, https://tmi.readthedocs.io
+Project-URL: Repository, https://github.com/angelolab/tmi
+Description-Content-Type: text/markdown
+
+# Alpineer
+
+Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout [ark-analysis](https://github.com/angelolab/ark-analysis), [mibi-bin-tools](https://github.com/angelolab/mibi-bin-tools), and [toffy](https://github.com/angelolab/toffy)
+
+- [alpineer](#alpineer)
+  - [Requirements](#requirements)
+  - [Setup](#setup)
+  - [Development Notes](#development-notes)
+  - [Questions?](#questions)
+
+## Requirements
+
+* [Python Poetry](https://python-poetry.org)
+  * Recommeded to install it with either:
+    * [**Official Installer:**](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
+        ```sh
+        curl -sSL https://install.python-poetry.org | python3 -
+        ```
+    * [**pipx**](https://python-poetry.org/docs/master/#installing-with-pipx), (requires [`pipx`](https://pypa.github.io/pipx/))
+      * If you are using `pipx`, run the following installation commands
+        ```sh
+        brew install pipx
+        pipx ensurepath
+        ```
+* [pre-commit](https://pre-commit.com)
+    ```sh
+    brew isntall pre-commit
+    ```
+
+## Setup
+
+1. Clone the repo: `git clone https://github.com/angelolab/alpineer.git`
+2. `cd` into `alpineer`.
+3. Install the pre-commit hooks with `pre-commit install`
+4. Set up `python-poetry` for `alpineer`
+   1. Run `poetry install` to install `alpineer` into your virtual environment. (Poetry utilizes [Python's Virtual Environments](https://docs.python.org/3/tutorial/venv.html))
+   2. Run `poetry install --with test`: Installs all the [dependencies needed for tests](pyproject.toml) (labeled under `tool.poetry.group.test.dependencies`)
+   3. Run `poetry install --with dev`: Installs all the [dependencies needed for development](pyproject.coml) (labeled under `tool.poetry.group.dev.dependencies`)
+   4. You may combine these as well with `poetry install --with dev,test`. Installing the base dependencies and the two optional groups.
+5. In order to test to see if Poetry is working properly, run `poetry show --tree`. This will output the dependency tree for the base dependencies (labeled under `tool.poetry.dependencies`).
+
+    Sample Output:
+
+   ```sh
+   matplotlib 3.6.1 Python plotting package
+   ├── contourpy >=1.0.1
+   │   └── numpy >=1.16
+   ├── cycler >=0.10
+   ├── fonttools >=4.22.0
+   ├── kiwisolver >=1.0.1
+   ├── numpy >=1.19
+   ├── packaging >=20.0
+   │   └── pyparsing >=2.0.2,<3.0.5 || >3.0.5
+   ├── pillow >=6.2.0
+   ├── pyparsing >=2.2.1
+   ├── python-dateutil >=2.7
+   │   └── six >=1.5
+   └── setuptools-scm >=7
+       ├── packaging >=20.0
+       │   └── pyparsing >=2.0.2,<3.0.5 || >3.0.5
+       ├── setuptools *
+       ├── tomli >=1.0.0
+       └── typing-extensions *
+   natsort 8.2.0 Simple yet flexible natural sorting in Python.
+   numpy 1.23.4 NumPy is the fundamental package for array computing with Python.
+   pillow 9.1.1 Python Imaging Library (Fork)
+   pip 22.3 The PyPA recommended tool for installing Python packages.
+   tifffile 2022.10.10 Read and write TIFF files
+   └── numpy >=1.19.2
+   ```
+
+
+## Development Notes
+
+1. I'd highly suggest refering to Poetry's extensive documentation on [installing packages](https://python-poetry.org/docs/master/cli/#add), [updating packages](https://python-poetry.org/docs/master/cli/#update) and more.
+2. Tests can be ran with `poetry run pytest`. No additional arguments needed, they are all stored in the [`pyproject.toml`](pyproject.toml) file.
+   1. As an aside, if you need to execute code in the poetry venv, use prefix your command with [`poetry run`](https://python-poetry.org/docs/master/cli/#run)
+
+## Updating
+
+* In order to update `alpineer`'s dependencies we can run:
+  *  `poetry update`: for all dependencies
+  *  `poetry update <package>`: where `<package>` can be something like `numpy`.
+* To update Poetry itself, run `poetry self update`.
+## Questions?
 
-package_dir = \
-{'': 'src'}
+Feel free to open an issue on our [GitHub page](https://github.com/angelolab/alpineer/issues)
 
-packages = \
-['alpineer']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['charset-normalizer>=2.1.1,<3.0.0',
- 'matplotlib>=3,<4',
- 'natsort>=8,<9',
- 'numpy>=1.0.0,<2.0.0',
- 'pillow>=9,<10',
- 'scikit-image<1.0.0',
- 'tifffile',
- 'xarray',
- 'xmltodict>=0.13.0,<0.14.0']
-
-setup_kwargs = {
-    'name': 'alpineer',
-    'version': '0.1.5',
-    'description': 'Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy.',
-    'long_description': "# Alpineer\n\nToolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout [ark-analysis](https://github.com/angelolab/ark-analysis), [mibi-bin-tools](https://github.com/angelolab/mibi-bin-tools), and [toffy](https://github.com/angelolab/toffy)\n\n- [alpineer](#alpineer)\n  - [Requirements](#requirements)\n  - [Setup](#setup)\n  - [Development Notes](#development-notes)\n  - [Questions?](#questions)\n\n## Requirements\n\n* [Python Poetry](https://python-poetry.org)\n  * Recommeded to install it with either:\n    * [**Official Installer:**](https://python-poetry.org/docs/master/#installing-with-the-official-installer)\n        ```sh\n        curl -sSL https://install.python-poetry.org | python3 -\n        ```\n    * [**pipx**](https://python-poetry.org/docs/master/#installing-with-pipx), (requires [`pipx`](https://pypa.github.io/pipx/))\n      * If you are using `pipx`, run the following installation commands\n        ```sh\n        brew install pipx\n        pipx ensurepath\n        ```\n* [pre-commit](https://pre-commit.com)\n    ```sh\n    brew isntall pre-commit\n    ```\n\n## Setup\n\n1. Clone the repo: `git clone https://github.com/angelolab/alpineer.git`\n2. `cd` into `alpineer`.\n3. Install the pre-commit hooks with `pre-commit install`\n4. Set up `python-poetry` for `alpineer`\n   1. Run `poetry install` to install `alpineer` into your virtual environment. (Poetry utilizes [Python's Virtual Environments](https://docs.python.org/3/tutorial/venv.html))\n   2. Run `poetry install --with test`: Installs all the [dependencies needed for tests](pyproject.toml) (labeled under `tool.poetry.group.test.dependencies`)\n   3. Run `poetry install --with dev`: Installs all the [dependencies needed for development](pyproject.coml) (labeled under `tool.poetry.group.dev.dependencies`)\n   4. You may combine these as well with `poetry install --with dev,test`. Installing the base dependencies and the two optional groups.\n5. In order to test to see if Poetry is working properly, run `poetry show --tree`. This will output the dependency tree for the base dependencies (labeled under `tool.poetry.dependencies`).\n\n    Sample Output:\n\n   ```sh\n   matplotlib 3.6.1 Python plotting package\n   ├── contourpy >=1.0.1\n   │   └── numpy >=1.16\n   ├── cycler >=0.10\n   ├── fonttools >=4.22.0\n   ├── kiwisolver >=1.0.1\n   ├── numpy >=1.19\n   ├── packaging >=20.0\n   │   └── pyparsing >=2.0.2,<3.0.5 || >3.0.5\n   ├── pillow >=6.2.0\n   ├── pyparsing >=2.2.1\n   ├── python-dateutil >=2.7\n   │   └── six >=1.5\n   └── setuptools-scm >=7\n       ├── packaging >=20.0\n       │   └── pyparsing >=2.0.2,<3.0.5 || >3.0.5\n       ├── setuptools *\n       ├── tomli >=1.0.0\n       └── typing-extensions *\n   natsort 8.2.0 Simple yet flexible natural sorting in Python.\n   numpy 1.23.4 NumPy is the fundamental package for array computing with Python.\n   pillow 9.1.1 Python Imaging Library (Fork)\n   pip 22.3 The PyPA recommended tool for installing Python packages.\n   tifffile 2022.10.10 Read and write TIFF files\n   └── numpy >=1.19.2\n   ```\n\n\n## Development Notes\n\n1. I'd highly suggest refering to Poetry's extensive documentation on [installing packages](https://python-poetry.org/docs/master/cli/#add), [updating packages](https://python-poetry.org/docs/master/cli/#update) and more.\n2. Tests can be ran with `poetry run pytest`. No additional arguments needed, they are all stored in the [`pyproject.toml`](pyproject.toml) file.\n   1. As an aside, if you need to execute code in the poetry venv, use prefix your command with [`poetry run`](https://python-poetry.org/docs/master/cli/#run)\n\n## Updating\n\n* In order to update `alpineer`'s dependencies we can run:\n  *  `poetry update`: for all dependencies\n  *  `poetry update <package>`: where `<package>` can be something like `numpy`.\n* To update Poetry itself, run `poetry self update`.\n## Questions?\n\nFeel free to open an issue on our [GitHub page](https://github.com/angelolab/alpineer/issues)\n",
-    'author': 'Noah Frey Greenwald',
-    'author_email': 'nfgreen@stanford.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/angelolab/tmi',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

