# Comparing `tmp/icecube-skyreader-0.1.0.tar.gz` & `tmp/icecube-skyreader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-0.1.0.tar", last modified: Tue Apr 18 19:43:41 2023, max compression
+gzip compressed data, was "icecube-skyreader-0.1.1.tar", last modified: Tue Apr 18 19:48:50 2023, max compression
```

## Comparing `icecube-skyreader-0.1.0.tar` & `icecube-skyreader-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:43:41.776216 icecube-skyreader-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1975 2023-04-18 19:43:41.776216 icecube-skyreader-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:43:41.772216 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1975 2023-04-18 19:43:41.000000 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-18 19:43:41.000000 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 19:43:41.000000 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-18 19:43:41.000000 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 19:43:41.000000 icecube-skyreader-0.1.0/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1750 2023-04-18 19:43:41.776216 icecube-skyreader-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:43:41.776216 icecube-skyreader-0.1.0/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 19:43:39.000000 icecube-skyreader-0.1.0/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:43:41.776216 icecube-skyreader-0.1.0/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9066 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47132 2023-04-18 19:43:38.000000 icecube-skyreader-0.1.0/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.552802 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 19:48:50.000000 icecube-skyreader-0.1.1/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.552802 icecube-skyreader-0.1.1/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 19:48:48.000000 icecube-skyreader-0.1.1/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:48:50.556802 icecube-skyreader-0.1.1/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9066 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    47132 2023-04-18 19:48:47.000000 icecube-skyreader-0.1.1/skyreader/result.py
```

### Comparing `icecube-skyreader-0.1.0/LICENSE` & `icecube-skyreader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.0/PKG-INFO` & `icecube-skyreader-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
 Project-URL: Source, https://github.com/icecube/skyreader
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skyreader-0.1.0/README.md` & `icecube-skyreader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.0/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-0.1.1/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
 Project-URL: Source, https://github.com/icecube/skyreader
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skyreader-0.1.0/setup.cfg` & `icecube-skyreader-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	skymap
 	HEALPix
 	neutrino
 	reconstruction
 	IceCube
 license = MIT
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 download_url = https://pypi.org/project/icecube-skyreader/
 project_urls =
```

### Comparing `icecube-skyreader-0.1.0/skyreader/__init__.py` & `icecube-skyreader-0.1.1/skyreader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-0.1.0/skyreader/event_metadata.py` & `icecube-skyreader-0.1.1/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.0/skyreader/plot/plotting_tools.py` & `icecube-skyreader-0.1.1/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-0.1.0/skyreader/result.py` & `icecube-skyreader-0.1.1/skyreader/result.py`

 * *Files identical despite different names*

