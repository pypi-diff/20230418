# Comparing `tmp/ez_transform-0.1.5.tar.gz` & `tmp/ez_transform-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_transform-0.1.5.tar", max compression
+gzip compressed data, was "ez_transform-0.1.6.tar", max compression
```

## Comparing `ez_transform-0.1.5.tar` & `ez_transform-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2022-01-16 18:58:28.853644 ez_transform-0.1.5/LICENSE
--rw-r--r--   0        0        0      910 2022-12-31 09:58:33.729105 ez_transform-0.1.5/README.md
--rw-r--r--   0        0        0       53 2022-06-04 13:04:51.824066 ez_transform-0.1.5/ezt/MANIFEST.in
--rw-r--r--   0        0        0      196 2023-03-29 17:19:37.929893 ez_transform-0.1.5/ezt/__init__.py
--rw-r--r--   0        0        0        0 2022-01-16 18:58:28.883643 ez_transform-0.1.5/ezt/build/__init__.py
--rw-r--r--   0        0        0        0 2022-01-16 18:58:28.903643 ez_transform-0.1.5/ezt/build/dfmodel/__init__.py
--rw-r--r--   0        0        0     4878 2023-01-27 18:21:03.824447 ez_transform-0.1.5/ezt/build/dfmodel/merge.py
--rw-r--r--   0        0        0     3518 2023-03-29 17:18:57.559893 ez_transform-0.1.5/ezt/build/dfmodel/models.py
--rw-r--r--   0        0        0     2383 2023-03-07 18:27:36.930756 ez_transform-0.1.5/ezt/build/dfmodel/persist_delta.py
--rw-r--r--   0        0        0      527 2022-11-07 19:50:02.019496 ez_transform-0.1.5/ezt/build/dfmodel/py_model.py
--rw-r--r--   0        0        0     6518 2023-03-23 19:58:01.792250 ez_transform-0.1.5/ezt/build/dfmodel/sources.py
--rw-r--r--   0        0        0    10146 2023-03-07 18:27:47.840756 ez_transform-0.1.5/ezt/build/process_model.py
--rw-r--r--   0        0        0     6709 2023-01-29 11:22:46.862566 ez_transform-0.1.5/ezt/build/run.py
--rw-r--r--   0        0        0        0 2022-05-23 16:52:52.412902 ez_transform-0.1.5/ezt/build/sqlmodel/__init__.py
--rw-r--r--   0        0        0      736 2022-10-04 18:55:36.395930 ez_transform-0.1.5/ezt/build/sqlmodel/base.py
--rw-r--r--   0        0        0      747 2022-10-04 18:55:35.775930 ez_transform-0.1.5/ezt/build/sqlmodel/execute.py
--rw-r--r--   0        0        0      913 2022-10-04 18:55:34.225930 ez_transform-0.1.5/ezt/build/sqlmodel/register_sources.py
--rw-r--r--   0        0        0      120 2022-04-30 19:08:55.905237 ez_transform-0.1.5/ezt/include/__init__.py
--rw-r--r--   0        0        0      183 2022-01-16 18:58:28.963643 ez_transform-0.1.5/ezt/include/macros/base_macros.sql
--rw-r--r--   0        0        0       87 2022-07-10 19:50:50.440239 ez_transform-0.1.5/ezt/include/starter_project/.gitignore
--rw-r--r--   0        0        0        0 2022-01-16 18:58:28.963643 ez_transform-0.1.5/ezt/include/starter_project/README.md
--rw-r--r--   0        0        0       51 2022-01-16 18:58:28.973644 ez_transform-0.1.5/ezt/include/starter_project/__init__.py
--rw-r--r--   0        0        0       80 2022-10-18 19:00:43.312774 ez_transform-0.1.5/ezt/include/starter_project/ezt_project.yml
--rw-r--r--   0        0        0        0 2022-07-10 19:09:33.650221 ez_transform-0.1.5/ezt/include/starter_project/models/__init__.py
--rw-r--r--   0        0        0      159 2022-07-10 19:37:48.390233 ez_transform-0.1.5/ezt/include/starter_project/models/models.yml
--rw-r--r--   0        0        0      548 2022-09-21 18:32:12.445083 ez_transform-0.1.5/ezt/include/starter_project/models/my_example.py
--rw-r--r--   0        0        0      123 2023-03-29 16:59:46.559903 ez_transform-0.1.5/ezt/include/starter_project/sources.yml
--rw-r--r--   0        0        0     3030 2023-03-05 14:33:06.570641 ez_transform-0.1.5/ezt/main_cli.py
--rw-r--r--   0        0        0        0 2022-08-29 17:12:36.094392 ez_transform-0.1.5/ezt/util/__init__.py
--rw-r--r--   0        0        0     5796 2023-03-29 16:59:10.869904 ez_transform-0.1.5/ezt/util/config.py
--rw-r--r--   0        0        0     2307 2023-01-26 16:35:43.761722 ez_transform-0.1.5/ezt/util/exceptions.py
--rw-r--r--   0        0        0      258 2022-09-17 16:17:52.589426 ez_transform-0.1.5/ezt/util/fs.py
--rw-r--r--   0        0        0     5251 2023-03-29 17:18:57.559893 ez_transform-0.1.5/ezt/util/helpers.py
--rw-r--r--   0        0        0     1381 2023-01-29 11:17:59.492563 ez_transform-0.1.5/ezt/util/logger.py
--rw-r--r--   0        0        0     1085 2022-09-17 16:14:25.469424 ez_transform-0.1.5/ezt/util/result.py
--rw-r--r--   0        0        0     5100 2022-09-26 19:15:29.734119 ez_transform-0.1.5/ezt/util/validator.py
--rw-r--r--   0        0        0      158 2022-10-18 19:04:00.962773 ez_transform-0.1.5/ezt/util/yaml_schemas/ezt_project_schema.yml
--rw-r--r--   0        0        0      457 2023-03-07 18:27:36.930756 ez_transform-0.1.5/ezt/util/yaml_schemas/ezt_sources_schema.yml
--rw-r--r--   0        0        0     1193 2023-03-29 17:19:38.489893 ez_transform-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 ez_transform-0.1.5/setup.py
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 ez_transform-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-01-16 18:58:28.853644 ez_transform-0.1.6/LICENSE
+-rw-r--r--   0        0        0      910 2022-12-31 09:58:33.729105 ez_transform-0.1.6/README.md
+-rw-r--r--   0        0        0       53 2022-06-04 13:04:51.824066 ez_transform-0.1.6/ezt/MANIFEST.in
+-rw-r--r--   0        0        0      196 2023-04-18 16:15:43.105836 ez_transform-0.1.6/ezt/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-16 18:58:28.883643 ez_transform-0.1.6/ezt/build/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-16 18:58:28.903643 ez_transform-0.1.6/ezt/build/dfmodel/__init__.py
+-rw-r--r--   0        0        0     4878 2023-04-16 13:02:48.593397 ez_transform-0.1.6/ezt/build/dfmodel/merge.py
+-rw-r--r--   0        0        0     3518 2023-03-29 17:18:57.559893 ez_transform-0.1.6/ezt/build/dfmodel/models.py
+-rw-r--r--   0        0        0     2383 2023-03-07 18:27:36.930756 ez_transform-0.1.6/ezt/build/dfmodel/persist_delta.py
+-rw-r--r--   0        0        0      527 2022-11-07 19:50:02.019496 ez_transform-0.1.6/ezt/build/dfmodel/py_model.py
+-rw-r--r--   0        0        0     6518 2023-03-23 19:58:01.792250 ez_transform-0.1.6/ezt/build/dfmodel/sources.py
+-rw-r--r--   0        0        0    10146 2023-04-18 15:47:16.805824 ez_transform-0.1.6/ezt/build/process_model.py
+-rw-r--r--   0        0        0     6896 2023-04-18 15:47:06.555823 ez_transform-0.1.6/ezt/build/run.py
+-rw-r--r--   0        0        0        0 2022-05-23 16:52:52.412902 ez_transform-0.1.6/ezt/build/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      736 2022-10-04 18:55:36.395930 ez_transform-0.1.6/ezt/build/sqlmodel/base.py
+-rw-r--r--   0        0        0      747 2022-10-04 18:55:35.775930 ez_transform-0.1.6/ezt/build/sqlmodel/execute.py
+-rw-r--r--   0        0        0      913 2022-10-04 18:55:34.225930 ez_transform-0.1.6/ezt/build/sqlmodel/register_sources.py
+-rw-r--r--   0        0        0      120 2022-04-30 19:08:55.905237 ez_transform-0.1.6/ezt/include/__init__.py
+-rw-r--r--   0        0        0      183 2022-01-16 18:58:28.963643 ez_transform-0.1.6/ezt/include/macros/base_macros.sql
+-rw-r--r--   0        0        0       87 2022-07-10 19:50:50.440239 ez_transform-0.1.6/ezt/include/starter_project/.gitignore
+-rw-r--r--   0        0        0        0 2022-01-16 18:58:28.963643 ez_transform-0.1.6/ezt/include/starter_project/README.md
+-rw-r--r--   0        0        0       51 2022-01-16 18:58:28.973644 ez_transform-0.1.6/ezt/include/starter_project/__init__.py
+-rw-r--r--   0        0        0       80 2022-10-18 19:00:43.312774 ez_transform-0.1.6/ezt/include/starter_project/ezt_project.yml
+-rw-r--r--   0        0        0        0 2022-07-10 19:09:33.650221 ez_transform-0.1.6/ezt/include/starter_project/models/__init__.py
+-rw-r--r--   0        0        0      159 2022-07-10 19:37:48.390233 ez_transform-0.1.6/ezt/include/starter_project/models/models.yml
+-rw-r--r--   0        0        0      548 2022-09-21 18:32:12.445083 ez_transform-0.1.6/ezt/include/starter_project/models/my_example.py
+-rw-r--r--   0        0        0      123 2023-03-29 16:59:46.559903 ez_transform-0.1.6/ezt/include/starter_project/sources.yml
+-rw-r--r--   0        0        0     3030 2023-03-05 14:33:06.570641 ez_transform-0.1.6/ezt/main_cli.py
+-rw-r--r--   0        0        0        0 2022-08-29 17:12:36.094392 ez_transform-0.1.6/ezt/util/__init__.py
+-rw-r--r--   0        0        0     5796 2023-04-16 14:02:57.693427 ez_transform-0.1.6/ezt/util/config.py
+-rw-r--r--   0        0        0     2307 2023-01-26 16:35:43.761722 ez_transform-0.1.6/ezt/util/exceptions.py
+-rw-r--r--   0        0        0      258 2022-09-17 16:17:52.589426 ez_transform-0.1.6/ezt/util/fs.py
+-rw-r--r--   0        0        0     5251 2023-03-29 17:18:57.559893 ez_transform-0.1.6/ezt/util/helpers.py
+-rw-r--r--   0        0        0     1381 2023-01-29 11:17:59.492563 ez_transform-0.1.6/ezt/util/logger.py
+-rw-r--r--   0        0        0     1085 2023-04-12 17:03:26.696538 ez_transform-0.1.6/ezt/util/result.py
+-rw-r--r--   0        0        0     5100 2022-09-26 19:15:29.734119 ez_transform-0.1.6/ezt/util/validator.py
+-rw-r--r--   0        0        0      158 2022-10-18 19:04:00.962773 ez_transform-0.1.6/ezt/util/yaml_schemas/ezt_project_schema.yml
+-rw-r--r--   0        0        0      457 2023-03-07 18:27:36.930756 ez_transform-0.1.6/ezt/util/yaml_schemas/ezt_sources_schema.yml
+-rw-r--r--   0        0        0     1219 2023-04-18 16:15:43.115836 ez_transform-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 ez_transform-0.1.6/setup.py
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 ez_transform-0.1.6/PKG-INFO
```

### Comparing `ez_transform-0.1.5/LICENSE` & `ez_transform-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/README.md` & `ez_transform-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/dfmodel/merge.py` & `ez_transform-0.1.6/ezt/build/dfmodel/merge.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/dfmodel/models.py` & `ez_transform-0.1.6/ezt/build/dfmodel/models.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/dfmodel/persist_delta.py` & `ez_transform-0.1.6/ezt/build/dfmodel/persist_delta.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/dfmodel/py_model.py` & `ez_transform-0.1.6/ezt/build/dfmodel/py_model.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/dfmodel/sources.py` & `ez_transform-0.1.6/ezt/build/dfmodel/sources.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/process_model.py` & `ez_transform-0.1.6/ezt/build/process_model.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/run.py` & `ez_transform-0.1.6/ezt/build/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import traceback
-from multiprocessing import Process, Queue
+import multiprocess as mp
+from multiprocess import Process, Queue
 
 from ezt.build.process_model import process_model
 from ezt.util.config import Config
 from ezt.util.logger import EztLogger
 from ezt.util.result import ExecutionResult, ModelResult
 from rich.console import Console
+from sys import platform
 
 
 class Runner:
+    """Class that is handling one ezt run invokation."""
+
     def __init__(self, config: Config):
         self.config = config
         self.logger = EztLogger(
             logs_destination=config.project["logs_destination"]
             if "logs_destination" in config.project
             else None
         )
 
     @property
     def model_order(self):
         return list(self.config.execution_order.static_order())
 
-    def Execute(self, model_name, model_group) -> ExecutionResult:
-
+    def Execute(self, model_name: str = None, model_group: str = None) -> ExecutionResult:
+        """Executes the models in a parallell fashion."""
         execution_result = ExecutionResult()
         console = Console()
 
         # log models to be processed
         try:
             self.logger.log_info(
                 f"Found {len(self.model_order)} models to be processed: {self.model_order}"
```

### Comparing `ez_transform-0.1.5/ezt/build/sqlmodel/base.py` & `ez_transform-0.1.6/ezt/build/sqlmodel/base.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/sqlmodel/execute.py` & `ez_transform-0.1.6/ezt/build/sqlmodel/execute.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/build/sqlmodel/register_sources.py` & `ez_transform-0.1.6/ezt/build/sqlmodel/register_sources.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/include/starter_project/models/my_example.py` & `ez_transform-0.1.6/ezt/include/starter_project/models/my_example.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/main_cli.py` & `ez_transform-0.1.6/ezt/main_cli.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/config.py` & `ez_transform-0.1.6/ezt/util/config.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/exceptions.py` & `ez_transform-0.1.6/ezt/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/helpers.py` & `ez_transform-0.1.6/ezt/util/helpers.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/logger.py` & `ez_transform-0.1.6/ezt/util/logger.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/result.py` & `ez_transform-0.1.6/ezt/util/result.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/ezt/util/validator.py` & `ez_transform-0.1.6/ezt/util/validator.py`

 * *Files identical despite different names*

### Comparing `ez_transform-0.1.5/pyproject.toml` & `ez_transform-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ez-transform"
-version = "0.1.5"
+version = "0.1.6"
 description = "Analytics engineering for data lakes."
 authors = ["John Kaustinen <jokausti@gmail.com>"]
 license = 'Apache-2.0'
 documentation = 'https://ez-transform.github.io/ezt-core/'
 repository = 'https://github.com/ez-transform/ezt-core'
 readme = 'README.md'
 packages = [
@@ -21,14 +21,15 @@
 deltalake = "^0.7.0"
 graphlib-backport = "^1.0.3"
 rich = "^12.2.0"
 rich-click = "^1.3.0"
 jsonschema = "^4.14.0"
 pyarrow = "11.0.0"
 adlfs = "^2023.1.0"
+multiprocess = "^0.70.14"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.2.1"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 isort = "^5.10.1"
 dprint = "^0.1.0"
```

### Comparing `ez_transform-0.1.5/setup.py` & `ez_transform-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,26 +18,27 @@
 ['Jinja2>=3.0.3,<4.0.0',
  'PyYAML>=6.0,<7.0',
  'adlfs>=2023.1.0,<2024.0.0',
  'click>=8.0.3,<9.0.0',
  'deltalake>=0.7.0,<0.8.0',
  'graphlib-backport>=1.0.3,<2.0.0',
  'jsonschema>=4.14.0,<5.0.0',
+ 'multiprocess>=0.70.14,<0.71.0',
  'polars>=0.15.17,<0.16.0',
  'pyarrow==11.0.0',
  'rich-click>=1.3.0,<2.0.0',
  'rich>=12.2.0,<13.0.0',
  's3fs>=2022.11.0,<2023.0.0']
 
 entry_points = \
 {'console_scripts': ['ezt = ezt.main_cli:ezt']}
 
 setup_kwargs = {
     'name': 'ez-transform',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Analytics engineering for data lakes.',
     'long_description': '💥 ez-transform (Ezt)\n================\n\nAnalytics Engineering for Data Lakes powered by\n[polars](https://github.com/pola-rs/polars),\n[arrow](https://github.com/apache/arrow) and\n[delta-rs](https://github.com/delta-io/delta-rs).\n\n👉 Installation\n------------\n\nWe recommend first setting up a Python virtual environment and activating it.\n\n```bash\n$ python -m venv .venv\n```\n\n```bash\n$ source .venv/bin/activate\n```\n\nAnd then install Ezt with pip into your virtual environment.\n\n```bash\n$ pip install ez-transform\n```\n\n👉 Getting started\n------------\n\nYou can test out Ezt by creating a project from the command line.\n\n```bash\n$ ezt init myproject && cd myproject\n```\n\nNow you have created a project and can use your IDE of choice to start\ndeveloping your data models. 🥳\n\nCheck out the documentation at <https://ez-transform.github.io/ezt-core/> to learn more about how to develop data models with Ezt.\n',
     'author': 'John Kaustinen',
     'author_email': 'jokausti@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ez-transform/ezt-core',
```

### Comparing `ez_transform-0.1.5/PKG-INFO` & `ez_transform-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-transform
-Version: 0.1.5
+Version: 0.1.6
 Summary: Analytics engineering for data lakes.
 Home-page: https://github.com/ez-transform/ezt-core
 License: Apache-2.0
 Author: John Kaustinen
 Author-email: jokausti@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: adlfs (>=2023.1.0,<2024.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: deltalake (>=0.7.0,<0.8.0)
 Requires-Dist: graphlib-backport (>=1.0.3,<2.0.0)
 Requires-Dist: jsonschema (>=4.14.0,<5.0.0)
+Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: polars (>=0.15.17,<0.16.0)
 Requires-Dist: pyarrow (==11.0.0)
 Requires-Dist: rich (>=12.2.0,<13.0.0)
 Requires-Dist: rich-click (>=1.3.0,<2.0.0)
 Requires-Dist: s3fs (>=2022.11.0,<2023.0.0)
 Project-URL: Documentation, https://ez-transform.github.io/ezt-core/
 Project-URL: Repository, https://github.com/ez-transform/ezt-core
```

