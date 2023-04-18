# Comparing `tmp/charsi-0.1.0.tar.gz` & `tmp/charsi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-0.1.0.tar", max compression
+gzip compressed data, was "charsi-0.3.0.tar", max compression
```

## Comparing `charsi-0.1.0.tar` & `charsi-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      894 2023-04-17 23:25:20.353233 charsi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-04-17 23:39:32.248013 charsi-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-0.1.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-0.1.0/src/charsi/__main__.py
--rw-r--r--   0        0        0       66 2023-04-17 22:14:26.163984 charsi-0.1.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      612 2023-04-17 23:10:32.327874 charsi-0.1.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0     1904 2023-04-17 22:20:45.432301 charsi-0.1.0/src/charsi/instruction.py
--rw-r--r--   0        0        0      684 2023-04-17 22:22:59.120619 charsi-0.1.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     1426 2023-04-17 23:13:46.207883 charsi-0.1.0/src/charsi/strings.py
--rw-r--r--   0        0        0      206 2023-04-17 21:30:18.257269 charsi-0.1.0/src/charsi/utils.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 charsi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      894 2023-04-18 03:54:20.060629 charsi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2428 2023-04-18 03:53:46.904216 charsi-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-0.3.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-0.3.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0       66 2023-04-17 22:14:26.163984 charsi-0.3.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      612 2023-04-17 23:10:32.327874 charsi-0.3.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0     2029 2023-04-18 03:42:15.519526 charsi-0.3.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0      762 2023-04-18 03:43:46.397471 charsi-0.3.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-0.3.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      206 2023-04-17 21:30:18.257269 charsi-0.3.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 charsi-0.3.0/PKG-INFO
```

### Comparing `charsi-0.1.0/pyproject.toml` & `charsi-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "0.1.0"
+version = "0.3.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
```

### Comparing `charsi-0.1.0/src/charsi/commands/build.py` & `charsi-0.3.0/src/charsi/commands/build.py`

 * *Files identical despite different names*

### Comparing `charsi-0.1.0/src/charsi/instruction.py` & `charsi-0.3.0/src/charsi/instruction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 import re
 from dataclasses import dataclass
-from typing import List, Dict, Callable
+from typing import List, Dict, Callable, Optional
 from .utils import split_text
 
 
 @dataclass
 class Instruction:
     name: str
     query: str
     args: List[str]
+    lang: Optional[str] = None
 
 
 class _InstructionError(Exception):
     ...
 
 
 class InstructionFormatError(_InstructionError):
@@ -21,23 +22,24 @@
 
 
 def parse(text: str) -> Instruction:
     fds = split_text(text, ':')
     if len(fds) < 2:
         raise InstructionFormatError(text)
 
-    m = re.match(r'^\s*(\w+)\s*(\[[^]]+])', fds[0])
+    m = re.match(r'^\s*(\w+)\s*(\[[^]]+])\s*(\[[^]]+])?', fds[0])
 
     if not m:
         raise InstructionFormatError(text)
 
     return Instruction(
         name=m.group(1),
         query=m.group(2).strip(' []'),
-        args=[arg.strip() for arg in fds[1].split(',')]
+        args=[arg.strip() for arg in fds[1].split(',')],
+        lang=None if m.group(3) is None else m.group(3).strip(' []')
     )
 
 
 class InstructionInvoker:
     _handlers: Dict[str, Callable]
 
     default: InstructionInvoker
```

### Comparing `charsi-0.1.0/src/charsi/recipe.py` & `charsi-0.3.0/src/charsi/recipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,9 +13,11 @@
     def load(self, fp: IO):
         self._instructions = [parse(line) for line in fp.readlines()]
 
         return self
 
     def build(self, stbl: GameStringTable, invoker: InstructionInvoker = InstructionInvoker.default):
         for inst in self._instructions:
-            s = stbl.find(inst.query)
-            s.update({lang: invoker.invoke(inst, s[lang]) for lang in GameStringLanguage.get_values()})
+            langs = GameStringLanguage.get_values() if inst.lang is None else [inst.lang]
+
+            for s in stbl.findall(inst.query):
+                s.update({lang: invoker.invoke(inst, s[lang]) for lang in langs})
```

### Comparing `charsi-0.1.0/src/charsi/strings.py` & `charsi-0.3.0/src/charsi/strings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import re
 import json
 from typing import TypedDict, IO, List, Dict, Optional
 from enum import Enum
+from functools import reduce
 
 
 # pylint: disable=invalid-name
 class GameStringLanguage(Enum):
     enUS = 'enUS'
     zhTW = 'zhTW'
     deDE = 'deDE'
@@ -63,10 +65,29 @@
     def dump(self, fp: IO):
         json.dump(self._strings, fp, ensure_ascii=False, indent=2)
 
         return self
 
     def find(self, key: str) -> Optional[GameString]:
         if key not in self._indices:
-            return None
+            raise LookupError(key)
 
         return self._strings[self._indices[key]]
+
+    def findall(self, query: str) -> List[dict]:
+        if query.find(',') > -1:
+            return reduce(lambda v, sl: v + sl, [self.findall(q.strip()) for q in query.split(',')], [])
+
+        m = re.match(r'^\s*([\w\s]+)\s*~\s*([\w\s]+)\s*$', query)
+
+        if not m:
+            return [self.find(query)]
+
+        if (m.group(1) not in self._indices) or (m.group(2) not in self._indices):
+            raise IndexError(query)
+
+        start_index = self._indices[m.group(1)]
+        end_index = self._indices[m.group(2)] + 1
+        if start_index > end_index:
+            raise IndexError(query)
+
+        return self._strings[start_index:end_index]
```

