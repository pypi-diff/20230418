# Comparing `tmp/kiwigrad-0.16.tar.gz` & `tmp/kiwigrad-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.16.tar", last modified: Sun Apr  9 13:08:51 2023, max compression
+gzip compressed data, was "kiwigrad-0.17.tar", last modified: Mon Apr 17 22:31:47 2023, max compression
```

## Comparing `kiwigrad-0.16.tar` & `kiwigrad-0.17.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.688492 kiwigrad-0.16/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.16/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.16/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 13:08:51.688051 kiwigrad-0.16/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.16/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.685555 kiwigrad-0.16/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-04-09 13:07:23.000000 kiwigrad-0.16/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.16/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.16/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3963 2023-04-09 13:05:19.000000 kiwigrad-0.16/kiwigrad/nn.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.687480 kiwigrad-0.16/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      276 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-09 13:08:03.000000 kiwigrad-0.16/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 13:08:51.688640 kiwigrad-0.16/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.910502 kiwigrad-0.17/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.17/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.17/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-17 22:31:47.909969 kiwigrad-0.17/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.17/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.907831 kiwigrad-0.17/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-04-17 22:25:10.000000 kiwigrad-0.17/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.17/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.17/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5514 2023-04-17 22:24:41.000000 kiwigrad-0.17/kiwigrad/nn.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.909442 kiwigrad-0.17/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      276 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-17 22:24:58.000000 kiwigrad-0.17/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-17 22:31:47.910661 kiwigrad-0.17/setup.cfg
```

### Comparing `kiwigrad-0.16/LICENSE` & `kiwigrad-0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.16/PKG-INFO` & `kiwigrad-0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.16
+Version: 0.17
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.16/kiwigrad/engine.py` & `kiwigrad-0.17/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.16/kiwigrad/graph.py` & `kiwigrad-0.17/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.16/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.17/kiwigrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.16
+Version: 0.17
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.16/pyproject.toml` & `kiwigrad-0.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.16"
+version = "0.17"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

