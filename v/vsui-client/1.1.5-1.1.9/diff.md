# Comparing `tmp/vsui_client-1.1.5.tar.gz` & `tmp/vsui_client-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.5.tar", max compression
+gzip compressed data, was "vsui_client-1.1.9.tar", max compression
```

## Comparing `vsui_client-1.1.5.tar` & `vsui_client-1.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.5/README.md
--rw-r--r--   0        0        0      887 2023-04-17 09:59:13.493390 vsui_client-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.5/vsui_client/__init__.py
--rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.5/vsui_client/_log.py
--rw-r--r--   0        0        0      982 2023-04-17 09:43:07.707763 vsui_client-1.1.5/vsui_client/_main.py
--rw-r--r--   0        0        0     5519 2023-04-17 09:29:01.652675 vsui_client-1.1.5/vsui_client/_oo_interface.py
--rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.5/vsui_client/_vsui_client.py
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.9/README.md
+-rw-r--r--   0        0        0      887 2023-04-18 10:45:02.343218 vsui_client-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.9/vsui_client/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.9/vsui_client/_log.py
+-rw-r--r--   0        0        0      982 2023-04-17 09:43:07.707763 vsui_client-1.1.9/vsui_client/_main.py
+-rw-r--r--   0        0        0     5539 2023-04-17 10:06:52.344383 vsui_client-1.1.9/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     4177 2023-04-18 10:44:49.468347 vsui_client-1.1.9/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.9/PKG-INFO
```

### Comparing `vsui_client-1.1.5/README.md` & `vsui_client-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.5/pyproject.toml` & `vsui_client-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.5"
+version = "1.1.9"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.1.5/vsui_client/_main.py` & `vsui_client-1.1.9/vsui_client/_main.py`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.5/vsui_client/_oo_interface.py` & `vsui_client-1.1.9/vsui_client/_oo_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Union
 import logging
 from abc import ABC, abstractmethod
 import vsui_client._vsui_client as _vsui_client
 
 class VSUIClient(ABC):
-    ''' Baseclass wrapper for vsui_client that allows for better control over enabling/disabling '''
     _handler = None
+    ''' Baseclass wrapper for vsui_client that allows for better control over enabling/disabling '''
     @abstractmethod
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         pass
     
     @abstractmethod
     def disconnect(self) -> None:
         pass
@@ -47,15 +47,15 @@
     ) -> str:
         pass
 
     @abstractmethod
     def get_handler(self) -> logging.Handler:
         pass
 
-class VSUIEnabled():
+class VSUIEnabled(VSUIClient):
     ''' OO interface for vsui client, when vsui is enabled '''
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         ''' Initiate a connection to the server om the given host and port. 
         Args:
             host (str): The host to connect to. Defaults to 'localhost'.
             port (str): The port to connect to. Defaults to '8000'.
         '''
@@ -118,15 +118,15 @@
     
     def get_handler(self) -> logging.Handler:
         ''' Provides access to the logging handler singleton.'''
         if self._handler is None:
             self._handler = _vsui_client.RequestHandler()
         return self._handler
 
-class VSUIDisabled():
+class VSUIDisabled(VSUIClient):
     ''' OO interface for vsui client, when vsui is disabled '''
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         ''' do nothing - not in UI mode '''
         pass
     
     def disconnect(self) -> None:
         ''' do nothing - not in UI mode '''
```

### Comparing `vsui_client-1.1.5/vsui_client/_vsui_client.py` & `vsui_client-1.1.9/vsui_client/_vsui_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
             _vsui_logger.info(f'running {func.__name__} as vsui process')
             r = None
             try:
                 r = func(*args, **kwargs)
             except (SystemExit, Exception) as e:
                 _vsui_logger.exception(f'exception caught: {e}')
                 safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
+                print('sleeping for 1 second before disconnecting')
+                time.sleep(1)
                 r = disconnect()
                 # print to the standart error stream
                 print(f'process {func.__name__} failed, exception: {e}', file=sys.stderr)
                 raise SystemExit(1)
             finally:
                 _vsui_logger.info(f'finished running {func.__name__} as vsui process')
                 return r
@@ -113,8 +115,9 @@
     fig = plt.figure(figsize=figsize)
     plt.imshow(arr, cmap=cmap)
     plt.suptitle(title, fontsize=16)
     my_stringIObytes = io.BytesIO()
     plt.savefig(my_stringIObytes, format=format)
     my_stringIObytes.seek(0)
     my_base64_jpgData = base64.b64encode(my_stringIObytes.read()).decode()
+    plt.close(fig)
     return my_base64_jpgData
```

### Comparing `vsui_client-1.1.5/PKG-INFO` & `vsui_client-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.1.5
+Version: 1.1.9
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

