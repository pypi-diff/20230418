# Comparing `tmp/discordwrap-0.8.0.tar.gz` & `tmp/discordwrap-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordwrap-0.8.0.tar", max compression
+gzip compressed data, was "discordwrap-0.9.0.tar", max compression
```

## Comparing `discordwrap-0.8.0.tar` & `discordwrap-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-04-17 04:32:29.112134 discordwrap-0.8.0/LICENSE
--rw-r--r--   0        0        0     1813 2023-04-17 04:32:55.559958 discordwrap-0.8.0/README.md
--rw-r--r--   0        0        0       74 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/Auth/Auth.py
--rw-r--r--   0        0        0       20 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/Auth/__init__.py
--rw-r--r--   0        0        0      584 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/Errors/Errors.py
--rw-r--r--   0        0        0       22 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/Errors/__init__.py
--rw-r--r--   0        0        0       85 2023-04-17 04:32:55.559958 discordwrap-0.8.0/discordwrap/__init__.py
--rw-r--r--   0        0        0       23 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/core/__init__.py
--rw-r--r--   0        0        0     5712 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/core/request.py
--rw-r--r--   0        0        0       22 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/methods/__init__.py
--rw-r--r--   0        0        0      682 2023-04-17 04:32:29.112134 discordwrap-0.8.0/discordwrap/methods/channel.py
--rw-r--r--   0        0        0     1521 2023-04-17 04:32:55.567958 discordwrap-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 discordwrap-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 02:35:39.327840 discordwrap-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1813 2023-04-18 02:36:11.756212 discordwrap-0.9.0/README.md
+-rw-r--r--   0        0        0       74 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/Auth/Auth.py
+-rw-r--r--   0        0        0       20 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/Auth/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/Errors/Errors.py
+-rw-r--r--   0        0        0       22 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/Errors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-18 02:36:11.756212 discordwrap-0.9.0/discordwrap/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/core/__init__.py
+-rw-r--r--   0        0        0     5705 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/core/request.py
+-rw-r--r--   0        0        0       22 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/methods/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-18 02:35:39.327840 discordwrap-0.9.0/discordwrap/methods/channel.py
+-rw-r--r--   0        0        0     1521 2023-04-18 02:36:11.768212 discordwrap-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 discordwrap-0.9.0/PKG-INFO
```

### Comparing `discordwrap-0.8.0/LICENSE` & `discordwrap-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discordwrap-0.8.0/README.md` & `discordwrap-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `discordwrap-0.8.0/discordwrap/Errors/Errors.py` & `discordwrap-0.9.0/discordwrap/Errors/Errors.py`

 * *Files identical despite different names*

### Comparing `discordwrap-0.8.0/discordwrap/core/request.py` & `discordwrap-0.9.0/discordwrap/core/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import datetime
 from types import TracebackType
-from typing import Optional, Union
+from typing import Optional
 
 import requests
 
 from discordwrap.Auth import Auth
 from discordwrap.Errors import *
```

### Comparing `discordwrap-0.8.0/discordwrap/methods/channel.py` & `discordwrap-0.9.0/discordwrap/methods/channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 from discordwrap.Errors import InvlaidBody
-from discordwrap.core import post
+from discordwrap.core import get, post
 
 
-def create_message(channel_id, json: Union[None, dict] = None) -> dict:
+def create_message(channel_id: Union[str, int], json: dict) -> dict:
     if json == None:
         raise InvlaidBody("JSON Body is None")
     if (
         json.get("content") == None
         and json.get("embeds") == None
         and json.get("sticker_ids") == None
         and json.get("components") == None
@@ -17,7 +17,12 @@
             "One of content, embeds, sticker_ids, or components must be set for a message"
         )
     res = post(
         f"/channels/{channel_id}/messages", json=json, bucket=f"channel:{channel_id}"
     )
 
     return res.json()
+
+
+def get_channel(channel_id: Union[str, int]) -> dict:
+    res = get(f"/channels/{channel_id}", bucket=f"channel:{channel_id}")
+    return res.json()
```

### Comparing `discordwrap-0.8.0/pyproject.toml` & `discordwrap-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordwrap"
-version = "0.8.0"
+version = "0.9.0"
 description = "A simple, intuitive wrapper around the underbelly of the discord API. This library is meant to be used with the discord docs. Responses from methods in the library will return JSON just as discords api details."
 authors = ["josh <josh@brunuslabs.com>"]
 readme = "README.md"
 license = 'MIT'
 homepage = "https://discordwrap.brunuslabs.com/"
 documentation = "https://discordwrap.brunuslabs.com/"
 repository = "https://github.com/Brunus-Labs/discordwrap"
```

### Comparing `discordwrap-0.8.0/PKG-INFO` & `discordwrap-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordwrap
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple, intuitive wrapper around the underbelly of the discord API. This library is meant to be used with the discord docs. Responses from methods in the library will return JSON just as discords api details.
 Home-page: https://discordwrap.brunuslabs.com/
 License: MIT
 Keywords: Discord,API,Lightweight,AsyncIO
 Author: josh
 Author-email: josh@brunuslabs.com
 Requires-Python: >=3.10,<4.0
```

