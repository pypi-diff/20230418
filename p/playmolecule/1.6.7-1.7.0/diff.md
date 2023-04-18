# Comparing `tmp/playmolecule-1.6.7.tar.gz` & `tmp/playmolecule-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.7.tar", last modified: Thu Apr 13 09:02:39 2023, max compression
+gzip compressed data, was "playmolecule-1.7.0.tar", last modified: Tue Apr 18 14:05:07 2023, max compression
```

## Comparing `playmolecule-1.6.7.tar` & `playmolecule-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-13 09:02:28.000000 playmolecule-1.6.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 09:02:28.000000 playmolecule-1.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 09:02:39.700542 playmolecule-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 09:02:28.000000 playmolecule-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 09:02:28.000000 playmolecule-1.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:02:39.700542 playmolecule-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 09:02:28.000000 playmolecule-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.676640 playmolecule-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-18 14:04:42.000000 playmolecule-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 14:04:42.000000 playmolecule-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 14:05:07.672640 playmolecule-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 14:04:42.000000 playmolecule-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.676640 playmolecule-1.7.0/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:05:07.676640 playmolecule-1.7.0/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.672640 playmolecule-1.7.0/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 14:04:42.000000 playmolecule-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:05:07.676640 playmolecule-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 14:04:42.000000 playmolecule-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.672640 playmolecule-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_func_to_argparse.py
```

### Comparing `playmolecule-1.6.7/LICENSE.md` & `playmolecule-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/PKG-INFO` & `playmolecule-1.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.7
-Summary: The playmolecule python code.
-Home-page: https://github.com/acellera/playmolecule-python-api/
-Author: Acellera
-Author-email: info@acellera.com
+Version: 1.7.0
+Summary: PlayMolecule python API
+Author-email: Acellera <info@acellera.com>
+Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
+Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PlayMolecule python API
 
 ## Docs
```

### Comparing `playmolecule-1.6.7/playmolecule/__init__.py` & `playmolecule-1.7.0/playmolecule/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     JobConfigNotLoadedError,
 )
 from playmolecule.datacenter import DataCenter, DataCenterError, Dataset
 from playmolecule.jsonlogger import enable_json_logger
 from playmolecule.config import loadConfig
 import logging.config
 import os
+from playmolecule import _version
+
+__version__ = _version.get_versions()["version"]
+
+
+def version():
+    return __version__
 
 
 __init__dir = os.path.dirname(os.path.abspath(__file__))
 
 try:
     logging.config.fileConfig(
         os.path.join(__init__dir, "logging.ini"), disable_existing_loggers=False
```

### Comparing `playmolecule-1.6.7/playmolecule/_test_funcs.py` & `playmolecule-1.7.0/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/config.py` & `playmolecule-1.7.0/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/datacenter.py` & `playmolecule-1.7.0/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/devutils.py` & `playmolecule-1.7.0/playmolecule/devutils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/func2argparse.py` & `playmolecule-1.7.0/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/job.py` & `playmolecule-1.7.0/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/jsonlogger.py` & `playmolecule-1.7.0/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/local.py` & `playmolecule-1.7.0/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/playqueue.py` & `playmolecule-1.7.0/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/session.py` & `playmolecule-1.7.0/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule/utils.py` & `playmolecule-1.7.0/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.7/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.7.0/playmolecule.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.7
-Summary: The playmolecule python code.
-Home-page: https://github.com/acellera/playmolecule-python-api/
-Author: Acellera
-Author-email: info@acellera.com
+Version: 1.7.0
+Summary: PlayMolecule python API
+Author-email: Acellera <info@acellera.com>
+Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
+Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PlayMolecule python API
 
 ## Docs
```

