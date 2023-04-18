# Comparing `tmp/nzshm_common-0.5.0.tar.gz` & `tmp/nzshm_common-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzshm_common-0.5.0.tar", max compression
+gzip compressed data, was "nzshm_common-0.5.1.tar", max compression
```

## Comparing `nzshm_common-0.5.0.tar` & `nzshm_common-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-17 04:07:36.289452 nzshm_common-0.5.0/LICENSE
--rw-r--r--   0        0        0     1109 2023-04-17 04:07:36.289452 nzshm_common-0.5.0/README.md
--rw-r--r--   0        0        0      111 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/__init__.py
--rw-r--r--   0        0        0      799 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/geometry/backarc_polygon.json
--rw-r--r--   0        0        0     1489 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/geometry/geometry.py
--rw-r--r--   0        0        0       47 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/__init__.py
--rw-r--r--   0        0        0      477 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/io.py
--rw-r--r--   0        0        0     2831 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v0.py
--rw-r--r--   0        0        0     3524 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v1.py
--rw-r--r--   0        0        0    47971 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_2_nb_1_1.py
--rw-r--r--   0        0        0     1511 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/region_grid.py
--rw-r--r--   0        0        0    38248 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/wlg_0_01_nb_1_1.py
--rw-r--r--   0        0        0     3260 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/wlg_0_05_nb_1_1.py
--rw-r--r--   0        0        0       41 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/code_location.py
--rw-r--r--   0        0        0     1631 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/location.py
--rw-r--r--   0        0        0  3218277 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/location/locations.json
--rw-r--r--   0        0        0      252 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/location/nz_ids.json
--rw-r--r--   0        0        0       75 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/util/__init__.py
--rw-r--r--   0        0        0     1440 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/util/compression.py
--rw-r--r--   0        0        0     2049 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1760 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_backarc.py
--rw-r--r--   0        0        0     3565 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_coded_location.py
--rw-r--r--   0        0        0     2317 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_compression.py
--rw-r--r--   0        0        0     4500 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_geometry.py
--rw-r--r--   0        0        0     1662 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_location.py
--rw-r--r--   0        0        0     1018 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_region_grid.py
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 nzshm_common-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1109 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/README.md
+-rw-r--r--   0        0        0      111 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/geometry/backarc_polygon.json
+-rw-r--r--   0        0        0     1444 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/geometry/geometry.py
+-rw-r--r--   0        0        0       47 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/io.py
+-rw-r--r--   0        0        0     2831 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v0.py
+-rw-r--r--   0        0        0     3524 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v1.py
+-rw-r--r--   0        0        0    47971 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/nz_0_2_nb_1_1.py
+-rw-r--r--   0        0        0     1511 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/region_grid.py
+-rw-r--r--   0        0        0    38248 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/wlg_0_01_nb_1_1.py
+-rw-r--r--   0        0        0     3260 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/grids/wlg_0_05_nb_1_1.py
+-rw-r--r--   0        0        0       41 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/code_location.py
+-rw-r--r--   0        0        0     1631 2023-04-18 00:48:38.923956 nzshm_common-0.5.1/nzshm_common/location/location.py
+-rw-r--r--   0        0        0  3218277 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/location/locations.json
+-rw-r--r--   0        0        0      252 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/location/nz_ids.json
+-rw-r--r--   0        0        0       75 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/util/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/nzshm_common/util/compression.py
+-rw-r--r--   0        0        0     2119 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1760 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_backarc.py
+-rw-r--r--   0        0        0     3565 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_coded_location.py
+-rw-r--r--   0        0        0     2317 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_compression.py
+-rw-r--r--   0        0        0     4500 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_geometry.py
+-rw-r--r--   0        0        0     1662 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_location.py
+-rw-r--r--   0        0        0     1018 2023-04-18 00:48:38.931957 nzshm_common-0.5.1/tests/test_region_grid.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nzshm_common-0.5.1/PKG-INFO
```

### Comparing `nzshm_common-0.5.0/LICENSE` & `nzshm_common-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/README.md` & `nzshm_common-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/geometry/backarc_polygon.json` & `nzshm_common-0.5.1/nzshm_common/geometry/backarc_polygon.json`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/geometry/geometry.py` & `nzshm_common-0.5.1/nzshm_common/geometry/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,10 +45,7 @@
 def create_backarc_polygon() -> GeoDataFrame:
     """
     Retrieve the backarc polygon from json and return geopandas object
     """
 
     poly_filepath = Path(Path(__file__).parent, 'backarc_polygon.json')
     return geopandas.read_file(poly_filepath)
-
-
-BACKARC_POLYGON = create_backarc_polygon()
```

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v0.py` & `nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v0.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v1.py` & `nzshm_common-0.5.1/nzshm_common/grids/nz_0_1_nb_1_v1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/nz_0_2_nb_1_1.py` & `nzshm_common-0.5.1/nzshm_common/grids/nz_0_2_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/region_grid.py` & `nzshm_common-0.5.1/nzshm_common/grids/region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/wlg_0_01_nb_1_1.py` & `nzshm_common-0.5.1/nzshm_common/grids/wlg_0_01_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/grids/wlg_0_05_nb_1_1.py` & `nzshm_common-0.5.1/nzshm_common/grids/wlg_0_05_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/location/code_location.py` & `nzshm_common-0.5.1/nzshm_common/location/code_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/location/location.py` & `nzshm_common-0.5.1/nzshm_common/location/location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/location/locations.json` & `nzshm_common-0.5.1/nzshm_common/location/locations.json`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/nzshm_common/util/compression.py` & `nzshm_common-0.5.1/nzshm_common/util/compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/pyproject.toml` & `nzshm_common-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nzshm-common"
-version = "0.5.0"
+version = "0.5.1"
 homepage = "https://github.com/GNS-Science/nzshm-common-py"
 description = "A small pure python library for shared NZ NSHM data like locations."
 authors = ["GNS Science <chrisbc@artisan.co.nz>"]
 readme = "README.md"
 license = "GNU Affero V3"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -17,21 +17,24 @@
     'Programming Language :: Python :: 3.10',
 ]
 packages = [
 	{ include = "nzshm_common" },
 	{ include = "tests", format = "sdist" }
 ]
 
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-geopandas = {version = "^0.12.2", optional = true}
 
-[tool.poetry.extras]
+[tool.poetry.group.geometry.dependencies]
+shapely = {version = "^2.0.1"}
+geopandas = {version = "^0.12.2"}
 
-geometry = ["geopandas"]
+[tool.poetry.extras]
+geometry = ["geopandas", "shapely"]
 
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
     "flake8",
@@ -50,14 +53,16 @@
 mypy = {version = "^0.900"}
 pytest-cov  = { version = "^2.12.0"}
 tox = "^4.2.8"
 virtualenv  = { version = "^20.2.2", optional = true}
 pip  = { version = "^20.3.1", optional = true}
 bump2version = "^1.0.1"
 
+
+
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ['py310', 'py39']
 include = '\.pyi?$'
 exclude = '''
 /(
```

### Comparing `nzshm_common-0.5.0/tests/test_backarc.py` & `nzshm_common-0.5.1/tests/test_backarc.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/tests/test_coded_location.py` & `nzshm_common-0.5.1/tests/test_coded_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/tests/test_compression.py` & `nzshm_common-0.5.1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/tests/test_geometry.py` & `nzshm_common-0.5.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/tests/test_location.py` & `nzshm_common-0.5.1/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/tests/test_region_grid.py` & `nzshm_common-0.5.1/tests/test_region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.5.0/PKG-INFO` & `nzshm_common-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzshm-common
-Version: 0.5.0
+Version: 0.5.1
 Summary: A small pure python library for shared NZ NSHM data like locations.
 Home-page: https://github.com/GNS-Science/nzshm-common-py
 License: GNU Affero V3
 Author: GNS Science
 Author-email: chrisbc@artisan.co.nz
 Requires-Python: >=3.8,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: geometry
 Provides-Extra: test
-Requires-Dist: geopandas (>=0.12.2,<0.13.0) ; extra == "geometry"
 Description-Content-Type: text/markdown
 
 # nzshm-common
 
 A pure python library of shared objects used in nzshm projects
 
 [![pypi](https://img.shields.io/pypi/v/nzshm-common.svg)](https://pypi.org/project/nzshm-common/)
```

