# Comparing `tmp/ntfy_lite-1.0.11.tar.gz` & `tmp/ntfy_lite-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntfy_lite-1.0.11.tar", max compression
+gzip compressed data, was "ntfy_lite-1.0.12.tar", max compression
```

## Comparing `ntfy_lite-1.0.11.tar` & `ntfy_lite-1.0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1552 2023-04-18 13:18:09.708251 ntfy_lite-1.0.11/LICENSE
--rw-r--r--   0        0        0     1445 2023-04-18 13:18:09.708251 ntfy_lite-1.0.11/README.md
--rw-r--r--   0        0        0      275 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/__init__.py
--rw-r--r--   0        0        0     3051 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/actions.py
--rw-r--r--   0        0        0      703 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/defaults.py
--rw-r--r--   0        0        0     3845 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/demo_logging.py
--rw-r--r--   0        0        0     2189 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/demo_push.py
--rw-r--r--   0        0        0      407 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/error.py
--rw-r--r--   0        0        0     5311 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/handler.py
--rw-r--r--   0        0        0     6692 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/ntfy.py
--rw-r--r--   0        0        0     1185 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/ntfy2logging.py
--rw-r--r--   0        0        0        0 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/py.typed
--rw-r--r--   0        0        0      565 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/utils.py
--rw-r--r--   0        0        0       76 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/version.py
--rw-r--r--   0        0        0      946 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/pyproject.toml
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 ntfy_lite-1.0.11/PKG-INFO
+-rw-r--r--   0        0        0     1552 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/LICENSE
+-rw-r--r--   0        0        0     1356 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/README.md
+-rw-r--r--   0        0        0      275 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/__init__.py
+-rw-r--r--   0        0        0     3051 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/actions.py
+-rw-r--r--   0        0        0      703 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/defaults.py
+-rw-r--r--   0        0        0     3845 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/demo_logging.py
+-rw-r--r--   0        0        0     2189 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/demo_push.py
+-rw-r--r--   0        0        0      407 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/error.py
+-rw-r--r--   0        0        0     5311 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/handler.py
+-rw-r--r--   0        0        0     6692 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/ntfy.py
+-rw-r--r--   0        0        0     1185 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/ntfy2logging.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/py.typed
+-rw-r--r--   0        0        0      565 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/utils.py
+-rw-r--r--   0        0        0       76 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/version.py
+-rw-r--r--   0        0        0      946 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 ntfy_lite-1.0.12/PKG-INFO
```

### Comparing `ntfy_lite-1.0.11/LICENSE` & `ntfy_lite-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/README.md` & `ntfy_lite-1.0.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)
-![mypy](https://github.com/MPI-IS/ntfy_lite/actions/workflows/python_mypy.yml/badge.svg)
 [![documentation](https://github.com/MPI-IS/ntfy_lite/actions/workflows/mkdocs.yaml/badge.svg)](https://mpi-is.github.io/ntfy_lite/)
 [![PyPI](https://github.com/MPI-IS/ntfy_lite/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/ntfy-lite/)
 
 
 
 # NTFY LITE
```

### Comparing `ntfy_lite-1.0.11/ntfy_lite/actions.py` & `ntfy_lite-1.0.12/ntfy_lite/actions.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/defaults.py` & `ntfy_lite-1.0.12/ntfy_lite/defaults.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/demo_logging.py` & `ntfy_lite-1.0.12/ntfy_lite/demo_logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/demo_push.py` & `ntfy_lite-1.0.12/ntfy_lite/demo_push.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/handler.py` & `ntfy_lite-1.0.12/ntfy_lite/handler.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/ntfy.py` & `ntfy_lite-1.0.12/ntfy_lite/ntfy.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/ntfy2logging.py` & `ntfy_lite-1.0.12/ntfy_lite/ntfy2logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/ntfy_lite/utils.py` & `ntfy_lite-1.0.12/ntfy_lite/utils.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.11/pyproject.toml` & `ntfy_lite-1.0.12/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntfy-lite"
-version = "1.0.11"
+version = "1.0.12"
 description = "minimalistic python API for sending ntfy notifications"
 authors = ["Vincent Berenz <vberenz@tuebingen.mpg.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "ntfy_lite"}]
 
 [[tool.poetry.source]]
```

### Comparing `ntfy_lite-1.0.11/PKG-INFO` & `ntfy_lite-1.0.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntfy-lite
-Version: 1.0.11
+Version: 1.0.12
 Summary: minimalistic python API for sending ntfy notifications
 License: BSD-3-Clause
 Author: Vincent Berenz
 Author-email: vberenz@tuebingen.mpg.de
 Requires-Python: >3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 ![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)
-![mypy](https://github.com/MPI-IS/ntfy_lite/actions/workflows/python_mypy.yml/badge.svg)
 [![documentation](https://github.com/MPI-IS/ntfy_lite/actions/workflows/mkdocs.yaml/badge.svg)](https://mpi-is.github.io/ntfy_lite/)
 [![PyPI](https://github.com/MPI-IS/ntfy_lite/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/ntfy-lite/)
 
 
 
 # NTFY LITE
```

