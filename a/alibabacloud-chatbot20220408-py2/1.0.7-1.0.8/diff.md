# Comparing `tmp/alibabacloud_chatbot20220408_py2-1.0.7.tar.gz` & `tmp/alibabacloud_chatbot20220408_py2-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.0.7.tar", last modified: Wed Mar 22 03:11:53 2023, max compression
+gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.0.8.tar", last modified: Tue Apr 18 13:01:55 2023, max compression
```

## Comparing `alibabacloud_chatbot20220408_py2-1.0.7.tar` & `alibabacloud_chatbot20220408_py2-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      426 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97927 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/client.py
--rw-r--r--   0 root         (0) root         (0)   399063 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2923 2023-03-22 03:11:53.000000 alibabacloud_chatbot20220408_py2-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97927 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/client.py
+-rw-r--r--   0 root         (0) root         (0)   399408 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/setup.py
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/LICENSE` & `alibabacloud_chatbot20220408_py2-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_chatbot20220408_py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/README-CN.md` & `alibabacloud_chatbot20220408_py2-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/README.md` & `alibabacloud_chatbot20220408_py2-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/client.py` & `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408/models.py` & `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,37 +244,42 @@
             self.agent_key = m.get('AgentKey')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class BeginSessionResponseBody(TeaModel):
-    def __init__(self, request_id=None, welcome_message=None):
+    def __init__(self, request_id=None, silence_reply_timeout=None, welcome_message=None):
         self.request_id = request_id  # type: str
+        self.silence_reply_timeout = silence_reply_timeout  # type: int
         self.welcome_message = welcome_message  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BeginSessionResponseBody, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('SilenceReplyTimeout') is not None:
+            self.silence_reply_timeout = m.get('SilenceReplyTimeout')
         if m.get('WelcomeMessage') is not None:
             self.welcome_message = m.get('WelcomeMessage')
         return self
 
 
 class BeginSessionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-chatbot20220408-py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.7/setup.py` & `alibabacloud_chatbot20220408_py2-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_chatbot20220408_py2.
 
-Created on 22/03/2023
+Created on 18/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_chatbot20220408"
 NAME = "alibabacloud_chatbot20220408_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Chatbot (20220408) SDK Library for Python2"
```

