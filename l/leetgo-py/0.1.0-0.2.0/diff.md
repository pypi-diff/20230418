# Comparing `tmp/leetgo-py-0.1.0.tar.gz` & `tmp/leetgo-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetgo-py-0.1.0.tar", max compression
+gzip compressed data, was "leetgo-py-0.2.0.tar", max compression
```

## Comparing `leetgo-py-0.1.0.tar` & `leetgo-py-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      514 2023-04-18 11:12:17.147022 leetgo-py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-04-18 08:54:40.808034 leetgo-py-0.1.0/src/leetgo_py/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 08:25:15.903854 leetgo-py-0.1.0/src/leetgo_py/list.py
--rw-r--r--   0        0        0        0 2023-04-18 08:25:07.733593 leetgo-py-0.1.0/src/leetgo_py/parse.py
--rw-r--r--   0        0        0        0 2023-04-18 08:25:27.461298 leetgo-py-0.1.0/src/leetgo_py/tree.py
--rw-r--r--   0        0        0        0 2023-04-18 08:26:34.992550 leetgo-py-0.1.0/src/leetgo_py/utils.py
--rw-r--r--   0        0        0      626 2023-04-18 11:12:20.842162 leetgo-py-0.1.0/setup.py
--rw-r--r--   0        0        0      665 2023-04-18 11:12:20.842454 leetgo-py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-04-18 12:19:35.119197 leetgo-py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-04-18 08:54:40.808034 leetgo-py-0.2.0/src/leetgo_py/__init__.py
+-rw-r--r--   0        0        0      735 2023-04-18 12:08:59.473446 leetgo-py-0.2.0/src/leetgo_py/list.py
+-rw-r--r--   0        0        0     1420 2023-04-18 11:53:02.522227 leetgo-py-0.2.0/src/leetgo_py/parse.py
+-rw-r--r--   0        0        0     1224 2023-04-18 12:15:38.689355 leetgo-py-0.2.0/src/leetgo_py/tree.py
+-rw-r--r--   0        0        0      179 2023-04-18 11:23:24.331859 leetgo-py-0.2.0/src/leetgo_py/utils.py
+-rw-r--r--   0        0        0      626 2023-04-18 12:19:38.824016 leetgo-py-0.2.0/setup.py
+-rw-r--r--   0        0        0      665 2023-04-18 12:19:38.824272 leetgo-py-0.2.0/PKG-INFO
```

### Comparing `leetgo-py-0.1.0/pyproject.toml` & `leetgo-py-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 [tool.poetry]
 name = "leetgo-py"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python test utils for leetgo"
 authors = ["j178 <10510431+j178@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/j178/leetgo"
 repository = "https://github.com/j178/leetgo"
 keywords = ["leetcode"]
+
 packages = [
     { include = "leetgo_py", from = "src"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `leetgo-py-0.1.0/setup.py` & `leetgo-py-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['leetgo_py']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'leetgo-py',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Python test utils for leetgo',
     'long_description': None,
     'author': 'j178',
     'author_email': '10510431+j178@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/j178/leetgo',
```

### Comparing `leetgo-py-0.1.0/PKG-INFO` & `leetgo-py-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetgo-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python test utils for leetgo
 Home-page: https://github.com/j178/leetgo
 License: MIT
 Keywords: leetcode
 Author: j178
 Author-email: 10510431+j178@users.noreply.github.com
 Requires-Python: >=3.6,<4.0
```

