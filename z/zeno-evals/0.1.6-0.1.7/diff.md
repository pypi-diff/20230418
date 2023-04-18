# Comparing `tmp/zeno_evals-0.1.6.tar.gz` & `tmp/zeno_evals-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.6.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.7.tar", max compression
```

## Comparing `zeno_evals-0.1.6.tar` & `zeno_evals-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.6/LICENSE.md
--rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.6/README.md
--rw-r--r--   0        0        0      538 2023-04-18 13:23:04.156190 zeno_evals-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       84 2023-04-18 13:13:07.961491 zeno_evals-0.1.6/zeno_evals/__init__.py
--rw-r--r--   0        0        0     5239 2023-04-18 13:22:54.114054 zeno_evals-0.1.6/zeno_evals/main.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.6/setup.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     1259 2023-04-18 17:05:50.193994 zeno_evals-0.1.7/README.md
+-rw-r--r--   0        0        0      537 2023-04-18 17:16:06.138189 zeno_evals-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-18 15:03:49.480326 zeno_evals-0.1.7/zeno_evals/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-18 15:06:35.651777 zeno_evals-0.1.7/zeno_evals/__main__.py
+-rw-r--r--   0        0        0     6316 2023-04-18 16:53:55.919011 zeno_evals-0.1.7/zeno_evals/main.py
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 zeno_evals-0.1.7/setup.py
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 zeno_evals-0.1.7/PKG-INFO
```

### Comparing `zeno_evals-0.1.6/LICENSE.md` & `zeno_evals-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.6/pyproject.toml` & `zeno_evals-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "zeno-evals"
-version = "0.1.6"
+version = "0.1.7"
 description = "Visualize OpenAI evals with Zeno"
 authors = ["Alex Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "zeno_evals" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<=3.11"
+python = ">=3.9,<=3.11"
 fire = "^0.5.0"
-zenoml = "^0.4.5"
+zenoml = "^0.4.10"
 pandas = "^1.5.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
```

### Comparing `zeno_evals-0.1.6/zeno_evals/main.py` & `zeno_evals-0.1.7/zeno_evals/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,27 @@
 import sys
 from contextlib import contextmanager
 from importlib import util
 from inspect import getmembers, isfunction
 
 import fire
 import pandas as pd
-from zeno import ModelReturn, ZenoParameters, metric, model, zeno
+from zeno import (
+    DistillReturn,
+    ModelReturn,
+    ZenoParameters,
+    distill,
+    metric,
+    model,
+    zeno,
+)
 from zeno.api import MetricReturn, ZenoOptions
 
+dfs = {}
+
 
 @contextmanager
 def add_to_path(p):
     old_path = sys.path
     sys.path = sys.path[:]
     sys.path.insert(0, p)
     try:
@@ -43,34 +53,50 @@
     return functions
 
 
 def get_metric_function(metric_name):
     def metric_function(df, ops: ZenoOptions):
         if len(df) == 0:
             return MetricReturn(metric=0.0)
-        if df[metric_name].dtype == "object" and df[metric_name].value_counts().shape[0] <= 2:
-            return MetricReturn(metric=df[metric_name].eq(df[metric_name][0]).mul(1).mean())
+        if (
+            df[metric_name].dtype == "object"
+            and df[metric_name].value_counts().shape[0] <= 2
+        ):
+            return MetricReturn(
+                metric=df[metric_name].eq(df[metric_name][0]).mul(1).mean()
+            )
         return MetricReturn(metric=df[metric_name].mean())
 
     metric_function.__name__ = metric_name
 
     return metric(metric_function)
 
 
 @model
 def model_fn(name):
+    model_df = dfs[name]
+
     def mod(df, ops):
-        return ModelReturn(model_output=df["sampled"])
+        return ModelReturn(model_output=model_df["sampled"].loc[df.index].tolist())
 
     return mod
 
 
-@metric
+@distill
 def correct(df, ops: ZenoOptions):
-    return MetricReturn(metric=df["correct"].astype(int).mean() * 100)
+    model_name = [i for i in dfs.keys() if i in ops.output_column]
+    model_df = dfs[model_name[0]]
+    return DistillReturn(distill_output=model_df["correct"].loc[df.index])
+
+
+@metric
+def avg_correct(df, ops: ZenoOptions):
+    return MetricReturn(
+        metric=df[ops.distill_columns["correct"]].astype(int).mean() * 100
+    )
 
 
 def read_results_file(data):
     sampling_df = pd.DataFrame(
         [
             {
                 "id": d["sample_id"],
@@ -111,61 +137,84 @@
 
     df = sampling_df
     if len(match_df) > 0:
         df = df.join(match_df.set_index("id"), on="id")
     if len(metrics_df) > 0:
         df = df.join(metrics_df.set_index("id"), on="id")
 
+    df.set_index("id", inplace=True, drop=False)
     return df, metric_names
 
 
+def get_model_name(data):
+    name = data[0]["spec"]["completion_fns"][0]
+    return name.replace(".", "_")
+
+
 def generate_zeno_config(
     results_file: str, second_results_file: str = None, functions_file: str = None
 ) -> ZenoParameters:
     if not os.path.exists(results_file):
         print("ERROR: file '{}' does not exist.".format(results_file))
         sys.exit(1)
 
     data = []
     with open(results_file) as f:
         for line in f:
             data.append(json.loads(line))
 
     df, metric_names = read_results_file(data)
+    dfs[get_model_name(data)] = df
+
+    models = [get_model_name(data)]
+    if second_results_file is not None:
+        data2 = []
+        with open(second_results_file) as f:
+            for line in f:
+                data2.append(json.loads(line))
+
+        models.append(get_model_name(data2))
+        df2, _ = read_results_file(data2)
+        dfs[get_model_name(data2)] = df2
 
     functions = [model_fn]
     if functions_file is not None:
         functions = functions + parse_testing_file(functions_file)
 
+    base_df_columns = ["id", "prompt"]
+
     for m in metric_names:
         functions = functions + [get_metric_function(m)]
 
     if "expected" in df.columns:
-        functions = functions + [correct]
+        functions = functions + [correct, avg_correct]
+        base_df_columns = base_df_columns + ["expected"]
 
     zeno_config = ZenoParameters(
-        metadata=df,
-        models=data[0]["spec"]["completion_fns"],
+        metadata=df[base_df_columns],
+        models=models,
         functions=functions,
         view="openai-chat",
         data_column="prompt",
         id_column="id",
-        cache_path="./.zeno_cache_" + os.path.basename(results_file).split("_")[0],
+        cache_path="./.zeno_cache_" + data[0]["spec"]["base_eval"],
         port=8080,
         batch_size=100,
         samples=5,
     )
 
     if "expected" in df.columns:
         zeno_config.label_column = "expected"
 
     return zeno_config
 
 
-def main(results_file: str, second_results_file: str = None, functions_file: str = None):
+def main(
+    results_file: str, second_results_file: str = None, functions_file: str = None
+):
     """Visualize a result from OpenAI evals using Zeno.
 
     Args:
             results_file (path): Result .jsonl file from OpenAI evals.
             Often stored in the /tmp/evallogs/ directory.
 
             second_results_file (path): Second result .jsonl file from OpenAI
```

### Comparing `zeno_evals-0.1.6/setup.py` & `zeno_evals-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['zeno_evals']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.5,<0.5.0']
+['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.10,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Visualize OpenAI evals with Zeno',
-    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\n```bash\nzeno-evals ./example/example.jsonl\n```\n',
+    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\nSingle example looking at US tort law questions:\n\n```bash\nzeno-evals ./examples/example.jsonl\n```\n\nAnd an example of comparison between two models:\n\n```bash\nzeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl\n```\n\nAnd lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:\n\n```bash\npip install wordfreq\nzeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<=3.11',
+    'python_requires': '>=3.9,<=3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `zeno_evals-0.1.6/PKG-INFO` & `zeno_evals-0.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
-Requires-Python: >=3.8.1,<=3.11
+Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: zenoml (>=0.4.5,<0.5.0)
+Requires-Dist: zenoml (>=0.4.10,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Zeno 🤝 OpenAI Evals
 
 Use [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).
 
 https://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov
@@ -34,11 +34,26 @@
 
 ```bash
 zeno-evals /tmp/evallogs/my_eval_cache.jsonl
 ```
 
 ### Example
 
+Single example looking at US tort law questions:
+
+```bash
+zeno-evals ./examples/example.jsonl
+```
+
+And an example of comparison between two models:
+
+```bash
+zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl
+```
+
+And lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:
+
 ```bash
-zeno-evals ./example/example.jsonl
+pip install wordfreq
+zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py
 ```
```

