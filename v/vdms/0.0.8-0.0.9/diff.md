# Comparing `tmp/vdms-0.0.8.tar.gz` & `tmp/vdms-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdms-0.0.8.tar", last modified: Thu Oct 11 18:02:17 2018, max compression
+gzip compressed data, was "dist/vdms-0.0.9.tar", last modified: Thu Oct 11 18:06:42 2018, max compression
```

## Comparing `vdms-0.0.8.tar` & `vdms-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:02:17.000000 vdms-0.0.8/
-drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms/
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)     3461 2018-10-11 18:01:35.000000 vdms-0.0.8/vdms/vdms.py
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)       35 2018-10-11 18:01:56.000000 vdms-0.0.8/vdms/__init__.py
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)     2317 2018-10-11 12:02:14.000000 vdms-0.0.8/vdms/queryMessage_pb2.py
-drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        9 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/requires.txt
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      610 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/PKG-INFO
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      212 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/SOURCES.txt
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        5 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/top_level.txt
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        1 2018-10-11 18:02:17.000000 vdms-0.0.8/vdms.egg-info/dependency_links.txt
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)       38 2018-10-11 18:02:17.000000 vdms-0.0.8/setup.cfg
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      120 2018-10-11 14:06:41.000000 vdms-0.0.8/README.md
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      676 2018-10-11 18:02:02.000000 vdms-0.0.8/setup.py
--rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      610 2018-10-11 18:02:17.000000 vdms-0.0.8/PKG-INFO
+drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:06:42.000000 vdms-0.0.9/
+drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms/
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)     3461 2018-10-11 18:01:35.000000 vdms-0.0.9/vdms/vdms.py
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)       38 2018-10-11 18:06:29.000000 vdms-0.0.9/vdms/__init__.py
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)     2317 2018-10-11 12:02:14.000000 vdms-0.0.9/vdms/queryMessage_pb2.py
+drwxrwxr-x   0 luisremi  (1001) luisremi  (1001)        0 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        9 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/requires.txt
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      610 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/PKG-INFO
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      212 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/SOURCES.txt
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        5 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/top_level.txt
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)        1 2018-10-11 18:06:42.000000 vdms-0.0.9/vdms.egg-info/dependency_links.txt
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)       38 2018-10-11 18:06:42.000000 vdms-0.0.9/setup.cfg
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      120 2018-10-11 14:06:41.000000 vdms-0.0.9/README.md
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      676 2018-10-11 18:06:36.000000 vdms-0.0.9/setup.py
+-rw-rw-r--   0 luisremi  (1001) luisremi  (1001)      610 2018-10-11 18:06:42.000000 vdms-0.0.9/PKG-INFO
```

### Comparing `vdms-0.0.8/vdms/vdms.py` & `vdms-0.0.9/vdms/vdms.py`

 * *Files identical despite different names*

### Comparing `vdms-0.0.8/vdms/queryMessage_pb2.py` & `vdms-0.0.9/vdms/queryMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `vdms-0.0.8/vdms.egg-info/PKG-INFO` & `vdms-0.0.9/vdms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdms
-Version: 0.0.8
+Version: 0.0.9
 Summary: VDMS Client Module
 Home-page: https://github.com/IntelLabs/vdms
 Author: Luis Remis
 Author-email: luis.remis@intel.com
 License: UNKNOWN
 Description: # VDMS Client Python Module
```

### Comparing `vdms-0.0.8/setup.py` & `vdms-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vdms",
-    version="0.0.8",
+    version="0.0.9",
     author="Luis Remis",
     author_email="luis.remis@intel.com",
     description="VDMS Client Module",
     install_requires=['protobuf'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IntelLabs/vdms",
```

### Comparing `vdms-0.0.8/PKG-INFO` & `vdms-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdms
-Version: 0.0.8
+Version: 0.0.9
 Summary: VDMS Client Module
 Home-page: https://github.com/IntelLabs/vdms
 Author: Luis Remis
 Author-email: luis.remis@intel.com
 License: UNKNOWN
 Description: # VDMS Client Python Module
```

