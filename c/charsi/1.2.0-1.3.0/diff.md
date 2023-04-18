# Comparing `tmp/charsi-1.2.0.tar.gz` & `tmp/charsi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-1.2.0.tar", max compression
+gzip compressed data, was "charsi-1.3.0.tar", max compression
```

## Comparing `charsi-1.2.0.tar` & `charsi-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      911 2023-04-18 12:30:17.231402 charsi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2856 2023-04-18 12:20:57.223743 charsi-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.2.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.2.0/src/charsi/__main__.py
--rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.2.0/src/charsi/asset.py
--rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.2.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.2.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.2.0/src/charsi/commands/build_manifest.py
--rw-r--r--   0        0        0     2378 2023-04-18 12:26:59.535260 charsi-1.2.0/src/charsi/instruction.py
--rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.2.0/src/charsi/manifest.py
--rw-r--r--   0        0        0      818 2023-04-18 12:28:26.212247 charsi-1.2.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.2.0/src/charsi/strings.py
--rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-1.2.0/src/charsi/utils.py
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 charsi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      911 2023-04-18 12:46:56.678839 charsi-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2970 2023-04-18 12:46:31.505531 charsi-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.3.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.3.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.3.0/src/charsi/asset.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.3.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.3.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.3.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2404 2023-04-18 12:41:16.038897 charsi-1.3.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.3.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0      818 2023-04-18 12:28:26.212247 charsi-1.3.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.3.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-1.3.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 charsi-1.3.0/PKG-INFO
```

### Comparing `charsi-1.2.0/pyproject.toml` & `charsi-1.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "1.2.0"
+version = "1.3.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
```

### Comparing `charsi-1.2.0/README.md` & `charsi-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Charsi
 
-![Charis](./docs/images/charsi-x16.png) **Charsi** is a command-line tool to
-help game modders build string resources for [Diablo II: Resurrected][1].
+![Charis](https://raw.githubusercontent.com/he-yaowen/charsi/main/docs/images/charsi-x16.png)
+**Charsi** is a command-line tool to help game modders build string resources
+for [Diablo II: Resurrected][1].
 
 ## Introduction
 
 In the classic Diablo era, there was a very famous hacking tool called
 d2maphack, which was powerful and easy to configure the display text of items in
 the game.
 
@@ -115,13 +116,17 @@
 ]
 ```
 
 ### Directory Structure
 
 * `/instructions/`: Lua scripts for instruction handlers
 
+### Variables
+
+* `{origin}`: Placeholder for original text
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

### Comparing `charsi-1.2.0/src/charsi/commands/build.py` & `charsi-1.3.0/src/charsi/commands/build.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/src/charsi/commands/build_manifest.py` & `charsi-1.3.0/src/charsi/commands/build_manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/src/charsi/instruction.py` & `charsi-1.3.0/src/charsi/instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def is_registered(self, name: str):
         return name in self._handlers
 
     def invoke(self, inst: Instruction, text: str) -> str:
         if not self.is_registered(inst.name):
             raise InstructionUndefinedError(inst.name)
 
-        return self._handlers[inst.name](text, *inst.args)
+        return self._handlers[inst.name](text, *inst.args).replace('{origin}', text)
 
     def load_lua(self, codes: str):
         self._lua.execute(codes)
 
 
 class _InstructionInvokeError(Exception):
     ...
```

### Comparing `charsi-1.2.0/src/charsi/manifest.py` & `charsi-1.3.0/src/charsi/manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/src/charsi/recipe.py` & `charsi-1.3.0/src/charsi/recipe.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/src/charsi/strings.py` & `charsi-1.3.0/src/charsi/strings.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/src/charsi/utils.py` & `charsi-1.3.0/src/charsi/utils.py`

 * *Files identical despite different names*

### Comparing `charsi-1.2.0/PKG-INFO` & `charsi-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 1.2.0
+Version: 1.3.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,16 +15,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: lupa (>=1.14.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Charsi
 
-![Charis](./docs/images/charsi-x16.png) **Charsi** is a command-line tool to
-help game modders build string resources for [Diablo II: Resurrected][1].
+![Charis](https://raw.githubusercontent.com/he-yaowen/charsi/main/docs/images/charsi-x16.png)
+**Charsi** is a command-line tool to help game modders build string resources
+for [Diablo II: Resurrected][1].
 
 ## Introduction
 
 In the classic Diablo era, there was a very famous hacking tool called
 d2maphack, which was powerful and easy to configure the display text of items in
 the game.
 
@@ -134,14 +135,18 @@
 ]
 ```
 
 ### Directory Structure
 
 * `/instructions/`: Lua scripts for instruction handlers
 
+### Variables
+
+* `{origin}`: Placeholder for original text
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

