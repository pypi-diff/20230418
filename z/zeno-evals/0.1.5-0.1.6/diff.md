# Comparing `tmp/zeno_evals-0.1.5.tar.gz` & `tmp/zeno_evals-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.5.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.6.tar", max compression
```

## Comparing `zeno_evals-0.1.5.tar` & `zeno_evals-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.5/LICENSE.md
--rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.5/README.md
--rw-r--r--   0        0        0      538 2023-04-18 13:15:26.682838 zeno_evals-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       84 2023-04-18 13:13:07.961491 zeno_evals-0.1.5/zeno_evals/__init__.py
--rw-r--r--   0        0        0     5242 2023-04-18 13:12:44.131377 zeno_evals-0.1.5/zeno_evals/main.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.5/setup.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.6/README.md
+-rw-r--r--   0        0        0      538 2023-04-18 13:23:04.156190 zeno_evals-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-18 13:13:07.961491 zeno_evals-0.1.6/zeno_evals/__init__.py
+-rw-r--r--   0        0        0     5239 2023-04-18 13:22:54.114054 zeno_evals-0.1.6/zeno_evals/main.py
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.6/setup.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.6/PKG-INFO
```

### Comparing `zeno_evals-0.1.5/LICENSE.md` & `zeno_evals-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.5/README.md` & `zeno_evals-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.5/pyproject.toml` & `zeno_evals-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeno-evals"
-version = "0.1.5"
+version = "0.1.6"
 description = "Visualize OpenAI evals with Zeno"
 authors = ["Alex Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "zeno_evals" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11"
```

### Comparing `zeno_evals-0.1.5/zeno_evals/main.py` & `zeno_evals-0.1.6/zeno_evals/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         cache_path="./.zeno_cache_" + os.path.basename(results_file).split("_")[0],
         port=8080,
         batch_size=100,
         samples=5,
     )
 
     if "expected" in df.columns:
-        zeno_config["label_column"] = "expected"
+        zeno_config.label_column = "expected"
 
     return zeno_config
 
 
 def main(results_file: str, second_results_file: str = None, functions_file: str = None):
     """Visualize a result from OpenAI evals using Zeno.
```

### Comparing `zeno_evals-0.1.5/setup.py` & `zeno_evals-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.5,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Visualize OpenAI evals with Zeno',
     'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\n```bash\nzeno-evals ./example/example.jsonl\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zeno_evals-0.1.5/PKG-INFO` & `zeno_evals-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.5
+Version: 0.1.6
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

