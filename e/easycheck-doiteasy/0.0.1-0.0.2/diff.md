# Comparing `tmp/easycheck_doiteasy-0.0.1.tar.gz` & `tmp/easycheck_doiteasy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.1.tar", last modified: Wed Apr 12 17:13:10 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.0.2.tar", last modified: Tue Apr 18 14:06:14 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.1.tar` & `easycheck_doiteasy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-12 17:13:10.015277 easycheck_doiteasy-0.0.1/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.1/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2905 2023-04-12 17:13:10.015277 easycheck_doiteasy-0.0.1/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.1/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-12 17:13:10.015277 easycheck_doiteasy-0.0.1/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       40 2023-04-12 17:08:43.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1795 2023-04-11 17:05:49.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-12 17:13:10.015277 easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2905 2023-04-12 17:13:10.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-12 17:13:10.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-12 17:13:10.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-12 17:13:10.000000 easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.1/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      678 2023-04-12 17:13:10.015277 easycheck_doiteasy-0.0.1/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.2/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.2/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       40 2023-04-12 17:08:43.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2999 2023-04-18 13:45:18.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.2/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.1/LICENSE.txt` & `easycheck_doiteasy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.1/PKG-INFO` & `easycheck_doiteasy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package example
-Home-page: https://github.com/kamicase24
+Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easycheck_doiteasy-0.0.1/README.md` & `easycheck_doiteasy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.1/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package example
-Home-page: https://github.com/kamicase24
+Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easycheck_doiteasy-0.0.1/setup.cfg` & `easycheck_doiteasy-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.1
+version = 0.0.2
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
-url = https://github.com/kamicase24
+url = https://etlcheck.com/
 project_urls = 
 	Bug Tracker = https://github.com/kamicase24/easycheck/-/issues
 	repository = https://github.com/kamicase24/easycheck
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

