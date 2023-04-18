# Comparing `tmp/arcane-core-1.9.0.tar.gz` & `tmp/arcane-core-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-core-1.9.0.tar", max compression
+gzip compressed data, was "arcane-core-1.9.1.tar", max compression
```

## Comparing `arcane-core-1.9.0.tar` & `arcane-core-1.9.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      179 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/__init__.py
--rw-r--r--   0        0        0      493 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/compute_names.py
--rw-r--r--   0        0        0      492 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/const.py
--rw-r--r--   0        0        0       53 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/datastore_kind.py
--rw-r--r--   0        0        0     1582 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/exceptions.py
--rw-r--r--   0        0        0      592 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/function_traces.py
--rw-r--r--   0        0        0    19104 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/types.py
--rw-r--r--   0        0        0      693 2022-08-17 13:17:15.859711 arcane-core-1.9.0/arcane/core/utils.py
--rw-r--r--   0        0        0      390 2022-08-17 13:17:15.859711 arcane-core-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      651 2022-08-17 13:17:30.206866 arcane-core-1.9.0/setup.py
--rw-r--r--   0        0        0      551 2022-08-17 13:17:30.207153 arcane-core-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      179 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/__init__.py
+-rw-r--r--   0        0        0      493 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/compute_names.py
+-rw-r--r--   0        0        0      492 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/const.py
+-rw-r--r--   0        0        0       53 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/datastore_kind.py
+-rw-r--r--   0        0        0     1582 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/exceptions.py
+-rw-r--r--   0        0        0      592 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/function_traces.py
+-rw-r--r--   0        0        0    19112 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/types.py
+-rw-r--r--   0        0        0      693 2022-08-22 07:09:28.308050 arcane-core-1.9.1/arcane/core/utils.py
+-rw-r--r--   0        0        0      390 2022-08-22 07:09:28.312050 arcane-core-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      651 2022-08-22 07:09:42.691072 arcane-core-1.9.1/setup.py
+-rw-r--r--   0        0        0      551 2022-08-22 07:09:42.691384 arcane-core-1.9.1/PKG-INFO
```

### Comparing `arcane-core-1.9.0/arcane/core/exceptions.py` & `arcane-core-1.9.1/arcane/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `arcane-core-1.9.0/arcane/core/function_traces.py` & `arcane-core-1.9.1/arcane/core/function_traces.py`

 * *Files identical despite different names*

### Comparing `arcane-core-1.9.0/arcane/core/types.py` & `arcane-core-1.9.1/arcane/core/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     SNOWFLAKE = "SNOWFLAKE"
     GA_4 = "GA_4"
 
 # To use when specifying typehints
 ImportTypeLiteral = Literal[
     "HTTP", "FTP", "SFTP", "GCS", "GOSPORT_SFTP", "SPREADSHEET",
     "BIG_QUERY", "ADWORDS_PRODUCT", "GA_ECOMMERCE", "ARCANE_SFTP", "DATALAB",
-    "MAGENTO","SHOPIFY", "UPLOAD_FROM_DEVICE", "SNOWFLAKE"
+    "MAGENTO","SHOPIFY", "UPLOAD_FROM_DEVICE", "SNOWFLAKE", "GA_4"
 ]
 
 # To use as values in code
 class ExportTypeEnum:
     HTTP = 'HTTP'
     DELTA_API_PUSH = 'DELTA_API_PUSH'
     SFTP = 'SFTP'
```

### Comparing `arcane-core-1.9.0/arcane/core/utils.py` & `arcane-core-1.9.1/arcane/core/utils.py`

 * *Files identical despite different names*

### Comparing `arcane-core-1.9.0/setup.py` & `arcane-core-1.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-cloud-core>=1.3,<2.0', 'typing-extensions>=3.7']
 
 setup_kwargs = {
     'name': 'arcane-core',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Common utility functions',
     'long_description': None,
     'author': 'Arcane',
     'author_email': 'product@arcane.run',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `arcane-core-1.9.0/PKG-INFO` & `arcane-core-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcane-core
-Version: 1.9.0
+Version: 1.9.1
 Summary: Common utility functions
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
```

