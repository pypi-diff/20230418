# Comparing `tmp/measure_dist-1.1.0.tar.gz` & `tmp/measure_dist-1.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "measure_dist-1.1.0.tar", last modified: Mon Apr 17 22:32:56 2023, max compression
+gzip compressed data, was "measure_dist-1.1.0.post1.tar", last modified: Tue Apr 18 07:44:33 2023, max compression
```

## Comparing `measure_dist-1.1.0.tar` & `measure_dist-1.1.0.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-17 22:32:56.631409 measure_dist-1.1.0/
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1063 2023-03-30 20:23:28.000000 measure_dist-1.1.0/LICENSE
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      117 2023-04-06 23:03:29.000000 measure_dist-1.1.0/MANIFEST.in
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1692 2023-04-17 22:32:56.631409 measure_dist-1.1.0/PKG-INFO
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       28 2023-04-06 23:04:54.000000 measure_dist-1.1.0/README.md
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      618 2023-04-17 22:32:26.000000 measure_dist-1.1.0/pyproject.toml
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       38 2023-04-17 22:32:56.631409 measure_dist-1.1.0/setup.cfg
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       37 2023-03-30 22:27:10.000000 measure_dist-1.1.0/setup.py
-drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-17 22:32:56.627409 measure_dist-1.1.0/src/
-drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-17 22:32:56.631409 measure_dist-1.1.0/src/measure_dist/
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       27 2023-04-06 23:15:40.000000 measure_dist-1.1.0/src/measure_dist/__init__.py
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    14579 2023-04-17 22:30:56.000000 measure_dist-1.1.0/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.h
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)  2849520 2023-04-17 22:30:56.000000 measure_dist-1.1.0/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.so
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    13836 2023-04-06 23:00:42.000000 measure_dist-1.1.0/src/measure_dist/build.py
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    49005 2023-04-06 23:00:42.000000 measure_dist-1.1.0/src/measure_dist/go.py
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    97991 2023-04-06 23:00:45.000000 measure_dist-1.1.0/src/measure_dist/measure_dist.c
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    32955 2023-04-06 23:00:42.000000 measure_dist-1.1.0/src/measure_dist/measure_dist.go
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    10564 2023-04-17 22:09:58.000000 measure_dist-1.1.0/src/measure_dist/measure_dist.py
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    11862 2023-04-06 23:00:45.000000 measure_dist-1.1.0/src/measure_dist/measure_dist_go.h
-drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-17 22:32:56.631409 measure_dist-1.1.0/src/measure_dist.egg-info/
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1692 2023-04-17 22:32:56.000000 measure_dist-1.1.0/src/measure_dist.egg-info/PKG-INFO
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      588 2023-04-17 22:32:56.000000 measure_dist-1.1.0/src/measure_dist.egg-info/SOURCES.txt
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)        1 2023-04-17 22:32:56.000000 measure_dist-1.1.0/src/measure_dist.egg-info/dependency_links.txt
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       10 2023-04-17 22:32:56.000000 measure_dist-1.1.0/src/measure_dist.egg-info/requires.txt
--rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       13 2023-04-17 22:32:56.000000 measure_dist-1.1.0/src/measure_dist.egg-info/top_level.txt
+drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-18 07:44:33.357757 measure_dist-1.1.0.post1/
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1063 2023-03-30 20:23:28.000000 measure_dist-1.1.0.post1/LICENSE
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      117 2023-04-06 23:03:29.000000 measure_dist-1.1.0.post1/MANIFEST.in
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1698 2023-04-18 07:44:33.357757 measure_dist-1.1.0.post1/PKG-INFO
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       28 2023-04-06 23:04:54.000000 measure_dist-1.1.0.post1/README.md
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      620 2023-04-18 07:44:17.000000 measure_dist-1.1.0.post1/pyproject.toml
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       38 2023-04-18 07:44:33.357757 measure_dist-1.1.0.post1/setup.cfg
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       37 2023-03-30 22:27:10.000000 measure_dist-1.1.0.post1/setup.py
+drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-18 07:44:33.353757 measure_dist-1.1.0.post1/src/
+drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-18 07:44:33.357757 measure_dist-1.1.0.post1/src/measure_dist/
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1483 2023-04-18 07:32:40.000000 measure_dist-1.1.0.post1/src/measure_dist/__init__.py
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    14579 2023-04-17 22:30:56.000000 measure_dist-1.1.0.post1/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.h
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)  2849520 2023-04-17 22:30:56.000000 measure_dist-1.1.0.post1/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.so
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    13836 2023-04-06 23:00:42.000000 measure_dist-1.1.0.post1/src/measure_dist/build.py
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    49005 2023-04-06 23:00:42.000000 measure_dist-1.1.0.post1/src/measure_dist/go.py
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    97991 2023-04-06 23:00:45.000000 measure_dist-1.1.0.post1/src/measure_dist/measure_dist.c
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    32955 2023-04-06 23:00:42.000000 measure_dist-1.1.0.post1/src/measure_dist/measure_dist.go
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    10564 2023-04-17 22:09:58.000000 measure_dist-1.1.0.post1/src/measure_dist/measure_dist.py
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)    11862 2023-04-06 23:00:45.000000 measure_dist-1.1.0.post1/src/measure_dist/measure_dist_go.h
+drwxrwxr-x   0 gmnx      (1000) gmnx      (1000)        0 2023-04-18 07:44:33.357757 measure_dist-1.1.0.post1/src/measure_dist.egg-info/
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)     1698 2023-04-18 07:44:33.000000 measure_dist-1.1.0.post1/src/measure_dist.egg-info/PKG-INFO
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)      588 2023-04-18 07:44:33.000000 measure_dist-1.1.0.post1/src/measure_dist.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)        1 2023-04-18 07:44:33.000000 measure_dist-1.1.0.post1/src/measure_dist.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       10 2023-04-18 07:44:33.000000 measure_dist-1.1.0.post1/src/measure_dist.egg-info/requires.txt
+-rw-rw-r--   0 gmnx      (1000) gmnx      (1000)       13 2023-04-18 07:44:33.000000 measure_dist-1.1.0.post1/src/measure_dist.egg-info/top_level.txt
```

### Comparing `measure_dist-1.1.0/LICENSE` & `measure_dist-1.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/PKG-INFO` & `measure_dist-1.1.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: measure_dist
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Measurement helper functions
 Author-email: Gegeco <gegeco06@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 gegeco
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `measure_dist-1.1.0/pyproject.toml` & `measure_dist-1.1.0.post1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "measure_dist"
-version = "1.1.0"
+version = "1.1.0-1"
 description = "Measurement helper functions"
 readme = "README.md"
 authors = [{ name = "Gegeco", email = "gegeco06@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `measure_dist-1.1.0/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.h` & `measure_dist-1.1.0.post1/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.h`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.so` & `measure_dist-1.1.0.post1/src/measure_dist/_measure_dist.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/build.py` & `measure_dist-1.1.0.post1/src/measure_dist/build.py`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/go.py` & `measure_dist-1.1.0.post1/src/measure_dist/go.py`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/measure_dist.c` & `measure_dist-1.1.0.post1/src/measure_dist/measure_dist.c`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/measure_dist.go` & `measure_dist-1.1.0.post1/src/measure_dist/measure_dist.go`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/measure_dist.py` & `measure_dist-1.1.0.post1/src/measure_dist/measure_dist.py`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist/measure_dist_go.h` & `measure_dist-1.1.0.post1/src/measure_dist/measure_dist_go.h`

 * *Files identical despite different names*

### Comparing `measure_dist-1.1.0/src/measure_dist.egg-info/PKG-INFO` & `measure_dist-1.1.0.post1/src/measure_dist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: measure-dist
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Measurement helper functions
 Author-email: Gegeco <gegeco06@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 gegeco
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `measure_dist-1.1.0/src/measure_dist.egg-info/SOURCES.txt` & `measure_dist-1.1.0.post1/src/measure_dist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

