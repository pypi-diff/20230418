# Comparing `tmp/pipen_board-0.0.7.tar.gz` & `tmp/pipen_board-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.0.7.tar", max compression
+gzip compressed data, was "pipen_board-0.0.8.tar", max compression
```

## Comparing `pipen_board-0.0.7.tar` & `pipen_board-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1780 2023-04-18 17:26:58.550042 pipen_board-0.0.7/README.md
--rw-r--r--   0        0        0      348 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/__init__.py
--rw-r--r--   0        0        0     7513 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/apis.py
--rw-r--r--   0        0        0     4134 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/cli.py
--rw-r--r--   0        0        0    22572 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/data_manager.py
--rw-r--r--   0        0        0     5895 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-04-18 17:26:58.550042 pipen_board-0.0.7/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   621271 2023-04-18 17:26:58.554042 pipen_board-0.0.7/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   725451 2023-04-18 17:26:58.558042 pipen_board-0.0.7/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-04-18 17:26:58.558042 pipen_board-0.0.7/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-04-18 17:26:58.558042 pipen_board-0.0.7/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7488 2023-04-18 17:26:58.562042 pipen_board-0.0.7/pipen_board/plugin.py
--rw-r--r--   0        0        0     3393 2023-04-18 17:26:58.562042 pipen_board-0.0.7/pipen_board/quart_app.py
--rw-r--r--   0        0        0      727 2023-04-18 17:26:58.562042 pipen_board-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pipen_board-0.0.7/setup.py
--rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 pipen_board-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1780 2023-04-18 17:41:22.082455 pipen_board-0.0.8/README.md
+-rw-r--r--   0        0        0      348 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/__init__.py
+-rw-r--r--   0        0        0     7513 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/apis.py
+-rw-r--r--   0        0        0     4134 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/cli.py
+-rw-r--r--   0        0        0    22572 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     5895 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   621271 2023-04-18 17:41:22.082455 pipen_board-0.0.8/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   725451 2023-04-18 17:41:22.086455 pipen_board-0.0.8/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-04-18 17:41:22.086455 pipen_board-0.0.8/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-04-18 17:41:22.086455 pipen_board-0.0.8/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7488 2023-04-18 17:41:22.090456 pipen_board-0.0.8/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3393 2023-04-18 17:41:22.090456 pipen_board-0.0.8/pipen_board/quart_app.py
+-rw-r--r--   0        0        0      727 2023-04-18 17:41:22.090456 pipen_board-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pipen_board-0.0.8/setup.py
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 pipen_board-0.0.8/PKG-INFO
```

### Comparing `pipen_board-0.0.7/README.md` & `pipen_board-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/apis.py` & `pipen_board-0.0.8/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/cli.py` & `pipen_board-0.0.8/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/data_manager.py` & `pipen_board-0.0.8/pipen_board/data_manager.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/defaults.py` & `pipen_board-0.0.8/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.0.8/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.0.8/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.0.8/pipen_board/frontend/build/assets/index.js`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.0.8/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/plugin.py` & `pipen_board-0.0.8/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pipen_board/quart_app.py` & `pipen_board-0.0.8/pipen_board/quart_app.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.7/pyproject.toml` & `pipen_board-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.0.7"
+version = "0.0.8"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
```

### Comparing `pipen_board-0.0.7/setup.py` & `pipen_board-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': "# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        '__main__'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n[1]: https://github.com/pwwang/pipen\n",
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.0.7/PKG-INFO` & `pipen_board-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.0.7
+Version: 0.0.8
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

