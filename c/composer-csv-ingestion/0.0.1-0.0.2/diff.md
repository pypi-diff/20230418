# Comparing `tmp/composer_csv_ingestion-0.0.1.tar.gz` & `tmp/composer_csv_ingestion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer_csv_ingestion-0.0.1.tar", last modified: Tue Apr 18 13:12:29 2023, max compression
+gzip compressed data, was "composer_csv_ingestion-0.0.2.tar", last modified: Tue Apr 18 18:44:37 2023, max compression
```

## Comparing `composer_csv_ingestion-0.0.1.tar` & `composer_csv_ingestion-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:12:29.350449 composer_csv_ingestion-0.0.1/
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     1073 2023-04-18 10:16:07.000000 composer_csv_ingestion-0.0.1/LICENSE
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     1846 2023-04-18 13:12:29.350273 composer_csv_ingestion-0.0.1/PKG-INFO
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:07.000000 composer_csv_ingestion-0.0.1/README.md
-drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:12:29.348763 composer_csv_ingestion-0.0.1/composer_csv_ingestion/
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion/__init__.py
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion/__main__.py
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     4625 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion.py
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     6250 2023-04-18 13:08:50.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion_to_landing_zone.py
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     3014 2023-04-18 13:08:55.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion_validation.py
-drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:12:29.349951 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     1846 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/PKG-INFO
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      532 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/SOURCES.txt
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        1 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/dependency_links.txt
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        1 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/not-zip-safe
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      182 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/requires.txt
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)       23 2023-04-18 13:12:29.000000 composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/top_level.txt
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      938 2023-04-18 13:12:19.000000 composer_csv_ingestion-0.0.1/pyproject.toml
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)       38 2023-04-18 13:12:29.350499 composer_csv_ingestion-0.0.1/setup.cfg
--rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      713 2023-04-18 13:10:31.000000 composer_csv_ingestion-0.0.1/setup.py
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.726310 composer_csv_ingestion-0.0.2/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     1073 2023-04-18 10:16:07.000000 composer_csv_ingestion-0.0.2/LICENSE
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      251 2023-04-18 18:44:37.726133 composer_csv_ingestion-0.0.2/PKG-INFO
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:07.000000 composer_csv_ingestion-0.0.2/README.md
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.723053 composer_csv_ingestion-0.0.2/composer_csv_ingestion/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/__init__.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/__main__.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     4625 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion.py
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.725080 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_funcs/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:01:20.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_funcs/__init__.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     8237 2023-04-18 13:09:35.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_funcs/normal_operation.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     1547 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_funcs/validation.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     6250 2023-04-18 13:08:50.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_to_landing_zone.py
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.725559 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_to_landing_zone_funcs/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:01:23.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_to_landing_zone_funcs/__init__.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     7224 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_to_landing_zone_funcs/plugins.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     3014 2023-04-18 13:08:55.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_validation.py
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.725840 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_validation_funcs/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 13:01:27.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_validation_funcs/__init__.py
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)     9158 2023-04-18 10:16:25.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_validation_funcs/main.py
+drwxr-xr-x   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:44:37.724473 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      251 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/PKG-INFO
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      976 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/SOURCES.txt
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        1 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/dependency_links.txt
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        1 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/not-zip-safe
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      138 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/requires.txt
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)       23 2023-04-18 18:44:37.000000 composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/top_level.txt
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)        0 2023-04-18 18:43:29.000000 composer_csv_ingestion-0.0.2/pyproject.toml
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)       38 2023-04-18 18:44:37.726356 composer_csv_ingestion-0.0.2/setup.cfg
+-rw-r--r--   0 phuonganhnguyen   (501) staff       (20)      878 2023-04-18 18:44:24.000000 composer_csv_ingestion-0.0.2/setup.py
```

### Comparing `composer_csv_ingestion-0.0.1/LICENSE` & `composer_csv_ingestion-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion.py` & `composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion.py`

 * *Files identical despite different names*

### Comparing `composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion_to_landing_zone.py` & `composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_to_landing_zone.py`

 * *Files identical despite different names*

### Comparing `composer_csv_ingestion-0.0.1/composer_csv_ingestion/csv_ingestion_validation.py` & `composer_csv_ingestion-0.0.2/composer_csv_ingestion/csv_ingestion_validation.py`

 * *Files identical despite different names*

### Comparing `composer_csv_ingestion-0.0.1/composer_csv_ingestion.egg-info/SOURCES.txt` & `composer_csv_ingestion-0.0.2/composer_csv_ingestion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,15 @@
 composer_csv_ingestion/csv_ingestion_to_landing_zone.py
 composer_csv_ingestion/csv_ingestion_validation.py
 composer_csv_ingestion.egg-info/PKG-INFO
 composer_csv_ingestion.egg-info/SOURCES.txt
 composer_csv_ingestion.egg-info/dependency_links.txt
 composer_csv_ingestion.egg-info/not-zip-safe
 composer_csv_ingestion.egg-info/requires.txt
-composer_csv_ingestion.egg-info/top_level.txt
+composer_csv_ingestion.egg-info/top_level.txt
+composer_csv_ingestion/csv_ingestion_funcs/__init__.py
+composer_csv_ingestion/csv_ingestion_funcs/normal_operation.py
+composer_csv_ingestion/csv_ingestion_funcs/validation.py
+composer_csv_ingestion/csv_ingestion_to_landing_zone_funcs/__init__.py
+composer_csv_ingestion/csv_ingestion_to_landing_zone_funcs/plugins.py
+composer_csv_ingestion/csv_ingestion_validation_funcs/__init__.py
+composer_csv_ingestion/csv_ingestion_validation_funcs/main.py
```

