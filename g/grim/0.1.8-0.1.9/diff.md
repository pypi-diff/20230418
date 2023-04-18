# Comparing `tmp/grim-0.1.8.tar.gz` & `tmp/grim-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grim-0.1.8.tar", last modified: Mon Apr 17 19:06:55 2023, max compression
+gzip compressed data, was "grim-0.1.9.tar", last modified: Tue Apr 18 18:11:52 2023, max compression
```

## Comparing `grim-0.1.8.tar` & `grim-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:06:55.969397 grim-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 19:06:45.000000 grim-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-17 19:06:55.969397 grim-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-17 19:06:45.000000 grim-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:06:55.965397 grim-0.1.8/grim/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 19:06:45.000000 grim-0.1.8/grim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-17 19:06:45.000000 grim-0.1.8/grim/mean_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:06:55.965397 grim-0.1.8/grim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-17 19:06:55.000000 grim-0.1.8/grim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 19:06:55.000000 grim-0.1.8/grim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:06:55.000000 grim-0.1.8/grim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 19:06:55.000000 grim-0.1.8/grim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:06:55.969397 grim-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 19:06:45.000000 grim-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:11:52.061955 grim-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 18:11:43.000000 grim-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-18 18:11:52.061955 grim-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-18 18:11:43.000000 grim-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:11:52.061955 grim-0.1.9/grim/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 18:11:43.000000 grim-0.1.9/grim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-18 18:11:43.000000 grim-0.1.9/grim/mean_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:11:52.061955 grim-0.1.9/grim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-18 18:11:52.000000 grim-0.1.9/grim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 18:11:52.000000 grim-0.1.9/grim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:11:52.000000 grim-0.1.9/grim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 18:11:52.000000 grim-0.1.9/grim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:11:52.061955 grim-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 18:11:43.000000 grim-0.1.9/setup.py
```

### Comparing `grim-0.1.8/LICENSE` & `grim-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grim-0.1.8/grim/mean_tester.py` & `grim-0.1.9/grim/mean_tester.py`

 * *Files identical despite different names*

### Comparing `grim-0.1.8/setup.py` & `grim-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grim",
-    version="0.1.8",
+    version="0.1.9",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="An implementation of the GRIM test, in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/grim_test",
     packages=setuptools.find_packages(),
```

