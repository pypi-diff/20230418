# Comparing `tmp/airflow-provider-sqream-blue-0.0.6.tar.gz` & `tmp/airflow-provider-sqream-blue-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-provider-sqream-blue-0.0.6.tar", last modified: Tue Apr 18 14:40:49 2023, max compression
+gzip compressed data, was "dist/airflow-provider-sqream-blue-0.0.7.tar", last modified: Tue Apr 18 15:43:52 2023, max compression
```

## Comparing `airflow-provider-sqream-blue-0.0.6.tar` & `airflow-provider-sqream-blue-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/hooks/sqream_blue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:40:49.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-18 14:39:57.000000 airflow-provider-sqream-blue-0.0.6/sqream_blue/operators/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:52.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-18 15:43:05.000000 airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/sqream_blue.py
```

### Comparing `airflow-provider-sqream-blue-0.0.6/LICENSE` & `airflow-provider-sqream-blue-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.6/PKG-INFO` & `airflow-provider-sqream-blue-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sqream-blue
-Version: 0.0.6
+Version: 0.0.7
 Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
 Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Framework :: Apache Airflow
```

### Comparing `airflow-provider-sqream-blue-0.0.6/README.rst` & `airflow-provider-sqream-blue-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.6/airflow_provider_sqream_blue.egg-info/PKG-INFO` & `airflow-provider-sqream-blue-0.0.7/airflow_provider_sqream_blue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sqream-blue
-Version: 0.0.6
+Version: 0.0.7
 Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
 Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Framework :: Apache Airflow
```

### Comparing `airflow-provider-sqream-blue-0.0.6/setup.py` & `airflow-provider-sqream-blue-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 """Perform the package sqream_blue-provider setup."""
 setup(
     name='airflow-provider-sqream-blue',
-    version="0.0.6",
+    version="0.0.7",
     description='About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         "apache_airflow_provider": [
             "provider_info=sqream_blue.__init__:get_provider_info"
         ]
```

### Comparing `airflow-provider-sqream-blue-0.0.6/sqream_blue/__init__.py` & `airflow-provider-sqream-blue-0.0.7/sqream_blue/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.6/sqream_blue/hooks/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.7/sqream_blue/hooks/sqream_blue.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.6/sqream_blue/operators/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.7/sqream_blue/operators/sqream_blue.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,18 +30,19 @@
             if not description:
                 raise RuntimeError(
                     f"The query did not return descriptions of the cursor for query number {idx}. "
                     "Cannot return values in a form of dictionary for that query."
                 )
             validated_descriptions.append(description)
         returned_results = []
-        for result_id, result_list in enumerate(results):
-            current_processed_result = []
-            if result_list is not None:
-                for row in result_list:
-                    dict_result: dict[Any, Any] = {}
-                    for idx, description in enumerate(validated_descriptions[result_id]):
-                        dict_result[description[0]] = row[idx]
-                    current_processed_result.append(dict_result)
-            returned_results.append(current_processed_result)
-        self.log.info("All results %s", returned_results)
-        return returned_results
+        if results is not None:
+            for result_id, result_list in enumerate(results):
+                current_processed_result = []
+                if result_list is not None:
+                    for row in result_list:
+                        dict_result: dict[Any, Any] = {}
+                        for idx, description in enumerate(validated_descriptions[result_id]):
+                            dict_result[description[0]] = row[idx]
+                        current_processed_result.append(dict_result)
+                returned_results.append(current_processed_result)
+            self.log.info("All results %s", returned_results)
+            return returned_results
```

