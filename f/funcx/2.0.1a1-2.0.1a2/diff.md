# Comparing `tmp/funcx-2.0.1a1.tar.gz` & `tmp/funcx-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.0.1a1.tar", last modified: Mon Apr 17 19:13:34 2023, max compression
+gzip compressed data, was "funcx-2.0.1a2.tar", last modified: Tue Apr 18 21:56:05 2023, max compression
```

## Comparing `funcx-2.0.1a1.tar` & `funcx-2.0.1a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854456 funcx-2.0.1a1/
--rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-2.0.1a1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 19:06:42.000000 funcx-2.0.1a1/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     1797 2023-04-17 19:13:34.854534 funcx-2.0.1a1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1051 2023-04-17 18:38:33.000000 funcx-2.0.1a1/PyPI.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.853217 funcx-2.0.1a1/funcx/
--rw-r--r--   0 chris      (501) staff       (20)      467 2023-04-12 14:51:48.000000 funcx-2.0.1a1/funcx/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854240 funcx-2.0.1a1/funcx/serialize/
--rw-r--r--   0 chris      (501) staff       (20)      110 2023-04-12 14:51:48.000000 funcx-2.0.1a1/funcx/serialize/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1146 2023-04-17 19:06:42.000000 funcx-2.0.1a1/funcx/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854082 funcx-2.0.1a1/funcx.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     1797 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      253 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       26 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        6 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:13:34.854866 funcx-2.0.1a1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1659 2023-04-17 18:38:33.000000 funcx-2.0.1a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.840100 funcx-2.0.1a2/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-2.0.1a2/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 funcx-2.0.1a2/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     2058 2023-04-18 21:56:05.840148 funcx-2.0.1a2/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1051 2023-04-18 19:39:56.000000 funcx-2.0.1a2/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839213 funcx-2.0.1a2/funcx/
+-rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-10 19:02:41.000000 funcx-2.0.1a2/funcx/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839949 funcx-2.0.1a2/funcx/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-10 19:02:41.000000 funcx-2.0.1a2/funcx/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1146 2023-04-18 21:17:41.000000 funcx-2.0.1a2/funcx/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839827 funcx-2.0.1a2/funcx.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     2058 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      253 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)       28 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)        6 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-18 21:56:05.840374 funcx-2.0.1a2/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     1976 2023-04-18 21:17:41.000000 funcx-2.0.1a2/setup.py
```

### Comparing `funcx-2.0.1a1/LICENSE` & `funcx-2.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.0.1a1/PKG-INFO` & `funcx-2.0.1a2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Source, https://github.com/funcx-faas/funcX
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
+Project-URL: Upgrade to globus-compute-sdk, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving,Globus Compute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `funcx-2.0.1a1/PyPI.md` & `funcx-2.0.1a2/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-2.0.1a1/funcx/version.py` & `funcx-2.0.1a2/funcx/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a1"
+__version__ = "2.0.1a2"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.0.1a1/funcx.egg-info/PKG-INFO` & `funcx-2.0.1a2/funcx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Source, https://github.com/funcx-faas/funcX
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
+Project-URL: Upgrade to globus-compute-sdk, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving,Globus Compute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

