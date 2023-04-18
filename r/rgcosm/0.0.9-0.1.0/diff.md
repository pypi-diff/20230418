# Comparing `tmp/rgcosm-0.0.9.tar.gz` & `tmp/rgcosm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.9.tar", last modified: Tue Apr 18 00:52:52 2023, max compression
+gzip compressed data, was "rgcosm-0.1.0.tar", last modified: Tue Apr 18 01:00:43 2023, max compression
```

## Comparing `rgcosm-0.0.9.tar` & `rgcosm-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 00:52:40.000000 rgcosm-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:52:52.110964 rgcosm-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-18 00:52:40.000000 rgcosm-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 00:52:40.000000 rgcosm-0.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 00:52:40.000000 rgcosm-0.0.9/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:52:52.110964 rgcosm-0.0.9/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:52:52.000000 rgcosm-0.0.9/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 00:52:52.114964 rgcosm-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:43.696698 rgcosm-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 01:00:32.000000 rgcosm-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 01:00:43.696698 rgcosm-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-18 01:00:32.000000 rgcosm-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 01:00:32.000000 rgcosm-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:43.696698 rgcosm-0.1.0/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 01:00:32.000000 rgcosm-0.1.0/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 01:00:32.000000 rgcosm-0.1.0/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 01:00:32.000000 rgcosm-0.1.0/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 01:00:32.000000 rgcosm-0.1.0/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:43.696698 rgcosm-0.1.0/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 01:00:43.000000 rgcosm-0.1.0/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 01:00:43.696698 rgcosm-0.1.0/setup.cfg
```

### Comparing `rgcosm-0.0.9/LICENSE` & `rgcosm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.9/PKG-INFO` & `rgcosm-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.9
+Version: 0.1.0
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -41,39 +41,46 @@
 ### CLI
 See cli commands by:
 ```bash
 python rgcosm -h
 ```
 output:
 ```bash
-usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
-              [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
+usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES] [-db DATABASE]
+                   [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS]
+                   [-mtc MIN_TAGS_COUNT] [-rd RETRIEVE_DEGREE] [-rt ROUND_TO]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
   -ci CINPUT, --cinput CINPUT
                         Path to input pbf file
   -co COUTPUT, --coutput COUTPUT
                         Path to output db file
   -ai ADD_INDEXES, --add_indexes ADD_INDEXES
-                        Add indexes for faster search default yes
+                        Add indexes for faster search default: True
   -db DATABASE, --database DATABASE
                         Path to db file
   -ltln LAT_LON, --lat_lon LAT_LON
                         latitude with longitude separated by space
   -lat LATITUDE, --latitude LATITUDE
                         latitude
   -lon LONGITUDE, --longitude LONGITUDE
                         longitude
   -st SEARCH_TAGS, --search_tags SEARCH_TAGS
                         tags to search, default: `addr:`
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
-                        Minimal tags count to filter
+                        Minimal tags count (for `-st/--search_tags`) to filter result,
+                        default: 1
+  -rd RETRIEVE_DEGREE, --retrieve_degree RETRIEVE_DEGREE
+                        Retrieve addresses within a +/- x degree range of the original
+                        coordinates, default: 0.001
+  -rt ROUND_TO, --round_to ROUND_TO
+                        Round degree to n decimals after dot, default: 8
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
 Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
```

### Comparing `rgcosm-0.0.9/README.md` & `rgcosm-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,39 +21,46 @@
 ### CLI
 See cli commands by:
 ```bash
 python rgcosm -h
 ```
 output:
 ```bash
-usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
-              [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
+usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES] [-db DATABASE]
+                   [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS]
+                   [-mtc MIN_TAGS_COUNT] [-rd RETRIEVE_DEGREE] [-rt ROUND_TO]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
   -ci CINPUT, --cinput CINPUT
                         Path to input pbf file
   -co COUTPUT, --coutput COUTPUT
                         Path to output db file
   -ai ADD_INDEXES, --add_indexes ADD_INDEXES
-                        Add indexes for faster search default yes
+                        Add indexes for faster search default: True
   -db DATABASE, --database DATABASE
                         Path to db file
   -ltln LAT_LON, --lat_lon LAT_LON
                         latitude with longitude separated by space
   -lat LATITUDE, --latitude LATITUDE
                         latitude
   -lon LONGITUDE, --longitude LONGITUDE
                         longitude
   -st SEARCH_TAGS, --search_tags SEARCH_TAGS
                         tags to search, default: `addr:`
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
-                        Minimal tags count to filter
+                        Minimal tags count (for `-st/--search_tags`) to filter result,
+                        default: 1
+  -rd RETRIEVE_DEGREE, --retrieve_degree RETRIEVE_DEGREE
+                        Retrieve addresses within a +/- x degree range of the original
+                        coordinates, default: 0.001
+  -rt ROUND_TO, --round_to ROUND_TO
+                        Round degree to n decimals after dot, default: 8
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
 Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
```

### Comparing `rgcosm-0.0.9/rgcosm/__main__.py` & `rgcosm-0.1.0/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.9/rgcosm/convert.py` & `rgcosm-0.1.0/rgcosm/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 	help='Path to input pbf file'
 )
 parser.add_argument(
 	'-co', '--coutput',
 	type=str,
 	help='Path to output db file'
 )
-parser.add_argument(
+_ai = parser.add_argument(
 	'-ai', '--add_indexes',
 	type=str,  # bool
 	default=True,
-	help='Add indexes for faster search default yes'
 )
+_ai.help = f'Add indexes for faster search default: {_ai.default}'
 
 
 def init_args(args):
 	if args.add_indexes in (True, 'Y', 'y', 'Yes', 'yes', 'True', 'true', '1'):
 		args.add_indexes = True
 	else:
 		args.add_indexes = False
```

### Comparing `rgcosm-0.0.9/rgcosm/geocoder.py` & `rgcosm-0.1.0/rgcosm/geocoder.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.9/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.1.0/rgcosm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.9
+Version: 0.1.0
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -41,39 +41,46 @@
 ### CLI
 See cli commands by:
 ```bash
 python rgcosm -h
 ```
 output:
 ```bash
-usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
-              [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
+usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES] [-db DATABASE]
+                   [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS]
+                   [-mtc MIN_TAGS_COUNT] [-rd RETRIEVE_DEGREE] [-rt ROUND_TO]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
   -ci CINPUT, --cinput CINPUT
                         Path to input pbf file
   -co COUTPUT, --coutput COUTPUT
                         Path to output db file
   -ai ADD_INDEXES, --add_indexes ADD_INDEXES
-                        Add indexes for faster search default yes
+                        Add indexes for faster search default: True
   -db DATABASE, --database DATABASE
                         Path to db file
   -ltln LAT_LON, --lat_lon LAT_LON
                         latitude with longitude separated by space
   -lat LATITUDE, --latitude LATITUDE
                         latitude
   -lon LONGITUDE, --longitude LONGITUDE
                         longitude
   -st SEARCH_TAGS, --search_tags SEARCH_TAGS
                         tags to search, default: `addr:`
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
-                        Minimal tags count to filter
+                        Minimal tags count (for `-st/--search_tags`) to filter result,
+                        default: 1
+  -rd RETRIEVE_DEGREE, --retrieve_degree RETRIEVE_DEGREE
+                        Retrieve addresses within a +/- x degree range of the original
+                        coordinates, default: 0.001
+  -rt ROUND_TO, --round_to ROUND_TO
+                        Round degree to n decimals after dot, default: 8
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
 Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
```

### Comparing `rgcosm-0.0.9/setup.cfg` & `rgcosm-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.9
+version = 0.1.0
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

