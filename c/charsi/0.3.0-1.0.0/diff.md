# Comparing `tmp/charsi-0.3.0.tar.gz` & `tmp/charsi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-0.3.0.tar", max compression
+gzip compressed data, was "charsi-1.0.0.tar", max compression
```

## Comparing `charsi-0.3.0.tar` & `charsi-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      894 2023-04-18 03:54:20.060629 charsi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2428 2023-04-18 03:53:46.904216 charsi-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-0.3.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-0.3.0/src/charsi/__main__.py
--rw-r--r--   0        0        0       66 2023-04-17 22:14:26.163984 charsi-0.3.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      612 2023-04-17 23:10:32.327874 charsi-0.3.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0     2029 2023-04-18 03:42:15.519526 charsi-0.3.0/src/charsi/instruction.py
--rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-0.3.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-0.3.0/src/charsi/strings.py
--rw-r--r--   0        0        0      206 2023-04-17 21:30:18.257269 charsi-0.3.0/src/charsi/utils.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 charsi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      894 2023-04-18 11:21:55.689366 charsi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2773 2023-04-18 11:19:28.428196 charsi-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.0.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.0.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.0.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      612 2023-04-17 23:10:32.327874 charsi-1.0.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      400 2023-04-18 11:03:01.586161 charsi-1.0.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2029 2023-04-18 03:42:15.519526 charsi-1.0.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.0.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-1.0.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.0.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      206 2023-04-17 21:30:18.257269 charsi-1.0.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 charsi-1.0.0/PKG-INFO
```

### Comparing `charsi-0.3.0/pyproject.toml` & `charsi-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "0.3.0"
+version = "1.0.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
```

### Comparing `charsi-0.3.0/README.md` & `charsi-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -87,14 +87,37 @@
 
 Build a string table with recipe:
 
 ```
 charsi build --recipe-file=/path/to/recipe path/to/stringtable
 ```
 
+Build string tables with manifest files:
+
+```
+charsi build-manfiest path/to/manifest
+```
+
+### Manifest
+
+In JSON format like:
+
+```json
+[
+    {
+        "input": "/path/to/stringtable",
+        "output": "/path/to/output",
+        "recipes": [
+            "/path/to/recipe1",
+            "/path/to/recipe2",
+            "..."
+        ]
+    }
+]
+```
 
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

### Comparing `charsi-0.3.0/src/charsi/commands/build.py` & `charsi-1.0.0/src/charsi/commands/build.py`

 * *Files identical despite different names*

### Comparing `charsi-0.3.0/src/charsi/instruction.py` & `charsi-1.0.0/src/charsi/instruction.py`

 * *Files identical despite different names*

### Comparing `charsi-0.3.0/src/charsi/recipe.py` & `charsi-1.0.0/src/charsi/recipe.py`

 * *Files identical despite different names*

### Comparing `charsi-0.3.0/src/charsi/strings.py` & `charsi-1.0.0/src/charsi/strings.py`

 * *Files identical despite different names*

### Comparing `charsi-0.3.0/PKG-INFO` & `charsi-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 0.3.0
+Version: 1.0.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -105,14 +105,37 @@
 
 Build a string table with recipe:
 
 ```
 charsi build --recipe-file=/path/to/recipe path/to/stringtable
 ```
 
+Build string tables with manifest files:
+
+```
+charsi build-manfiest path/to/manifest
+```
+
+### Manifest
+
+In JSON format like:
+
+```json
+[
+    {
+        "input": "/path/to/stringtable",
+        "output": "/path/to/output",
+        "recipes": [
+            "/path/to/recipe1",
+            "/path/to/recipe2",
+            "..."
+        ]
+    }
+]
+```
 
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

