# Comparing `tmp/pyNetSocket-1.1.3.tar.gz` & `tmp/pyNetSocket-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNetSocket-1.1.3.tar", last modified: Thu May 13 14:28:27 2021, max compression
+gzip compressed data, was "pyNetSocket-1.1.4.tar", last modified: Tue Apr 18 06:43:16 2023, max compression
```

## Comparing `pyNetSocket-1.1.3.tar` & `pyNetSocket-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 14:28:27.054765 pyNetSocket-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-05-13 14:28:27.050765 pyNetSocket-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 14:28:27.050765 pyNetSocket-1.1.3/pyNetSocket/
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/pyNetSocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 14:28:27.050765 pyNetSocket-1.1.3/pyNetSocket/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/pyNetSocket/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/pyNetSocket/docs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/pyNetSocket/docs/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/pyNetSocket/docs/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 14:28:27.050765 pyNetSocket-1.1.3/pyNetSocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-05-13 14:28:26.000000 pyNetSocket-1.1.3/pyNetSocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-05-13 14:28:26.000000 pyNetSocket-1.1.3/pyNetSocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-13 14:28:26.000000 pyNetSocket-1.1.3/pyNetSocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-13 14:28:26.000000 pyNetSocket-1.1.3/pyNetSocket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-13 14:28:27.054765 pyNetSocket-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-05-13 14:28:17.000000 pyNetSocket-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/pyNetSocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/pyNetSocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/pyNetSocket/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/pyNetSocket/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/pyNetSocket/docs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/pyNetSocket/docs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/pyNetSocket/docs/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/pyNetSocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-18 06:43:16.000000 pyNetSocket-1.1.4/pyNetSocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-18 06:43:16.000000 pyNetSocket-1.1.4/pyNetSocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:43:16.000000 pyNetSocket-1.1.4/pyNetSocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 06:43:16.000000 pyNetSocket-1.1.4/pyNetSocket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:43:16.950642 pyNetSocket-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-18 06:42:58.000000 pyNetSocket-1.1.4/setup.py
```

### Comparing `pyNetSocket-1.1.3/LICENSE` & `pyNetSocket-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/README.md` & `pyNetSocket-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/pyNetSocket/__init__.py` & `pyNetSocket-1.1.4/pyNetSocket/__init__.py`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/pyNetSocket/docs/__init__.py` & `pyNetSocket-1.1.4/pyNetSocket/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/pyNetSocket/docs/callbacks.py` & `pyNetSocket-1.1.4/pyNetSocket/docs/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def ondisconnect():
     print('To add disconnection callbacks to a connector:',
           'myConnector.onDisconnect(CALLBACK, args=args, kwargs=kwargs)',
           'The function will be given the address, then the args and kwargs',
           'It will not get the connection object since the connection is closed',
           sep='\n')
 
-def onmessage()
+def onmessage():
     print('To add message-receive calbacks to a connector:',
           'myConnector.onMessage(CALLBACK, args=args, kwargs=kwargs)',
           'The function will be given the address, connection object, message, and then the args and kwargs',
           sep='\n')
  
 try:
     topics = [
```

### Comparing `pyNetSocket-1.1.3/pyNetSocket/docs/client.py` & `pyNetSocket-1.1.4/pyNetSocket/docs/client.py`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/pyNetSocket/docs/server.py` & `pyNetSocket-1.1.4/pyNetSocket/docs/server.py`

 * *Files identical despite different names*

### Comparing `pyNetSocket-1.1.3/setup.py` & `pyNetSocket-1.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open('README.md') as fl:
     l_desc = fl.read()
 
 setuptools.setup(
     name="pyNetSocket",
-    version="1.1.3",
-    author="DrSparky2k7",
+    version="1.1.4",
+    author="AdityaIyer2k7",
     author_email="adityaiyer2007@gmail.com",
     description="A simple networking library for python",
     long_description=l_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/DrSparky2k7/PyNetSocket",
     packages=setuptools.find_packages(),
     classifiers=[
```

