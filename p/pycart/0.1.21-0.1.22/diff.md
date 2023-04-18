# Comparing `tmp/pycart-0.1.21.tar.gz` & `tmp/pycart-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycart-0.1.21.tar", max compression
+gzip compressed data, was "pycart-0.1.22.tar", max compression
```

## Comparing `pycart-0.1.21.tar` & `pycart-0.1.22.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1546 2023-04-16 15:16:24.512787 pycart-0.1.21/LICENSE
--rw-r--r--   0        0        0        0 2023-04-09 13:06:33.395735 pycart-0.1.21/pycart/__init__.py
--rw-r--r--   0        0        0     3721 2023-04-16 17:12:51.613513 pycart-0.1.21/pycart/border_util.py
--rw-r--r--   0        0        0    18424 2023-04-16 17:06:15.292214 pycart-0.1.21/pycart/cartogram.py
--rw-r--r--   0        0        0     1602 2023-04-16 17:15:39.602954 pycart-0.1.21/pyproject.toml
--rw-r--r--   0        0        0     1599 2023-04-11 11:41:24.063439 pycart-0.1.21/README.md
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 pycart-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0     1546 2023-04-16 15:16:24.512787 pycart-0.1.22/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-09 13:06:33.395735 pycart-0.1.22/pycart/__init__.py
+-rw-r--r--   0        0        0     3721 2023-04-16 17:12:51.613513 pycart-0.1.22/pycart/border_util.py
+-rw-r--r--   0        0        0    18582 2023-04-18 15:50:53.394526 pycart-0.1.22/pycart/cartogram.py
+-rw-r--r--   0        0        0     1716 2023-04-18 16:04:02.263976 pycart-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0     2649 2023-04-18 16:48:08.417830 pycart-0.1.22/README.md
+-rw-r--r--   0        0        0    63368 2023-04-18 15:58:05.207779 pycart-0.1.22/requirements.txt
+-rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 pycart-0.1.22/PKG-INFO
```

### Comparing `pycart-0.1.21/LICENSE` & `pycart-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pycart-0.1.21/pycart/border_util.py` & `pycart-0.1.22/pycart/border_util.py`

 * *Files identical despite different names*

### Comparing `pycart-0.1.21/pycart/cartogram.py` & `pycart-0.1.22/pycart/cartogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         """
         A Cartogram object acts as a generator on a specific dataset, through which
         generation algorithms can be run.
 
         ###**Parameters**
 
         - **gdf  :  *[geopandas.GeoDataFrame](https://geopandas.org/en/stable/docs/reference/api/geopandas.GeoDataFrame.html)*** - The dataset that you want to apply cartogram techniques to
-        - **value_field  :  *String*** - Field in the dataset to apply cartogram techniques to
-        - **id_field  :  *String*** - Field of the identifier for each region in the dataset
+        - **value_field  :  *String*** - Field in the dataset to apply cartogram techniques to; the values themselves should be integer or float values
+        - **id_field  :  *String*** - Field of the identifier for each region in the dataset; the id values should be unique so that the generated cartograms can be linked back to original data
         - **geometry_field  :  *String, optional, default 'geometry'*** - Field containing the geometries of each region
 
         ###**Example**
         ```python
         from pycart import cartogram
         import geopandas as gpd
```

### Comparing `pycart-0.1.21/pyproject.toml` & `pycart-0.1.22/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycart"
-version = "0.1.21"
+version = "0.1.22"
 description = "A Python package for generating Cartograms using GeoDataFrames."
 authors = ["Alex Rundle <alexrundle01@gmail.com>"]
 readme = ["README.md"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ARundle01/ecmm428-pycart"
 documentation = "https://ecmm428-pycart.readthedocs.io/"
 
@@ -14,14 +14,19 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering :: Visualization"
 ]
 
+include = [
+    {path = "README.md", format = "sdist"},
+    {path = "requirements.txt", format = "sdist"}
+]
+
 [tool.poetry.dependencies]
 python = ">=3.9.7, <3.10"
 matplotlib = "3.7.1"
 geopandas = "0.12.2"
 geojson = "3.0.1"
 numpy = "1.24.2"
 libpysal = "4.7.0"
```

### Comparing `pycart-0.1.21/PKG-INFO` & `pycart-0.1.22/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycart
-Version: 0.1.21
+Version: 0.1.22
 Summary: A Python package for generating Cartograms using GeoDataFrames.
 Home-page: https://github.com/ARundle01/ecmm428-pycart
 License: BSD-3-Clause
 Author: Alex Rundle
 Author-email: alexrundle01@gmail.com
 Requires-Python: >=3.9.7,<3.10
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -40,14 +40,15 @@
 ==============================
 
 ![GitHub](https://img.shields.io/github/license/ARundle01/ecmm428-pycart)
 ![GitHub code size in bytes](https://img.shields.io/github/repo-size/ARundle01/ecmm428-pycart)
 ![GitHub last commit](https://img.shields.io/github/last-commit/ARundle01/ecmm428-pycart)
 ![GitHub top language](https://img.shields.io/github/languages/top/ARundle01/ecmm428-pycart)
 [![Documentation Status](https://readthedocs.org/projects/ecmm428-pycart/badge/?version=latest)](https://ecmm428-pycart.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/pycart)
 
 ## Contributors
 Contributors to this project are
 - Alex Rundle (ARundle01)
 
 ## License
 This project is licensed under the BSD 3-Clause License
@@ -73,12 +74,28 @@
 py -m pip install -i https://test.pypi.org/simple/ pycart
 ```
 
 ## Pre-requisites
 All code in this Repository and Package was developed and tested on Windows 10.
 
 This Repository requires:
-- **Python >=3.9**
+- **Python >=3.9.7, <3.10**
 
 ## Read the Docs!
 Further information about `pycart` can be found [here](https://ecmm428-pycart.readthedocs.io/en/latest/), 
 including further installation and dependency details, a quickstart guide and API reference.
+
+### Key Dependencies
+To use `pycart`, you will need Python>=3.9, alongside the following 
+fixed version dependencies:
+
+| Package                                                    | Version      |
+|------------------------------------------------------------|--------------|
+| [Python](https://www.python.org/downloads/)                | >=3.9, <3.12 |
+| [matplotlib](https://pypi.org/project/matplotlib/)         | 3.7.1        |
+| [geopandas](https://pypi.org/project/geopandas/)           | 0.12.2       |
+| [geojson](https://pypi.org/project/geojson/)               | 3.0.1        |
+| [pandas](https://pypi.org/project/pandas/)                 | 1.5.3        |
+| [numpy](https://pypi.org/project/numpy/)                   | 1.24.2       |
+| [libpysal](https://pypi.org/project/libpysal/)             | 4.7.0        |
+| [shapely](https://pypi.org/project/shapely/)               | 2.0.1        |
+| [alive-progress](https://pypi.org/project/alive-progress/) | >3.1.1       |
```

