# Comparing `tmp/gbstats-0.4.0.tar.gz` & `tmp/gbstats-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbstats-0.4.0.tar", max compression
+gzip compressed data, was "gbstats-0.5.0.tar", max compression
```

## Comparing `gbstats-0.4.0.tar` & `gbstats-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1075 2023-02-15 16:41:58.472739 gbstats-0.4.0/LICENSE
--rw-r--r--   0        0        0      177 2023-01-20 21:11:32.546026 gbstats-0.4.0/README.md
--rw-r--r--   0        0        0       69 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 21:11:32.546026 gbstats-0.4.0/gbstats/bayesian/__init__.py
--rw-r--r--   0        0        0       55 2023-01-20 21:11:32.546026 gbstats-0.4.0/gbstats/bayesian/constants.py
--rw-r--r--   0        0        0     3943 2023-01-26 14:37:19.743416 gbstats-0.4.0/gbstats/bayesian/dists.py
--rw-r--r--   0        0        0     2535 2023-01-20 21:11:32.546026 gbstats-0.4.0/gbstats/bayesian/orthogonal.py
--rw-r--r--   0        0        0     5800 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/bayesian/tests.py
--rw-r--r--   0        0        0        0 2023-01-20 21:11:32.550026 gbstats-0.4.0/gbstats/frequentist/__init__.py
--rw-r--r--   0        0        0     4028 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/frequentist/tests.py
--rw-r--r--   0        0        0    12071 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/gbstats.py
--rw-r--r--   0        0        0     6271 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/gen_notebook.py
--rw-r--r--   0        0        0      107 2023-01-20 21:11:32.550026 gbstats-0.4.0/gbstats/shared/constants.py
--rw-r--r--   0        0        0     2260 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/shared/models.py
--rw-r--r--   0        0        0      347 2023-02-17 22:33:48.517459 gbstats-0.4.0/gbstats/shared/tests.py
--rw-r--r--   0        0        0     1423 2023-02-17 22:33:48.517459 gbstats-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-01-20 21:11:32.550026 gbstats-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 21:11:32.550026 gbstats-0.4.0/tests/bayesian/__init__.py
--rw-r--r--   0        0        0     5373 2023-01-26 14:37:19.743416 gbstats-0.4.0/tests/bayesian/test_dists.py
--rw-r--r--   0        0        0     3695 2023-02-17 22:33:48.521459 gbstats-0.4.0/tests/bayesian/test_tests.py
--rw-r--r--   0        0        0        0 2023-01-20 21:11:32.550026 gbstats-0.4.0/tests/frequentist/__init__.py
--rw-r--r--   0        0        0     1421 2023-02-17 22:33:48.521459 gbstats-0.4.0/tests/frequentist/test_tests.py
--rw-r--r--   0        0        0     9477 2023-02-17 22:33:48.521459 gbstats-0.4.0/tests/test_gbstats.py
--rw-r--r--   0        0        0     2053 2023-02-17 22:33:48.521459 gbstats-0.4.0/tests/test_shared_models.py
--rw-r--r--   0        0        0     1085 2023-02-17 22:36:04.066326 gbstats-0.4.0/setup.py
--rw-r--r--   0        0        0     1089 2023-02-17 22:36:04.066698 gbstats-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 00:06:10.588659 gbstats-0.5.0/LICENSE
+-rw-r--r--   0        0        0      177 2023-04-13 00:06:10.588659 gbstats-0.5.0/README.md
+-rw-r--r--   0        0        0       69 2023-04-18 17:40:11.087308 gbstats-0.5.0/gbstats/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:06:10.588659 gbstats-0.5.0/gbstats/bayesian/__init__.py
+-rw-r--r--   0        0        0     3953 2023-04-17 13:02:09.896940 gbstats-0.5.0/gbstats/bayesian/dists.py
+-rw-r--r--   0        0        0     2535 2023-04-13 00:06:10.588659 gbstats-0.5.0/gbstats/bayesian/orthogonal.py
+-rw-r--r--   0        0        0     7223 2023-04-17 13:02:09.896940 gbstats-0.5.0/gbstats/bayesian/tests.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:06:10.588659 gbstats-0.5.0/gbstats/frequentist/__init__.py
+-rw-r--r--   0        0        0     6447 2023-04-17 13:02:09.900940 gbstats-0.5.0/gbstats/frequentist/tests.py
+-rw-r--r--   0        0        0    13395 2023-04-17 13:02:09.900940 gbstats-0.5.0/gbstats/gbstats.py
+-rw-r--r--   0        0        0     7253 2023-04-18 17:40:11.087308 gbstats-0.5.0/gbstats/gen_notebook.py
+-rw-r--r--   0        0        0      552 2023-04-13 00:06:10.592659 gbstats-0.5.0/gbstats/messages.py
+-rw-r--r--   0        0        0      107 2023-04-13 00:06:10.592659 gbstats-0.5.0/gbstats/shared/constants.py
+-rw-r--r--   0        0        0     5221 2023-04-13 00:06:10.592659 gbstats-0.5.0/gbstats/shared/models.py
+-rw-r--r--   0        0        0      513 2023-04-13 00:06:10.592659 gbstats-0.5.0/gbstats/shared/tests.py
+-rw-r--r--   0        0        0      478 2023-04-18 17:40:11.087308 gbstats-0.5.0/gbstats/utils.py
+-rw-r--r--   0        0        0     1451 2023-04-18 17:40:11.087308 gbstats-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-13 00:06:10.592659 gbstats-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:06:10.592659 gbstats-0.5.0/tests/bayesian/__init__.py
+-rw-r--r--   0        0        0     5373 2023-04-13 00:06:10.592659 gbstats-0.5.0/tests/bayesian/test_dists.py
+-rw-r--r--   0        0        0     5667 2023-04-17 13:02:09.900940 gbstats-0.5.0/tests/bayesian/test_tests.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:06:10.592659 gbstats-0.5.0/tests/frequentist/__init__.py
+-rw-r--r--   0        0        0     6493 2023-04-17 13:02:09.900940 gbstats-0.5.0/tests/frequentist/test_tests.py
+-rw-r--r--   0        0        0    25966 2023-04-17 13:02:09.900940 gbstats-0.5.0/tests/test_gbstats.py
+-rw-r--r--   0        0        0     6207 2023-04-17 13:02:09.900940 gbstats-0.5.0/tests/test_shared_models.py
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 gbstats-0.5.0/PKG-INFO
```

### Comparing `gbstats-0.4.0/LICENSE` & `gbstats-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gbstats-0.4.0/gbstats/bayesian/dists.py` & `gbstats-0.5.0/gbstats/bayesian/dists.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 from warnings import warn
 import numpy as np
 from scipy.stats import beta, norm, rv_continuous
 from scipy.special import digamma, polygamma, roots_hermitenorm
 from .orthogonal import roots_sh_jacobi
-from gbstats.bayesian.constants import EPSILON
 
 
 class BayesABDist(ABC):
     dist: rv_continuous
 
     @staticmethod
     @abstractmethod
@@ -18,19 +17,20 @@
         :type data: Iterable
         :rtype: Tuple[ndarray, ndarray]
         """
         raise NotImplementedError
 
     @staticmethod
     @abstractmethod
-    def moments(par1, par2, log=False):
+    def moments(par1, par2, log=False, epsilon=1e-4):
         """
         :type par1: float or ndarray
         :type par2: float or ndarray
         :type log: bool
+        :type epsilon: float
         :rtype: Tuple[float or ndarray, float or ndarray]
         """
         raise NotImplementedError
 
     @staticmethod
     @abstractmethod
     def gq(n, par1, par2):
@@ -102,26 +102,26 @@
         var = 1 / (inv_var_0 + inv_var_d)
 
         loc = var * (inv_var_0 * prior[0] + inv_var_d * data[0])
         scale = np.sqrt(var)
         return loc, scale
 
     @staticmethod
-    def moments(par1, par2, log=False):
+    def moments(par1, par2, log=False, epsilon=1e-4):
         if np.sum(par2 < 0):
             raise RuntimeError("got negative standard deviation.")
 
         if log:
             if np.sum(par1 <= 0):
                 raise RuntimeError("got mu <= 0. cannot use log approximation.")
 
             max_prob = np.max(norm.cdf(0, par1, par2))
-            if max_prob > EPSILON:
+            if max_prob > epsilon:
                 warn(
-                    f"probability of being negative is higher than {EPSILON} (={max_prob}). "
+                    f"probability of being negative is higher than {epsilon} (={max_prob}). "
                     f"log approximation is in-exact",
                     RuntimeWarning,
                 )
 
             mean = np.log(par1)
             var = np.power(par2 / par1, 2)
         else:
```

### Comparing `gbstats-0.4.0/gbstats/bayesian/orthogonal.py` & `gbstats-0.5.0/gbstats/bayesian/orthogonal.py`

 * *Files identical despite different names*

### Comparing `gbstats-0.4.0/gbstats/gen_notebook.py` & `gbstats-0.5.0/gbstats/gen_notebook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .gbstats import (
     detect_unknown_variations,
     analyze_metric_df,
     get_metric_df,
     reduce_dimensionality,
 )
+from gbstats.shared.constants import StatsEngine
 import nbformat
 from nbformat import v4 as nbf
 from nbformat.v4.nbjson import from_dict
 
 
 def code_cell_df(df, source=""):
     return nbf.new_code_cell(
@@ -35,53 +36,68 @@
     hypothesis="",
     name="",
     var_id_map={},
     var_names=[],
     weights=[],
     run_query="",
     metrics=[],
-    needs_correction=False,
+    stats_engine=StatsEngine.BAYESIAN,
+    engine_config={},
 ):
     summary_cols = [
         "dimension",
         "baseline_name",
         "baseline_users",
         "baseline_cr",
         "baseline_risk",
     ]
     for i in range(1, len(var_names)):
         summary_cols.append(f"v{i}_name")
         summary_cols.append(f"v{i}_users")
         summary_cols.append(f"v{i}_cr")
-        summary_cols.append(f"v{i}_risk")
         summary_cols.append(f"v{i}_expected")
         summary_cols.append(f"v{i}_ci")
-        summary_cols.append(f"v{i}_prob_beat_baseline")
+        if stats_engine == StatsEngine.BAYESIAN:
+            summary_cols.append(f"v{i}_risk")
+            summary_cols.append(f"v{i}_prob_beat_baseline")
+        elif stats_engine == StatsEngine.FREQUENTIST:
+
+            summary_cols.append(f"v{i}_p_value")
 
     cells = [
         nbf.new_markdown_cell(
             f"# {name}\n"
             f"[View on GrowthBook]({url})\n\n"
             f"**Hypothesis:** {hypothesis}"
         ),
         nbf.new_markdown_cell("## Notebook Setup"),
         nbf.new_code_cell(
-            "# Requires gbstats version 0.4.0 or higher\n"
+            "# This notebook requires gbstats version 0.5.0 or later\n"
+            "try:\n"
+            "    import gbstats.utils\n"
+            "    gbstats.utils.check_gbstats_compatibility('0.5.0')\n"
+            "except ModuleNotFoundError:\n"
+            "    raise ValueError('Upgrade gbstats to 0.5.0 or later from PyPI using `pip install gbstats`')\n"
             "from gbstats.gbstats import (\n"
-            "  detect_unknown_variations,\n"
-            "  analyze_metric_df,\n"
-            "  get_metric_df,\n"
-            "  reduce_dimensionality\n"
-            ")\n\n"
+            "    detect_unknown_variations,\n"
+            "    analyze_metric_df,\n"
+            "    get_metric_df,\n"
+            "    reduce_dimensionality\n"
+            ")\n"
+            "from gbstats.shared.constants import StatsEngine\n\n"
             "# Mapping of variation id to index\n"
             f"var_id_map = {str(var_id_map)}\n\n"
             "# Display names of variations\n"
             f"var_names = {str(var_names)}\n\n"
             "# Expected traffic split between variations\n"
             f"weights = {str(weights)}\n"
+            "# Statistics engine to use\n"
+            f"stats_engine = {str(stats_engine)}\n"
+            "# Engine config\n"
+            f"engine_config = {str(engine_config)}\n"
             f"# Columns to show in the result summary\n"
             f"summary_cols = {str(summary_cols)}"
         ),
         nbf.new_code_cell("# User defined runQuery function\n" f"{run_query}"),
     ]
 
     for i, metric in enumerate(metrics):
@@ -140,37 +156,41 @@
         )
 
         df = reduce_dimensionality(df, max=20)
         cells.append(
             code_cell_df(
                 df=df,
                 source=(
-                    "# If there are too many dimensions, marge the smaller ones together\n"
+                    "# If there are too many dimensions, merge the smaller ones together\n"
                     f"m{i}_reduced = reduce_dimensionality(m{i}, max=20)\n"
                     f"display(m{i}_reduced)"
                 ),
             )
         )
 
         cells.append(nbf.new_markdown_cell("### Result"))
 
         result = analyze_metric_df(
             df=df,
             weights=weights,
             inverse=inverse,
+            engine=stats_engine,
+            engine_config=engine_config,
         )
         cells.append(
             code_cell_df(
                 df=result[summary_cols].T,
                 source=(
                     "# Run the analysis and show a summary of results\n"
                     f"m{i}_result = analyze_metric_df(\n"
                     f"    df=m{i}_reduced,\n"
                     f"    weights=weights,\n"
-                    f"    inverse={inverse}\n"
+                    f"    inverse={inverse},\n"
+                    f"    engine=stats_engine,\n"
+                    f"    engine_config=engine_config,\n"
                     f")\n"
                     f"display(m{i}_result[summary_cols].T)"
                 ),
             )
         )
 
     nb = nbf.new_notebook(
```

### Comparing `gbstats-0.4.0/pyproject.toml` & `gbstats-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "gbstats"
-version = "0.4.0"
+version = "0.5.0"
 homepage = "https://github.com/growthbook/growthbook/tree/main/packages/stats"
 description = "Stats engine for GrowthBook, the open source feature flagging and A/B testing platform."
 authors = ["Jeremy Dorn <jeremy@growthbook.io>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -25,15 +25,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pandas = "^1.5.1"
 scipy = "^1.9.2"
 numpy = "^1.23.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+certifi = "2022.12.7"
 tox = "^3.20.1"
 virtualenv = "^20.2.2"
 twine = "^3.3.0"
 toml = "^0.10.2"
 black = "22.3.0"
 isort = "5.6.4"
 flake8 = "3.8.4"
```

### Comparing `gbstats-0.4.0/tests/bayesian/test_dists.py` & `gbstats-0.5.0/tests/bayesian/test_dists.py`

 * *Files identical despite different names*

### Comparing `gbstats-0.4.0/PKG-INFO` & `gbstats-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: gbstats
-Version: 0.4.0
+Version: 0.5.0
 Summary: Stats engine for GrowthBook, the open source feature flagging and A/B testing platform.
 Home-page: https://github.com/growthbook/growthbook/tree/main/packages/stats
 License: MIT
 Author: Jeremy Dorn
 Author-email: jeremy@growthbook.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: scipy (>=1.9.2,<2.0.0)
```

