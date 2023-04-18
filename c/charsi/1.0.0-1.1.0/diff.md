# Comparing `tmp/charsi-1.0.0.tar.gz` & `tmp/charsi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-1.0.0.tar", max compression
+gzip compressed data, was "charsi-1.1.0.tar", max compression
```

## Comparing `charsi-1.0.0.tar` & `charsi-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      894 2023-04-18 11:21:55.689366 charsi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2773 2023-04-18 11:19:28.428196 charsi-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.0.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.0.0/src/charsi/__main__.py
--rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.0.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      612 2023-04-17 23:10:32.327874 charsi-1.0.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0      400 2023-04-18 11:03:01.586161 charsi-1.0.0/src/charsi/commands/build_manifest.py
--rw-r--r--   0        0        0     2029 2023-04-18 03:42:15.519526 charsi-1.0.0/src/charsi/instruction.py
--rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.0.0/src/charsi/manifest.py
--rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-1.0.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.0.0/src/charsi/strings.py
--rw-r--r--   0        0        0      206 2023-04-17 21:30:18.257269 charsi-1.0.0/src/charsi/utils.py
--rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 charsi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      911 2023-04-18 12:21:47.728742 charsi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2856 2023-04-18 12:20:57.223743 charsi-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.1.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.1.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.1.0/src/charsi/asset.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.1.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.1.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.1.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2358 2023-04-18 11:35:39.767582 charsi-1.1.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.1.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-1.1.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.1.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      385 2023-04-18 12:01:27.221767 charsi-1.1.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 charsi-1.1.0/PKG-INFO
```

### Comparing `charsi-1.0.0/pyproject.toml` & `charsi-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "charsi"
-version = "1.0.0"
+version = "1.1.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = "^8.1.3"
+lupa = "^1.14.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 pyinstaller = "^5.10.1"
 pylint = "^2.17.2"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
```

### Comparing `charsi-1.0.0/README.md` & `charsi-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,13 +111,17 @@
             "/path/to/recipe2",
             "..."
         ]
     }
 ]
 ```
 
+### Directory Structure
+
+* `/instructions/`: Lua scripts for instruction handlers
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

### Comparing `charsi-1.0.0/src/charsi/instruction.py` & `charsi-1.1.0/src/charsi/instruction.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 import re
 from dataclasses import dataclass
 from typing import List, Dict, Callable, Optional
+from lupa import LuaRuntime
+
 from .utils import split_text
 
 
 @dataclass
 class Instruction:
     name: str
     query: str
@@ -37,19 +39,27 @@
         args=[arg.strip() for arg in fds[1].split(',')],
         lang=None if m.group(3) is None else m.group(3).strip(' []')
     )
 
 
 class InstructionInvoker:
     _handlers: Dict[str, Callable]
+    _lua: LuaRuntime
 
     default: InstructionInvoker
 
     def __init__(self):
         self._handlers = {}
+        self._lua = LuaRuntime(unpack_returned_tuples=True, register_builtins=False)
+
+        lua_globals = self._lua.globals()
+        lua_globals['python'] = None
+        lua_globals['RegisterInstruction'] = self.register
+        lua_globals['UnregisterInstruction'] = self.unregister
+        lua_globals['InstructionRegistered'] = self.is_registered
 
     def register(self, name: str, handler: Callable):
         if name in self._handlers:
             raise InstructionConflictError(name)
 
         self._handlers[name] = handler
 
@@ -64,26 +74,24 @@
 
     def invoke(self, inst: Instruction, text: str) -> str:
         if not self.is_registered(inst.name):
             raise InstructionUndefinedError(inst.name)
 
         return self._handlers[inst.name](text, *inst.args)
 
+    def load_lua(self, codes: str):
+        self._lua.execute(codes)
+
 
 class _InstructionInvokeError(Exception):
     ...
 
 
 class InstructionConflictError(_InstructionInvokeError):
     ...
 
 
 class InstructionUndefinedError(_InstructionInvokeError):
     ...
 
 
-def replace_text_handler(_, *args):
-    return args[0].replace('\\n', '\n')
-
-
 InstructionInvoker.default = InstructionInvoker()
-InstructionInvoker.default.register('Text', replace_text_handler)
```

### Comparing `charsi-1.0.0/src/charsi/manifest.py` & `charsi-1.1.0/src/charsi/manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.0.0/src/charsi/recipe.py` & `charsi-1.1.0/src/charsi/recipe.py`

 * *Files identical despite different names*

### Comparing `charsi-1.0.0/src/charsi/strings.py` & `charsi-1.1.0/src/charsi/strings.py`

 * *Files identical despite different names*

### Comparing `charsi-1.0.0/PKG-INFO` & `charsi-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 1.0.0
+Version: 1.1.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: lupa (>=1.14.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Charsi
 
 ![Charis](./docs/images/charsi-x16.png) **Charsi** is a command-line tool to
 help game modders build string resources for [Diablo II: Resurrected][1].
 
@@ -129,14 +130,18 @@
             "/path/to/recipe2",
             "..."
         ]
     }
 ]
 ```
 
+### Directory Structure
+
+* `/instructions/`: Lua scripts for instruction handlers
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

