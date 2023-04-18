# Comparing `tmp/SocketSwap-0.1.0-py2.py3-none-any.whl.zip` & `tmp/SocketSwap-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5618 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      430 b- defN 23-Apr-18 18:13 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat     1149 b- defN 23-Apr-18 19:17 SocketSwap/context_manager.py
--rw-rw-rw-  2.0 fat     7907 b- defN 23-Apr-18 19:44 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-18 19:44 SocketSwap-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1067 b- defN 23-Apr-18 19:44 SocketSwap-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-18 19:44 SocketSwap-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-18 19:44 SocketSwap-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-18 19:44 SocketSwap-0.1.0.dist-info/RECORD
-8 files, 12372 bytes uncompressed, 4500 bytes compressed:  63.6%
+Zip file size: 5616 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      436 b- defN 23-Apr-18 19:59 SocketSwap/__init__.py
+-rw-rw-rw-  2.0 fat     1146 b- defN 23-Apr-18 19:59 SocketSwap/context_manager.py
+-rw-rw-rw-  2.0 fat     7907 b- defN 23-Apr-18 19:59 SocketSwap/proxy.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      642 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/RECORD
+8 files, 12375 bytes uncompressed, 4498 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.0.dist-info/LICENSE
+Filename: SocketSwap-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.0.dist-info/METADATA
+Filename: SocketSwap-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.0.dist-info/WHEEL
+Filename: SocketSwap-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.0.dist-info/top_level.txt
+Filename: SocketSwap-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.0.dist-info/RECORD
+Filename: SocketSwap-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/__init__.py

```diff
@@ -11,9 +11,10 @@
 import socketswap.proxy 
 from socketswap.proxy import start_local_proxy
 from socketswap.context_manager import ProxySwapContext
 
 __all__ = [
     socketswap.proxy,
     start_local_proxy,
+    
     ProxySwapContext
 ]
```

## SocketSwap/context_manager.py

```diff
@@ -1,10 +1,10 @@
 
 import multiprocessing
-from socketswap.proxy_mp import start_local_proxy
+from socketswap.proxy import start_local_proxy
 import socket
 import time
 
 
 # def wrap_start_proxy(args):
 #     start_local_proxy(*args)
```

## Comparing `SocketSwap-0.1.0.dist-info/LICENSE` & `SocketSwap-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.0.dist-info/METADATA` & `SocketSwap-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocketSwap
-Version: 0.1.0
+Version: 0.1.1
 Summary: SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 Home-page: https://github.com/fyx99/SocketSwap
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

