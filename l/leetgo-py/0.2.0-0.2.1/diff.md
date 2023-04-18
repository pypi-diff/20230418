# Comparing `tmp/leetgo-py-0.2.0.tar.gz` & `tmp/leetgo-py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetgo-py-0.2.0.tar", max compression
+gzip compressed data, was "leetgo-py-0.2.1.tar", max compression
```

## Comparing `leetgo-py-0.2.0.tar` & `leetgo-py-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      515 2023-04-18 12:19:35.119197 leetgo-py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-04-18 08:54:40.808034 leetgo-py-0.2.0/src/leetgo_py/__init__.py
--rw-r--r--   0        0        0      735 2023-04-18 12:08:59.473446 leetgo-py-0.2.0/src/leetgo_py/list.py
--rw-r--r--   0        0        0     1420 2023-04-18 11:53:02.522227 leetgo-py-0.2.0/src/leetgo_py/parse.py
--rw-r--r--   0        0        0     1224 2023-04-18 12:15:38.689355 leetgo-py-0.2.0/src/leetgo_py/tree.py
--rw-r--r--   0        0        0      179 2023-04-18 11:23:24.331859 leetgo-py-0.2.0/src/leetgo_py/utils.py
--rw-r--r--   0        0        0      626 2023-04-18 12:19:38.824016 leetgo-py-0.2.0/setup.py
--rw-r--r--   0        0        0      665 2023-04-18 12:19:38.824272 leetgo-py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-04-18 12:55:08.792499 leetgo-py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-04-18 12:31:03.321405 leetgo-py-0.2.1/src/leetgo_py/__init__.py
+-rw-r--r--   0        0        0      735 2023-04-18 12:08:59.473446 leetgo-py-0.2.1/src/leetgo_py/list.py
+-rw-r--r--   0        0        0     1415 2023-04-18 12:49:05.492076 leetgo-py-0.2.1/src/leetgo_py/parse.py
+-rw-r--r--   0        0        0     1224 2023-04-18 12:15:38.689355 leetgo-py-0.2.1/src/leetgo_py/tree.py
+-rw-r--r--   0        0        0      179 2023-04-18 11:23:24.331859 leetgo-py-0.2.1/src/leetgo_py/utils.py
+-rw-r--r--   0        0        0      626 2023-04-18 12:55:17.343622 leetgo-py-0.2.1/setup.py
+-rw-r--r--   0        0        0      665 2023-04-18 12:55:17.343870 leetgo-py-0.2.1/PKG-INFO
```

### Comparing `leetgo-py-0.2.0/pyproject.toml` & `leetgo-py-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "leetgo-py"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python test utils for leetgo"
 authors = ["j178 <10510431+j178@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/j178/leetgo"
 repository = "https://github.com/j178/leetgo"
 keywords = ["leetcode"]
```

### Comparing `leetgo-py-0.2.0/src/leetgo_py/list.py` & `leetgo-py-0.2.1/src/leetgo_py/list.py`

 * *Files identical despite different names*

### Comparing `leetgo-py-0.2.0/src/leetgo_py/parse.py` & `leetgo-py-0.2.1/src/leetgo_py/parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 from typing import Any, List
 
-from src.leetgo_py import ListNode, TreeNode
+from . import ListNode, TreeNode
 
 
 def split_array(s: str) -> List[str]:
     s = s.strip()
     if len(s) <= 1 or s[0] != "[" or s[-1] != "]":
         raise Exception("Invalid array: " + s)
 
     splits = json.loads(s)
-    res = [str(split) for split in splits]
+    res = [json.dumps(split) for split in splits]
     return res
 
 
 def serialize(val: Any) -> str:
     if isinstance(val, int):
         return str(val)
     elif isinstance(val, float):
```

### Comparing `leetgo-py-0.2.0/src/leetgo_py/tree.py` & `leetgo-py-0.2.1/src/leetgo_py/tree.py`

 * *Files identical despite different names*

### Comparing `leetgo-py-0.2.0/setup.py` & `leetgo-py-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['leetgo_py']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'leetgo-py',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python test utils for leetgo',
     'long_description': None,
     'author': 'j178',
     'author_email': '10510431+j178@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/j178/leetgo',
```

### Comparing `leetgo-py-0.2.0/PKG-INFO` & `leetgo-py-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetgo-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python test utils for leetgo
 Home-page: https://github.com/j178/leetgo
 License: MIT
 Keywords: leetcode
 Author: j178
 Author-email: 10510431+j178@users.noreply.github.com
 Requires-Python: >=3.6,<4.0
```

