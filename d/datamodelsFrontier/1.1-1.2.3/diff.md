# Comparing `tmp/datamodelsFrontier-1.1.tar.gz` & `tmp/datamodelsFrontier-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamodelsFrontier-1.1.tar", last modified: Thu Apr 13 12:00:04 2023, max compression
+gzip compressed data, was "datamodelsFrontier-1.2.3.tar", last modified: Tue Apr 18 15:51:17 2023, max compression
```

## Comparing `datamodelsFrontier-1.1.tar` & `datamodelsFrontier-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.551535 datamodelsFrontier-1.1/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-06 10:34:10.000000 datamodelsFrontier-1.1/.coveragerc
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1069 2023-04-12 16:30:40.000000 datamodelsFrontier-1.1/LICENSE.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       75 2023-04-12 15:31:53.000000 datamodelsFrontier-1.1/MANIFEST.in
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1728 2023-04-13 12:00:04.551352 datamodelsFrontier-1.1/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1320 2023-04-13 11:59:37.000000 datamodelsFrontier-1.1/README.md
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       38 2023-04-13 12:00:04.551590 datamodelsFrontier-1.1/setup.cfg
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      775 2023-04-13 11:57:50.000000 datamodelsFrontier-1.1/setup.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.546856 datamodelsFrontier-1.1/src/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:09:59.000000 datamodelsFrontier-1.1/src/__init__.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.548312 datamodelsFrontier-1.1/src/datamodels/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 11:58:24.000000 datamodelsFrontier-1.1/src/datamodels/__init__.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      236 2023-04-13 10:57:10.000000 datamodelsFrontier-1.1/src/datamodels/downstream.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      711 2023-04-13 10:57:10.000000 datamodelsFrontier-1.1/src/datamodels/external.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.549980 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1728 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      445 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/SOURCES.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        1 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/dependency_links.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       40 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/requires.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       21 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/top_level.txt
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.550903 datamodelsFrontier-1.1/test/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:29:31.000000 datamodelsFrontier-1.1/test/__init__.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      640 2023-04-13 11:58:34.000000 datamodelsFrontier-1.1/test/test_downstream.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1629 2023-04-13 11:58:34.000000 datamodelsFrontier-1.1/test/test_external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/src/datamodels/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 15:51:17.000000 datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:17.776777 datamodelsFrontier-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/test_downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-18 15:51:07.000000 datamodelsFrontier-1.2.3/test/test_external.py
```

### Comparing `datamodelsFrontier-1.1/LICENSE.txt` & `datamodelsFrontier-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.1/PKG-INFO` & `datamodelsFrontier-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.1
+Version: 1.2.3
 Summary: Datamodels needed for Frontier API
+Home-page: UNKNOWN
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
@@ -27,15 +30,15 @@
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
 from datamodels.external import Barcode
 
-from dtatamodels.downstream import ChildProduct
+from datamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
@@ -79,7 +82,8 @@
   - rrp: str
   - length: str
   - height: str
   - width: str
   - weight: str
   - releaseDateEstimated: bool
 
+
```

### Comparing `datamodelsFrontier-1.1/README.md` & `datamodelsFrontier-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
 from datamodels.external import Barcode
 
-from dtatamodels.downstream import ChildProduct
+from datamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
@@ -65,8 +65,7 @@
   - releaseDate: str
   - rrp: str
   - length: str
   - height: str
   - width: str
   - weight: str
   - releaseDateEstimated: bool
-
```

### Comparing `datamodelsFrontier-1.1/src/datamodels/external.py` & `datamodelsFrontier-1.2.3/src/datamodels/external.py`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/PKG-INFO` & `datamodelsFrontier-1.2.3/src/datamodelsFrontier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.1
+Version: 1.2.3
 Summary: Datamodels needed for Frontier API
+Home-page: UNKNOWN
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
@@ -27,15 +30,15 @@
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
 from datamodels.external import Barcode
 
-from dtatamodels.downstream import ChildProduct
+from datamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
@@ -79,7 +82,8 @@
   - rrp: str
   - length: str
   - height: str
   - width: str
   - weight: str
   - releaseDateEstimated: bool
 
+
```

### Comparing `datamodelsFrontier-1.1/test/test_downstream.py` & `datamodelsFrontier-1.2.3/test/test_downstream.py`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.1/test/test_external.py` & `datamodelsFrontier-1.2.3/test/test_external.py`

 * *Files identical despite different names*

