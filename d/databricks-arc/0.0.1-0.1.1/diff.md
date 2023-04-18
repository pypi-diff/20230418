# Comparing `tmp/databricks-arc-0.0.1.tar.gz` & `tmp/databricks-arc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-arc-0.0.1.tar", last modified: Thu Mar  2 19:26:25 2023, max compression
+gzip compressed data, was "databricks-arc-0.1.1.tar", last modified: Tue Apr 18 19:20:19 2023, max compression
```

## Comparing `databricks-arc-0.0.1.tar` & `databricks-arc-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,37 @@
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-03-02 19:26:25.466400 databricks-arc-0.0.1/
--rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-03-02 19:26:25.466561 databricks-arc-0.0.1/PKG-INFO
--rw-r--r--   0 milos.colic   (502) staff       (20)       12 2023-02-28 19:57:43.000000 databricks-arc-0.0.1/README.md
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-03-02 19:26:25.459173 databricks-arc-0.0.1/arc/
--rw-r--r--   0 milos.colic   (502) staff       (20)       24 2023-02-28 19:33:41.000000 databricks-arc-0.0.1/arc/__init__.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-03-02 19:26:25.462884 databricks-arc-0.0.1/databricks_arc.egg-info/
--rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-03-02 19:26:25.000000 databricks-arc-0.0.1/databricks_arc.egg-info/PKG-INFO
--rw-r--r--   0 milos.colic   (502) staff       (20)      286 2023-03-02 19:26:25.000000 databricks-arc-0.0.1/databricks_arc.egg-info/SOURCES.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)        1 2023-03-02 19:26:25.000000 databricks-arc-0.0.1/databricks_arc.egg-info/dependency_links.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)       41 2023-03-02 19:26:25.000000 databricks-arc-0.0.1/databricks_arc.egg-info/requires.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)        9 2023-03-02 19:26:25.000000 databricks-arc-0.0.1/databricks_arc.egg-info/top_level.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)     1184 2023-03-02 19:26:25.467414 databricks-arc-0.0.1/setup.cfg
--rw-r--r--   0 milos.colic   (502) staff       (20)      104 2022-10-14 11:37:53.000000 databricks-arc-0.0.1/setup.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-03-02 19:26:25.465360 databricks-arc-0.0.1/test/
--rw-r--r--   0 milos.colic   (502) staff       (20)        0 2022-06-19 17:01:44.000000 databricks-arc-0.0.1/test/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)      343 2023-02-28 19:51:23.000000 databricks-arc-0.0.1/test/arc_test.py
--rw-r--r--   0 milos.colic   (502) staff       (20)      167 2023-03-02 10:54:03.000000 databricks-arc-0.0.1/test/dummy_test.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.008158 databricks-arc-0.1.1/
+-rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-04-18 19:20:19.008400 databricks-arc-0.1.1/PKG-INFO
+-rw-r--r--   0 milos.colic   (502) staff       (20)       12 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/README.md
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.956431 databricks-arc-0.1.1/arc/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       51 2023-04-18 19:17:37.000000 databricks-arc-0.1.1/arc/__init__.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.960488 databricks-arc-0.1.1/arc/autolinker/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-03-21 16:51:08.000000 databricks-arc-0.1.1/arc/autolinker/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)    37669 2023-04-14 16:24:50.000000 databricks-arc-0.1.1/arc/autolinker/autolinker.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)    12472 2023-03-18 11:32:06.000000 databricks-arc-0.1.1/arc/autolinker/splink_mlflow.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.988706 databricks-arc-0.1.1/arc/lib/
+-rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-03-16 14:35:13.000000 databricks-arc-0.1.1/arc/lib/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)  5327450 2023-04-18 19:10:13.000000 databricks-arc-0.1.1/arc/lib/arc-0.0.1-jar-with-dependencies.jar
+-rw-r--r--   0 milos.colic   (502) staff       (20)   104860 2023-04-18 19:10:13.000000 databricks-arc-0.1.1/arc/lib/arc-0.0.1.jar
+-rw-r--r--   0 milos.colic   (502) staff       (20)  5327451 2023-04-18 19:19:27.000000 databricks-arc-0.1.1/arc/lib/arc-0.1.1-jar-with-dependencies.jar
+-rw-r--r--   0 milos.colic   (502) staff       (20)   104861 2023-04-18 19:19:27.000000 databricks-arc-0.1.1/arc/lib/arc-0.1.1.jar
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.991100 databricks-arc-0.1.1/arc/sql/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       50 2023-03-21 10:57:09.000000 databricks-arc-0.1.1/arc/sql/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      466 2023-03-21 16:51:08.000000 databricks-arc-0.1.1/arc/sql/enable_arc.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.994359 databricks-arc-0.1.1/arc/sql/functions/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       56 2023-03-21 11:00:23.000000 databricks-arc-0.1.1/arc/sql/functions/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     2663 2023-04-14 15:50:48.000000 databricks-arc-0.1.1/arc/sql/functions/functions.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     3561 2023-03-21 10:51:29.000000 databricks-arc-0.1.1/arc/sql/functions/library_handler.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.001293 databricks-arc-0.1.1/databricks_arc.egg-info/
+-rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/PKG-INFO
+-rw-r--r--   0 milos.colic   (502) staff       (20)      727 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)        1 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)       41 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/requires.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)        9 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/top_level.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)     1184 2023-04-18 19:20:19.009712 databricks-arc-0.1.1/setup.cfg
+-rw-r--r--   0 milos.colic   (502) staff       (20)      104 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/setup.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.003054 databricks-arc-0.1.1/test/
+-rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/test/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      667 2023-04-14 15:50:48.000000 databricks-arc-0.1.1/test/test_arc_sql.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.006795 databricks-arc-0.1.1/test/utils/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-03-16 16:33:36.000000 databricks-arc-0.1.1/test/utils/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      827 2023-03-16 15:12:28.000000 databricks-arc-0.1.1/test/utils/arc_test.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     1160 2023-03-18 23:48:54.000000 databricks-arc-0.1.1/test/utils/spark_test_case.py
```

### Comparing `databricks-arc-0.0.1/PKG-INFO` & `databricks-arc-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-arc
-Version: 0.0.1
+Version: 0.1.1
 Summary: ARC: data linking solution for Databricks with Splink
 Home-page: https://github.com/databricks-industry-solutions/splink-public-sector-hackathon
 Author: Databricks
 License: Databricks License
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
```

### Comparing `databricks-arc-0.0.1/databricks_arc.egg-info/PKG-INFO` & `databricks-arc-0.1.1/databricks_arc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-arc
-Version: 0.0.1
+Version: 0.1.1
 Summary: ARC: data linking solution for Databricks with Splink
 Home-page: https://github.com/databricks-industry-solutions/splink-public-sector-hackathon
 Author: Databricks
 License: Databricks License
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
```

### Comparing `databricks-arc-0.0.1/setup.cfg` & `databricks-arc-0.1.1/setup.cfg`

 * *Files identical despite different names*

