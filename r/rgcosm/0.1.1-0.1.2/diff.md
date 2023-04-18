# Comparing `tmp/rgcosm-0.1.1.tar.gz` & `tmp/rgcosm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgcosm-0.1.1.tar", last modified: Tue Apr 18 16:39:42 2023, max compression
+gzip compressed data, was "rgcosm-0.1.2.tar", last modified: Tue Apr 18 16:56:44 2023, max compression
```

## Comparing `rgcosm-0.1.1.tar` & `rgcosm-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:42.557637 rgcosm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:39:27.000000 rgcosm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 16:39:42.557637 rgcosm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-18 16:39:27.000000 rgcosm-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 16:39:27.000000 rgcosm-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:42.557637 rgcosm-0.1.1/rgcosm/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 16:39:27.000000 rgcosm-0.1.1/rgcosm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 16:39:27.000000 rgcosm-0.1.1/rgcosm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 16:39:27.000000 rgcosm-0.1.1/rgcosm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 16:39:27.000000 rgcosm-0.1.1/rgcosm/geocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:42.557637 rgcosm-0.1.1/rgcosm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:39:42.000000 rgcosm-0.1.1/rgcosm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 16:39:42.561637 rgcosm-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:56:44.874456 rgcosm-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:56:33.000000 rgcosm-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 16:56:44.874456 rgcosm-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-18 16:56:33.000000 rgcosm-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 16:56:33.000000 rgcosm-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:56:44.874456 rgcosm-0.1.2/rgcosm/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 16:56:33.000000 rgcosm-0.1.2/rgcosm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 16:56:33.000000 rgcosm-0.1.2/rgcosm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 16:56:33.000000 rgcosm-0.1.2/rgcosm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 16:56:33.000000 rgcosm-0.1.2/rgcosm/geocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:56:44.874456 rgcosm-0.1.2/rgcosm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:56:44.000000 rgcosm-0.1.2/rgcosm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 16:56:44.874456 rgcosm-0.1.2/setup.cfg
```

### Comparing `rgcosm-0.1.1/LICENSE` & `rgcosm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rgcosm-0.1.1/PKG-INFO` & `rgcosm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.1.1
+Version: 0.1.2
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.1.1/README.md` & `rgcosm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rgcosm-0.1.1/rgcosm/__main__.py` & `rgcosm-0.1.2/rgcosm/__main__.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.1.1/rgcosm/convert.py` & `rgcosm-0.1.2/rgcosm/convert.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.1.1/rgcosm/geocoder.py` & `rgcosm-0.1.2/rgcosm/geocoder.py`

 * *Files identical despite different names*

### Comparing `rgcosm-0.1.1/rgcosm.egg-info/PKG-INFO` & `rgcosm-0.1.2/rgcosm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgcosm
-Version: 0.1.1
+Version: 0.1.2
 Summary: rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 Home-page: https://github.com/BlackCatDevel0per/rgcosm
 Author: bcdev
 Author-email: bcdev@mail.ru
 Project-URL: Bug Tracker, https://github.com/BlackCatDevel0per/rgcosm/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rgcosm-0.1.1/setup.cfg` & `rgcosm-0.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rgcosm
-version = 0.1.1
+version = 0.1.2
 author = bcdev
 author_email = bcdev@mail.ru
 description = rgcosm simple reverse geocoding library from converted osm(.pbf) GIS data by converter in this lib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackCatDevel0per/rgcosm
 project_urls = 
@@ -25,15 +25,15 @@
 	= .
 packages = find:
 install_requires = 
 	osmium>=3.6.0
 
 [options.entry_points]
 console_scripts = 
-	pdf4cat = rgcosm:__main__
+	rgcosm = rgcosm:__main__
 
 [options.packages.find]
 where = .
 exclude = 
 	examples*
 	docs*
 	tests*
```

