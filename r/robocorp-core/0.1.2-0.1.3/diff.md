# Comparing `tmp/robocorp_core-0.1.2.tar.gz` & `tmp/robocorp_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_core-0.1.2.tar", max compression
+gzip compressed data, was "robocorp_core-0.1.3.tar", max compression
```

## Comparing `robocorp_core-0.1.2.tar` & `robocorp_core-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      403 2023-03-31 07:13:28.254599 robocorp_core-0.1.2/README.md
--rw-r--r--   0        0        0      608 2023-04-06 08:21:01.059993 robocorp_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       29 2023-03-31 07:13:28.255292 robocorp_core-0.1.2/src/robo/__init__.py
--rw-r--r--   0        0        0       69 2023-03-31 07:13:28.255363 robocorp_core-0.1.2/src/robo/__main__.py
--rw-r--r--   0        0        0     3017 2023-03-31 07:13:28.255498 robocorp_core-0.1.2/src/robo/_argdispatch.py
--rw-r--r--   0        0        0     1327 2023-03-31 07:13:28.255578 robocorp_core-0.1.2/src/robo/_callback.py
--rw-r--r--   0        0        0     4961 2023-03-31 07:13:28.255670 robocorp_core-0.1.2/src/robo/_collect_tasks.py
--rw-r--r--   0        0        0      160 2023-03-31 07:13:28.255746 robocorp_core-0.1.2/src/robo/_exceptions.py
--rw-r--r--   0        0        0      607 2023-03-31 07:13:28.255825 robocorp_core-0.1.2/src/robo/_hooks.py
--rw-r--r--   0        0        0     1432 2023-03-31 07:13:28.255911 robocorp_core-0.1.2/src/robo/_logging_setup.py
--rw-r--r--   0        0        0     1599 2023-03-31 07:13:28.256039 robocorp_core-0.1.2/src/robo/_protocols.py
--rw-r--r--   0        0        0      904 2023-03-31 07:13:28.256162 robocorp_core-0.1.2/src/robo/_task.py
--rw-r--r--   0        0        0     4455 2023-04-06 08:13:22.494349 robocorp_core-0.1.2/src/robo/cli.py
--rw-r--r--   0        0        0       95 2023-03-31 07:13:28.256384 robocorp_core-0.1.2/src/robo/decorators.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 robocorp_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      403 2023-03-31 07:13:28.254599 robocorp_core-0.1.3/README.md
+-rw-r--r--   0        0        0      608 2023-04-18 07:59:34.472954 robocorp_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-03-31 07:13:28.255292 robocorp_core-0.1.3/src/robo/__init__.py
+-rw-r--r--   0        0        0       69 2023-03-31 07:13:28.255363 robocorp_core-0.1.3/src/robo/__main__.py
+-rw-r--r--   0        0        0     3462 2023-04-18 07:51:15.335899 robocorp_core-0.1.3/src/robo/_argdispatch.py
+-rw-r--r--   0        0        0     1327 2023-03-31 07:13:28.255578 robocorp_core-0.1.3/src/robo/_callback.py
+-rw-r--r--   0        0        0     4961 2023-03-31 07:13:28.255670 robocorp_core-0.1.3/src/robo/_collect_tasks.py
+-rw-r--r--   0        0        0      160 2023-03-31 07:13:28.255746 robocorp_core-0.1.3/src/robo/_exceptions.py
+-rw-r--r--   0        0        0      607 2023-04-18 07:51:15.336647 robocorp_core-0.1.3/src/robo/_hooks.py
+-rw-r--r--   0        0        0     5051 2023-04-18 07:51:19.127737 robocorp_core-0.1.3/src/robo/_log_auto_setup.py
+-rw-r--r--   0        0        0     2323 2023-04-18 07:51:19.127811 robocorp_core-0.1.3/src/robo/_log_output_setup.py
+-rw-r--r--   0        0        0     1699 2023-04-18 07:51:15.337039 robocorp_core-0.1.3/src/robo/_protocols.py
+-rw-r--r--   0        0        0      903 2023-04-11 07:17:37.821464 robocorp_core-0.1.3/src/robo/_task.py
+-rw-r--r--   0        0        0     5474 2023-04-18 07:51:19.127957 robocorp_core-0.1.3/src/robo/cli.py
+-rw-r--r--   0        0        0      578 2023-04-18 07:51:15.337418 robocorp_core-0.1.3/src/robo/decorators.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 robocorp_core-0.1.3/PKG-INFO
```

### Comparing `robocorp_core-0.1.2/pyproject.toml` & `robocorp_core-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "robocorp-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "The automation framework for Python"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robo", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-logging = "^0.0.1"
+robocorp-logging = "0.0.8"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ruff = "^0.0.255"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-xdist = "^3.2.1"
```

### Comparing `robocorp_core-0.1.2/src/robo/_argdispatch.py` & `robocorp_core-0.1.3/src/robo/_argdispatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -62,14 +62,27 @@
         run_parser.add_argument(
             "-o",
             "--output-dir",
             dest="output_dir",
             help="The directory where the logging output files will be stored.",
             default="./output",
         )
+        run_parser.add_argument(
+            "--max-log-files",
+            dest="max_log_files",
+            type=int,
+            help="The maximum number of output files to store the logs.",
+            default=5,
+        )
+        run_parser.add_argument(
+            "--max-log-file-size",
+            dest="max_log_file_size",
+            help="The maximum size for the log files (i.e.: 1MB, 500kb).",
+            default="1MB",
+        )
 
         # List tasks
         list_parser = subparsers.add_parser(
             "list",
             help="Provides output to stdout with json contents of the tasks available.",
         )
         list_parser.add_argument(
```

### Comparing `robocorp_core-0.1.2/src/robo/_callback.py` & `robocorp_core-0.1.3/src/robo/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_core-0.1.2/src/robo/_collect_tasks.py` & `robocorp_core-0.1.3/src/robo/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_core-0.1.2/src/robo/_hooks.py` & `robocorp_core-0.1.3/src/robo/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_core-0.1.2/src/robo/_protocols.py` & `robocorp_core-0.1.3/src/robo/_protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 
     Mypy should complain if `self` is not implementing the IExpectedProtocol.
     """
     return x
 
 
 class Status:
-    NOT_RUN = "NOT RUN"
+    NOT_RUN = "NOT_RUN"  # Initial status for a task which is not run.
     PASS = "PASS"
     ERROR = "ERROR"
+    FAIL = "FAIL"
+    INFO = "INFO"
+    WARN = "WARN"
 
 
 class ITask(typing.Protocol):
-    package_name: str
+    module_name: str
     filename: str
     method: typing.Callable
 
     status: str
     message: str
 
     @property
```

### Comparing `robocorp_core-0.1.2/src/robo/_task.py` & `robocorp_core-0.1.3/src/robo/_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 from types import ModuleType
 from robo._protocols import Status
 
 
 class Task:
     def __init__(self, module: ModuleType, method: typing.Callable):
-        self.package_name = module.__name__
+        self.module_name = module.__name__
         self.filename = module.__file__ or "<filename unavailable>"
         self.method = method
         self.status = Status.NOT_RUN
         self.message = ""
 
     @property
     def name(self):
```

### Comparing `robocorp_core-0.1.2/PKG-INFO` & `robocorp_core-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: The automation framework for Python
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: robocorp-logging (>=0.0.1,<0.0.2)
+Requires-Dist: robocorp-logging (==0.0.8)
 Description-Content-Type: text/markdown
 
 # Robo
 
 Robo is a python framework to ease RPA development in Python.
```

