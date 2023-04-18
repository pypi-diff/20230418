# Comparing `tmp/datamodelsFrontier-1.0.tar.gz` & `tmp/datamodelsFrontier-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamodelsFrontier-1.0.tar", last modified: Thu Apr 13 09:49:58 2023, max compression
+gzip compressed data, was "datamodelsFrontier-1.1.tar", last modified: Thu Apr 13 12:00:04 2023, max compression
```

## Comparing `datamodelsFrontier-1.0.tar` & `datamodelsFrontier-1.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.664609 datamodelsFrontier-1.0/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-06 10:34:10.000000 datamodelsFrontier-1.0/.coveragerc
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1069 2023-04-12 16:30:40.000000 datamodelsFrontier-1.0/LICENSE.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       75 2023-04-12 15:31:53.000000 datamodelsFrontier-1.0/MANIFEST.in
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1456 2023-04-13 09:49:58.664417 datamodelsFrontier-1.0/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1048 2023-04-13 09:48:54.000000 datamodelsFrontier-1.0/README.md
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       38 2023-04-13 09:49:58.664662 datamodelsFrontier-1.0/setup.cfg
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      827 2023-04-13 09:34:48.000000 datamodelsFrontier-1.0/setup.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.660840 datamodelsFrontier-1.0/src/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:09:59.000000 datamodelsFrontier-1.0/src/__init__.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.662493 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1456 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/PKG-INFO
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      374 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/SOURCES.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        1 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/dependency_links.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       40 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/requires.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-13 09:49:58.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/top_level.txt
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)      733 2023-04-13 09:49:33.000000 datamodelsFrontier-1.0/src/datamodelsFrontier.py
-drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 09:49:58.663869 datamodelsFrontier-1.0/test/
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:29:31.000000 datamodelsFrontier-1.0/test/__init__.py
--rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1626 2023-04-13 09:33:14.000000 datamodelsFrontier-1.0/test/test_datamodelsFrontier.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.551535 datamodelsFrontier-1.1/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       19 2023-04-06 10:34:10.000000 datamodelsFrontier-1.1/.coveragerc
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1069 2023-04-12 16:30:40.000000 datamodelsFrontier-1.1/LICENSE.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       75 2023-04-12 15:31:53.000000 datamodelsFrontier-1.1/MANIFEST.in
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1728 2023-04-13 12:00:04.551352 datamodelsFrontier-1.1/PKG-INFO
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1320 2023-04-13 11:59:37.000000 datamodelsFrontier-1.1/README.md
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       38 2023-04-13 12:00:04.551590 datamodelsFrontier-1.1/setup.cfg
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      775 2023-04-13 11:57:50.000000 datamodelsFrontier-1.1/setup.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.546856 datamodelsFrontier-1.1/src/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:09:59.000000 datamodelsFrontier-1.1/src/__init__.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.548312 datamodelsFrontier-1.1/src/datamodels/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 11:58:24.000000 datamodelsFrontier-1.1/src/datamodels/__init__.py
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      236 2023-04-13 10:57:10.000000 datamodelsFrontier-1.1/src/datamodels/downstream.py
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      711 2023-04-13 10:57:10.000000 datamodelsFrontier-1.1/src/datamodels/external.py
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.549980 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1728 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/PKG-INFO
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      445 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        1 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       40 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/requires.txt
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)       21 2023-04-13 12:00:04.000000 datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/top_level.txt
+drwxr-xr-x   0 ruchika.scott63   (502) staff       (20)        0 2023-04-13 12:00:04.550903 datamodelsFrontier-1.1/test/
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)        0 2023-04-06 10:29:31.000000 datamodelsFrontier-1.1/test/__init__.py
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)      640 2023-04-13 11:58:34.000000 datamodelsFrontier-1.1/test/test_downstream.py
+-rw-r--r--   0 ruchika.scott63   (502) staff       (20)     1629 2023-04-13 11:58:34.000000 datamodelsFrontier-1.1/test/test_external.py
```

### Comparing `datamodelsFrontier-1.0/LICENSE.txt` & `datamodelsFrontier-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datamodelsFrontier-1.0/PKG-INFO` & `datamodelsFrontier-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.0
+Version: 1.1
 Summary: Datamodels needed for Frontier API
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -25,24 +25,27 @@
 
 *Command Line*
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodelsFrontier import barcode
+from datamodels.external import Barcode
+
+from dtatamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
 ```
 #### Each Model and Input Value
+##### External
 The models that can be imported are:
 
 - InventoryItemDimension:
    - height_mm: int
    - width_mm: int
    - depth_mm: int
    - mass_kg: int
@@ -62,7 +65,21 @@
   - has_hazmat: bool
   - barcodes: list[Barcode]
   - dimensions: InventoryItemDimension
   - alternative_inventory_items: list[str]
   - thg_id: str 
   - status: str
 
+##### Downstream
+
+- ChildProduct:
+  - id: str
+  - title: str
+  - barcode: str
+  - releaseDate: str
+  - rrp: str
+  - length: str
+  - height: str
+  - width: str
+  - weight: str
+  - releaseDateEstimated: bool
+
```

### Comparing `datamodelsFrontier-1.0/README.md` & `datamodelsFrontier-1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 
 *Command Line*
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodelsFrontier import barcode
+from datamodels.external import Barcode
+
+from dtatamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
 ```
 #### Each Model and Input Value
+##### External
 The models that can be imported are:
 
 - InventoryItemDimension:
    - height_mm: int
    - width_mm: int
    - depth_mm: int
    - mass_kg: int
@@ -49,7 +52,21 @@
   - has_hazmat: bool
   - barcodes: list[Barcode]
   - dimensions: InventoryItemDimension
   - alternative_inventory_items: list[str]
   - thg_id: str 
   - status: str
 
+##### Downstream
+
+- ChildProduct:
+  - id: str
+  - title: str
+  - barcode: str
+  - releaseDate: str
+  - rrp: str
+  - length: str
+  - height: str
+  - width: str
+  - weight: str
+  - releaseDateEstimated: bool
+
```

### Comparing `datamodelsFrontier-1.0/setup.py` & `datamodelsFrontier-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from setuptools import setup
 
-from src.datamodelsFrontier import __version__
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extra_test = [
     'pytest>=4',
     'pytest-cov>=2',
 ]
 
 setup(
     name='datamodelsFrontier',
-    version=__version__,
+    version="1.1",
     description="Datamodels needed for Frontier API",
 
     author='THG-Frontier',
     author_email='DL-TechAPIGateway@thehutgroup.com',
 
     install_requires=['pydantic', ],
     extras_require={
         'dev': extra_test
     },
 
-    py_modules=['datamodelsFrontier'],
+    py_modules=['downstream, external'],
     package_dir={"": "src"},
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
```

### Comparing `datamodelsFrontier-1.0/src/datamodelsFrontier.egg-info/PKG-INFO` & `datamodelsFrontier-1.1/src/datamodelsFrontier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodelsFrontier
-Version: 1.0
+Version: 1.1
 Summary: Datamodels needed for Frontier API
 Author: THG-Frontier
 Author-email: DL-TechAPIGateway@thehutgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -25,24 +25,27 @@
 
 *Command Line*
 ```bash
 $ pip install datamodelsFrontier
 ```
 *Python*
 ```python
-from datamodelsFrontier import barcode
+from datamodels.external import Barcode
+
+from dtatamodels.downstream import ChildProduct
 ```
 
 
 ### Code Information
 #### Example Code:
 ```python
 InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
 ```
 #### Each Model and Input Value
+##### External
 The models that can be imported are:
 
 - InventoryItemDimension:
    - height_mm: int
    - width_mm: int
    - depth_mm: int
    - mass_kg: int
@@ -62,7 +65,21 @@
   - has_hazmat: bool
   - barcodes: list[Barcode]
   - dimensions: InventoryItemDimension
   - alternative_inventory_items: list[str]
   - thg_id: str 
   - status: str
 
+##### Downstream
+
+- ChildProduct:
+  - id: str
+  - title: str
+  - barcode: str
+  - releaseDate: str
+  - rrp: str
+  - length: str
+  - height: str
+  - width: str
+  - weight: str
+  - releaseDateEstimated: bool
+
```

### Comparing `datamodelsFrontier-1.0/src/datamodelsFrontier.py` & `datamodelsFrontier-1.1/src/datamodels/external.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,7 @@
     barcodes: list[Barcode]
     dimensions: InventoryItemDimension
     # if this inventory item is out of stock then use the first on in this
     # list at is in stock
     alternative_inventory_items: list[str]
     thg_id: str
     status: str
-
-
-__version__ = '1.0'
```

### Comparing `datamodelsFrontier-1.0/test/test_datamodelsFrontier.py` & `datamodelsFrontier-1.1/test/test_external.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from src.datamodelsFrontier import InventoryItemDimension
-from src.datamodelsFrontier import Barcode
-from src.datamodelsFrontier import InventoryItem
+from src.datamodels.external import InventoryItemDimension
+from src.datamodels.external import Barcode
+from src.datamodels.external import InventoryItem
 
 
 def test_inventory_item_dimension():
     iid = InventoryItemDimension(height_mm=3, width_mm=4, depth_mm=5, mass_kg=5)
     assert iid.height_mm == 3
     assert iid.width_mm == 4
     assert iid.depth_mm == 5
```

