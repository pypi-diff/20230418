# Comparing `tmp/fastpolvo-0.0.2.tar.gz` & `tmp/fastpolvo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastpolvo-0.0.2.tar", last modified: Fri Jan  6 17:50:21 2023, max compression
+gzip compressed data, was "dist/fastpolvo-0.0.3.tar", last modified: Tue Apr 18 14:28:51 2023, max compression
```

## Comparing `fastpolvo-0.0.2.tar` & `fastpolvo-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)    11337 2022-09-05 16:31:43.000000 fastpolvo-0.0.2/LICENSE
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)      111 2022-09-05 16:31:43.000000 fastpolvo-0.0.2/MANIFEST.in
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1055 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/PKG-INFO
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      301 2023-01-03 19:22:08.000000 fastpolvo-0.0.2/README.md
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       22 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/fastpolvo/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1949 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/fastpolvo/_modidx.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo/classification/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/fastpolvo/classification/__init__.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      658 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/fastpolvo/classification/explorer.py
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1850 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/fastpolvo/core.py
-drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1055 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/PKG-INFO
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      418 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/SOURCES.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/dependency_links.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       40 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/entry_points.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-01-06 17:37:45.000000 fastpolvo-0.0.2/fastpolvo.egg-info/not-zip-safe
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        7 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/requires.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       10 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/fastpolvo.egg-info/top_level.txt
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      772 2023-01-06 17:50:15.000000 fastpolvo-0.0.2/settings.ini
--rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       38 2023-01-06 17:50:21.000000 fastpolvo-0.0.2/setup.cfg
--rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)     2541 2022-09-05 16:31:43.000000 fastpolvo-0.0.2/setup.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)    11337 2022-09-05 16:31:43.000000 fastpolvo-0.0.3/LICENSE
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)      111 2022-09-05 16:31:43.000000 fastpolvo-0.0.3/MANIFEST.in
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1055 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/PKG-INFO
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      301 2023-01-03 19:22:08.000000 fastpolvo-0.0.3/README.md
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       90 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     7138 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/_modidx.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo/classification/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       89 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/classification/__init__.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo/classification/baseline/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/classification/baseline/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1842 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/classification/baseline/baseline.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      774 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/classification/explorer.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1850 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/core.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo/data/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       25 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/data/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1244 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/data/transforms.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo/segmentation/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/segmentation/__init__.py
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     2221 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/fastpolvo/segmentation/core.py
+drwxr-xr-x   0 lgvaz     (1000) lgvaz     (1000)        0 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)     1055 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/PKG-INFO
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      632 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/SOURCES.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/dependency_links.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       40 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/entry_points.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        1 2023-01-06 17:37:45.000000 fastpolvo-0.0.3/fastpolvo.egg-info/not-zip-safe
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)        7 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/requires.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       10 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/fastpolvo.egg-info/top_level.txt
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)      790 2023-04-18 14:28:45.000000 fastpolvo-0.0.3/settings.ini
+-rw-r--r--   0 lgvaz     (1000) lgvaz     (1000)       38 2023-04-18 14:28:51.000000 fastpolvo-0.0.3/setup.cfg
+-rw-rw-r--   0 lgvaz     (1000) lgvaz     (1000)     2541 2022-09-05 16:31:43.000000 fastpolvo-0.0.3/setup.py
```

### Comparing `fastpolvo-0.0.2/LICENSE` & `fastpolvo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpolvo-0.0.2/PKG-INFO` & `fastpolvo-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpolvo
-Version: 0.0.2
+Version: 0.0.3
 Summary: polvo tentacle for fastai
 Home-page: https://github.com/lgvaz/fastpolvo
 Author: lgvaz
 Author-email: lgvaz42@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fastpolvo-0.0.2/fastpolvo/classification/explorer.py` & `fastpolvo-0.0.3/fastpolvo/classification/explorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05a_classification.explorer.ipynb.
 
 # %% auto 0
-__all__ = ['DataExplorer']
+__all__ = ['show_tfms', 'DataExplorer']
 
 # %% ../../nbs/05a_classification.explorer.ipynb 4
 from fastai.vision.all import *
 import polvo as pv
+import fastpolvo as fpv
 
 # %% ../../nbs/05a_classification.explorer.ipynb 5
 class DataExplorer(pv.classification.DataExplorer):
     def __init__(self, x_tl, y_tl): 
         id2label = y_tl.vocab.__getitem__
         label2id = {l: i for i, l in enumerate(y_tl.vocab)}.__getitem__
         super().__init__(y_tl, x_tl.__getitem__, id2label, label2id)
         
     @classmethod
     def from_datasets(cls, dss):
         return cls(dss.tls[0], dss.tls[1])
+
+# %% ../../nbs/05a_classification.explorer.ipynb 12
+show_tfms = fpv.show_tfms
```

### Comparing `fastpolvo-0.0.2/fastpolvo/core.py` & `fastpolvo-0.0.3/fastpolvo/core.py`

 * *Files identical despite different names*

### Comparing `fastpolvo-0.0.2/fastpolvo.egg-info/PKG-INFO` & `fastpolvo-0.0.3/fastpolvo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpolvo
-Version: 0.0.2
+Version: 0.0.3
 Summary: polvo tentacle for fastai
 Home-page: https://github.com/lgvaz/fastpolvo
 Author: lgvaz
 Author-email: lgvaz42@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fastpolvo-0.0.2/settings.ini` & `fastpolvo-0.0.3/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = fastpolvo
 lib_name = fastpolvo
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = fastpolvo
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -28,8 +28,9 @@
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 custom_quarto_yml = False
+clear_all = False
```

### Comparing `fastpolvo-0.0.2/setup.py` & `fastpolvo-0.0.3/setup.py`

 * *Files identical despite different names*

