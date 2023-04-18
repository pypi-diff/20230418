# Comparing `tmp/pysqream_blue_sqlalchemy-0.1.tar.gz` & `tmp/pysqream_blue_sqlalchemy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.1.tar", last modified: Wed Feb  8 08:25:39 2023, max compression
+gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.2.tar", last modified: Tue Apr 18 10:02:23 2023, max compression
```

## Comparing `pysqream_blue_sqlalchemy-0.1.tar` & `pysqream_blue_sqlalchemy-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-08 08:25:30.000000 pysqream_blue_sqlalchemy-0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 08:25:30.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-02-08 08:25:30.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 08:25:39.000000 pysqream_blue_sqlalchemy-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-08 08:25:30.000000 pysqream_blue_sqlalchemy-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 10:02:22.000000 pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:02:23.000000 pysqream_blue_sqlalchemy-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 10:02:07.000000 pysqream_blue_sqlalchemy-0.2/setup.py
```

### Comparing `pysqream_blue_sqlalchemy-0.1/PKG-INFO` & `pysqream_blue_sqlalchemy-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: pysqream_blue_sqlalchemy
-Version: 0.1
+Version: 0.2
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
         **********************************
         
         Requirements
         =====================
         
-        * Python > 3.7. Python 3.8.1+ recommended
+        * Python > 3.9.
         * SQLAlchemy > 1.3.18
-        * SQream Blue DB-API Connector >= 1.0.22
+        * SQream Blue DB-API Connector >= 1.0.26
         
         Installation
         =====================
         
         Install from the PyPi repository using `pip`:
         
         .. code-block:: bash
@@ -31,31 +31,33 @@
         
         Integrating with SQLAlchemy
         ----------------------------
         
         .. code-block:: python
         
             import sqlalchemy as sa
-            conn_string = 'sqream_blue://username:password@url/database'
-            engine = sa.create_engine(conn_string)
+            _access_token = "ACCESS TOKEN"
+            conn_str = f"sqream_blue://domain:443/database"
+            connect_args = {'access_token': _access_token}
+            engine = sa.create_engine(conn_string, connect_args=connect_args)
             conn = engine.connect()
             res = conn.execute("select 'Success' as Test").fetchall()
             print(res)
         
         Integrating with the IPython/Jupyter SQL Magic
         -----------------------------------------------
         
         .. code-block:: python
         
             %load_ext sql
             %config SqlMagic.autocommit=False
             %config SqlMagic.displaycon=False
             %config SqlMagic.autopandas=True
-            %env DATABASE_URL sqream_blue://sqream:sqream@product.isqream.com/master
+            %sql sqream_blue://product.isqream.com/master?access_token=<ACCESS_TOKEN>
             %sql select 'Success' as Test
         
 Keywords: database sqlalchemy sqream sqreamdb
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
```

### Comparing `pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy/dialect.py` & `pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `pysqream_blue_sqlalchemy-0.1/pysqream_blue_sqlalchemy.egg-info/PKG-INFO` & `pysqream_blue_sqlalchemy-0.2/pysqream_blue_sqlalchemy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: pysqream-blue-sqlalchemy
-Version: 0.1
+Version: 0.2
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
         **********************************
         
         Requirements
         =====================
         
-        * Python > 3.7. Python 3.8.1+ recommended
+        * Python > 3.9.
         * SQLAlchemy > 1.3.18
-        * SQream Blue DB-API Connector >= 1.0.22
+        * SQream Blue DB-API Connector >= 1.0.26
         
         Installation
         =====================
         
         Install from the PyPi repository using `pip`:
         
         .. code-block:: bash
@@ -31,31 +31,33 @@
         
         Integrating with SQLAlchemy
         ----------------------------
         
         .. code-block:: python
         
             import sqlalchemy as sa
-            conn_string = 'sqream_blue://username:password@url/database'
-            engine = sa.create_engine(conn_string)
+            _access_token = "ACCESS TOKEN"
+            conn_str = f"sqream_blue://domain:443/database"
+            connect_args = {'access_token': _access_token}
+            engine = sa.create_engine(conn_string, connect_args=connect_args)
             conn = engine.connect()
             res = conn.execute("select 'Success' as Test").fetchall()
             print(res)
         
         Integrating with the IPython/Jupyter SQL Magic
         -----------------------------------------------
         
         .. code-block:: python
         
             %load_ext sql
             %config SqlMagic.autocommit=False
             %config SqlMagic.displaycon=False
             %config SqlMagic.autopandas=True
-            %env DATABASE_URL sqream_blue://sqream:sqream@product.isqream.com/master
+            %sql sqream_blue://product.isqream.com/master?access_token=<ACCESS_TOKEN>
             %sql select 'Success' as Test
         
 Keywords: database sqlalchemy sqream sqreamdb
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
```

### Comparing `pysqream_blue_sqlalchemy-0.1/setup.py` & `pysqream_blue_sqlalchemy-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from setuptools import setup
 
 
 setup_params = dict(
     
     name =             'pysqream_blue_sqlalchemy',
-    version =          '0.1',
+    version =          '0.2',
     description =      'SQLAlchemy dialect for SQream Blue', 
     long_description = open("README.rst", "r", encoding="utf-8").read(),
     url=               "https://github.com/SQream/pysqream_blue_sqlalchemy",
     
     author =           'SQream',
     author_email =     'info@sqream.com',
     
     classifiers =      [
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     keywords = 'database sqlalchemy sqream sqreamdb',
 
-    python_requires =  '>=3.7',
+    python_requires =  '>=3.9',
     
     install_requires = ['sqlalchemy>=1.3.18',
-                        'pysqream-blue>=1.0.22',
+                        'pysqream-blue>=1.0.26',
                         'setuptools==57.4.0',
                         'pytest==6.2.3',
                         'pudb==2022.1.2',
                         'pandas==1.1.5',
                         'numpy==1.20',
                         'alembic==1.5.8'],
```

