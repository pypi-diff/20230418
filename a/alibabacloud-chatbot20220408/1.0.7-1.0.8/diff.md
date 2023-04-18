# Comparing `tmp/alibabacloud_chatbot20220408-1.0.7.tar.gz` & `tmp/alibabacloud_chatbot20220408-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_chatbot20220408-1.0.7.tar", last modified: Wed Mar 22 03:12:13 2023, max compression
+gzip compressed data, was "dist/alibabacloud_chatbot20220408-1.0.8.tar", last modified: Tue Apr 18 13:02:28 2023, max compression
```

## Comparing `alibabacloud_chatbot20220408-1.0.7.tar` & `alibabacloud_chatbot20220408-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      426 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   237423 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/client.py
--rw-r--r--   0 root         (0) root         (0)   397818 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2023-03-22 03:12:13.000000 alibabacloud_chatbot20220408-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   237423 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/client.py
+-rw-r--r--   0 root         (0) root         (0)   398165 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-04-18 13:02:28.000000 alibabacloud_chatbot20220408-1.0.8/setup.py
```

### Comparing `alibabacloud_chatbot20220408-1.0.7/LICENSE` & `alibabacloud_chatbot20220408-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408-1.0.7/PKG-INFO` & `alibabacloud_chatbot20220408-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_chatbot20220408
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408-1.0.7/README-CN.md` & `alibabacloud_chatbot20220408-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408-1.0.7/README.md` & `alibabacloud_chatbot20220408-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/client.py` & `alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408/models.py` & `alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,38 +281,44 @@
         return self
 
 
 class BeginSessionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
+        silence_reply_timeout: int = None,
         welcome_message: str = None,
     ):
         self.request_id = request_id
+        self.silence_reply_timeout = silence_reply_timeout
         self.welcome_message = welcome_message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.silence_reply_timeout is not None:
+            result['SilenceReplyTimeout'] = self.silence_reply_timeout
         if self.welcome_message is not None:
             result['WelcomeMessage'] = self.welcome_message
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('SilenceReplyTimeout') is not None:
+            self.silence_reply_timeout = m.get('SilenceReplyTimeout')
         if m.get('WelcomeMessage') is not None:
             self.welcome_message = m.get('WelcomeMessage')
         return self
 
 
 class BeginSessionResponse(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_chatbot20220408-1.0.7/alibabacloud_chatbot20220408.egg-info/PKG-INFO` & `alibabacloud_chatbot20220408-1.0.8/alibabacloud_chatbot20220408.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-chatbot20220408
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408-1.0.7/setup.py` & `alibabacloud_chatbot20220408-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_chatbot20220408.
 
-Created on 22/03/2023
+Created on 18/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_chatbot20220408"
 NAME = "alibabacloud_chatbot20220408" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Chatbot (20220408) SDK Library for Python"
```

