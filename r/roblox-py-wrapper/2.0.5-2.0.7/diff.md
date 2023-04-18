# Comparing `tmp/roblox-py-wrapper-2.0.5.tar.gz` & `tmp/roblox-py-wrapper-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-py-wrapper-2.0.5.tar", last modified: Tue Apr 18 02:25:34 2023, max compression
+gzip compressed data, was "roblox-py-wrapper-2.0.7.tar", last modified: Tue Apr 18 05:01:07 2023, max compression
```

## Comparing `roblox-py-wrapper-2.0.5.tar` & `roblox-py-wrapper-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:25:34.175308 roblox-py-wrapper-2.0.5/
--rw-rw-rw-   0        0        0      296 2023-04-18 02:25:34.174306 roblox-py-wrapper-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-18 02:25:34.175806 roblox-py-wrapper-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:25:17.000000 roblox-py-wrapper-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:25:34.066808 roblox-py-wrapper-2.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:25:34.134312 roblox-py-wrapper-2.0.5/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 roblox-py-wrapper-2.0.5/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 roblox-py-wrapper-2.0.5/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 roblox-py-wrapper-2.0.5/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 roblox-py-wrapper-2.0.5/src/roblox_api_wrapper/message.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:25:34.168819 roblox-py-wrapper-2.0.5/src/roblox_py_wrapper.egg-info/
--rw-rw-rw-   0        0        0      296 2023-04-18 02:25:33.000000 roblox-py-wrapper-2.0.5/src/roblox_py_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-04-18 02:25:33.000000 roblox-py-wrapper-2.0.5/src/roblox_py_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:25:33.000000 roblox-py-wrapper-2.0.5/src/roblox_py_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 02:25:33.000000 roblox-py-wrapper-2.0.5/src/roblox_py_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:01:07.557806 roblox-py-wrapper-2.0.7/
+-rw-rw-rw-   0        0        0      296 2023-04-18 05:01:07.556308 roblox-py-wrapper-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:01:07.557806 roblox-py-wrapper-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-04-18 05:00:59.000000 roblox-py-wrapper-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:01:07.490311 roblox-py-wrapper-2.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:01:07.515311 roblox-py-wrapper-2.0.7/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 roblox-py-wrapper-2.0.7/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 roblox-py-wrapper-2.0.7/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 roblox-py-wrapper-2.0.7/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 roblox-py-wrapper-2.0.7/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:01:07.550806 roblox-py-wrapper-2.0.7/src/roblox_py_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-04-18 05:01:06.000000 roblox-py-wrapper-2.0.7/src/roblox_py_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-04-18 05:01:07.000000 roblox-py-wrapper-2.0.7/src/roblox_py_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:01:06.000000 roblox-py-wrapper-2.0.7/src/roblox_py_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 05:01:06.000000 roblox-py-wrapper-2.0.7/src/roblox_py_wrapper.egg-info/top_level.txt
```

### Comparing `roblox-py-wrapper-2.0.5/setup.py` & `roblox-py-wrapper-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools, base64
 
 
 setuptools.setup(
     name="roblox-py-wrapper",
-    version="2.0.5",
+    version="2.0.7",
     author="roblox-py-wrapper",
     #description="Official python wrapper for the Roblox API (this is a dummy package used to demonstrate vulnerable packages and SHOULD NOT be installed",
     description="Roblox python wrapper",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

