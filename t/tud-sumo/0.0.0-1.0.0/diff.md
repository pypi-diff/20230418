# Comparing `tmp/tud_sumo-0.0.0.tar.gz` & `tmp/tud_sumo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-0.0.0.tar", last modified: Tue Apr 18 16:10:58 2023, max compression
+gzip compressed data, was "tud_sumo-1.0.0.tar", last modified: Tue Apr 18 16:17:38 2023, max compression
```

## Comparing `tud_sumo-0.0.0.tar` & `tud_sumo-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:10:58.610087 tud_sumo-0.0.0/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-0.0.0/.gitattributes
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:10:58.607725 tud_sumo-0.0.0/.github/
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:10:58.608896 tud_sumo-0.0.0/.github/workflows/
--rw-r--r--   0 callumevans (50765939) 1653728465     1084 2023-04-18 15:38:19.000000 tud_sumo-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 callumevans (50765939) 1653728465        8 2023-04-18 15:02:55.000000 tud_sumo-0.0.0/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-0.0.0/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:10:58.609937 tud_sumo-0.0.0/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      760 2023-04-18 15:15:39.000000 tud_sumo-0.0.0/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      532 2023-04-18 16:09:04.000000 tud_sumo-0.0.0/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-04-18 16:10:58.610134 tud_sumo-0.0.0/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-0.0.0/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:10:58.609017 tud_sumo-0.0.0/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    22888 2023-04-18 15:04:51.000000 tud_sumo-0.0.0/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:10:58.609712 tud_sumo-0.0.0/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:10:58.000000 tud_sumo-0.0.0/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      284 2023-04-18 16:10:58.000000 tud_sumo-0.0.0/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-04-18 16:10:58.000000 tud_sumo-0.0.0/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-04-18 16:10:58.000000 tud_sumo-0.0.0/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-04-18 16:10:58.000000 tud_sumo-0.0.0/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.571575 tud_sumo-1.0.0/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.0.0/.gitattributes
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.569332 tud_sumo-1.0.0/.github/
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.570456 tud_sumo-1.0.0/.github/workflows/
+-rw-r--r--   0 callumevans (50765939) 1653728465     1084 2023-04-18 15:38:19.000000 tud_sumo-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 callumevans (50765939) 1653728465        8 2023-04-18 15:02:55.000000 tud_sumo-1.0.0/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.0.0/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:17:38.571428 tud_sumo-1.0.0/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      760 2023-04-18 15:15:39.000000 tud_sumo-1.0.0/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-04-18 16:17:33.000000 tud_sumo-1.0.0/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-04-18 16:17:38.571619 tud_sumo-1.0.0/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.0.0/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.570585 tud_sumo-1.0.0/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    22888 2023-04-18 15:04:51.000000 tud_sumo-1.0.0/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.571231 tud_sumo-1.0.0/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      284 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-0.0.0/.github/workflows/python-publish.yml` & `tud_sumo-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tud_sumo-0.0.0/LICENSE` & `tud_sumo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-0.0.0/PKG-INFO` & `tud_sumo-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud_sumo
-Version: 0.0.0
+Version: 1.0.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tud_sumo-0.0.0/README.md` & `tud_sumo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tud_sumo-0.0.0/pyproject.toml` & `tud_sumo-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
+version = "1.0.0"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "traci", "matplotlib", "tqdm",
-]
-dynamic = ["version"]
+]
```

### Comparing `tud_sumo-0.0.0/tud_sumo/tud_sumo.py` & `tud_sumo-1.0.0/tud_sumo/tud_sumo.py`

 * *Files identical despite different names*

### Comparing `tud_sumo-0.0.0/tud_sumo.egg-info/PKG-INFO` & `tud_sumo-1.0.0/tud_sumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud-sumo
-Version: 0.0.0
+Version: 1.0.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

