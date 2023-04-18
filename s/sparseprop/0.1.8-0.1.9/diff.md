# Comparing `tmp/sparseprop-0.1.8.tar.gz` & `tmp/sparseprop-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparseprop-0.1.8.tar", last modified: Tue Feb 21 10:42:27 2023, max compression
+gzip compressed data, was "dist/sparseprop-0.1.9.tar", last modified: Tue Feb 21 10:56:31 2023, max compression
```

## Comparing `sparseprop-0.1.8.tar` & `sparseprop-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:42:27.000000 sparseprop-0.1.8/
-drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop/
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     3458 2023-02-21 10:36:11.000000 sparseprop-0.1.8/sparseprop/utils.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       14 2023-02-20 15:13:30.000000 sparseprop-0.1.8/sparseprop/__init__.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1482 2023-02-20 14:24:07.000000 sparseprop-0.1.8/sparseprop/backend.cpp
-drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop/modules/
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     6143 2023-02-20 15:24:10.000000 sparseprop-0.1.8/sparseprop/modules/functions.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4571 2023-02-21 10:35:28.000000 sparseprop-0.1.8/sparseprop/modules/__init__.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1913 2023-02-21 10:36:19.000000 sparseprop-0.1.8/sparseprop/modules/linear.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     3654 2023-02-21 10:38:45.000000 sparseprop-0.1.8/sparseprop/modules/conv2d.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      888 2023-02-21 10:34:58.000000 sparseprop-0.1.8/sparseprop/modules/utils.py
-drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop/lib/
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    16755 2023-02-16 17:19:56.000000 sparseprop-0.1.8/sparseprop/lib/sparse_conv2d_over_on.cpp
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     7820 2023-02-17 10:19:37.000000 sparseprop-0.1.8/sparseprop/lib/utils.cpp
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    24140 2023-02-16 17:19:53.000000 sparseprop-0.1.8/sparseprop/lib/sparse_conv2d.cpp
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4460 2023-02-16 17:20:48.000000 sparseprop-0.1.8/sparseprop/lib/sparse_linear.cpp
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4454 2023-02-21 10:17:18.000000 sparseprop-0.1.8/README.md
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       28 2023-02-20 15:29:53.000000 sparseprop-0.1.8/MANIFEST.in
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      705 2023-02-21 10:42:27.000000 sparseprop-0.1.8/PKG-INFO
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    11357 2023-02-16 14:14:57.000000 sparseprop-0.1.8/LICENSE
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1474 2023-02-21 10:17:30.000000 sparseprop-0.1.8/setup.py
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       38 2023-02-21 10:42:27.000000 sparseprop-0.1.8/setup.cfg
-drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)        1 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/dependency_links.txt
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      705 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/PKG-INFO
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       19 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/top_level.txt
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      554 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/SOURCES.txt
--rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       39 2023-02-21 10:42:27.000000 sparseprop-0.1.8/sparseprop.egg-info/requires.txt
+drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:56:31.000000 sparseprop-0.1.9/
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4454 2023-02-21 10:17:18.000000 sparseprop-0.1.9/README.md
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    11357 2023-02-16 14:14:57.000000 sparseprop-0.1.9/LICENSE
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1474 2023-02-21 10:55:44.000000 sparseprop-0.1.9/setup.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      705 2023-02-21 10:56:31.000000 sparseprop-0.1.9/PKG-INFO
+drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop/
+drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop/lib/
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    16755 2023-02-16 17:19:56.000000 sparseprop-0.1.9/sparseprop/lib/sparse_conv2d_over_on.cpp
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4460 2023-02-16 17:20:48.000000 sparseprop-0.1.9/sparseprop/lib/sparse_linear.cpp
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     7820 2023-02-17 10:19:37.000000 sparseprop-0.1.9/sparseprop/lib/utils.cpp
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)    24140 2023-02-16 17:19:53.000000 sparseprop-0.1.9/sparseprop/lib/sparse_conv2d.cpp
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     3485 2023-02-21 10:45:19.000000 sparseprop-0.1.9/sparseprop/utils.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1482 2023-02-20 14:24:07.000000 sparseprop-0.1.9/sparseprop/backend.cpp
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       14 2023-02-20 15:13:30.000000 sparseprop-0.1.9/sparseprop/__init__.py
+drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop/modules/
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      888 2023-02-21 10:34:58.000000 sparseprop-0.1.9/sparseprop/modules/utils.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     1913 2023-02-21 10:36:19.000000 sparseprop-0.1.9/sparseprop/modules/linear.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     3654 2023-02-21 10:38:45.000000 sparseprop-0.1.9/sparseprop/modules/conv2d.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     6143 2023-02-20 15:24:10.000000 sparseprop-0.1.9/sparseprop/modules/functions.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)     4571 2023-02-21 10:35:28.000000 sparseprop-0.1.9/sparseprop/modules/__init__.py
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       28 2023-02-20 15:29:53.000000 sparseprop-0.1.9/MANIFEST.in
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       38 2023-02-21 10:56:31.000000 sparseprop-0.1.9/setup.cfg
+drwxr-sr-x   0 mnikdan  (1005279) alistgrp (1000941)        0 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      554 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/SOURCES.txt
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)      705 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/PKG-INFO
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       19 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/top_level.txt
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)       39 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/requires.txt
+-rw-r--r--   0 mnikdan  (1005279) alistgrp (1000941)        1 2023-02-21 10:56:31.000000 sparseprop-0.1.9/sparseprop.egg-info/dependency_links.txt
```

### Comparing `sparseprop-0.1.8/sparseprop/utils.py` & `sparseprop-0.1.9/sparseprop/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import torch
+from copy import deepcopy
+
 from sparseprop.modules.linear import SparseLinear
 from sparseprop.modules.conv2d import SparseConv2d
 from sparseprop.modules import sparsify_if_faster
 
 @torch.no_grad()
 def sparsity(module):
     if hasattr(module, 'weight'):
```

### Comparing `sparseprop-0.1.8/sparseprop/backend.cpp` & `sparseprop-0.1.9/sparseprop/backend.cpp`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/modules/functions.py` & `sparseprop-0.1.9/sparseprop/modules/functions.py`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/modules/__init__.py` & `sparseprop-0.1.9/sparseprop/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/modules/linear.py` & `sparseprop-0.1.9/sparseprop/modules/linear.py`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/modules/conv2d.py` & `sparseprop-0.1.9/sparseprop/modules/conv2d.py`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/modules/utils.py` & `sparseprop-0.1.9/sparseprop/modules/utils.py`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/lib/sparse_conv2d_over_on.cpp` & `sparseprop-0.1.9/sparseprop/lib/sparse_conv2d_over_on.cpp`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/lib/utils.cpp` & `sparseprop-0.1.9/sparseprop/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/lib/sparse_conv2d.cpp` & `sparseprop-0.1.9/sparseprop/lib/sparse_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/sparseprop/lib/sparse_linear.cpp` & `sparseprop-0.1.9/sparseprop/lib/sparse_linear.cpp`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/README.md` & `sparseprop-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/PKG-INFO` & `sparseprop-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseprop
-Version: 0.1.8
+Version: 0.1.9
 Summary: SparseProp: Efficient Sparse Backpropagation for Faster Training of Neural Networks
 Home-page: https://github.com/IST-DASLab/sparseprop
 Author: Mahdi Nikdan, Tommaso Pegolotti, Eugenia Iofinova, Eldar Kurtic, Dan Alistarh
 Author-email: mahdi.nikdan@ist.ac.at, tommaso.pegolotti@inf.ethz.ch, eugenia.iofinova@ist.ac.at, eldar.kurtic@ist.ac.at, dan.alistarh@ist.ac.at
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sparseprop-0.1.8/LICENSE` & `sparseprop-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sparseprop-0.1.8/setup.py` & `sparseprop-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 proc = subprocess.Popen(["python3 -m pybind11 --includes"], stdout=subprocess.PIPE, shell=True)
 (out, err) = proc.communicate()
 out = out.decode('ascii').strip().split()
 
 setup(
     name='sparseprop',
-    version='0.1.8',    
+    version='0.1.9',    
     description='SparseProp: Efficient Sparse Backpropagation for Faster Training of Neural Networks',
     url='https://github.com/IST-DASLab/sparseprop',
     author='Mahdi Nikdan, Tommaso Pegolotti, Eugenia Iofinova, Eldar Kurtic, Dan Alistarh',
     author_email='mahdi.nikdan@ist.ac.at, tommaso.pegolotti@inf.ethz.ch, eugenia.iofinova@ist.ac.at, eldar.kurtic@ist.ac.at, dan.alistarh@ist.ac.at',
     license='Apache License 2.0',
     packages=find_packages(exclude=['tests', 'tests.*']),
     ext_modules=[Extension(
```

### Comparing `sparseprop-0.1.8/sparseprop.egg-info/PKG-INFO` & `sparseprop-0.1.9/sparseprop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseprop
-Version: 0.1.8
+Version: 0.1.9
 Summary: SparseProp: Efficient Sparse Backpropagation for Faster Training of Neural Networks
 Home-page: https://github.com/IST-DASLab/sparseprop
 Author: Mahdi Nikdan, Tommaso Pegolotti, Eugenia Iofinova, Eldar Kurtic, Dan Alistarh
 Author-email: mahdi.nikdan@ist.ac.at, tommaso.pegolotti@inf.ethz.ch, eugenia.iofinova@ist.ac.at, eldar.kurtic@ist.ac.at, dan.alistarh@ist.ac.at
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sparseprop-0.1.8/sparseprop.egg-info/SOURCES.txt` & `sparseprop-0.1.9/sparseprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

