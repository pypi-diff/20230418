# Comparing `tmp/opentelemetry-instrumentation-kser-0.1.8.tar.gz` & `tmp/opentelemetry-instrumentation-kser-0.38b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-instrumentation-kser-0.1.8.tar", last modified: Tue May 24 16:25:06 2022, max compression
+gzip compressed data, was "opentelemetry-instrumentation-kser-0.38b0.tar", last modified: Tue Apr 18 10:05:02 2023, max compression
```

## Comparing `opentelemetry-instrumentation-kser-0.1.8.tar` & `opentelemetry-instrumentation-kser-0.38b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.473750 opentelemetry-instrumentation-kser-0.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2022-05-24 16:25:06.473750 opentelemetry-instrumentation-kser-0.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      716 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2022-05-24 16:25:06.473750 opentelemetry-instrumentation-kser-0.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1983 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.469753 opentelemetry-instrumentation-kser-0.1.8/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.469753 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.469753 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.469753 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/kser/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5715 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/kser/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/kser/package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2022-05-24 16:24:48.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/kser/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 16:25:06.473750 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2022-05-24 16:25:05.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2022-05-24 16:25:06.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-05-24 16:25:05.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2022-05-24 16:25:06.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      158 2022-05-24 16:25:06.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2022-05-24 16:25:06.000000 opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/top_level.txt
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.044335 opentelemetry-instrumentation-kser-0.38b0/
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)       60 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.38b0/MANIFEST.in
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)     1452 2023-04-18 10:05:02.044335 opentelemetry-instrumentation-kser-0.38b0/PKG-INFO
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      716 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.38b0/README.rst
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      146 2023-04-18 09:53:20.000000 opentelemetry-instrumentation-kser-0.38b0/requirements.txt
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)     1065 2023-04-18 10:05:02.044335 opentelemetry-instrumentation-kser-0.38b0/setup.cfg
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)     1983 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.38b0/setup.py
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.028335 opentelemetry-instrumentation-kser-0.38b0/src/
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.028335 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.028335 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.044335 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/kser/
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)     5715 2022-05-24 16:11:17.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/kser/__init__.py
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      147 2022-05-24 16:12:37.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/kser/package.py
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      134 2023-04-18 09:53:20.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/kser/version.py
+drwxrwxr-x   0 cdumay    (1000) cdumay    (1000)        0 2023-04-18 10:05:02.044335 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)     1452 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      583 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)        1 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)       89 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/entry_points.txt
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)      159 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/requires.txt
+-rw-rw-r--   0 cdumay    (1000) cdumay    (1000)       14 2023-04-18 10:05:01.000000 opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/top_level.txt
```

### Comparing `opentelemetry-instrumentation-kser-0.1.8/PKG-INFO` & `opentelemetry-instrumentation-kser-0.38b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-kser
-Version: 0.1.8
+Version: 0.38b0
 Summary: OpenTelemetry kser instrumentation
 Home-page: https://github.com/cdumay/opentelemetry-instrumentation-kser
 Author: Cédric Dumay
 Author-email: cedric.dumay@gmail.com
 License: BSD 3-Clause License
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -31,7 +31,8 @@
    :target: https://travis-ci.com/ovh/python-opentelemetry-instrumentation-kser
    :alt: Latest version
 
 
 .. image:: https://readthedocs.org/projects/opentelemetry-instrumentation-kser/badge/?version=latest
    :target: http://opentelemetry-instrumentation-kser.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
+
```

### Comparing `opentelemetry-instrumentation-kser-0.1.8/README.rst` & `opentelemetry-instrumentation-kser-0.38b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.1.8/setup.cfg` & `opentelemetry-instrumentation-kser-0.38b0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
-	opentelemetry-api == 1.4.1
+	opentelemetry-api == 1.17.0
 	opentelemetry-semantic-conventions
 	opentelemetry-instrumentation
 
 [options.extras_require]
 test = 
 	opentelemetry-test
```

### Comparing `opentelemetry-instrumentation-kser-0.1.8/setup.py` & `opentelemetry-instrumentation-kser-0.38b0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry/instrumentation/kser/__init__.py` & `opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry/instrumentation/kser/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO` & `opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-kser
-Version: 0.1.8
+Version: 0.38b0
 Summary: OpenTelemetry kser instrumentation
 Home-page: https://github.com/cdumay/opentelemetry-instrumentation-kser
 Author: Cédric Dumay
 Author-email: cedric.dumay@gmail.com
 License: BSD 3-Clause License
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -31,7 +31,8 @@
    :target: https://travis-ci.com/ovh/python-opentelemetry-instrumentation-kser
    :alt: Latest version
 
 
 .. image:: https://readthedocs.org/projects/opentelemetry-instrumentation-kser/badge/?version=latest
    :target: http://opentelemetry-instrumentation-kser.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
+
```

### Comparing `opentelemetry-instrumentation-kser-0.1.8/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt` & `opentelemetry-instrumentation-kser-0.38b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

