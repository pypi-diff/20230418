# Comparing `tmp/zeno_evals-0.1.4.tar.gz` & `tmp/zeno_evals-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.4.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.5.tar", max compression
```

## Comparing `zeno_evals-0.1.4.tar` & `zeno_evals-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.4/README.md
--rw-r--r--   0        0        0      520 2023-04-11 22:57:53.193770 zeno_evals-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 21:01:32.056333 zeno_evals-0.1.4/zeno_evals/__init__.py
--rw-r--r--   0        0        0     5128 2023-04-11 22:57:06.636732 zeno_evals-0.1.4/zeno_evals/main.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.4/setup.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.5/README.md
+-rw-r--r--   0        0        0      538 2023-04-18 13:15:26.682838 zeno_evals-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-18 13:13:07.961491 zeno_evals-0.1.5/zeno_evals/__init__.py
+-rw-r--r--   0        0        0     5242 2023-04-18 13:12:44.131377 zeno_evals-0.1.5/zeno_evals/main.py
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.5/setup.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.5/PKG-INFO
```

### Comparing `zeno_evals-0.1.4/LICENSE.md` & `zeno_evals-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.4/README.md` & `zeno_evals-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.4/pyproject.toml` & `zeno_evals-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "zeno-evals"
-version = "0.1.4"
+version = "0.1.5"
 description = "Visualize OpenAI evals with Zeno"
 authors = ["Alex Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "zeno_evals" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11"
 fire = "^0.5.0"
 zenoml = "^0.4.5"
 pandas = "^1.5.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 zeno-evals = "zeno_evals.main:cli"
```

### Comparing `zeno_evals-0.1.4/zeno_evals/main.py` & `zeno_evals-0.1.5/zeno_evals/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from contextlib import contextmanager
-from inspect import getmembers, isfunction
 import json
 import os
 import sys
+from contextlib import contextmanager
 from importlib import util
+from inspect import getmembers, isfunction
 
 import fire
 import pandas as pd
-from zeno import ModelReturn, metric, model, zeno
+from zeno import ModelReturn, ZenoParameters, metric, model, zeno
 from zeno.api import MetricReturn, ZenoOptions
 
 
 @contextmanager
 def add_to_path(p):
     old_path = sys.path
     sys.path = sys.path[:]
@@ -43,21 +43,16 @@
     return functions
 
 
 def get_metric_function(metric_name):
     def metric_function(df, ops: ZenoOptions):
         if len(df) == 0:
             return MetricReturn(metric=0.0)
-        if (
-            df[metric_name].dtype == "object"
-            and df[metric_name].value_counts().shape[0] <= 2
-        ):
-            return MetricReturn(
-                metric=df[metric_name].eq(df[metric_name][0]).mul(1).mean()
-            )
+        if df[metric_name].dtype == "object" and df[metric_name].value_counts().shape[0] <= 2:
+            return MetricReturn(metric=df[metric_name].eq(df[metric_name][0]).mul(1).mean())
         return MetricReturn(metric=df[metric_name].mean())
 
     metric_function.__name__ = metric_name
 
     return metric(metric_function)
 
 
@@ -119,30 +114,17 @@
         df = df.join(match_df.set_index("id"), on="id")
     if len(metrics_df) > 0:
         df = df.join(metrics_df.set_index("id"), on="id")
 
     return df, metric_names
 
 
-def main(
+def generate_zeno_config(
     results_file: str, second_results_file: str = None, functions_file: str = None
-):
-    """Visualize a result from OpenAI evals using Zeno.
-
-    Args:
-            results_file (path): Result .jsonl file from OpenAI evals.
-            Often stored in the /tmp/evallogs/ directory.
-
-            second_results_file (path): Second result .jsonl file from OpenAI
-            evals for comparison. Often stored in the /tmp/evallogs/ directory.
-
-            functions_file (path, optional): Path to a Python file containing
-            additional Zeno processing functions. Defaults to None.
-    """
-
+) -> ZenoParameters:
     if not os.path.exists(results_file):
         print("ERROR: file '{}' does not exist.".format(results_file))
         sys.exit(1)
 
     data = []
     with open(results_file) as f:
         for line in f:
@@ -156,32 +138,46 @@
 
     for m in metric_names:
         functions = functions + [get_metric_function(m)]
 
     if "expected" in df.columns:
         functions = functions + [correct]
 
-    zeno_config = {
-        "metadata": df,
-        "models": data[0]["spec"]["completion_fns"],
-        "functions": functions,
-        "view": "openai-chat",
-        "data_column": "prompt",
-        "id_column": "id",
-        "cache_path": "./.zeno_cache_" + os.path.basename(results_file).split("_")[0],
-        "port": 8080,
-        "batch_size": 100,
-        "samples": 5,
-    }
+    zeno_config = ZenoParameters(
+        metadata=df,
+        models=data[0]["spec"]["completion_fns"],
+        functions=functions,
+        view="openai-chat",
+        data_column="prompt",
+        id_column="id",
+        cache_path="./.zeno_cache_" + os.path.basename(results_file).split("_")[0],
+        port=8080,
+        batch_size=100,
+        samples=5,
+    )
 
     if "expected" in df.columns:
         zeno_config["label_column"] = "expected"
 
-    zeno(zeno_config)
+    return zeno_config
 
 
-def cli():
-    fire.Fire(main)
+def main(results_file: str, second_results_file: str = None, functions_file: str = None):
+    """Visualize a result from OpenAI evals using Zeno.
 
+    Args:
+            results_file (path): Result .jsonl file from OpenAI evals.
+            Often stored in the /tmp/evallogs/ directory.
 
-if __name__ == "__main__":
+            second_results_file (path): Second result .jsonl file from OpenAI
+            evals for comparison. Often stored in the /tmp/evallogs/ directory.
+
+            functions_file (path, optional): Path to a Python file containing
+            additional Zeno processing functions. Defaults to None.
+    """
+
+    config = generate_zeno_config(results_file, second_results_file, functions_file)
+    zeno(config)
+
+
+def cli():
     fire.Fire(main)
```

### Comparing `zeno_evals-0.1.4/setup.py` & `zeno_evals-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.5,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Visualize OpenAI evals with Zeno',
     'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\n```bash\nzeno-evals ./example/example.jsonl\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zeno_evals-0.1.4/PKG-INFO` & `zeno_evals-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.4
+Version: 0.1.5
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

