# Comparing `tmp/pokepastes-scraper-0.1.0.tar.gz` & `tmp/pokepastes-scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokepastes-scraper-0.1.0.tar", last modified: Thu Apr  6 01:21:12 2023, max compression
+gzip compressed data, was "pokepastes-scraper-0.2.0.tar", last modified: Tue Apr 18 07:32:23 2023, max compression
```

## Comparing `pokepastes-scraper-0.1.0.tar` & `pokepastes-scraper-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 01:21:12.596666 pokepastes-scraper-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2816 2023-04-06 01:21:12.594634 pokepastes-scraper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-06 00:49:45.000000 pokepastes-scraper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 01:21:12.565371 pokepastes-scraper-0.1.0/pokepastes_scraper/
--rw-rw-rw-   0        0        0     7557 2023-04-06 01:16:56.000000 pokepastes-scraper-0.1.0/pokepastes_scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 01:21:12.589686 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/
--rw-rw-rw-   0        0        0     2816 2023-04-06 01:21:12.000000 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-06 01:21:12.000000 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 01:21:12.000000 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-06 01:21:12.000000 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-06 01:21:12.000000 pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      680 2023-04-06 00:57:21.000000 pokepastes-scraper-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 01:21:12.597117 pokepastes-scraper-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.872592 pokepastes-scraper-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2951 2023-04-18 07:32:23.871107 pokepastes-scraper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2023-04-18 07:19:09.000000 pokepastes-scraper-0.2.0/README.md
+-rw-rw-rw-   0        0        0      718 2023-04-18 07:30:59.000000 pokepastes-scraper-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:32:23.873090 pokepastes-scraper-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.820014 pokepastes-scraper-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.834900 pokepastes-scraper-0.2.0/src/pokepastes_scraper/
+-rw-rw-rw-   0        0        0     7906 2023-04-18 07:11:43.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.864158 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/
+-rw-rw-rw-   0        0        0     2951 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.868623 pokepastes-scraper-0.2.0/test/
+-rw-rw-rw-   0        0        0      745 2023-04-18 07:13:19.000000 pokepastes-scraper-0.2.0/test/test_json_conversion.py
```

### Comparing `pokepastes-scraper-0.1.0/LICENSE` & `pokepastes-scraper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pokepastes-scraper-0.1.0/PKG-INFO` & `pokepastes-scraper-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.1.0
-Summary: Extracts Pokémon team information from a https://pokepast.es/ URL.
+Version: 0.2.0
+Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,47 +24,49 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/MyApaulogies/pokepastes-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pokepastes-scraper
 
-A simple library that converts a Pokemon team from https://pokepast.es to an object in Python.
+A simple library that converts a Pokemon team from https://pokepast.es to a object in Python. Supports conversion to and from JSON.
 
 ### Installation
 
-`pip install -U pokepastes-scraper`
+```
+pip install -U pokepastes-scraper
+```
 
 ### Usage 
 
 Let's say we want to parse [this team](https://pokepast.es/5c46f9ec443664cb) which Gavin Michaels used to win the [Oceania World Championships](https://victoryroadvgc.com/2023-ocic/). Simply call `team_from_url`:
 
 ```python
 import pokepastes_scraper as pastes
 
 team = pastes.team_from_url("https://pokepast.es/5c46f9ec443664cb")
 
 for mon in team.members:
-    print(f"{mon.species} with {mon.item}")
+    print(f'{mon.species} with {mon.item or "no item"} (Tera: {mon.tera_type})')
 ```
 
 Output: 
 
 ```
-Iron Hands with Assault Vest
-Amoonguss with Sitrus Berry
-Pelipper with Focus Sash
-Palafin with Mystic Water
-Baxcalibur with Dragon Fang
-Dragonite with Lum Berry
+Iron Hands with Assault Vest (Tera: Grass)
+Amoonguss with Sitrus Berry (Tera: Steel)
+Pelipper with Focus Sash (Tera: Flying)
+Palafin with Mystic Water (Tera: Water)
+Baxcalibur with Dragon Fang (Tera: Poison)
+Dragonite with Lum Berry (Tera: Flying)
 ```
 
 For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.7+. Feel freet to contact me about functionality you would like implemented.
+Tested in python 3.11, but likely compatible with 3.10+.
```

### Comparing `pokepastes-scraper-0.1.0/README.md` & `pokepastes-scraper-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 
 # pokepastes-scraper
 
-A simple library that converts a Pokemon team from https://pokepast.es to an object in Python.
+A simple library that converts a Pokemon team from https://pokepast.es to a object in Python. Supports conversion to and from JSON.
 
 ### Installation
 
-`pip install -U pokepastes-scraper`
+```
+pip install -U pokepastes-scraper
+```
 
 ### Usage 
 
 Let's say we want to parse [this team](https://pokepast.es/5c46f9ec443664cb) which Gavin Michaels used to win the [Oceania World Championships](https://victoryroadvgc.com/2023-ocic/). Simply call `team_from_url`:
 
 ```python
 import pokepastes_scraper as pastes
 
 team = pastes.team_from_url("https://pokepast.es/5c46f9ec443664cb")
 
 for mon in team.members:
-    print(f"{mon.species} with {mon.item}")
+    print(f'{mon.species} with {mon.item or "no item"} (Tera: {mon.tera_type})')
 ```
 
 Output: 
 
 ```
-Iron Hands with Assault Vest
-Amoonguss with Sitrus Berry
-Pelipper with Focus Sash
-Palafin with Mystic Water
-Baxcalibur with Dragon Fang
-Dragonite with Lum Berry
+Iron Hands with Assault Vest (Tera: Grass)
+Amoonguss with Sitrus Berry (Tera: Steel)
+Pelipper with Focus Sash (Tera: Flying)
+Palafin with Mystic Water (Tera: Water)
+Baxcalibur with Dragon Fang (Tera: Poison)
+Dragonite with Lum Berry (Tera: Flying)
 ```
 
 For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.7+. Feel freet to contact me about functionality you would like implemented.
+Tested in python 3.11, but likely compatible with 3.10+.
```

### Comparing `pokepastes-scraper-0.1.0/pokepastes_scraper.egg-info/PKG-INFO` & `pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.1.0
-Summary: Extracts Pokémon team information from a https://pokepast.es/ URL.
+Version: 0.2.0
+Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,47 +24,49 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/MyApaulogies/pokepastes-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pokepastes-scraper
 
-A simple library that converts a Pokemon team from https://pokepast.es to an object in Python.
+A simple library that converts a Pokemon team from https://pokepast.es to a object in Python. Supports conversion to and from JSON.
 
 ### Installation
 
-`pip install -U pokepastes-scraper`
+```
+pip install -U pokepastes-scraper
+```
 
 ### Usage 
 
 Let's say we want to parse [this team](https://pokepast.es/5c46f9ec443664cb) which Gavin Michaels used to win the [Oceania World Championships](https://victoryroadvgc.com/2023-ocic/). Simply call `team_from_url`:
 
 ```python
 import pokepastes_scraper as pastes
 
 team = pastes.team_from_url("https://pokepast.es/5c46f9ec443664cb")
 
 for mon in team.members:
-    print(f"{mon.species} with {mon.item}")
+    print(f'{mon.species} with {mon.item or "no item"} (Tera: {mon.tera_type})')
 ```
 
 Output: 
 
 ```
-Iron Hands with Assault Vest
-Amoonguss with Sitrus Berry
-Pelipper with Focus Sash
-Palafin with Mystic Water
-Baxcalibur with Dragon Fang
-Dragonite with Lum Berry
+Iron Hands with Assault Vest (Tera: Grass)
+Amoonguss with Sitrus Berry (Tera: Steel)
+Pelipper with Focus Sash (Tera: Flying)
+Palafin with Mystic Water (Tera: Water)
+Baxcalibur with Dragon Fang (Tera: Poison)
+Dragonite with Lum Berry (Tera: Flying)
 ```
 
 For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.7+. Feel freet to contact me about functionality you would like implemented.
+Tested in python 3.11, but likely compatible with 3.10+.
```

### Comparing `pokepastes-scraper-0.1.0/pyproject.toml` & `pokepastes-scraper-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pokepastes-scraper"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="MyApaulogies", email="myapaulogies@tuta.io" },
 ]
-description = "Extracts Pokémon team information from a https://pokepast.es/ URL."
+description = "Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 license.file = "LICENSE"
 dependencies = [
```

