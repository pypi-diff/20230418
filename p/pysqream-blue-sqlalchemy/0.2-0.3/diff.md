# Comparing `tmp/pysqream_blue_sqlalchemy-0.2.tar.gz` & `tmp/pysqream_blue_sqlalchemy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.2.tar", last modified: Tue Apr 18 10:02:23 2023, max compression
+gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.3.tar", last modified: Tue Apr 18 12:45:09 2023, max compression
```

## Comparing `pysqream_blue_sqlalchemy-0.2.tar` & `pysqream_blue_sqlalchemy-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-18 12:44:54.000000 pysqream_blue_sqlalchemy-0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:44:54.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-18 12:44:54.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 12:45:08.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:45:08.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 12:45:08.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 12:45:08.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 12:45:08.000000 pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:45:09.000000 pysqream_blue_sqlalchemy-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-18 12:44:54.000000 pysqream_blue_sqlalchemy-0.3/setup.py
```

### Comparing `pysqream_blue_sqlalchemy-0.2/PKG-INFO` & `pysqream_blue_sqlalchemy-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pysqream_blue_sqlalchemy
-Version: 0.2
+Version: 0.3
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
```

### Comparing `pysqream_blue_sqlalchemy-0.2/README.rst` & `pysqream_blue_sqlalchemy-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/dialect.py` & `pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/PKG-INFO` & `pysqream_blue_sqlalchemy-0.3/pysqream_blue_sqlalchemy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pysqream-blue-sqlalchemy
-Version: 0.2
+Version: 0.3
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
```

### Comparing `pysqream_blue_sqlalchemy-0.2/setup.py` & `pysqream_blue_sqlalchemy-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 
 setup_params = dict(
     
     name =             'pysqream_blue_sqlalchemy',
-    version =          '0.2',
+    version =          '0.3',
     description =      'SQLAlchemy dialect for SQream Blue', 
     long_description = open("README.rst", "r", encoding="utf-8").read(),
     url=               "https://github.com/SQream/pysqream_blue_sqlalchemy",
     
     author =           'SQream',
     author_email =     'info@sqream.com',
     
@@ -19,20 +19,19 @@
     ],
     keywords = 'database sqlalchemy sqream sqreamdb',
 
     python_requires =  '>=3.9',
     
     install_requires = ['sqlalchemy>=1.3.18',
                         'pysqream-blue>=1.0.26',
-                        'setuptools==57.4.0',
-                        'pytest==6.2.3',
+                        'setuptools>=57.4.0',
                         'pudb==2022.1.2',
                         'pandas==1.1.5',
                         'numpy==1.20',
-                        'alembic==1.5.8'],
+                        'alembic>=1.6.3'],
     
     packages         = ['pysqream_blue_sqlalchemy'], 
     
     entry_points =     {'sqlalchemy.dialects': 
         ['sqream_blue = pysqream_blue_sqlalchemy.dialect:SqreamBlueDialect']
     },
     # sqream://sqream:sqream@localhost/master
```

