# Comparing `tmp/zcatalyst_runtime_39-0.0.3.tar.gz` & `tmp/zcatalyst_runtime_39-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcatalyst_runtime_39-0.0.3.tar", last modified: Fri Apr  7 05:23:18 2023, max compression
+gzip compressed data, was "zcatalyst_runtime_39-0.0.4.tar", last modified: Mon Apr 17 05:38:06 2023, max compression
```

## Comparing `zcatalyst_runtime_39-0.0.3.tar` & `zcatalyst_runtime_39-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      639 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/LICENSE
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      129 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/MANIFEST.in
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/PKG-INFO
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      251 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/README.md
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       38 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/setup.cfg
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1392 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/setup.py
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/__init__.py
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     2494 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/__init__.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      306 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/applogic.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1899 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/basicio.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1705 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/cron.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1926 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/event.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1075 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/integration.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      794 2023-04-07 05:22:03.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/utils.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1805 2023-04-06 05:53:57.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/init_handler.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1829 2023-03-10 07:50:09.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/log_handler.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     7283 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/main.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      271 2023-04-07 05:22:03.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/meta.json
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       25 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/requirements-prod.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       10 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/requirements.txt
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/PKG-INFO
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      747 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/SOURCES.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/dependency_links.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       21 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/top_level.txt
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-17 05:38:06.673607 zcatalyst_runtime_39-0.0.4/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      639 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/LICENSE
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      129 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/MANIFEST.in
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-17 05:38:06.673607 zcatalyst_runtime_39-0.0.4/PKG-INFO
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      251 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/README.md
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       38 2023-04-17 05:38:06.673607 zcatalyst_runtime_39-0.0.4/setup.cfg
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1392 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/setup.py
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-17 05:38:06.669608 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/__init__.py
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-17 05:38:06.673607 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     2744 2023-04-17 05:29:08.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/__init__.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      306 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/applogic.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1838 2023-04-17 05:29:08.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/basicio.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1705 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/cron.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1926 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/event.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1075 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/integration.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      794 2023-04-07 05:22:03.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/utils.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1805 2023-04-06 05:53:57.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/init_handler.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1829 2023-03-10 07:50:09.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/log_handler.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     7283 2023-04-10 04:18:10.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/main.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      271 2023-04-17 05:37:50.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/meta.json
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       25 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/requirements-prod.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       10 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/requirements.txt
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-17 05:38:06.669608 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-17 05:38:06.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/PKG-INFO
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      747 2023-04-17 05:38:06.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/SOURCES.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-04-17 05:38:06.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/dependency_links.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       21 2023-04-17 05:38:06.000000 zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/top_level.txt
```

### Comparing `zcatalyst_runtime_39-0.0.3/LICENSE` & `zcatalyst_runtime_39-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/PKG-INFO` & `zcatalyst_runtime_39-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zcatalyst_runtime_39
-Version: 0.0.3
-Summary: Catalyst runtime for Python 3.9-fd917f8
+Version: 0.0.4
+Summary: Catalyst runtime for Python 3.9-c2adabd
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 Maintainer: Catalyst by Zoho
 Maintainer-email: support@zohocatalyst.com
 License: Apache 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless
```

### Comparing `zcatalyst_runtime_39-0.0.3/setup.py` & `zcatalyst_runtime_39-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/__init__.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import threading
 from importlib.util import spec_from_file_location, module_from_spec
 
 from flask import g
 
 from init_handler import InitHandler
-from flavours.utils import get_catalyst_headers
+from flavours.utils import get_catalyst_headers, send_json_response
 
 CUSTOMER_CODE_ENTRYPOINT = None
 
 class FlavourHandler:
     def __init__(self) -> None:
         with open(InitHandler.get_code_location().joinpath('catalyst-config.json'), 'r') as config_file:
             catalyst_config = json.loads(config_file.read())
@@ -48,14 +48,17 @@
             spec = spec_from_file_location('', self.__entrypoint)
             module = module_from_spec(spec)
             spec.loader.exec_module(module)
             CUSTOMER_CODE_ENTRYPOINT = module.handler
 
         RET = CUSTOMER_CODE_ENTRYPOINT(*(self.__construct_function_parameters()))
 
-        # User can return their own response object from applogic functions.
-        if RET and (self.__flavour == 'applogic' or self.__flavour == 'advancedio'):
+        if self.__flavour == 'basicio':
+            # Refer: !25. Useful when `context.close()`` is not called by user.
+            send_json_response(g.response.status_code, { 'output': g.response.get_data(as_text=True) })
+        elif RET and (self.__flavour == 'applogic' or self.__flavour == 'advancedio'):
+            # User can return their own response object from applogic functions.
             g.response = RET
 
     def return_error_response(self, error = None):
         return self.__get_flavour().return_error_response(error)
```

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/basicio.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/basicio.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     def __init__(self) -> None:
         max_execution_buffer_time_ms = 500
         max_execution_hidden_time_ms = self.__max_execution_time_ms - max_execution_buffer_time_ms
 
         self.__endtime_timestamp = int(time.time() * 1000) + max_execution_hidden_time_ms
         
     def close(self) -> None:
-        send_json_response(g.response.status_code, { 'output': g.response.get_data(as_text=True) })
+        # `send_json_response` will be called in `init.py`.
+        pass
 
     def log(self, *args):
         Context.__logger.info(*args)
 
     def get_remaining_execution_time_ms(self):
         time_remaining = self.__endtime_timestamp - int(time.time() * 1000)
         return 0 if time_remaining < 0 else time_remaining
@@ -44,16 +45,15 @@
 
         return arguments
 
     def set_status(self, status_code: int):
         g.response.status_code = status_code
 
     def write(self, message: str):
-        old_message = g.response.get_data(as_text=True) or ''
-        g.response.set_data(old_message + message)
+        g.response.set_data(g.response.get_data(as_text=True) or '' + message)
 
 class BasicIOHandler(FlavourHandler):
     def construct_function_parameters():
         return (Context(), BasicIO())
 
     def return_error_response(error):
         send_json_response(500, { 'error': error })
```

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/cron.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/cron.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/event.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/event.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/integration.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/integration.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/utils.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/flavours/utils.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/init_handler.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/init_handler.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/log_handler.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/log_handler.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/main.py` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39/main.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/PKG-INFO` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zcatalyst-runtime-39
-Version: 0.0.3
-Summary: Catalyst runtime for Python 3.9-fd917f8
+Version: 0.0.4
+Summary: Catalyst runtime for Python 3.9-c2adabd
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 Maintainer: Catalyst by Zoho
 Maintainer-email: support@zohocatalyst.com
 License: Apache 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless
```

### Comparing `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/SOURCES.txt` & `zcatalyst_runtime_39-0.0.4/zcatalyst_runtime_39.egg-info/SOURCES.txt`

 * *Files identical despite different names*

