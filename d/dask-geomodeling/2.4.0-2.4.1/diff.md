# Comparing `tmp/dask-geomodeling-2.4.0.tar.gz` & `tmp/dask-geomodeling-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-geomodeling-2.4.0.tar", last modified: Thu Apr 13 13:02:34 2023, max compression
+gzip compressed data, was "dask-geomodeling-2.4.1.tar", last modified: Tue Apr 18 13:13:33 2023, max compression
```

## Comparing `dask-geomodeling-2.4.0.tar` & `dask-geomodeling-2.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/
--rw-rw-r--   0 casper    (1000) casper    (1000)    18932 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/CHANGES.rst
--rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/LICENSE
--rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/MANIFEST.in
--rw-rw-r--   0 casper    (1000) casper    (1000)    20802 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/README.rst
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/
--rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/config.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/core/
--rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/core/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/core/graphs.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/geometry/
--rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    22769 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/aggregate.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/constructive.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/field_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/geom_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/merge.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/set_operations.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/sinks.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/text.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/ipyleaflet_plugin.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/measurements.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/dask_geomodeling/raster/
--rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/__init__.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/base.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/combine.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/elemwise.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/misc.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/parallelize.py
--rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/reduction.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/sources.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/spatial.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    32375 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/temporal.py
--rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/utils.py
-drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/
--rw-rw-r--   0 casper    (1000) casper    (1000)    20802 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/PKG-INFO
--rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/SOURCES.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/dependency_links.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/not-zip-safe
--rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/requires.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/top_level.txt
--rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/setup.cfg
--rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/setup.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    19112 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/CHANGES.rst
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/LICENSE
+-rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/MANIFEST.in
+-rw-rw-r--   0 casper    (1000) casper    (1000)    20982 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/README.rst
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.721328 dask-geomodeling-2.4.1/dask_geomodeling/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/config.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling/core/
+-rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/core/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/core/graphs.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling/geometry/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    23038 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/aggregate.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/constructive.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/field_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/geom_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/merge.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/set_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/sinks.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/geometry/text.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/ipyleaflet_plugin.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/measurements.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/dask_geomodeling/raster/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/combine.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/elemwise.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/misc.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/reduction.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/spatial.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    32375 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/raster/temporal.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling/utils.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-18 13:13:33.725328 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    20982 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/not-zip-safe
+-rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/requires.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/dask_geomodeling.egg-info/top_level.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-04-18 13:13:33.729328 dask-geomodeling-2.4.1/setup.cfg
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-04-18 13:13:33.000000 dask-geomodeling-2.4.1/setup.py
```

### Comparing `dask-geomodeling-2.4.0/CHANGES.rst` & `dask-geomodeling-2.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.1 (2023-04-18)
+------------------
+
+- AggregateRaster will do a point request to the raster if only 1 cell is required
+  (instead of a box request that encompasses the cell).
+
+
 2.4.0 (2023-04-13)
 ------------------
 
 - Change Block.get_data; instead of always computing in the main thread, use
   the scheduler that is setup via dask.config.
```

### Comparing `dask-geomodeling-2.4.0/LICENSE` & `dask-geomodeling-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/PKG-INFO` & `dask-geomodeling-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.0
+Version: 2.4.1
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,21 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.1 (2023-04-18)
+------------------
+
+- AggregateRaster will do a point request to the raster if only 1 cell is required
+  (instead of a box request that encompasses the cell).
+
+
 2.4.0 (2023-04-13)
 ------------------
 
 - Change Block.get_data; instead of always computing in the main thread, use
   the scheduler that is setup via dask.config.
```

### Comparing `dask-geomodeling-2.4.0/README.rst` & `dask-geomodeling-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/core/graphs.py` & `dask-geomodeling-2.4.1/dask_geomodeling/core/graphs.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/aggregate.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,21 +457,28 @@
         x2 = ceil(x2 / pixel_size) * pixel_size
         y2 = ceil(y2 / pixel_size) * pixel_size
 
         # compute the width and height
         width = max(int((x2 - x1) / pixel_size), 1)
         height = max(int((y2 - y1) / pixel_size), 1)
 
+        # change point-like requests in real point requests
+        # (reducing possible edge effects)
+        if width == 1 and height == 1:
+            raster_req_bbox = ((x1 + x2) / 2, (y1 + y2) / 2 ) * 2
+        else:
+            raster_req_bbox = (x1, y1, x2, y2)
+
         raster_request = {
             "mode": "vals",
             "projection": agg_srs,
             "start": request.get("start"),
             "stop": request.get("stop"),
             "aggregation": None,  # TODO
-            "bbox": (x1, y1, x2, y2),
+            "bbox": raster_req_bbox,
             "width": width,
             "height": height,
         }
 
         # only propagate if provided
         if "time_resolution" in request:
             raster_request["time_resolution"] = request["time_resolution"]
```

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/base.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/constructive.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/constructive.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/field_operations.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/field_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/geom_operations.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/geom_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/merge.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/merge.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/parallelize.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/set_operations.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/set_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/sinks.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/sinks.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/sources.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/geometry/text.py` & `dask-geomodeling-2.4.1/dask_geomodeling/geometry/text.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/ipyleaflet_plugin.py` & `dask-geomodeling-2.4.1/dask_geomodeling/ipyleaflet_plugin.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/measurements.py` & `dask-geomodeling-2.4.1/dask_geomodeling/measurements.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/base.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/combine.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/combine.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/elemwise.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/elemwise.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/misc.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/misc.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/parallelize.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/reduction.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/reduction.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/sources.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/sources.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/spatial.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/spatial.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/raster/temporal.py` & `dask-geomodeling-2.4.1/dask_geomodeling/raster/temporal.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling/utils.py` & `dask-geomodeling-2.4.1/dask_geomodeling/utils.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling.egg-info/PKG-INFO` & `dask-geomodeling-2.4.1/dask_geomodeling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-geomodeling
-Version: 2.4.0
+Version: 2.4.1
 Summary: On-the-fly operations on geographical maps.
 Home-page: https://github.com/nens/dask-geomodeling
 Author: Casper van der Wel
 Author-email: casper.vanderwel@nelen-schuurmans.nl
 License: BSD 3-Clause License
 Keywords: dask
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,21 @@
 
 `Read the docs <https://dask-geomodeling.readthedocs.org/>`_ for further information.
 
 
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.1 (2023-04-18)
+------------------
+
+- AggregateRaster will do a point request to the raster if only 1 cell is required
+  (instead of a box request that encompasses the cell).
+
+
 2.4.0 (2023-04-13)
 ------------------
 
 - Change Block.get_data; instead of always computing in the main thread, use
   the scheduler that is setup via dask.config.
```

### Comparing `dask-geomodeling-2.4.0/dask_geomodeling.egg-info/SOURCES.txt` & `dask-geomodeling-2.4.1/dask_geomodeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.4.0/setup.py` & `dask-geomodeling-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = '2.4.0'
+version = '2.4.1'
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 
 install_requires = (
     [
         "dask[delayed]>=0.20",
         "pandas>=0.23",
```

