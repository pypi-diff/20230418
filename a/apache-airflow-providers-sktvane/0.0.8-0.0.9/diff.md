# Comparing `tmp/apache-airflow-providers-sktvane-0.0.8.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.0.8.tar", last modified: Thu Mar  9 02:14:59 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.0.9.tar", last modified: Thu Mar  9 02:26:42 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.0.8.tar` & `apache-airflow-providers-sktvane-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.172587 apache-airflow-providers-sktvane-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-09 02:14:59.172587 apache-airflow-providers-sktvane-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.168588 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:14:59.172587 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-09 02:14:59.000000 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-09 02:14:59.000000 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 02:14:59.000000 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-09 02:14:59.000000 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 02:14:59.000000 apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-09 02:14:59.172587 apache-airflow-providers-sktvane-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 02:14:55.000000 apache-airflow-providers-sktvane-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.0.8/PKG-INFO` & `apache-airflow-providers-sktvane-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.0.8
-Summary: apache-airflow-providers-sktvane
+Version: 0.0.9
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: UNKNOWN
 Author: lapetus
 Author-email: lapetus@sktai.io
 License: MIT
 Project-URL: Homepage, https://github.com/sktaiflow/apache-airflow-providers-sktvane
 Project-URL: Source Code, https://github.com/sktaiflow/apache-airflow-providers-sktvane
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/nes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.0.8/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.0.8
-Summary: apache-airflow-providers-sktvane
+Version: 0.0.9
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: UNKNOWN
 Author: lapetus
 Author-email: lapetus@sktai.io
 License: MIT
 Project-URL: Homepage, https://github.com/sktaiflow/apache-airflow-providers-sktvane
 Project-URL: Source Code, https://github.com/sktaiflow/apache-airflow-providers-sktvane
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.0.8/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.0.8/setup.cfg` & `apache-airflow-providers-sktvane-0.0.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = apache-airflow-providers-sktvane
 version = attr: airflow.providers.sktvane.VERSION
 author = lapetus
 author_email = lapetus@sktai.io
-description = apache-airflow-providers-sktvane
+description = Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = airflow, sktvane
 license = MIT
 license_files = LICENSE.txt
 python_requires = ">=3.9"
 project_urls =
```

