# Comparing `tmp/rgcosm-0.0.8.tar.gz` & `tmp/rgcosm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.8.tar", last modified: Tue Apr 18 00:31:34 2023, max compression
+gzip compressed data, was "rgcosm-0.0.9.tar", last modified: Tue Apr 18 00:52:52 2023, max compression
```

## Comparing `rgcosm-0.0.8.tar` & `rgcosm-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:31:34.188307 rgcosm-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 00:31:21.000000 rgcosm-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:31:34.188307 rgcosm-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-18 00:31:21.000000 rgcosm-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 00:31:21.000000 rgcosm-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:31:34.184307 rgcosm-0.0.8/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 00:31:21.000000 rgcosm-0.0.8/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 00:31:21.000000 rgcosm-0.0.8/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-18 00:31:21.000000 rgcosm-0.0.8/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-18 00:31:21.000000 rgcosm-0.0.8/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:31:34.184307 rgcosm-0.0.8/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:31:34.000000 rgcosm-0.0.8/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 00:31:34.188307 rgcosm-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 00:52:40.000000 rgcosm-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:52:52.110964 rgcosm-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-18 00:52:40.000000 rgcosm-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 00:52:40.000000 rgcosm-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 00:52:52.114964 rgcosm-0.0.9/setup.cfg
```

### Comparing `rgcosm-0.0.8/LICENSE` & `rgcosm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.8/PKG-INFO` & `rgcosm-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.8
+Version: 0.0.9
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.8/README.md` & `rgcosm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.8/rgcosm/__main__.py` & `rgcosm-0.0.9/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.8/rgcosm/convert.py` & `rgcosm-0.0.9/rgcosm/convert.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.8/rgcosm/geocoder.py` & `rgcosm-0.0.9/rgcosm/geocoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlite3
+from pathlib import Path
 import json
 import math
 
 import argparse
 
 from typing import TYPE_CHECKING
 
@@ -29,38 +30,38 @@
 	help='latitude'
 )
 parser.add_argument(
 	'-lon', '--longitude',
 	type=str,  # float
 	help='longitude'
 )
-st = parser.add_argument(
+_st = parser.add_argument(
 	'-st', '--search_tags',
 	type=str,
-	default='addr:',
-	help='tags to search, default: `addr:`'
+	default='addr:'
 )
-parser.add_argument(
+_st.help = f'tags to search, default: `{_st.default}`'
+_mtc = parser.add_argument(
 	'-mtc', '--min_tags_count',
 	type=int,
-	default=1,
-	help=f'Minimal tags count (for `{st.option_strings[0]}/{st.option_strings[1]}`) to filter result'
+	default=1
 )
-parser.add_argument(
+_mtc.help = f'Minimal tags count (for `{_st.option_strings[0]}/{_st.option_strings[1]}`) to filter result, default: {_mtc.default}'
+_rd = parser.add_argument(
 	'-rd', '--retrieve_degree',
 	type=float,
-	default=0.001,
-	help='Retrieve addresses within a +/- x degree range of the original coordinates, default: 0.001'
+	default=0.001
 )
-parser.add_argument(
+_rd.help = f'Retrieve addresses within a +/- x degree range of the original coordinates, default: {_rd.default}'
+_rt = parser.add_argument(
 	'-rt', '--round_to',
 	type=int,
-	default=8,
-	help='Round degree to n decimals after dot, default: 8'
+	default=8
 )
+_rt.help = f'Round degree to n decimals after dot, default: {_rt.default}'
 
 
 def init_args(args):
 	if not args.latitude and not args.longitude:
 		if not args.lat_lon:
 			print('Give coordinates in lat & lon')
 			exit(1)
@@ -70,14 +71,17 @@
 	args.latitude = float(args.latitude)
 	args.longitude = float(args.longitude)
 
 
 class RGeocoder():
 	def __init__(self, db_path: 'Union[str, Path]'):
 		# Connect to the database
+		if not Path(db_path).exists():
+			self.conn = None
+			raise FileNotFoundError(f'DB file `{db_path}` does not exist!')
 		self.conn = sqlite3.connect(db_path)
 		self.cursor = self.conn.cursor()
 
 
 	def find(self, lat: float, lon: float, search_tags: str = 'addr:', min_tags_count: int = 1, retrieve_degree: float = 0.001, round_to: int = 8) -> 'Optional[dict]':
 		self.cursor.execute('''
 			SELECT id, lat, lon, tags
@@ -131,17 +135,18 @@
 			min_address = self.find(lat, lon, search_tags, min_tags_count, retrieve_degree, round_to)
 			if min_address:
 				addresses.append(min_address)
 		return addresses if addresses else None
 
 
 	def __del__(self):
-		self.conn.close()
-		del self.cursor
-		del self.conn
+		if self.conn:
+			self.conn.close()
+			del self.cursor
+			del self.conn
 
 
 	def __enter__(self):
 		return self
 
 
 	def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `rgcosm-0.0.8/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.0.9/rgcosm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.8
+Version: 0.0.9
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.8/setup.cfg` & `rgcosm-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.8
+version = 0.0.9
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

