# Comparing `tmp/termcs-0.1.1.tar.gz` & `tmp/termcs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yu/code/python/binance/termcs/dist/.tmp-ojjm2ogg/termcs-0.1.1.tar", last modified: Sun Apr 16 12:16:11 2023, max compression
+gzip compressed data, was "/home/yu/code/python/binance/termcs/dist/.tmp-xt5k4euv/termcs-0.1.2.tar", last modified: Tue Apr 18 13:20:48 2023, max compression
```

## Comparing `termcs-0.1.1.tar` & `termcs-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/
--rw-r--r--   0 yu        (1000) yu        (1000)     1049 2023-01-08 18:41:43.000000 termcs-0.1.1/LICENSE
--rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-16 12:16:11.000000 termcs-0.1.1/PKG-INFO
--rw-r--r--   0 yu        (1000) yu        (1000)     4372 2023-04-12 13:08:54.000000 termcs-0.1.1/README.md
--rw-r--r--   0 yu        (1000) yu        (1000)     1232 2023-04-16 12:15:45.000000 termcs-0.1.1/pyproject.toml
--rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-16 12:16:11.000000 termcs-0.1.1/setup.cfg
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs/
--rw-r--r--   0 yu        (1000) yu        (1000)       51 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/__init__.py
--rw-r--r--   0 yu        (1000) yu        (1000)     4306 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/bottomWidget.py
--rw-r--r--   0 yu        (1000) yu        (1000)     2239 2023-04-12 18:25:43.000000 termcs-0.1.1/termcs/screener.py
--rw-r--r--   0 yu        (1000) yu        (1000)     7282 2023-04-16 11:48:35.000000 termcs-0.1.1/termcs/screenerTable.py
--rw-r--r--   0 yu        (1000) yu        (1000)     2376 2023-04-12 15:02:50.000000 termcs-0.1.1/termcs/termcs.css
--rw-r--r--   0 yu        (1000) yu        (1000)      563 2023-04-12 15:17:07.000000 termcs-0.1.1/termcs/termcs.py
--rw-r--r--   0 yu        (1000) yu        (1000)      642 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/topWidget.py
--rw-r--r--   0 yu        (1000) yu        (1000)     1511 2023-04-12 15:13:39.000000 termcs-0.1.1/termcs/utils.py
--rw-r--r--   0 yu        (1000) yu        (1000)     8557 2023-04-16 11:44:43.000000 termcs-0.1.1/termcs/worker.py
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/
--rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/PKG-INFO
--rw-r--r--   0 yu        (1000) yu        (1000)      387 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/SOURCES.txt
--rw-r--r--   0 yu        (1000) yu        (1000)        1 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/dependency_links.txt
--rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/entry_points.txt
--rw-r--r--   0 yu        (1000) yu        (1000)       34 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/requires.txt
--rw-r--r--   0 yu        (1000) yu        (1000)        7 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/top_level.txt
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-18 13:20:48.000000 termcs-0.1.2/
+-rw-r--r--   0 yu        (1000) yu        (1000)     1049 2023-01-08 18:41:43.000000 termcs-0.1.2/LICENSE
+-rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-18 13:20:48.000000 termcs-0.1.2/PKG-INFO
+-rw-r--r--   0 yu        (1000) yu        (1000)     4372 2023-04-12 13:08:54.000000 termcs-0.1.2/README.md
+-rw-r--r--   0 yu        (1000) yu        (1000)     1232 2023-04-18 13:19:44.000000 termcs-0.1.2/pyproject.toml
+-rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-18 13:20:48.000000 termcs-0.1.2/setup.cfg
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs/
+-rw-r--r--   0 yu        (1000) yu        (1000)       51 2023-04-12 13:08:54.000000 termcs-0.1.2/termcs/__init__.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     4264 2023-04-18 12:05:07.000000 termcs-0.1.2/termcs/bottomWidget.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     2239 2023-04-18 10:57:06.000000 termcs-0.1.2/termcs/screener.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     7282 2023-04-18 08:11:06.000000 termcs-0.1.2/termcs/screenerTable.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     2376 2023-04-18 10:00:37.000000 termcs-0.1.2/termcs/termcs.css
+-rw-r--r--   0 yu        (1000) yu        (1000)      563 2023-04-18 10:00:37.000000 termcs-0.1.2/termcs/termcs.py
+-rw-r--r--   0 yu        (1000) yu        (1000)      642 2023-04-12 13:08:54.000000 termcs-0.1.2/termcs/topWidget.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     1511 2023-04-18 10:00:37.000000 termcs-0.1.2/termcs/utils.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     8557 2023-04-18 08:11:06.000000 termcs-0.1.2/termcs/worker.py
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/
+-rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/PKG-INFO
+-rw-r--r--   0 yu        (1000) yu        (1000)      387 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/SOURCES.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)        1 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/dependency_links.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/entry_points.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)       34 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/requires.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)        7 2023-04-18 13:20:48.000000 termcs-0.1.2/termcs.egg-info/top_level.txt
```

### Comparing `termcs-0.1.1/LICENSE` & `termcs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/PKG-INFO` & `termcs-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termcs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Terminal crypto screener
 Author: Riyum
 License: Copyright (c) 2023 Riyum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termcs Version: 0.1.1 Summary: Terminal crypto
+Metadata-Version: 2.1 Name: termcs Version: 0.1.2 Summary: Terminal crypto
 screener Author: Riyum License: Copyright (c) 2023 Riyum Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `termcs-0.1.1/README.md` & `termcs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/pyproject.toml` & `termcs-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "termcs"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name="Riyum" }]
 description = "Terminal crypto screener"
 requires-python = ">=3.7"
 readme = "README.md"
 license = {file = 'LICENSE'}
 classifiers = [
     "Environment :: Console",
```

### Comparing `termcs-0.1.1/termcs/bottomWidget.py` & `termcs-0.1.2/termcs/bottomWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from typing import Dict
 
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.containers import Container
 from textual.reactive import reactive
 from textual.widget import Widget
-from textual.binding import Binding
-from textual.widgets import Button, Footer, Input
+from textual.widgets import Footer, Input
 
 
 class MyFooter(Footer):
 
     """
     Footer override for styling
     """
@@ -35,15 +34,15 @@
         return self._active_keys
 
     @active_keys.setter
     def active_keys(self, arg: dict) -> None:
         self._active_keys = arg
 
     def watch__active_keys(self, _active_keys: dict) -> None:
-        self._key_text = self.make_key_text()
+        self._key_text = self._make_key_text()
 
     def toggleKey(self, key: str) -> None:
         """active key setter & force watch call"""
         if key == "b":
             self.active_keys["b"] = True
             self.active_keys["t"] = False
             self.active_keys["o"] = False
@@ -56,15 +55,15 @@
             self.active_keys["t"] = False
             self.active_keys["o"] = True
         else:
             self.active_keys[key] = not self.active_keys[key]
         """textual issue #1098, Assign the reactive to itself to force a watch_"""
         self.active_keys = self.active_keys
 
-    def make_key_text(self) -> Text:
+    def _make_key_text(self) -> Text:
         """Create text containing all the keys."""
         base_style = self.rich_style
         text = Text(
             style=self.rich_style,
             no_wrap=True,
             overflow="ellipsis",
             justify="left",
```

### Comparing `termcs-0.1.1/termcs/screener.py` & `termcs-0.1.2/termcs/screener.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/screenerTable.py` & `termcs-0.1.2/termcs/screenerTable.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/termcs.css` & `termcs-0.1.2/termcs/termcs.css`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/termcs.py` & `termcs-0.1.2/termcs/termcs.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/topWidget.py` & `termcs-0.1.2/termcs/topWidget.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/utils.py` & `termcs-0.1.2/termcs/utils.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs/worker.py` & `termcs-0.1.2/termcs/worker.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.1/termcs.egg-info/PKG-INFO` & `termcs-0.1.2/termcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termcs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Terminal crypto screener
 Author: Riyum
 License: Copyright (c) 2023 Riyum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termcs Version: 0.1.1 Summary: Terminal crypto
+Metadata-Version: 2.1 Name: termcs Version: 0.1.2 Summary: Terminal crypto
 screener Author: Riyum License: Copyright (c) 2023 Riyum Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

