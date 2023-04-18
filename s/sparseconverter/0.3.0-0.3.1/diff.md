# Comparing `tmp/sparseconverter-0.3.0.tar.gz` & `tmp/sparseconverter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparseconverter-0.3.0.tar", last modified: Tue Feb  7 07:19:42 2023, max compression
+gzip compressed data, was "sparseconverter-0.3.1.tar", last modified: Tue Apr 18 12:52:48 2023, max compression
```

## Comparing `sparseconverter-0.3.0.tar` & `sparseconverter-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-07 07:19:33.000000 sparseconverter-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-07 07:19:33.000000 sparseconverter-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-07 07:19:33.000000 sparseconverter-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/src/sparseconverter/
--rw-r--r--   0 runner    (1001) docker     (123)    46727 2023-02-07 07:19:33.000000 sparseconverter-0.3.0/src/sparseconverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/src/sparseconverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-02-07 07:19:42.000000 sparseconverter-0.3.0/src/sparseconverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-07 07:19:42.000000 sparseconverter-0.3.0/src/sparseconverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 07:19:42.000000 sparseconverter-0.3.0/src/sparseconverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-07 07:19:42.000000 sparseconverter-0.3.0/src/sparseconverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-07 07:19:42.000000 sparseconverter-0.3.0/src/sparseconverter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:19:42.375157 sparseconverter-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-02-07 07:19:33.000000 sparseconverter-0.3.0/tests/test_sparseconverters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/sparseconverter/
+-rw-r--r--   0 runner    (1001) docker     (123)    46727 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/src/sparseconverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/sparseconverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/tests/test_sparseconverters.py
```

### Comparing `sparseconverter-0.3.0/LICENSE` & `sparseconverter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparseconverter-0.3.0/PKG-INFO` & `sparseconverter-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.1
+
+* Include version constraint for `sparse`.
+
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
   between two backends.
 
 ### 0.2.0
```

### Comparing `sparseconverter-0.3.0/README.md` & `sparseconverter-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.1
+
+* Include version constraint for `sparse`.
+
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
   between two backends.
 
 ### 0.2.0
```

### Comparing `sparseconverter-0.3.0/pyproject.toml` & `sparseconverter-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 license = {file = "LICENSE"}
 keywords = ["numpy", "scipy.sparse", "sparse", "array", "matrix", "cupy", "cupyx.scipy.sparse"]
 requires-python = ">=3.7"
 dynamic = ["version", "readme"]
 dependencies = [
     "numpy",
     "scipy",
-    "sparse",
+    "sparse>=0.12",
     "typing-extensions",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `sparseconverter-0.3.0/src/sparseconverter/__init__.py` & `sparseconverter-0.3.1/src/sparseconverter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Literal
 
 import numpy as np
 import scipy.sparse as sp
 import sparse
 
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 NUMPY = 'numpy'
 NUMPY_MATRIX = 'numpy.matrix'
 CUDA = 'cuda'
 CUPY = 'cupy'
 SPARSE_COO = 'sparse.COO'
 SPARSE_GCXS = 'sparse.GCXS'
```

### Comparing `sparseconverter-0.3.0/src/sparseconverter.egg-info/PKG-INFO` & `sparseconverter-0.3.1/src/sparseconverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.1
+
+* Include version constraint for `sparse`.
+
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
   between two backends.
 
 ### 0.2.0
```

### Comparing `sparseconverter-0.3.0/tests/test_sparseconverters.py` & `sparseconverter-0.3.1/tests/test_sparseconverters.py`

 * *Files identical despite different names*

