# Comparing `tmp/asyncbg-0.7.0.tar.gz` & `tmp/asyncbg-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncbg-0.7.0.tar", last modified: Tue Jul  9 06:06:06 2019, max compression
+gzip compressed data, was "dist/asyncbg-0.8.0.tar", last modified: Mon Aug  3 10:23:43 2020, max compression
```

## Comparing `asyncbg-0.7.0.tar` & `asyncbg-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-07-09 06:06:06.000000 asyncbg-0.7.0/
--rw-rw-r--   0 erik      (1000) erik      (1000)       38 2019-07-09 06:06:06.000000 asyncbg-0.7.0/setup.cfg
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-07-09 06:06:06.000000 asyncbg-0.7.0/tests/
--rw-rw-r--   0 erik      (1000) erik      (1000)      914 2019-07-09 04:17:43.000000 asyncbg-0.7.0/tests/test_asyncbg.py
--rw-rw-r--   0 erik      (1000) erik      (1000)        0 2019-07-09 03:57:48.000000 asyncbg-0.7.0/tests/__init__.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg/
--rw-rw-r--   0 erik      (1000) erik      (1000)       22 2019-07-09 06:05:31.000000 asyncbg-0.7.0/asyncbg/version.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1566 2019-07-09 06:04:27.000000 asyncbg-0.7.0/asyncbg/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1702 2019-07-09 04:09:04.000000 asyncbg-0.7.0/README.rst
--rw-rw-r--   0 erik      (1000) erik      (1000)      315 2019-07-09 03:57:48.000000 asyncbg-0.7.0/Makefile
--rw-rw-r--   0 erik      (1000) erik      (1000)     1080 2019-07-09 03:57:48.000000 asyncbg-0.7.0/LICENSE
--rw-rw-r--   0 erik      (1000) erik      (1000)     2696 2019-07-09 06:06:06.000000 asyncbg-0.7.0/PKG-INFO
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg.egg-info/
--rw-rw-r--   0 erik      (1000) erik      (1000)        8 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg.egg-info/top_level.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)      251 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg.egg-info/SOURCES.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)        1 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg.egg-info/dependency_links.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     2696 2019-07-09 06:06:06.000000 asyncbg-0.7.0/asyncbg.egg-info/PKG-INFO
--rw-rw-r--   0 erik      (1000) erik      (1000)      784 2019-07-09 03:57:48.000000 asyncbg-0.7.0/setup.py
--rw-rw-r--   0 erik      (1000) erik      (1000)       61 2019-07-09 03:57:48.000000 asyncbg-0.7.0/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-03 10:23:43.000000 asyncbg-0.8.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-08-03 10:23:21.000000 asyncbg-0.8.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-08-03 10:23:21.000000 asyncbg-0.8.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      315 2020-08-03 10:23:21.000000 asyncbg-0.8.0/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2020-08-03 10:23:43.000000 asyncbg-0.8.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1702 2020-08-03 10:23:21.000000 asyncbg-0.8.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2020-08-03 10:23:21.000000 asyncbg-0.8.0/asyncbg/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-08-03 10:23:21.000000 asyncbg-0.8.0/asyncbg/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      251 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-08-03 10:23:43.000000 asyncbg-0.8.0/asyncbg.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-08-03 10:23:43.000000 asyncbg-0.8.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      784 2020-08-03 10:23:21.000000 asyncbg-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-03 10:23:43.000000 asyncbg-0.8.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-03 10:23:21.000000 asyncbg-0.8.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2020-08-03 10:23:21.000000 asyncbg-0.8.0/tests/test_asyncbg.py
```

### Comparing `asyncbg-0.7.0/tests/test_asyncbg.py` & `asyncbg-0.8.0/tests/test_asyncbg.py`

 * *Files identical despite different names*

### Comparing `asyncbg-0.7.0/asyncbg/__init__.py` & `asyncbg-0.8.0/asyncbg/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import concurrent.futures
-import multiprocessing
 
 from .version import __version__
 
 
 class ProcessPoolExecutor(concurrent.futures.ProcessPoolExecutor):
     """Same as ``concurrent.futures.ProcessPoolExecutor``, but with the
     ``call()`` method added.
```

### Comparing `asyncbg-0.7.0/README.rst` & `asyncbg-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `asyncbg-0.7.0/LICENSE` & `asyncbg-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncbg-0.7.0/PKG-INFO` & `asyncbg-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: asyncbg
-Version: 0.7.0
+Version: 0.8.0
 Summary: Asyncio background tasks.
 Home-page: https://github.com/eerimoq/asyncbg
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: |buildstatus|_
         |coverage|_
         
         Asyncio background tasks
         ========================
         
         Asyncio background tasks in Python 3.7 and later.
```

### Comparing `asyncbg-0.7.0/asyncbg.egg-info/PKG-INFO` & `asyncbg-0.8.0/asyncbg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: asyncbg
-Version: 0.7.0
+Version: 0.8.0
 Summary: Asyncio background tasks.
 Home-page: https://github.com/eerimoq/asyncbg
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: |buildstatus|_
         |coverage|_
         
         Asyncio background tasks
         ========================
         
         Asyncio background tasks in Python 3.7 and later.
```

### Comparing `asyncbg-0.7.0/setup.py` & `asyncbg-0.8.0/setup.py`

 * *Files identical despite different names*

