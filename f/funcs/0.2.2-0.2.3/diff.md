# Comparing `tmp/funcs-0.2.2.tar.gz` & `tmp/funcs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.2.2.tar", max compression
+gzip compressed data, was "funcs-0.2.3.tar", max compression
```

## Comparing `funcs-0.2.2.tar` & `funcs-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1092 2023-04-17 13:12:16.876319 funcs-0.2.2/LICENSE
--rw-r--r--   0        0        0     2872 2023-04-17 13:12:16.876319 funcs-0.2.2/README.md
--rw-r--r--   0        0        0     1664 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/application.py
--rw-r--r--   0        0        0      563 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/callers.py
--rw-r--r--   0        0        0     4121 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/composition.py
--rw-r--r--   0        0        0      431 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/decorators.py
--rw-r--r--   0        0        0     3595 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/flow.py
--rw-r--r--   0        0        0      899 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/getters.py
--rw-r--r--   0        0        0      264 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/py.typed
--rw-r--r--   0        0        0      492 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/reduction.py
--rw-r--r--   0        0        0      475 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/types.py
--rw-r--r--   0        0        0     2878 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/typing.py
--rw-r--r--   0        0        0     1369 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/unpacking.py
--rw-r--r--   0        0        0     3022 2023-04-17 13:12:16.880319 funcs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-18 12:00:58.059008 funcs-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-18 12:00:58.059008 funcs-0.2.3/README.md
+-rw-r--r--   0        0        0     1664 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/application.py
+-rw-r--r--   0        0        0      563 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/callers.py
+-rw-r--r--   0        0        0     4121 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/composition.py
+-rw-r--r--   0        0        0      431 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/decorators.py
+-rw-r--r--   0        0        0     3595 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/flow.py
+-rw-r--r--   0        0        0      899 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/getters.py
+-rw-r--r--   0        0        0      264 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/py.typed
+-rw-r--r--   0        0        0      492 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/reduction.py
+-rw-r--r--   0        0        0      475 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/types.py
+-rw-r--r--   0        0        0     3324 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/typing.py
+-rw-r--r--   0        0        0     1369 2023-04-18 12:00:58.063007 funcs-0.2.3/funcs/unpacking.py
+-rw-r--r--   0        0        0     3022 2023-04-18 12:00:58.063007 funcs-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.3/PKG-INFO
```

### Comparing `funcs-0.2.2/LICENSE` & `funcs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/README.md` & `funcs-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.2"
+funcs = "^0.2.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.2.2/funcs/__init__.py` & `funcs-0.2.3/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.2.2/funcs/application.py` & `funcs-0.2.3/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/funcs/callers.py` & `funcs-0.2.3/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/funcs/composition.py` & `funcs-0.2.3/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/funcs/flow.py` & `funcs-0.2.3/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/funcs/functions.py` & `funcs-0.2.3/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/funcs/unpacking.py` & `funcs-0.2.3/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.2/pyproject.toml` & `funcs-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.2.2"
+version = "0.2.3"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -126,15 +126,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.2.2"
+version = "0.2.3"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.2.2/PKG-INFO` & `funcs-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.2"
+funcs = "^0.2.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

