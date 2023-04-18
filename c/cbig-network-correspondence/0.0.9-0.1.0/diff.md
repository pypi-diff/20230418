# Comparing `tmp/cbig_network_correspondence-0.0.9.tar.gz` & `tmp/cbig_network_correspondence-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.0.9.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.1.0.tar", max compression
```

## Comparing `cbig_network_correspondence-0.0.9.tar` & `cbig_network_correspondence-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3180 2023-04-17 09:43:18.799261 cbig_network_correspondence-0.0.9/README.md
--rw-r--r--   0        0        0     2376 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      490 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    14137 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     3143 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0     5430 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    16811 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/README.md
+-rw-r--r--   0        0        0     2303 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    14151 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     3143 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0    12032 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0    18205 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.1.0/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.0.9/pyproject.toml` & `cbig_network_correspondence-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.0.9"
+version = "0.1.0"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
-documentation = "https://rubykong.github.io/cbig_network_correspondence"
 homepage = "https://rubykong.github.io/cbig_network_correspondence"
 repository = "https://github.com/rubykong/cbig_network_correspondence"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
```

### Comparing `cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """"Modules used for calculating overlap between data and atlases"""
 import copy
 from os import path
 from os import listdir
 from natsort import natsorted
 import numpy as np
 import nibabel as nib
-import grab_data_info as grab_info
-import visualize_overlap_lib as vis
+from . import grab_data_info as grab_info
+from . import visualize_overlap_lib as vis
 from scipy.io import loadmat
 
 # define path
 PROJECT_PATH = path.dirname(path.abspath(__file__))
 ATLASES_PATH = path.join(PROJECT_PATH, "data", "atlases")
 NETWORK_ASSIGN_PATH = path.join(PROJECT_PATH, "data", "network_assignment")
 RESULTS_PATH = path.join(PROJECT_PATH, "data", "overlap_results")
```

### Comparing `cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

