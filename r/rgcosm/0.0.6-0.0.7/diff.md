# Comparing `tmp/rgcosm-0.0.6.tar.gz` & `tmp/rgcosm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.6.tar", last modified: Mon Apr 17 23:07:51 2023, max compression
+gzip compressed data, was "rgcosm-0.0.7.tar", last modified: Tue Apr 18 00:00:00 2023, max compression
```

## Comparing `rgcosm-0.0.6.tar` & `rgcosm-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 23:07:36.000000 rgcosm-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 23:07:51.071729 rgcosm-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-17 23:07:36.000000 rgcosm-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 23:07:36.000000 rgcosm-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 23:07:51.071729 rgcosm-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:00:00.891901 rgcosm-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 23:59:48.000000 rgcosm-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:00:00.891901 rgcosm-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-17 23:59:48.000000 rgcosm-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 23:59:48.000000 rgcosm-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:00:00.891901 rgcosm-0.0.7/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 23:59:48.000000 rgcosm-0.0.7/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-17 23:59:48.000000 rgcosm-0.0.7/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-17 23:59:48.000000 rgcosm-0.0.7/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-17 23:59:48.000000 rgcosm-0.0.7/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:00:00.891901 rgcosm-0.0.7/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:00:00.000000 rgcosm-0.0.7/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 00:00:00.891901 rgcosm-0.0.7/setup.cfg
```

### Comparing `rgcosm-0.0.6/LICENSE` & `rgcosm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.6/PKG-INFO` & `rgcosm-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.6
+Version: 0.0.7
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.6/README.md` & `rgcosm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.6/rgcosm/__main__.py` & `rgcosm-0.0.7/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.6/rgcosm/convert.py` & `rgcosm-0.0.7/rgcosm/convert.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.6/rgcosm/geocoder.py` & `rgcosm-0.0.7/rgcosm/geocoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 
 import argparse
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-	from typing import Union
+	from typing import Union, Optional
 	from typing import Mapping
 	from pathlib import Path
 
 parser = argparse.ArgumentParser(add_help=False)
 parser.add_argument(
 	'-db', '--database',
 	type=str,
@@ -29,25 +29,25 @@
 	help='latitude'
 )
 parser.add_argument(
 	'-lon', '--longitude',
 	type=str,  # float
 	help='longitude'
 )
-parser.add_argument(
+st = parser.add_argument(
 	'-st', '--search_tags',
 	type=str,
 	default='addr:',
 	help='tags to search, default: `addr:`'
 )
 parser.add_argument(
 	'-mtc', '--min_tags_count',
 	type=str,  # int
 	default=1,
-	help='Minimal tags count to filter'
+	help=f'Minimal tags count (for `{st.option_strings[0]}/{st.option_strings[1]}`) to filter result'
 )
 
 
 def init_args(args):
 	args.min_tags_count = int(args.min_tags_count)
 	if not args.latitude and not args.longitude:
 		if not args.lat_lon:
@@ -64,20 +64,27 @@
 	def __init__(self, db_path: 'Union[str, Path]'):
 		# Connect to the database
 		self.conn = sqlite3.connect(db_path)
 		self.cursor = self.conn.cursor()
 
 
 	def find(self, lat: float, lon: float, search_tags: str = 'addr:', min_tags_count: int = 1) -> 'Optional[dict]':
-		# Retrieve addresses within a +/- 0.01 degree range of the original coordinates
+		# Retrieve addresses within a +/- 0.001 degree range of the original coordinates
+		retrieve_degree = 0.001
+		# round to 8 decimals after dot
+		round_to = 8
 		self.cursor.execute('''
 			SELECT id, lat, lon, tags
 			FROM nodes
 			WHERE lat >= ? AND lat <= ? AND lon >= ? AND lon <= ?
-		''', (lat - 0.001, lat + 0.001, lon - 0.001, lon + 0.001))
+		''', (
+			round(lat - retrieve_degree, round_to), round(lat + retrieve_degree, round_to),
+			round(lon - retrieve_degree, round_to), round(lon + retrieve_degree, round_to)
+			)
+		)
 		rows = self.cursor.fetchall()
 		# print('Found nodes:', len(rows))
 		if len(rows) == 0:
 			return None
 
 		# Find the address with the smallest distance from the original coordinates
 		min_distance = float('inf')
```

### Comparing `rgcosm-0.0.6/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.0.7/rgcosm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.6
+Version: 0.0.7
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.0.6/setup.cfg` & `rgcosm-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.6
+version = 0.0.7
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

