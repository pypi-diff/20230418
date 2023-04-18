# Comparing `tmp/pipen_board-0.0.4.tar.gz` & `tmp/pipen_board-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.0.4.tar", max compression
+gzip compressed data, was "pipen_board-0.0.5.tar", max compression
```

## Comparing `pipen_board-0.0.4.tar` & `pipen_board-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1780 2023-04-17 23:57:42.241046 pipen_board-0.0.4/README.md
--rw-r--r--   0        0        0      348 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/__init__.py
--rw-r--r--   0        0        0     7170 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/apis.py
--rw-r--r--   0        0        0     4081 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/cli.py
--rw-r--r--   0        0        0    21706 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/data_manager.py
--rw-r--r--   0        0        0     5895 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-04-17 23:57:42.241046 pipen_board-0.0.4/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   621271 2023-04-17 23:57:42.245046 pipen_board-0.0.4/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   723656 2023-04-17 23:57:42.249046 pipen_board-0.0.4/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-04-17 23:57:42.249046 pipen_board-0.0.4/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-04-17 23:57:42.249046 pipen_board-0.0.4/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7488 2023-04-17 23:57:42.253046 pipen_board-0.0.4/pipen_board/plugin.py
--rw-r--r--   0        0        0     3341 2023-04-17 23:57:42.253046 pipen_board-0.0.4/pipen_board/quart_app.py
--rw-r--r--   0        0        0      783 2023-04-17 23:57:42.253046 pipen_board-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 pipen_board-0.0.4/setup.py
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 pipen_board-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1780 2023-04-18 03:46:49.609347 pipen_board-0.0.5/README.md
+-rw-r--r--   0        0        0      348 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/__init__.py
+-rw-r--r--   0        0        0     7170 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/apis.py
+-rw-r--r--   0        0        0     4081 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/cli.py
+-rw-r--r--   0        0        0    21706 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     5895 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   621271 2023-04-18 03:46:49.613347 pipen_board-0.0.5/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   723656 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7488 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3341 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pipen_board/quart_app.py
+-rw-r--r--   0        0        0      766 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 pipen_board-0.0.5/setup.py
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 pipen_board-0.0.5/PKG-INFO
```

### Comparing `pipen_board-0.0.4/README.md` & `pipen_board-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/apis.py` & `pipen_board-0.0.5/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/cli.py` & `pipen_board-0.0.5/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/data_manager.py` & `pipen_board-0.0.5/pipen_board/data_manager.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/defaults.py` & `pipen_board-0.0.5/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.0.5/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.0.5/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.0.5/pipen_board/frontend/build/assets/index.js`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.0.5/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/plugin.py` & `pipen_board-0.0.5/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pipen_board/quart_app.py` & `pipen_board-0.0.5/pipen_board/quart_app.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.4/pyproject.toml` & `pipen_board-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.0.4"
+version = "0.0.5"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [
-    { include = "pipen_board/**/*.py" },
-]
-include = ["pipen_board/frontend/build"]
+exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pipen = "^0.9"
```

### Comparing `pipen_board-0.0.4/setup.py` & `pipen_board-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pipen_board']
 
 package_data = \
-{'': ['*'],
- 'pipen_board': ['frontend/*',
-                 'frontend/build/*',
-                 'frontend/build/assets/*',
-                 'frontend/public/assets/*',
-                 'frontend/src/*',
-                 'frontend/src/assets/*',
-                 'frontend/src/lib/*',
-                 'frontend/src/lib/configuration/*',
-                 'frontend/src/lib/configuration/options/*',
-                 'frontend/src/lib/run/*']}
+{'': ['*'], 'pipen_board': ['frontend/build/*', 'frontend/build/assets/*']}
 
 install_requires = \
 ['cmdy>=0.5,<0.6',
  'pipen-annotate>=0.7,<0.8',
  'pipen-args>=0.9.5,<0.10.0',
  'pipen-log2file>=0.2.1,<0.3.0',
  'pipen>=0.9,<0.10',
@@ -28,15 +18,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': "# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        '__main__'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n[1]: https://github.com/pwwang/pipen\n",
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.0.4/PKG-INFO` & `pipen_board-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.0.4
+Version: 0.0.5
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

