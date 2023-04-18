# Comparing `tmp/hsf-1.1.2.tar.gz` & `tmp/hsf-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsf-1.1.2.tar", max compression
+gzip compressed data, was "hsf-1.1.3.tar", max compression
```

## Comparing `hsf-1.1.2.tar` & `hsf-1.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1072 2023-04-18 07:38:21.317162 hsf-1.1.2/LICENSE.md
--rw-r--r--   0        0        0    10971 2023-04-18 11:32:34.270968 hsf-1.1.2/README.rst
--rw-r--r--   0        0        0       22 2023-04-18 09:59:42.848045 hsf-1.1.2/hsf/__init__.py
--rw-r--r--   0        0        0     1946 2023-04-18 08:46:28.068106 hsf-1.1.2/hsf/augmentation.py
--rw-r--r--   0        0        0        0 2023-04-18 07:38:21.351163 hsf-1.1.2/hsf/conf/__init__.py
--rw-r--r--   0        0        0      244 2023-04-18 07:38:21.351163 hsf-1.1.2/hsf/conf/augmentation/default.yaml
--rw-r--r--   0        0        0      202 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/config.yaml
--rw-r--r--   0        0        0       78 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/files/default.yaml
--rw-r--r--   0        0        0       67 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hardware/deepsparse.yaml
--rw-r--r--   0        0        0      126 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hardware/onnxruntime.yaml
--rw-r--r--   0        0        0     1514 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hydra/help/hsf.yaml
--rw-r--r--   0        0        0       75 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/multispectrality/default.yaml
--rw-r--r--   0        0        0      139 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/roiloc/default_corot2.yaml
--rw-r--r--   0        0        0      137 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/roiloc/default_t2iso.yaml
--rw-r--r--   0        0        0      951 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_accurate.yaml
--rw-r--r--   0        0        0      955 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_fast.yaml
--rw-r--r--   0        0        0     1112 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_sq.yaml
--rw-r--r--   0        0        0      393 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_accurate.yaml
--rw-r--r--   0        0        0      398 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_fast.yaml
--rw-r--r--   0        0        0      506 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_sq.yaml
--rw-r--r--   0        0        0     4322 2023-04-18 10:07:31.648039 hsf-1.1.2/hsf/engines.py
--rw-r--r--   0        0        0     7646 2023-04-18 08:47:20.656105 hsf-1.1.2/hsf/factory.py
--rw-r--r--   0        0        0     1887 2023-04-18 08:47:28.240105 hsf-1.1.2/hsf/fetch_models.py
--rw-r--r--   0        0        0     3769 2023-04-18 08:45:26.889107 hsf-1.1.2/hsf/multispectrality.py
--rw-r--r--   0        0        0     3377 2023-04-18 08:45:37.718107 hsf-1.1.2/hsf/roiloc_wrapper.py
--rw-r--r--   0        0        0     5743 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/segment.py
--rw-r--r--   0        0        0     1017 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/uncertainty.py
--rw-r--r--   0        0        0     2357 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/welcome.py
--rw-r--r--   0        0        0     1520 2023-04-18 11:49:31.103954 hsf-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    12381 1970-01-01 00:00:00.000000 hsf-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-18 07:38:21.317162 hsf-1.1.3/LICENSE.md
+-rw-r--r--   0        0        0    11035 2023-04-18 18:14:24.612380 hsf-1.1.3/README.rst
+-rw-r--r--   0        0        0       22 2023-04-18 18:13:27.650034 hsf-1.1.3/hsf/__init__.py
+-rw-r--r--   0        0        0     1946 2023-04-18 08:46:28.068106 hsf-1.1.3/hsf/augmentation.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:38:21.351163 hsf-1.1.3/hsf/conf/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-18 07:38:21.351163 hsf-1.1.3/hsf/conf/augmentation/default.yaml
+-rw-r--r--   0        0        0      202 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/config.yaml
+-rw-r--r--   0        0        0       78 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/files/default.yaml
+-rw-r--r--   0        0        0       67 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/hardware/deepsparse.yaml
+-rw-r--r--   0        0        0      126 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/hardware/onnxruntime.yaml
+-rw-r--r--   0        0        0     1514 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/hydra/help/hsf.yaml
+-rw-r--r--   0        0        0       75 2023-04-18 07:38:21.352162 hsf-1.1.3/hsf/conf/multispectrality/default.yaml
+-rw-r--r--   0        0        0      139 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/roiloc/default_corot2.yaml
+-rw-r--r--   0        0        0      137 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/roiloc/default_t2iso.yaml
+-rw-r--r--   0        0        0      951 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/bagging_accurate.yaml
+-rw-r--r--   0        0        0      955 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/bagging_fast.yaml
+-rw-r--r--   0        0        0     1112 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/bagging_sq.yaml
+-rw-r--r--   0        0        0      393 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/single_accurate.yaml
+-rw-r--r--   0        0        0      398 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/single_fast.yaml
+-rw-r--r--   0        0        0      506 2023-04-18 07:38:21.353162 hsf-1.1.3/hsf/conf/segmentation/single_sq.yaml
+-rw-r--r--   0        0        0     4322 2023-04-18 10:07:31.648039 hsf-1.1.3/hsf/engines.py
+-rw-r--r--   0        0        0     7646 2023-04-18 08:47:20.656105 hsf-1.1.3/hsf/factory.py
+-rw-r--r--   0        0        0     1887 2023-04-18 08:47:28.240105 hsf-1.1.3/hsf/fetch_models.py
+-rw-r--r--   0        0        0     3769 2023-04-18 08:45:26.889107 hsf-1.1.3/hsf/multispectrality.py
+-rw-r--r--   0        0        0     3377 2023-04-18 08:45:37.718107 hsf-1.1.3/hsf/roiloc_wrapper.py
+-rw-r--r--   0        0        0     5743 2023-04-18 07:38:21.355162 hsf-1.1.3/hsf/segment.py
+-rw-r--r--   0        0        0     1017 2023-04-18 07:38:21.355162 hsf-1.1.3/hsf/uncertainty.py
+-rw-r--r--   0        0        0     2357 2023-04-18 07:38:21.355162 hsf-1.1.3/hsf/welcome.py
+-rw-r--r--   0        0        0     1736 2023-04-18 18:13:09.443839 hsf-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    12429 1970-01-01 00:00:00.000000 hsf-1.1.3/PKG-INFO
```

### Comparing `hsf-1.1.2/LICENSE.md` & `hsf-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/README.rst` & `hsf-1.1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,18 @@
 
 Changelogs
 ==========
 
 HSF
 ---
 
+**Version 1.1.3**
+
+* Lower onnxruntime dependency to min 1.8.0
+
 **Version 1.1.2**
 
 * ***BREAKING CHANGE***: HSF needs to be installed using extra dependencies depending on the backend you want to use.
   See the [installation guide](https://hsf.readthedocs.io/en/latest/user-guide/installation/) for more details.
 * Updated dependencies
 * Fixed installation on MacOS
```

### Comparing `hsf-1.1.2/hsf/augmentation.py` & `hsf-1.1.3/hsf/augmentation.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/conf/hydra/help/hsf.yaml` & `hsf-1.1.3/hsf/conf/hydra/help/hsf.yaml`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/conf/segmentation/bagging_accurate.yaml` & `hsf-1.1.3/hsf/conf/segmentation/bagging_accurate.yaml`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/conf/segmentation/bagging_fast.yaml` & `hsf-1.1.3/hsf/conf/segmentation/bagging_fast.yaml`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/conf/segmentation/bagging_sq.yaml` & `hsf-1.1.3/hsf/conf/segmentation/bagging_sq.yaml`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/engines.py` & `hsf-1.1.3/hsf/engines.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/factory.py` & `hsf-1.1.3/hsf/factory.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/fetch_models.py` & `hsf-1.1.3/hsf/fetch_models.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/multispectrality.py` & `hsf-1.1.3/hsf/multispectrality.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/roiloc_wrapper.py` & `hsf-1.1.3/hsf/roiloc_wrapper.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/segment.py` & `hsf-1.1.3/hsf/segment.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/uncertainty.py` & `hsf-1.1.3/hsf/uncertainty.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/hsf/welcome.py` & `hsf-1.1.3/hsf/welcome.py`

 * *Files identical despite different names*

### Comparing `hsf-1.1.2/pyproject.toml` & `hsf-1.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HSF"
-version = "1.1.2"
+version = "1.1.3"
 description = "A simple yet exhaustive segmentation tool of the Hippocampal Subfields in T1w and T2w MRIs."
 authors = ["Clément POIRET <poiret.clement@outlook.fr>"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["mri", "brain", "hippocampus", "segmentation", "deep learning"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -24,16 +24,16 @@
 torchio = "^0.18.56"
 roiloc = ">0.2.8"
 hydra-core = "^1.1.1"
 wget = "^3.2"
 antspyx = ">0.3.0"
 xxhash = "^3.2.0"
 rich = ">11.0.0"
-onnxruntime = {version = "^1.14.0", optional = true}
-onnxruntime-gpu = {version = "^1.14.0", optional = true}
+onnxruntime = {version = ">=1.8.0", optional = true}
+onnxruntime-gpu = {version = ">=1.8.0", optional = true}
 deepsparse = {version = "^1.4.0", optional = true}
 
 [tool.poetry.extras]
 cpu = ["onnxruntime"]
 gpu = ["onnxruntime-gpu"]
 sparse = ["deepsparse", "onnxruntime"]
 
@@ -46,7 +46,11 @@
 
 [tool.coverage.report]
 omit = ["hsf/welcome.py"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+# The command to install deps manually
+# pip install hsf --no-deps
+# pip install "torchio>=0.18.56" "roiloc>0.2.8" "hydra-core>=1.1.1" "wget>=3.2" "antspyx>0.3.0" "xxhash>=3.2.0" "rich>11.0.0" "onnxruntime>=1.14.0"
```

### Comparing `hsf-1.1.2/PKG-INFO` & `hsf-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsf
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple yet exhaustive segmentation tool of the Hippocampal Subfields in T1w and T2w MRIs.
 Home-page: https://hippomnesis.dev
 License: MIT
 Keywords: mri,brain,hippocampus,segmentation,deep learning
 Author: Clément POIRET
 Author-email: poiret.clement@outlook.fr
 Requires-Python: >=3.7.1,<3.11
@@ -18,16 +18,16 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Provides-Extra: cpu
 Provides-Extra: gpu
 Provides-Extra: sparse
 Requires-Dist: antspyx (>0.3.0)
 Requires-Dist: deepsparse (>=1.4.0,<2.0.0) ; extra == "sparse"
 Requires-Dist: hydra-core (>=1.1.1,<2.0.0)
-Requires-Dist: onnxruntime (>=1.14.0,<2.0.0) ; extra == "cpu" or extra == "sparse"
-Requires-Dist: onnxruntime-gpu (>=1.14.0,<2.0.0) ; extra == "gpu"
+Requires-Dist: onnxruntime (>=1.8.0) ; extra == "cpu" or extra == "sparse"
+Requires-Dist: onnxruntime-gpu (>=1.8.0) ; extra == "gpu"
 Requires-Dist: rich (>11.0.0)
 Requires-Dist: roiloc (>0.2.8)
 Requires-Dist: torchio (>=0.18.56,<0.19.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/clementpoiret/HSF
 Description-Content-Type: text/x-rst
@@ -250,14 +250,18 @@
 
 Changelogs
 ==========
 
 HSF
 ---
 
+**Version 1.1.3**
+
+* Lower onnxruntime dependency to min 1.8.0
+
 **Version 1.1.2**
 
 * ***BREAKING CHANGE***: HSF needs to be installed using extra dependencies depending on the backend you want to use.
   See the [installation guide](https://hsf.readthedocs.io/en/latest/user-guide/installation/) for more details.
 * Updated dependencies
 * Fixed installation on MacOS
```

