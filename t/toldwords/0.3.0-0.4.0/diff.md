# Comparing `tmp/toldwords-0.3.0.tar.gz` & `tmp/toldwords-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toldwords-0.3.0.tar", max compression
+gzip compressed data, was "toldwords-0.4.0.tar", max compression
```

## Comparing `toldwords-0.3.0.tar` & `toldwords-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.3.0/README.md
--rw-r--r--   0        0        0     1992 2023-04-18 07:47:15.901799 toldwords-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      579 2023-04-18 07:47:21.645229 toldwords-0.3.0/toldwords/__init__.py
--rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.3.0/toldwords/openai.py
--rw-r--r--   0        0        0      771 2023-03-26 01:00:49.949118 toldwords-0.3.0/toldwords/pretalx.py
--rw-r--r--   0        0        0      243 2023-03-23 15:43:42.992952 toldwords-0.3.0/toldwords/utils.py
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 toldwords-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.4.0/README.md
+-rw-r--r--   0        0        0     1992 2023-04-18 08:13:29.987570 toldwords-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      579 2023-04-18 08:13:34.136292 toldwords-0.4.0/toldwords/__init__.py
+-rw-r--r--   0        0        0      365 2023-04-18 08:11:54.604553 toldwords-0.4.0/toldwords/__init__.pyi
+-rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.4.0/toldwords/openai.py
+-rw-r--r--   0        0        0      883 2023-04-18 08:11:54.604823 toldwords-0.4.0/toldwords/openai.pyi
+-rw-r--r--   0        0        0      771 2023-03-26 01:00:49.949118 toldwords-0.4.0/toldwords/pretalx.py
+-rw-r--r--   0        0        0      508 2023-04-18 08:11:54.605103 toldwords-0.4.0/toldwords/pretalx.pyi
+-rw-r--r--   0        0        0      243 2023-03-23 15:43:42.992952 toldwords-0.4.0/toldwords/utils.py
+-rw-r--r--   0        0        0       76 2023-04-18 08:11:54.605597 toldwords-0.4.0/toldwords/utils.pyi
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 toldwords-0.4.0/PKG-INFO
```

### Comparing `toldwords-0.3.0/LICENSE.txt` & `toldwords-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toldwords-0.3.0/pyproject.toml` & `toldwords-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toldwords"
-version = "0.3.0"
+version = "0.4.0"
 description = "Using ChatGPT to make keywords for the papers from COSCUP."
 authors = ["Toomore Chiang <toomore0929@gmail.com>"]
 license = 'MIT'
 readme = "README.md"
 homepage = 'https://github.com/toomore/toldwords'
 repository = 'https://github.com/toomore/toldwords'
 packages = [
```

### Comparing `toldwords-0.3.0/toldwords/__init__.py` & `toldwords-0.4.0/toldwords/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ''' __init__ '''
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 from .openai import Choice
 from .openai import Message
 from .openai import OpenAIAPI
 from .openai import RespCompletions
 from .openai import Role
 from .openai import TokenUsage
 from .pretalx import Item
```

### Comparing `toldwords-0.3.0/toldwords/openai.py` & `toldwords-0.4.0/toldwords/openai.py`

 * *Files identical despite different names*

### Comparing `toldwords-0.3.0/toldwords/pretalx.py` & `toldwords-0.4.0/toldwords/pretalx.py`

 * *Files identical despite different names*

### Comparing `toldwords-0.3.0/PKG-INFO` & `toldwords-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toldwords
-Version: 0.3.0
+Version: 0.4.0
 Summary: Using ChatGPT to make keywords for the papers from COSCUP.
 Home-page: https://github.com/toomore/toldwords
 License: MIT
 Keywords: API,ChatGPT,pretalx,COSCUP,openai
 Author: Toomore Chiang
 Author-email: toomore0929@gmail.com
 Requires-Python: >=3.9,<4.0
```

