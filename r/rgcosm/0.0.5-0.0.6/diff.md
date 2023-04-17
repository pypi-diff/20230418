# Comparing `tmp/rgcosm-0.0.5.tar.gz` & `tmp/rgcosm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.0.5.tar", last modified: Thu Apr 13 23:45:55 2023, max compression
+gzip compressed data, was "rgcosm-0.0.6.tar", last modified: Mon Apr 17 23:07:51 2023, max compression
```

## Comparing `rgcosm-0.0.5.tar` & `rgcosm-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:45:55.747064 rgcosm-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 23:45:41.000000 rgcosm-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 23:45:55.747064 rgcosm-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-13 23:45:41.000000 rgcosm-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 23:45:41.000000 rgcosm-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:45:55.743064 rgcosm-0.0.5/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 23:45:41.000000 rgcosm-0.0.5/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 23:45:41.000000 rgcosm-0.0.5/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-13 23:45:41.000000 rgcosm-0.0.5/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-13 23:45:41.000000 rgcosm-0.0.5/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:45:55.747064 rgcosm-0.0.5/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 23:45:55.000000 rgcosm-0.0.5/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 23:45:55.747064 rgcosm-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 23:07:36.000000 rgcosm-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 23:07:51.071729 rgcosm-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-17 23:07:36.000000 rgcosm-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 23:07:36.000000 rgcosm-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-17 23:07:36.000000 rgcosm-0.0.6/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:07:51.071729 rgcosm-0.0.6/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 23:07:51.000000 rgcosm-0.0.6/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 23:07:51.071729 rgcosm-0.0.6/setup.cfg
```

### Comparing `rgcosm-0.0.5/LICENSE` & `rgcosm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.5/PKG-INFO` & `rgcosm-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.5
+Version: 0.0.6
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -36,19 +36,19 @@
 ```
 
 ### Dependencies
 1. osmium
 
 ### CLI
 See cli commands by:
-```
-python coordinates_to_address.py -h
+```bash
+python rgcosm -h
 ```
 output:
-```
+```bash
 usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
               [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -71,15 +71,15 @@
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
                         Minimal tags count to filter
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
-Then use convert.py to create the database (speedupped by using db in ram & dump in to disk):
+Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
 python rgcosm -ci some-place.osm.pbf -co some-place.db
 ```
 
 The output file can be x7-13 (for maldives file ~12.74 times) times larger then the source file, for example [maldives](https://download.geofabrik.de/asia/maldives-latest.osm.pbf) file size is 2.7 mb, and after conversion size increased to 34.4 mb (time: ~14 sec.) with added indexes and 20.1 mb without (time: ~13 sec.).
 
 You can disable adding indexes by `-ai=no` or `--add_indexes=no` arg.
@@ -91,41 +91,41 @@
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = (6.5506617, 72.9530232)
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
+```python
 [{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}]
 ```
 or with multiple coordinates:
 ```python
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = [(6.5506617, 72.9530232), (4.172474, 73.5083067), (4.1718557, 73.5154427)]
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
-: 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
+```python
+[{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
 ```
 
 Advanced (for keep connection to db):
 ```python
 from rgcosm import RGeocoder
 db_path = 'maldives-latest.db'
 geo = RGeocoder(db_path)
 coordinates = [(4.1758869, 73.5094013), (-0.6699146, 73.1228688), (5.159217, 73.1312907)]
 addrs = geo.locate(coordinates, 'addr:', 1)
 print(addrs)
 ```
 result:
-```
+```python
 [{'id': 10300135473, 'lat': 4.1758869, 'lon': 73.5094013, 'tags': {'addr:city': "Male'", 'email': 'silverlinehotelsupplier@gmail.com', 'name': 'Silverline Hotel Supplies', 'office': 'company', 'phone': '732-9577', 'website': 'http://www.silverlineenterprise.com/'}}, {'id': 9446166886, 'lat': -0.6699146, 'lon': 73.1228688, 'tags': {'addr:city': 'Addu City', 'addr:housenumber': 'Mushkuraanaage', 'addr:postcode': '19030', 'addr:street': 'Dhandivara Maga'}}, {'id': 8439302155, 'lat': 5.159217, 'lon': 73.1312907, 'tags': {'addr:city': 'Dharavandhoo', 'addr:postcode': '06060', 'amenity': 'courthouse', 'name': 'Dharavandhoo Magistrate Court', 'opening_hours': 'Sa-Th 08:00-14:00', 'operator': 'Government of Maldives'}}]
 ```
 
 ### In plans:
 - [ ] db serializing with lz4 compression & etc.
 - [ ] Add more formats for addresses
 - [ ] Add caching results
```

### Comparing `rgcosm-0.0.5/README.md` & `rgcosm-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 ```
 
 ### Dependencies
 1. osmium
 
 ### CLI
 See cli commands by:
-```
-python coordinates_to_address.py -h
+```bash
+python rgcosm -h
 ```
 output:
-```
+```bash
 usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
               [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -51,15 +51,15 @@
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
                         Minimal tags count to filter
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
-Then use convert.py to create the database (speedupped by using db in ram & dump in to disk):
+Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
 python rgcosm -ci some-place.osm.pbf -co some-place.db
 ```
 
 The output file can be x7-13 (for maldives file ~12.74 times) times larger then the source file, for example [maldives](https://download.geofabrik.de/asia/maldives-latest.osm.pbf) file size is 2.7 mb, and after conversion size increased to 34.4 mb (time: ~14 sec.) with added indexes and 20.1 mb without (time: ~13 sec.).
 
 You can disable adding indexes by `-ai=no` or `--add_indexes=no` arg.
@@ -71,41 +71,41 @@
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = (6.5506617, 72.9530232)
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
+```python
 [{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}]
 ```
 or with multiple coordinates:
 ```python
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = [(6.5506617, 72.9530232), (4.172474, 73.5083067), (4.1718557, 73.5154427)]
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
-: 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
+```python
+[{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
 ```
 
 Advanced (for keep connection to db):
 ```python
 from rgcosm import RGeocoder
 db_path = 'maldives-latest.db'
 geo = RGeocoder(db_path)
 coordinates = [(4.1758869, 73.5094013), (-0.6699146, 73.1228688), (5.159217, 73.1312907)]
 addrs = geo.locate(coordinates, 'addr:', 1)
 print(addrs)
 ```
 result:
-```
+```python
 [{'id': 10300135473, 'lat': 4.1758869, 'lon': 73.5094013, 'tags': {'addr:city': "Male'", 'email': 'silverlinehotelsupplier@gmail.com', 'name': 'Silverline Hotel Supplies', 'office': 'company', 'phone': '732-9577', 'website': 'http://www.silverlineenterprise.com/'}}, {'id': 9446166886, 'lat': -0.6699146, 'lon': 73.1228688, 'tags': {'addr:city': 'Addu City', 'addr:housenumber': 'Mushkuraanaage', 'addr:postcode': '19030', 'addr:street': 'Dhandivara Maga'}}, {'id': 8439302155, 'lat': 5.159217, 'lon': 73.1312907, 'tags': {'addr:city': 'Dharavandhoo', 'addr:postcode': '06060', 'amenity': 'courthouse', 'name': 'Dharavandhoo Magistrate Court', 'opening_hours': 'Sa-Th 08:00-14:00', 'operator': 'Government of Maldives'}}]
 ```
 
 ### In plans:
 - [ ] db serializing with lz4 compression & etc.
 - [ ] Add more formats for addresses
 - [ ] Add caching results
```

### Comparing `rgcosm-0.0.5/rgcosm/__main__.py` & `rgcosm-0.0.6/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.5/rgcosm/convert.py` & `rgcosm-0.0.6/rgcosm/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import osmium
 import json
 import sqlite3
+import datetime
 
 import argparse
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-	from typing import Optional
+	from typing import Union
 	from pathlib import Path
 
 parser = argparse.ArgumentParser(add_help=False)
 parser.add_argument(
 	'-ci', '--cinput',
 	type=str,
 	help='Path to input pbf file'
@@ -41,19 +42,19 @@
 		args.coutput = ''.join((fn, '.db'))
 	if args.cinput == args.coutput:
 		print('You want to save file with the same name as the input file!')
 		exit(1)
 
 
 class OsmHandler(osmium.SimpleHandler):
-	def __init__(self, output: 'Optional[str]' = None):
+	def __init__(self, output: 'Union[str, Path]' = ''):
 		osmium.SimpleHandler.__init__(self)
 		self.conn = sqlite3.connect(':memory:')
-		self.output = output
-		self.conn_file = sqlite3.connect(output)
+		self.output = output if output else datetime.datetime.strftime(datetime.datetime.now(), "osm-%y-%m-%d-%H-%M-%S.db")
+		self.conn_file = sqlite3.connect(self.output)
 		self.cursor = self.conn.cursor()
 		self.cursor.execute('''CREATE TABLE IF NOT EXISTS nodes (id INTEGER PRIMARY KEY, lat REAL, lon REAL, tags TEXT)''')
 		self.cursor.execute('''CREATE TABLE IF NOT EXISTS ways (id INTEGER PRIMARY KEY, nodes INTEGER, tags TEXT)''')
 		self.conn.commit()
 
 
 	def node(self, n):
@@ -74,26 +75,28 @@
 
 
 	def add_indexes(self):
 		self.cursor.execute('''CREATE INDEX "nodes index lat" ON "nodes" ( "lat" )''')
 		self.cursor.execute('''CREATE INDEX "nodes index lon" ON "nodes" ( "lon" )''')
 
 
-def osm2sqlite3(input_fpath: 'Union[str, Path]', output_fpath: 'Union[str, Path]', add_indexes: bool = True) -> 'Path':
+def osm2sqlite3(input_fpath: 'Union[str, Path]', output_fpath: 'Union[str, Path]', add_indexes: bool = True) -> bool:
 	# Conversion by handler
 	handler = OsmHandler(output_fpath)
 	handler.apply_file(input_fpath)
 
 	# Add indexes in db to speedup search
 	if add_indexes:
 		handler.add_indexes()
 	handler.conn.commit()
 	handler.save()
 	handler.conn.close()
 
+	return True
+
 
 def main():
 	args = parser.parse_args()
 
 	osm2sqlite3(args.input, args.output, args.add_indexes)
```

### Comparing `rgcosm-0.0.5/rgcosm/geocoder.py` & `rgcosm-0.0.6/rgcosm/geocoder.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.0.5/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.0.6/rgcosm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.0.5
+Version: 0.0.6
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -36,19 +36,19 @@
 ```
 
 ### Dependencies
 1. osmium
 
 ### CLI
 See cli commands by:
-```
-python coordinates_to_address.py -h
+```bash
+python rgcosm -h
 ```
 output:
-```
+```bash
 usage: rgcosm [-h] [-ci CINPUT] [-co COUTPUT] [-ai ADD_INDEXES]
               [-db DATABASE] [-ltln LAT_LON] [-lat LATITUDE] [-lon LONGITUDE] [-st SEARCH_TAGS] [-mtc MIN_TAGS_COUNT]
 
 rgcosm cli
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -71,15 +71,15 @@
   -mtc MIN_TAGS_COUNT, --min_tags_count MIN_TAGS_COUNT
                         Minimal tags count to filter
 ```
 
 ### First convert downloaded osm(.pbf) files from:
 https://download.geofabrik.de/
 
-Then use convert.py to create the database (speedupped by using db in ram & dump in to disk):
+Then use cli to create the database (speedupped by using db in ram & dump in to disk):
 ```bash
 python rgcosm -ci some-place.osm.pbf -co some-place.db
 ```
 
 The output file can be x7-13 (for maldives file ~12.74 times) times larger then the source file, for example [maldives](https://download.geofabrik.de/asia/maldives-latest.osm.pbf) file size is 2.7 mb, and after conversion size increased to 34.4 mb (time: ~14 sec.) with added indexes and 20.1 mb without (time: ~13 sec.).
 
 You can disable adding indexes by `-ai=no` or `--add_indexes=no` arg.
@@ -91,41 +91,41 @@
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = (6.5506617, 72.9530232)
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
+```python
 [{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}]
 ```
 or with multiple coordinates:
 ```python
 from rgcosm import get_address
 db_path = 'maldives-latest.db'
 coordinates = [(6.5506617, 72.9530232), (4.172474, 73.5083067), (4.1718557, 73.5154427)]
 addr = get_address(db_path, coordinates)
 print(addr)
 ```
 result:
-```bash
-: 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
+```python
+[{'id': 9508099415, 'lat': 6.5506617, 'lon': 72.9530232, 'tags': {'addr:block_number': '26', 'generator:method': 'combustion', 'generator:output:electricity': '200 kV', 'generator:source': 'diesel', 'name': 'Vaikaradhoo Fenaka Power Plant 3', 'operator': 'Fenaka Corporation Limited Vaikaradhoo', 'power': 'generator'}}, {'id': 2521220337, 'lat': 4.172474, 'lon': 73.5083067, 'tags': {'addr:city': "Male'", 'addr:housename': 'Ma.Seventy Flower', 'addr:street': 'Iskandharu Magu', 'amenity': 'cafe', 'cuisine': 'coffee_shop', 'internet_access': 'yes', 'name': "Chili's Café"}}, {'id': 7987147424, 'lat': 4.1718557, 'lon': 73.5154427, 'tags': {'addr:city': "Male'", 'addr:housenumber': 'H.Hostside', 'addr:postcode': '20053', 'addr:street': 'Irudheymaa Hingun', 'clothes': 'women;wedding;men;suits;fashion;children', 'contact:facebook': 'https://m.facebook.com/Aiccet/', 'currency:EUR': 'yes', 'currency:GBP': 'yes', 'currency:USD': 'yes', 'name': 'Aiccet', 'opening_hours': '24/7', 'operator': 'Aiccet', 'payment:american_express': 'yes', 'payment:cash': 'yes', 'payment:credit_cards': 'yes', 'payment:mastercard': 'yes', 'payment:visa': 'yes', 'payment:visa_debit': 'yes', 'phone': '+960 7997323', 'shop': 'clothes'}}]
 ```
 
 Advanced (for keep connection to db):
 ```python
 from rgcosm import RGeocoder
 db_path = 'maldives-latest.db'
 geo = RGeocoder(db_path)
 coordinates = [(4.1758869, 73.5094013), (-0.6699146, 73.1228688), (5.159217, 73.1312907)]
 addrs = geo.locate(coordinates, 'addr:', 1)
 print(addrs)
 ```
 result:
-```
+```python
 [{'id': 10300135473, 'lat': 4.1758869, 'lon': 73.5094013, 'tags': {'addr:city': "Male'", 'email': 'silverlinehotelsupplier@gmail.com', 'name': 'Silverline Hotel Supplies', 'office': 'company', 'phone': '732-9577', 'website': 'http://www.silverlineenterprise.com/'}}, {'id': 9446166886, 'lat': -0.6699146, 'lon': 73.1228688, 'tags': {'addr:city': 'Addu City', 'addr:housenumber': 'Mushkuraanaage', 'addr:postcode': '19030', 'addr:street': 'Dhandivara Maga'}}, {'id': 8439302155, 'lat': 5.159217, 'lon': 73.1312907, 'tags': {'addr:city': 'Dharavandhoo', 'addr:postcode': '06060', 'amenity': 'courthouse', 'name': 'Dharavandhoo Magistrate Court', 'opening_hours': 'Sa-Th 08:00-14:00', 'operator': 'Government of Maldives'}}]
 ```
 
 ### In plans:
 - [ ] db serializing with lz4 compression & etc.
 - [ ] Add more formats for addresses
 - [ ] Add caching results
```

### Comparing `rgcosm-0.0.5/setup.cfg` & `rgcosm-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.0.5
+version = 0.0.6
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls =
```

