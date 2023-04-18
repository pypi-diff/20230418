# Comparing `tmp/statgis-1.0.7.tar.gz` & `tmp/statgis-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statgis-1.0.7.tar", max compression
+gzip compressed data, was "statgis-1.1.1.tar", max compression
```

## Comparing `statgis-1.0.7.tar` & `statgis-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,34 @@
--rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.0.7/LICENSE
--rw-r--r--   0        0        0      890 2023-04-16 05:22:36.960544 statgis-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.0.7/README.md
--rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.0.7/src/statgis/__init__.py
--rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.0.7/src/statgis/gee/__init__.py
--rw-r--r--   0        0        0     4294 2023-04-15 23:07:05.575665 statgis-1.0.7/src/statgis/gee/classification.py
--rw-r--r--   0        0        0     3717 2023-04-16 01:25:14.903252 statgis-1.0.7/src/statgis/gee/landsat_functions.py
--rw-r--r--   0        0        0     2816 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/river_analysis.py
--rw-r--r--   0        0        0     1904 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/sample.py
--rw-r--r--   0        0        0      932 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/sentinel_functions.py
--rw-r--r--   0        0        0     1334 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/shoreline_analysis.py
--rw-r--r--   0        0        0     1238 2023-04-15 01:57:55.417245 statgis-1.0.7/src/statgis/gee/terrain_analysis.py
--rw-r--r--   0        0        0     7501 2023-04-16 04:53:14.229067 statgis-1.0.7/src/statgis/gee/time_series_analysis.py
--rw-r--r--   0        0        0     1835 2023-04-15 05:14:49.801143 statgis-1.0.7/src/statgis/gee/utils.py
--rw-r--r--   0        0        0     4621 2023-04-16 05:07:36.177091 statgis-1.0.7/src/statgis/gee/zonal_statistics.py
--rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.0.7/src/statgis/statgis.py
--rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.0.7/src/statgis/statutils/__init__.py
--rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.0.7/src/statgis/statutils/plots.py
--rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.0.7/src/statgis/statutils/stats.py
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 statgis-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.1.1/LICENSE
+-rw-r--r--   0        0        0      953 2023-04-18 20:26:57.929677 statgis-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.1.1/README.md
+-rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.1.1/src/statgis/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.1.1/src/statgis/gee/__init__.py
+-rw-r--r--   0        0        0      662 2023-04-15 19:25:50.282753 statgis-1.1.1/src/statgis/gee/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4292 2023-04-18 18:36:45.403720 statgis-1.1.1/src/statgis/gee/__pycache__/classification.cpython-311.pyc
+-rw-r--r--   0        0        0     8193 2023-04-18 19:53:34.000024 statgis-1.1.1/src/statgis/gee/__pycache__/landsat_functions.cpython-311.pyc
+-rw-r--r--   0        0        0     4269 2023-04-18 18:37:02.000763 statgis-1.1.1/src/statgis/gee/__pycache__/river_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5220 2023-04-18 20:08:06.219058 statgis-1.1.1/src/statgis/gee/__pycache__/sample.cpython-311.pyc
+-rw-r--r--   0        0        0     3303 2023-04-18 19:53:39.000491 statgis-1.1.1/src/statgis/gee/__pycache__/sentinel_functions.cpython-311.pyc
+-rw-r--r--   0        0        0     2467 2023-04-18 18:37:10.082006 statgis-1.1.1/src/statgis/gee/__pycache__/shoreline_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     2141 2023-04-18 18:37:12.925211 statgis-1.1.1/src/statgis/gee/__pycache__/terrain_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0    13396 2023-04-18 19:53:43.675907 statgis-1.1.1/src/statgis/gee/__pycache__/time_series_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5461 2023-04-18 19:54:00.302889 statgis-1.1.1/src/statgis/gee/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     7900 2023-04-18 19:53:47.145468 statgis-1.1.1/src/statgis/gee/__pycache__/zonal_statistics.cpython-311.pyc
+-rw-r--r--   0        0        0     2720 2023-04-17 22:52:39.257683 statgis-1.1.1/src/statgis/gee/classification.py
+-rw-r--r--   0        0        0     6056 2023-04-18 19:37:44.895652 statgis-1.1.1/src/statgis/gee/landsat_functions.py
+-rw-r--r--   0        0        0     2815 2023-04-17 23:24:07.530781 statgis-1.1.1/src/statgis/gee/river_analysis.py
+-rw-r--r--   0        0        0     3943 2023-04-18 20:03:49.199286 statgis-1.1.1/src/statgis/gee/sample.py
+-rw-r--r--   0        0        0     2532 2023-04-18 19:41:30.512138 statgis-1.1.1/src/statgis/gee/sentinel_functions.py
+-rw-r--r--   0        0        0     1334 2023-04-17 23:25:00.413231 statgis-1.1.1/src/statgis/gee/shoreline_analysis.py
+-rw-r--r--   0        0        0     1237 2023-04-17 23:31:38.297087 statgis-1.1.1/src/statgis/gee/terrain_analysis.py
+-rw-r--r--   0        0        0     8975 2023-04-18 19:44:54.106465 statgis-1.1.1/src/statgis/gee/time_series_analysis.py
+-rw-r--r--   0        0        0     4101 2023-04-18 19:50:59.397654 statgis-1.1.1/src/statgis/gee/utils.py
+-rw-r--r--   0        0        0     5579 2023-04-18 19:52:58.304434 statgis-1.1.1/src/statgis/gee/zonal_statistics.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.1.1/src/statgis/statgis.py
+-rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.1.1/src/statgis/statutils/__init__.py
+-rw-r--r--   0        0        0      266 2023-04-15 19:26:21.949342 statgis-1.1.1/src/statgis/statutils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4421 2023-04-15 19:26:41.745766 statgis-1.1.1/src/statgis/statutils/__pycache__/plots.cpython-311.pyc
+-rw-r--r--   0        0        0     2761 2023-04-15 19:26:22.074352 statgis-1.1.1/src/statgis/statutils/__pycache__/stats.cpython-311.pyc
+-rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.1.1/src/statgis/statutils/plots.py
+-rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.1.1/src/statgis/statutils/stats.py
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 statgis-1.1.1/PKG-INFO
```

### Comparing `statgis-1.0.7/LICENSE` & `statgis-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statgis-1.0.7/README.md` & `statgis-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `statgis-1.0.7/src/statgis/gee/river_analysis.py` & `statgis-1.1.1/src/statgis/gee/river_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Analyse rivers with sattelite images"""
+"""Analyze rivers with satellite images"""
 import ee
 
 ee.Initialize()
 
 
 def plume_characterization(
     image: ee.Image,
@@ -17,15 +17,15 @@
 
     Parameters
     ----------
     Image : ee.Image
         Image to be classified.
 
     sample_region : ee.Geometry
-        Polygon that enclosess a region of the Image that the user indetifies as
+        Polygon that encloses a region of the Image that the user identified as
         river plume.
 
     blue : str
         Blue band name.
 
     green : str
         Green band name.
```

### Comparing `statgis-1.0.7/src/statgis/gee/shoreline_analysis.py` & `statgis-1.1.1/src/statgis/gee/shoreline_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ) -> ee.FeatureCollection:
     """
     Extract shoreline from image classified.
 
     Parameters
     ----------
     image : ee.Image
-        Classified image to analyse.
+        Classified image to analyze.
 
     region : ee.Geometry
         Region of interest to clip the image and shorelines.
 
     scale : float
         Image scale.
```

### Comparing `statgis-1.0.7/src/statgis/gee/terrain_analysis.py` & `statgis-1.1.1/src/statgis/gee/terrain_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,33 +12,33 @@
     catchment: ee.Geometry,
     dem: ee.Image,
     scale: float,
     band: str,
     bins: int = 100,
 ) -> list:
     """
-    Calculate the cumulative area and comulative height from a catchment for the
+    Calculate the cumulative area and cumulative height from a catchment for the
     hypsometric curve.
 
     Parameters
     ----------
     catchment : ee.Geometry
-        Catchment area to analyse.
+        Catchment area to analyze.
 
     dem : ee.Image
-        Digital elevation model (DEM) to analyse.
+        Digital elevation model (DEM) to analyze.
 
     scale : float
         Scale of DEM.
 
     band : str
-        Band of DEM with elevetaion information.
+        Band of DEM with elevation information.
 
     bins : int
-        Number of bins for cumalitive area an height.
+        Number of bins for cumulative area an height.
 
     Returns
     -------
     area : ArrayLike
         Normalized area.
 
     height : ArrayLike
```

### Comparing `statgis-1.0.7/src/statgis/gee/time_series_analysis.py` & `statgis-1.1.1/src/statgis/gee/time_series_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     image_collection : ee.ImageCollection
         Collection of image.
 
     Returns
     -------
     dates : pd.Series
         Series with the dates of the images.
+
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import time_series_analysis
+    >>> ee.Initialize()
+    >>> chirps = ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY").filterDate("1985-01-01", "2022-12-31")
+    >>> dates = time_series_analysis.extract_dates(chirps)
     """
     dates = (
         image_collection.reduceColumns(ee.Reducer.toList(), ["system:time_start"])
         .get("list")
         .getInfo()
     )
 
@@ -49,16 +57,23 @@
         - monthly-stat.
         - monthly-stat-repeated.
 
     Returns
     -------
     final_collection : ee.ImageCollection
         Collection resampled.
+    
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import time_series_analysis
+    >>> ee.Initialize()
+    >>> chirps = ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY").filterDate("1985-01-01", "2022-12-31")
+    >>> annual_precipitation = time_series_analysis.resample(chirps, ee.Reducer.sum(), "annual")
     """
-
     dates = image_collection.reduceColumns(
         reducer=ee.Reducer.min().combine(ee.Reducer.max(), sharedInputs=True),
         selectors=["system:time_start"],
     ).getInfo()
 
     for key, val in dates.items():
         dates[key] = ee.Date(val).get("year").getInfo()
@@ -148,14 +163,22 @@
         If `True`, the data mean wil lbe restored in the seasonality.
 
     Returns
     -------
     image_collection : ee.ImageCollection
         Image collection with linear trend and seasonality.
 
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import time_series_analysis
+    >>> ee.Initialize()
+    >>> chirps = ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY").filterDate("1985-01-01", "2022-12-31")
+    >>> annual_precipitation = time_series_analysis.resample(chirps, ee.Reducer.sum(), "annual")
+    >>> seasonal_precipitation = time_series_analysis.detrend(annual_precipitation, "precipitation")
     """
     image_collection = image_collection.map(lambda img: img.addBands(img.metadata("system:time_start").rename("time")))
     image_collection = image_collection.select(["time", band])
 
     mean = image_collection.select(band).mean()
 
     fitted = image_collection.reduce(ee.Reducer.linearFit())
@@ -197,14 +220,23 @@
     restore_mean : bool = True
         If `True`, the data mean wil lbe restored in the seasonality.
 
     Returns
     -------
     final_collection : ee.ImageCollection
         Image collection with time series components.
+
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import time_series_analysis
+    >>> ee.Initialize()
+    >>> chirps = ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY").filterDate("1985-01-01", "2022-12-31")
+    >>> monthly_precipitation = time_series_analysis.resample(chirps, ee.Reducer.sum(), "monthly")
+    >>> precipitation_ts = time_series_analysis.seasonal_decompose(monthly_precipitation, "precipitation")
     """
     image_collection = detrend(image_collection, band, restore_mean)
 
     def calculate_anomalies(detrended_collection: ee.ImageCollection) -> ee.ImageCollection:
         """Add the anomalies to a detrended image collection"""
         mean_repeated_collection = resample(detrended_collection, ee.Reducer.mean(), "monthly-stat-repeated")
```

### Comparing `statgis-1.0.7/src/statgis/gee/zonal_statistics.py` & `statgis-1.1.1/src/statgis/gee/zonal_statistics.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,27 @@
     tile_scale : int (optional)
         Scale of the mosaic to allow EarthEngine to split the task to more cores.
 
     Returns
     -------
     data : pandas.DataFrame
         DataFrame with all the stats for all specified bands.
+
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import zonal_statistics
+    >>> ee.Initialize()
+    >>> roi = ee.Geometry.BBox(-75.2671803, 4.4104561 ,-75.2691803, 4.4124561)
+    >>> mean_precipitation_2022 = (
+    ...     ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY")
+    ...     .filterDate("2022-01-01", "2022-12-31")
+    ...     .mean()
+    ... )
+    >>> stats = zonal_statistics.zonal_statistics_image(mean_precipitation_2022, roi, 30, "precipitation")
     """
     if bands != "all":
         image = image.select(bands)
 
     if reducer == "all":
         reducer = ee.Reducer.mean().combine(
             ee.Reducer.stdDev().combine(
@@ -107,14 +120,25 @@
     tile_scale : int (optional)
         Scale of the mosaic to allow EarthEngine to split the task to more cores.
 
     Returns
     ------
     data : pandas.DataFrame
         DataFrame with all the stats for all specified bands.
+        
+    Example
+    -------
+    >>> import ee
+    >>> from statgis.gee import zonal_statistics
+    >>> ee.Initialize()
+    >>> roi = ee.Geometry.BBox(-75.2671803, 4.4104561 ,-75.2691803, 4.4124561)
+    >>> chirps = ee.ImageCollection("UCSB-CHG/CHIRPS/DAILY").filterDate("2022-01-01", "2022-12-31")
+    >>> daily_mean_precipitation = zonal_statistics.zonal_statistics_collection(
+    ...     chirps, roi, 30, "precipitation", ee.Reducer.mean()
+    ... )
     """
     if bands != "all":
         image_collection = image_collection.select(bands)
 
     if reducer == "all":
         reducer = ee.Reducer.mean().combine(
             ee.Reducer.stdDev().combine(
```

### Comparing `statgis-1.0.7/src/statgis/statutils/plots.py` & `statgis-1.1.1/src/statgis/statutils/plots.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.7/src/statgis/statutils/stats.py` & `statgis-1.1.1/src/statgis/statutils/stats.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.7/PKG-INFO` & `statgis-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: statgis
-Version: 1.0.7
+Version: 1.1.1
 Summary: Tools for improve work with geospatial data in Python
 License: MIT
 Author: Sebástian Narváez-Salcedo
 Author-email: sanarvaezstatgis@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: accessible-pygments (==0.0.4)
 Requires-Dist: earthengine-api (>=0.1.335)
 Requires-Dist: matplotlib (>=3.2.2)
 Requires-Dist: pandas (>=1.3.5)
+Requires-Dist: pydata-sphinx-theme (==0.13.3)
 Requires-Dist: scipy (>=1.7.3)
 Description-Content-Type: text/markdown
 
 # StatGIS Python Package
 
 ![PyPI](https://img.shields.io/pypi/v/statgis) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/statgis?color=yellow) [![Documentation Status](https://readthedocs.org/projects/statgis/badge/?version=latest)](https://statgis.readthedocs.io/en/latest/?badge=latest)
```

