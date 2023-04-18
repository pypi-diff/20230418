# Comparing `tmp/iconsdk-2.4.1.tar.gz` & `tmp/iconsdk-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iconsdk-2.4.1.tar", last modified: Thu Apr 13 23:54:47 2023, max compression
+gzip compressed data, was "dist/iconsdk-2.4.2.tar", last modified: Tue Apr 18 06:09:16 2023, max compression
```

## Comparing `iconsdk-2.4.1.tar` & `iconsdk-2.4.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 23:54:47.000000 iconsdk-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-13 23:54:42.000000 iconsdk-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/call_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/transaction_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/icon_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/libs/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/in_memory_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/signed_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/convert_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/hexadecimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/utils/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/typing/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 23:54:47.000000 iconsdk-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 23:54:42.000000 iconsdk-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-18 06:09:16.000000 iconsdk-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-18 06:09:05.000000 iconsdk-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/builder/call_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/builder/transaction_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/icon_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/libs/in_memory_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/libs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/libs/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/providers/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/signed_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/convert_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/hexadecimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/utils/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/typing/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-18 06:09:05.000000 iconsdk-2.4.2/iconsdk/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:09:16.000000 iconsdk-2.4.2/iconsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-18 06:09:15.000000 iconsdk-2.4.2/iconsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 06:09:15.000000 iconsdk-2.4.2/iconsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:09:15.000000 iconsdk-2.4.2/iconsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 06:09:15.000000 iconsdk-2.4.2/iconsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 06:09:15.000000 iconsdk-2.4.2/iconsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 06:09:16.000000 iconsdk-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-18 06:09:05.000000 iconsdk-2.4.2/setup.py
```

### Comparing `iconsdk-2.4.1/PKG-INFO` & `iconsdk-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.1
+Version: 2.4.2
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.4.1/README.md` & `iconsdk-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/__init__.py` & `iconsdk-2.4.2/iconsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/builder/__init__.py` & `iconsdk-2.4.2/iconsdk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/builder/call_builder.py` & `iconsdk-2.4.2/iconsdk/builder/call_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/builder/transaction_builder.py` & `iconsdk-2.4.2/iconsdk/builder/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/exception.py` & `iconsdk-2.4.2/iconsdk/exception.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/icon_service.py` & `iconsdk-2.4.2/iconsdk/icon_service.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/libs/__init__.py` & `iconsdk-2.4.2/iconsdk/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/libs/in_memory_zip.py` & `iconsdk-2.4.2/iconsdk/libs/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/libs/serializer.py` & `iconsdk-2.4.2/iconsdk/libs/serializer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/libs/signer.py` & `iconsdk-2.4.2/iconsdk/libs/signer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/monitor.py` & `iconsdk-2.4.2/iconsdk/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from typing import List, Dict, Any
 
 from iconsdk.providers.provider import MonitorSpec
 from iconsdk.utils.typing.conversion import object_to_str
 
 
 class EventFilter:
-    def __init__(self, addr: str, event: str, indexed: int, *args):
-        self.__addr = addr
+    def __init__(self, event: str, addr: str, indexed: int, *args):
         self.__event = event
+        self.__addr = addr
         self.__indexed = list(args[0:indexed])
         self.__data = list(args[indexed:])
 
     def apply_to(self, obj: Dict[str, Any]):
         obj.update({
             "event": self.__event,
             "indexed": self.__indexed,
```

### Comparing `iconsdk-2.4.1/iconsdk/providers/__init__.py` & `iconsdk-2.4.2/iconsdk/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/providers/http_provider.py` & `iconsdk-2.4.2/iconsdk/providers/http_provider.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/providers/provider.py` & `iconsdk-2.4.2/iconsdk/providers/provider.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/signed_transaction.py` & `iconsdk-2.4.2/iconsdk/signed_transaction.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/__init__.py` & `iconsdk-2.4.2/iconsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/convert_type.py` & `iconsdk-2.4.2/iconsdk/utils/convert_type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/converter.py` & `iconsdk-2.4.2/iconsdk/utils/converter.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/hexadecimal.py` & `iconsdk-2.4.2/iconsdk/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/templates.py` & `iconsdk-2.4.2/iconsdk/utils/templates.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/type.py` & `iconsdk-2.4.2/iconsdk/utils/type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/typing/__init__.py` & `iconsdk-2.4.2/iconsdk/utils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/typing/conversion.py` & `iconsdk-2.4.2/iconsdk/utils/typing/conversion.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/utils/validation.py` & `iconsdk-2.4.2/iconsdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/wallet/__init__.py` & `iconsdk-2.4.2/iconsdk/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk/wallet/wallet.py` & `iconsdk-2.4.2/iconsdk/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/iconsdk.egg-info/PKG-INFO` & `iconsdk-2.4.2/iconsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.1
+Version: 2.4.2
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.4.1/iconsdk.egg-info/SOURCES.txt` & `iconsdk-2.4.2/iconsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.1/setup.py` & `iconsdk-2.4.2/setup.py`

 * *Files identical despite different names*

