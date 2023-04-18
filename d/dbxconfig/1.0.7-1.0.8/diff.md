# Comparing `tmp/dbxconfig-1.0.7.tar.gz` & `tmp/dbxconfig-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.7.tar", last modified: Tue Apr 18 14:12:46 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.8.tar", last modified: Tue Apr 18 16:03:39 2023, max compression
```

## Comparing `dbxconfig-1.0.7.tar` & `dbxconfig-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.433217 dbxconfig-1.0.7/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 14:12:46.433093 dbxconfig-1.0.7/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.7/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.432036 dbxconfig-1.0.7/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      435 2023-04-18 13:06:37.000000 dbxconfig-1.0.7/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1962 2023-04-18 13:56:25.000000 dbxconfig-1.0.7/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      166 2023-04-18 13:12:17.000000 dbxconfig-1.0.7/dbxconfig/_stage_type.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      780 2023-04-18 08:59:52.000000 dbxconfig-1.0.7/dbxconfig/_table.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3479 2023-04-18 13:00:31.000000 dbxconfig-1.0.7/dbxconfig/_tables.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.7/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.7/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.432921 dbxconfig-1.0.7/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      367 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.7/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-18 14:12:46.433257 dbxconfig-1.0.7/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-18 14:12:24.000000 dbxconfig-1.0.7/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 16:03:39.020072 dbxconfig-1.0.8/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 16:03:39.019952 dbxconfig-1.0.8/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.8/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 16:03:39.018180 dbxconfig-1.0.8/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      435 2023-04-18 13:06:37.000000 dbxconfig-1.0.8/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1962 2023-04-18 13:56:25.000000 dbxconfig-1.0.8/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      166 2023-04-18 13:12:17.000000 dbxconfig-1.0.8/dbxconfig/_stage_type.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      780 2023-04-18 08:59:52.000000 dbxconfig-1.0.8/dbxconfig/_table.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3479 2023-04-18 13:00:31.000000 dbxconfig-1.0.8/dbxconfig/_tables.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.8/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.8/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 16:03:39.019776 dbxconfig-1.0.8/dbxconfig/dataset/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      200 2023-04-18 13:51:05.000000 dbxconfig-1.0.8/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      869 2023-04-18 13:38:17.000000 dbxconfig-1.0.8/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3088 2023-04-18 13:38:17.000000 dbxconfig-1.0.8/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2680 2023-04-18 13:55:24.000000 dbxconfig-1.0.8/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4910 2023-04-18 13:24:41.000000 dbxconfig-1.0.8/dbxconfig/dataset/_read.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      259 2023-04-18 13:38:17.000000 dbxconfig-1.0.8/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 16:03:39.019051 dbxconfig-1.0.8/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 16:03:39.000000 dbxconfig-1.0.8/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      544 2023-04-18 16:03:39.000000 dbxconfig-1.0.8/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-18 16:03:39.000000 dbxconfig-1.0.8/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.8/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-18 16:03:39.000000 dbxconfig-1.0.8/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-18 16:03:39.000000 dbxconfig-1.0.8/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-18 16:03:39.020117 dbxconfig-1.0.8/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1103 2023-04-18 16:03:28.000000 dbxconfig-1.0.8/setup.py
```

### Comparing `dbxconfig-1.0.7/PKG-INFO` & `dbxconfig-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.7
+Version: 1.0.8
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.7/README.md` & `dbxconfig-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig/_config.py` & `dbxconfig-1.0.8/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig/_table.py` & `dbxconfig-1.0.8/dbxconfig/_table.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig/_tables.py` & `dbxconfig-1.0.8/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig/_timeslice.py` & `dbxconfig-1.0.8/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig/_utils.py` & `dbxconfig-1.0.8/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.7/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.8/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.7
+Version: 1.0.8
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.7/setup.py` & `dbxconfig-1.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.7",
+    version="1.0.8",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
@@ -24,15 +24,17 @@
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=[
-        "dbxconfig"],
+        "dbxconfig",
+        "dbxconfig.dataset"
+    ],
     install_requires=[
           'pyspark',
           'PyYAML',
           'jinja2',
           'pydantic'
       ],
     zip_safe=False
```

