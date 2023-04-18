# Comparing `tmp/charsi-1.1.0.tar.gz` & `tmp/charsi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-1.1.0.tar", max compression
+gzip compressed data, was "charsi-1.2.0.tar", max compression
```

## Comparing `charsi-1.1.0.tar` & `charsi-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      911 2023-04-18 12:21:47.728742 charsi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2856 2023-04-18 12:20:57.223743 charsi-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.1.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.1.0/src/charsi/__main__.py
--rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.1.0/src/charsi/asset.py
--rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.1.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.1.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.1.0/src/charsi/commands/build_manifest.py
--rw-r--r--   0        0        0     2358 2023-04-18 11:35:39.767582 charsi-1.1.0/src/charsi/instruction.py
--rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.1.0/src/charsi/manifest.py
--rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-1.1.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.1.0/src/charsi/strings.py
--rw-r--r--   0        0        0      385 2023-04-18 12:01:27.221767 charsi-1.1.0/src/charsi/utils.py
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 charsi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      911 2023-04-18 12:30:17.231402 charsi-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2856 2023-04-18 12:20:57.223743 charsi-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.2.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.2.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.2.0/src/charsi/asset.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.2.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.2.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.2.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2378 2023-04-18 12:26:59.535260 charsi-1.2.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.2.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0      818 2023-04-18 12:28:26.212247 charsi-1.2.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.2.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-1.2.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 charsi-1.2.0/PKG-INFO
```

### Comparing `charsi-1.1.0/pyproject.toml` & `charsi-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "1.1.0"
+version = "1.2.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
```

### Comparing `charsi-1.1.0/README.md` & `charsi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `charsi-1.1.0/src/charsi/commands/build.py` & `charsi-1.2.0/src/charsi/commands/build.py`

 * *Files identical despite different names*

### Comparing `charsi-1.1.0/src/charsi/commands/build_manifest.py` & `charsi-1.2.0/src/charsi/commands/build_manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.1.0/src/charsi/instruction.py` & `charsi-1.2.0/src/charsi/instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     if not m:
         raise InstructionFormatError(text)
 
     return Instruction(
         name=m.group(1),
         query=m.group(2).strip(' []'),
-        args=[arg.strip() for arg in fds[1].split(',')],
+        args=[arg.strip() for arg in split_text(fds[1], '#')[0].split(',')],
         lang=None if m.group(3) is None else m.group(3).strip(' []')
     )
 
 
 class InstructionInvoker:
     _handlers: Dict[str, Callable]
     _lua: LuaRuntime
```

### Comparing `charsi-1.1.0/src/charsi/manifest.py` & `charsi-1.2.0/src/charsi/manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.1.0/src/charsi/recipe.py` & `charsi-1.2.0/src/charsi/recipe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import List, IO
 from .instruction import parse, Instruction, InstructionInvoker
 from .strings import GameStringTable, GameStringLanguage
+from .utils import filter_irrelevant
 
 
 class Recipe:
     _instructions: List[Instruction]
 
     @property
     def instructions(self):
         return self._instructions
 
     def load(self, fp: IO):
-        self._instructions = [parse(line) for line in fp.readlines()]
+        self._instructions = [parse(line) for line in filter_irrelevant(fp.readlines())]
 
         return self
 
     def build(self, stbl: GameStringTable, invoker: InstructionInvoker = InstructionInvoker.default):
         for inst in self._instructions:
             langs = GameStringLanguage.get_values() if inst.lang is None else [inst.lang]
```

### Comparing `charsi-1.1.0/src/charsi/strings.py` & `charsi-1.2.0/src/charsi/strings.py`

 * *Files identical despite different names*

### Comparing `charsi-1.1.0/PKG-INFO` & `charsi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 1.1.0
+Version: 1.2.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

