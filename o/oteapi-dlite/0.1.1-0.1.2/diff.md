# Comparing `tmp/oteapi-dlite-0.1.1.tar.gz` & `tmp/oteapi-dlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oteapi-dlite-0.1.1.tar", last modified: Mon Jan  2 09:34:56 2023, max compression
+gzip compressed data, was "oteapi-dlite-0.1.2.tar", last modified: Tue Apr 18 14:20:15 2023, max compression
```

## Comparing `oteapi-dlite-0.1.1.tar` & `oteapi-dlite-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.383825 oteapi-dlite-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-02 09:34:56.383825 oteapi-dlite-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.379825 oteapi-dlite-0.1.1/oteapi_dlite/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-02 09:34:35.000000 oteapi-dlite-0.1.1/oteapi_dlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.379825 oteapi-dlite-0.1.1/oteapi_dlite/models/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/models/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.383825 oteapi-dlite-0.1.1/oteapi_dlite/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/strategies/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.383825 oteapi-dlite-0.1.1/oteapi_dlite/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/utils/nputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/oteapi_dlite/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 09:34:56.379825 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-02 09:34:56.000000 oteapi-dlite-0.1.1/oteapi_dlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-02 09:34:56.383825 oteapi-dlite-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-02 09:29:04.000000 oteapi-dlite-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 14:19:42.000000 oteapi-dlite-0.1.2/oteapi_dlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/models/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/oteapi_dlite/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/oteapi_dlite/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/nputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 14:20:15.486499 oteapi-dlite-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/setup.py
```

### Comparing `oteapi-dlite-0.1.1/LICENSE` & `oteapi-dlite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/PKG-INFO` & `oteapi-dlite-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-dlite
-Version: 0.1.1
+Version: 0.1.2
 Summary: DLite plugin for OTEAPI.
 Home-page: https://github.com/EMMC-ASBL/oteapi-dlite
 Author: team4.0@sintef.no
 Author-email: team4.0@sintef.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-dlite-0.1.1/README.md` & `oteapi-dlite-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/filter.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/filter.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/function.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/function.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/mapping.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/mapping.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse_excel.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_excel.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/parse_image.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_image.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/strategies/serialise.py` & `oteapi-dlite-0.1.2/oteapi_dlite/strategies/serialise.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/utils/nputils.py` & `oteapi-dlite-0.1.2/oteapi_dlite/utils/nputils.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite/utils/utils.py` & `oteapi-dlite-0.1.2/oteapi_dlite/utils/utils.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite.egg-info/PKG-INFO` & `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-dlite
-Version: 0.1.1
+Version: 0.1.2
 Summary: DLite plugin for OTEAPI.
 Home-page: https://github.com/EMMC-ASBL/oteapi-dlite
 Author: team4.0@sintef.no
 Author-email: team4.0@sintef.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite.egg-info/SOURCES.txt` & `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/oteapi_dlite.egg-info/entry_points.txt` & `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/pyproject.toml` & `oteapi-dlite-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/setup.cfg` & `oteapi-dlite-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.1/setup.py` & `oteapi-dlite-0.1.2/setup.py`

 * *Files identical despite different names*

