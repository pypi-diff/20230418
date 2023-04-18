# Comparing `tmp/ntfy_lite-1.0.12.tar.gz` & `tmp/ntfy_lite-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntfy_lite-1.0.12.tar", max compression
+gzip compressed data, was "ntfy_lite-1.0.14.tar", max compression
```

## Comparing `ntfy_lite-1.0.12.tar` & `ntfy_lite-1.0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1552 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/LICENSE
--rw-r--r--   0        0        0     1356 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/README.md
--rw-r--r--   0        0        0      275 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/__init__.py
--rw-r--r--   0        0        0     3051 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/actions.py
--rw-r--r--   0        0        0      703 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/defaults.py
--rw-r--r--   0        0        0     3845 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/demo_logging.py
--rw-r--r--   0        0        0     2189 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/demo_push.py
--rw-r--r--   0        0        0      407 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/error.py
--rw-r--r--   0        0        0     5311 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/handler.py
--rw-r--r--   0        0        0     6692 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/ntfy.py
--rw-r--r--   0        0        0     1185 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/ntfy2logging.py
--rw-r--r--   0        0        0        0 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/py.typed
--rw-r--r--   0        0        0      565 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/utils.py
--rw-r--r--   0        0        0       76 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/ntfy_lite/version.py
--rw-r--r--   0        0        0      946 2023-04-18 14:44:41.243518 ntfy_lite-1.0.12/pyproject.toml
--rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 ntfy_lite-1.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1552 2023-04-18 15:25:31.462494 ntfy_lite-1.0.14/LICENSE
+-rw-r--r--   0        0        0     1356 2023-04-18 15:25:31.462494 ntfy_lite-1.0.14/README.md
+-rw-r--r--   0        0        0      275 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/__init__.py
+-rw-r--r--   0        0        0     3051 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/actions.py
+-rw-r--r--   0        0        0      703 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/defaults.py
+-rw-r--r--   0        0        0     3845 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/demo_logging.py
+-rw-r--r--   0        0        0     2189 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/demo_push.py
+-rw-r--r--   0        0        0      407 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/error.py
+-rw-r--r--   0        0        0     5311 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/handler.py
+-rw-r--r--   0        0        0     6692 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/ntfy.py
+-rw-r--r--   0        0        0     1185 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/ntfy2logging.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/py.typed
+-rw-r--r--   0        0        0      565 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/utils.py
+-rw-r--r--   0        0        0       76 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/ntfy_lite/version.py
+-rw-r--r--   0        0        0      946 2023-04-18 15:25:31.466495 ntfy_lite-1.0.14/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 ntfy_lite-1.0.14/PKG-INFO
```

### Comparing `ntfy_lite-1.0.12/LICENSE` & `ntfy_lite-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/README.md` & `ntfy_lite-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/actions.py` & `ntfy_lite-1.0.14/ntfy_lite/actions.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/defaults.py` & `ntfy_lite-1.0.14/ntfy_lite/defaults.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/demo_logging.py` & `ntfy_lite-1.0.14/ntfy_lite/demo_logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/demo_push.py` & `ntfy_lite-1.0.14/ntfy_lite/demo_push.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/handler.py` & `ntfy_lite-1.0.14/ntfy_lite/handler.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/ntfy.py` & `ntfy_lite-1.0.14/ntfy_lite/ntfy.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/ntfy2logging.py` & `ntfy_lite-1.0.14/ntfy_lite/ntfy2logging.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/ntfy_lite/utils.py` & `ntfy_lite-1.0.14/ntfy_lite/utils.py`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.12/pyproject.toml` & `ntfy_lite-1.0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntfy-lite"
-version = "1.0.12"
+version = "1.0.14"
 description = "minimalistic python API for sending ntfy notifications"
 authors = ["Vincent Berenz <vberenz@tuebingen.mpg.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "ntfy_lite"}]
 
 [[tool.poetry.source]]
```

### Comparing `ntfy_lite-1.0.12/PKG-INFO` & `ntfy_lite-1.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntfy-lite
-Version: 1.0.12
+Version: 1.0.14
 Summary: minimalistic python API for sending ntfy notifications
 License: BSD-3-Clause
 Author: Vincent Berenz
 Author-email: vberenz@tuebingen.mpg.de
 Requires-Python: >3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

