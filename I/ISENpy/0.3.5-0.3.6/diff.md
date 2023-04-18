# Comparing `tmp/ISENpy-0.3.5.tar.gz` & `tmp/ISENpy-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISENpy-0.3.5.tar", last modified: Mon Apr 10 18:21:06 2023, max compression
+gzip compressed data, was "ISENpy-0.3.6.tar", last modified: Tue Apr 18 12:55:03 2023, max compression
```

## Comparing `ISENpy-0.3.5.tar` & `ISENpy-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-10 18:21:06.626256 ISENpy-0.3.5/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-10 18:21:06.625115 ISENpy-0.3.5/ISENpy/
--rwxrwxrwx   0 corentin   (501) staff       (20)     1343 2023-04-10 18:20:48.000000 ISENpy-0.3.5/ISENpy/__init__.py
--rwxrwxrwx   0 corentin   (501) staff       (20)     6318 2023-03-22 13:06:10.000000 ISENpy-0.3.5/ISENpy/client.py
--rwxrwxrwx   0 corentin   (501) staff       (20)    23617 2023-04-10 18:15:01.000000 ISENpy-0.3.5/ISENpy/dataClasses.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-10 18:21:06.625970 ISENpy-0.3.5/ISENpy.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     5166 2023-04-10 18:21:06.000000 ISENpy-0.3.5/ISENpy.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      233 2023-04-10 18:21:06.000000 ISENpy-0.3.5/ISENpy.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-04-10 18:21:06.000000 ISENpy-0.3.5/ISENpy.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       18 2023-04-10 18:21:06.000000 ISENpy-0.3.5/ISENpy.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)        7 2023-04-10 18:21:06.000000 ISENpy-0.3.5/ISENpy.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.3.5/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     5166 2023-04-10 18:21:06.626133 ISENpy-0.3.5/PKG-INFO
--rwxrwxrwx   0 corentin   (501) staff       (20)     4730 2023-03-22 13:41:56.000000 ISENpy-0.3.5/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-04-10 18:21:06.626292 ISENpy-0.3.5/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      848 2023-04-10 18:20:46.000000 ISENpy-0.3.5/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-18 12:55:03.134698 ISENpy-0.3.6/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-18 12:55:03.133801 ISENpy-0.3.6/ISENpy/
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1343 2023-04-18 12:54:49.000000 ISENpy-0.3.6/ISENpy/__init__.py
+-rwxrwxrwx   0 corentin   (501) staff       (20)     6318 2023-03-22 13:06:10.000000 ISENpy-0.3.6/ISENpy/client.py
+-rwxrwxrwx   0 corentin   (501) staff       (20)    29767 2023-04-18 12:53:40.000000 ISENpy-0.3.6/ISENpy/dataClasses.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-04-18 12:55:03.134408 ISENpy-0.3.6/ISENpy.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     5166 2023-04-18 12:55:03.000000 ISENpy-0.3.6/ISENpy.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      233 2023-04-18 12:55:03.000000 ISENpy-0.3.6/ISENpy.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-04-18 12:55:03.000000 ISENpy-0.3.6/ISENpy.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       18 2023-04-18 12:55:03.000000 ISENpy-0.3.6/ISENpy.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        7 2023-04-18 12:55:03.000000 ISENpy-0.3.6/ISENpy.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.3.6/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     5166 2023-04-18 12:55:03.134585 ISENpy-0.3.6/PKG-INFO
+-rwxrwxrwx   0 corentin   (501) staff       (20)     4730 2023-03-22 13:41:56.000000 ISENpy-0.3.6/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-04-18 12:55:03.134736 ISENpy-0.3.6/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      848 2023-04-18 12:54:46.000000 ISENpy-0.3.6/setup.py
```

### Comparing `ISENpy-0.3.5/ISENpy/__init__.py` & `ISENpy-0.3.6/ISENpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 """
 
 
 __title__ = "ISENpy"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 
 
 from .dataClasses import *
 from .client import *
```

### Comparing `ISENpy-0.3.5/ISENpy/client.py` & `ISENpy-0.3.6/ISENpy/client.py`

 * *Files identical despite different names*

### Comparing `ISENpy-0.3.5/ISENpy.egg-info/PKG-INFO` & `ISENpy-0.3.6/ISENpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.3.5/LICENSE` & `ISENpy-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ISENpy-0.3.5/PKG-INFO` & `ISENpy-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.3.5/README.md` & `ISENpy-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ISENpy-0.3.5/setup.py` & `ISENpy-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ISENpy',
-    version='0.3.5',    
+    version='0.3.6',    
     description='A python API wrapper for ISEN-OUEST',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/ISENpy',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

