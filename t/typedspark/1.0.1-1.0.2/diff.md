# Comparing `tmp/typedspark-1.0.1.tar.gz` & `tmp/typedspark-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.1.tar", last modified: Thu Mar 30 13:52:51 2023, max compression
+gzip compressed data, was "typedspark-1.0.2.tar", last modified: Tue Apr 18 09:39:53 2023, max compression
```

## Comparing `typedspark-1.0.1.tar` & `typedspark-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.327527 typedspark-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 13:52:33.000000 typedspark-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-30 13:52:51.327527 typedspark-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-30 13:52:33.000000 typedspark-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-30 13:52:33.000000 typedspark-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 13:52:51.327527 typedspark-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-30 13:52:33.000000 typedspark-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.323527 typedspark-1.0.1/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.323527 typedspark-1.0.1/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.327527 typedspark-1.0.1/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.327527 typedspark-1.0.1/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.327527 typedspark-1.0.1/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:33.000000 typedspark-1.0.1/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:52:51.323527 typedspark-1.0.1/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-30 13:52:51.000000 typedspark-1.0.1/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-30 13:52:51.000000 typedspark-1.0.1/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:52:51.000000 typedspark-1.0.1/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 13:52:51.000000 typedspark-1.0.1/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-30 13:52:51.000000 typedspark-1.0.1/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.691731 typedspark-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 09:39:40.000000 typedspark-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-18 09:39:53.691731 typedspark-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-18 09:39:40.000000 typedspark-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-18 09:39:40.000000 typedspark-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:39:53.691731 typedspark-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-18 09:39:40.000000 typedspark-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.1/LICENSE.txt` & `typedspark-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/PKG-INFO` & `typedspark-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.1
+Version: 1.0.2
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.1/README.rst` & `typedspark-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/pyproject.toml` & `typedspark-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/setup.py` & `typedspark-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/__init__.py` & `typedspark-1.0.2/typedspark/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from typedspark._core.column import Column
 from typedspark._core.column_meta import ColumnMeta
 from typedspark._core.dataset import DataSet
 from typedspark._core.datatypes import ArrayType, DecimalType, MapType, StructType
 from typedspark._schema.schema import MetaSchema, Schema
 from typedspark._transforms.structtype_column import structtype_column
 from typedspark._transforms.transform_to_schema import transform_to_schema
-from typedspark._utils.create_dataset import create_empty_dataset, create_partially_filled_dataset
+from typedspark._utils.create_dataset import (
+    create_empty_dataset,
+    create_partially_filled_dataset,
+    create_structtype_row,
+)
 from typedspark._utils.load_table import load_table
 from typedspark._utils.register_schema_to_dataset import register_schema_to_dataset
 
 __all__ = [
     "ArrayType",
     "Column",
     "ColumnMeta",
@@ -19,12 +23,13 @@
     "DecimalType",
     "MapType",
     "MetaSchema",
     "Schema",
     "StructType",
     "create_empty_dataset",
     "create_partially_filled_dataset",
+    "create_structtype_row",
     "load_table",
     "register_schema_to_dataset",
     "structtype_column",
     "transform_to_schema",
 ]
```

### Comparing `typedspark-1.0.1/typedspark/_core/column.py` & `typedspark-1.0.2/typedspark/_core/column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_core/column_meta.py` & `typedspark-1.0.2/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_core/dataset.py` & `typedspark-1.0.2/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_core/datatypes.py` & `typedspark-1.0.2/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_core/validate_schema.py` & `typedspark-1.0.2/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.2/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.2/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_schema/schema.py` & `typedspark-1.0.2/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_schema/structfield.py` & `typedspark-1.0.2/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.2/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.2/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_transforms/utils.py` & `typedspark-1.0.2/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_utils/load_table.py` & `typedspark-1.0.2/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.2/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.1/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.2/typedspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.1
+Version: 1.0.2
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.1/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.2/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

