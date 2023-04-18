# Comparing `tmp/torch-interpol-0.2.2.tar.gz` & `tmp/torch-interpol-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch-interpol-0.2.2.tar", last modified: Tue Apr 18 00:39:05 2023, max compression
+gzip compressed data, was "dist/torch-interpol-0.2.3.tar", last modified: Tue Apr 18 00:46:50 2023, max compression
```

## Comparing `torch-interpol-0.2.2.tar` & `torch-interpol-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18789 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/iso0.py
--rw-r--r--   0 runner    (1001) docker     (123)    42938 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/iso1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/jit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/jitfields.py
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/nd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/pushpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/restrict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/tests/test_gradcheck_pushpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/interpol/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/interpol/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18789 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/iso0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42938 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/iso1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/jit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/jitfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/restrict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/interpol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/tests/test_gradcheck_pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/interpol/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 00:46:50.000000 torch-interpol-0.2.3/torch_interpol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-18 00:46:08.000000 torch-interpol-0.2.3/versioneer.py
```

### Comparing `torch-interpol-0.2.2/LICENSE` & `torch-interpol-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/PKG-INFO` & `torch-interpol-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-interpol
-Version: 0.2.2
+Version: 0.2.3
 Summary: High-order spline interpolation in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-interpol
 Description: # torch-interpol
```

### Comparing `torch-interpol-0.2.2/README.md` & `torch-interpol-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/api.py` & `torch-interpol-0.2.3/interpol/api.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/autograd.py` & `torch-interpol-0.2.3/interpol/autograd.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/bounds.py` & `torch-interpol-0.2.3/interpol/bounds.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/coeff.py` & `torch-interpol-0.2.3/interpol/coeff.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/iso0.py` & `torch-interpol-0.2.3/interpol/iso0.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/iso1.py` & `torch-interpol-0.2.3/interpol/iso1.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/jit_utils.py` & `torch-interpol-0.2.3/interpol/jit_utils.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/jitfields.py` & `torch-interpol-0.2.3/interpol/jitfields.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/nd.py` & `torch-interpol-0.2.3/interpol/nd.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/pushpull.py` & `torch-interpol-0.2.3/interpol/pushpull.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/resize.py` & `torch-interpol-0.2.3/interpol/resize.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/restrict.py` & `torch-interpol-0.2.3/interpol/restrict.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/splines.py` & `torch-interpol-0.2.3/interpol/splines.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/tests/test_gradcheck_pushpull.py` & `torch-interpol-0.2.3/interpol/tests/test_gradcheck_pushpull.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/interpol/utils.py` & `torch-interpol-0.2.3/interpol/utils.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/setup.cfg` & `torch-interpol-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/torch_interpol.egg-info/PKG-INFO` & `torch-interpol-0.2.3/torch_interpol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-interpol
-Version: 0.2.2
+Version: 0.2.3
 Summary: High-order spline interpolation in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-interpol
 Description: # torch-interpol
```

### Comparing `torch-interpol-0.2.2/torch_interpol.egg-info/SOURCES.txt` & `torch-interpol-0.2.3/torch_interpol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.2/versioneer.py` & `torch-interpol-0.2.3/versioneer.py`

 * *Files identical despite different names*

