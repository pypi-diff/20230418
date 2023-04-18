# Comparing `tmp/dbxconfig-1.0.6.tar.gz` & `tmp/dbxconfig-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.6.tar", last modified: Mon Apr 17 21:42:41 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.7.tar", last modified: Tue Apr 18 14:12:46 2023, max compression
```

## Comparing `dbxconfig-1.0.6.tar` & `dbxconfig-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.122561 dbxconfig-1.0.6/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 21:42:41.122432 dbxconfig-1.0.6/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.6/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.121301 dbxconfig-1.0.6/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      428 2023-04-17 12:50:14.000000 dbxconfig-1.0.6/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3853 2023-04-17 21:24:13.000000 dbxconfig-1.0.6/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2935 2023-04-17 15:55:15.000000 dbxconfig-1.0.6/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4892 2023-04-17 15:50:34.000000 dbxconfig-1.0.6/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      110 2023-04-17 12:57:48.000000 dbxconfig-1.0.6/dbxconfig/_stage_type.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4187 2023-04-17 12:57:48.000000 dbxconfig-1.0.6/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.6/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.6/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.122239 dbxconfig-1.0.6/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      397 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.6/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-17 21:42:41.122623 dbxconfig-1.0.6/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-17 21:42:30.000000 dbxconfig-1.0.6/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.433217 dbxconfig-1.0.7/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 14:12:46.433093 dbxconfig-1.0.7/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.7/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.432036 dbxconfig-1.0.7/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      435 2023-04-18 13:06:37.000000 dbxconfig-1.0.7/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1962 2023-04-18 13:56:25.000000 dbxconfig-1.0.7/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      166 2023-04-18 13:12:17.000000 dbxconfig-1.0.7/dbxconfig/_stage_type.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      780 2023-04-18 08:59:52.000000 dbxconfig-1.0.7/dbxconfig/_table.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3479 2023-04-18 13:00:31.000000 dbxconfig-1.0.7/dbxconfig/_tables.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.7/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.7/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-18 14:12:46.432921 dbxconfig-1.0.7/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      367 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.7/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-18 14:12:46.000000 dbxconfig-1.0.7/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-18 14:12:46.433257 dbxconfig-1.0.7/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-18 14:12:24.000000 dbxconfig-1.0.7/setup.py
```

### Comparing `dbxconfig-1.0.6/PKG-INFO` & `dbxconfig-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.6
+Version: 1.0.7
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.6/README.md` & `dbxconfig-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.6/dbxconfig/_table_index.py` & `dbxconfig-1.0.7/dbxconfig/_tables.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,17 @@
 from pydantic import BaseModel, Field
-from typing import Union, List, Any, Dict
-from enum import Enum
+from typing import Union, Any, Dict
+from ._stage_type import StageType
 import fnmatch
+from ._table import Table, TableMapping
 
 
 _INDEX_WILDCARD = "*"
 
 
-class StageType(str, Enum):
-    landing = "landing"
-    raw = "raw"
-    base = "base"
-
-
-class BaseTable(BaseModel):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    stage: StageType = Field(...)
-    database: str = Field(...)
-    name: str = Field(...)
-    id: Union[str, List[str]] = Field(default=[])
-
-
-class Table(BaseTable):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    depends_on: List[str] = Field(default=[])
-    table_properties: Dict[str, str] = Field(default=None)
-
-
-class TableMapping(BaseModel):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    destination: Table = Field(...)
-    source: Union[Dict[str, Table], Table] = Field(...)
-
-
 class Tables(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._load_index()
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
@@ -55,15 +24,15 @@
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
     ):
         return f"{stage.name}.{database}.{table}"
 
     def _load_index(self):
         for stage in StageType:
-            stage_data = self.table_data.get(stage.value)
+            stage_data = self.table_data.get(stage.name)
             if stage_data:
                 stage_table_properties = stage_data.get("table_properties", {})
 
                 for database, tables in stage_data.items():
                     if database == "table_properties":
                         continue
 
@@ -83,15 +52,15 @@
                         if table_properties:
                             table_details["table_properties"] = table_properties
 
                         # create a table object
                         table = Table(**table_details)
 
                         # index the table object
-                        index = f"{stage.value}.{database}.{table.name}"
+                        index = f"{stage.name}.{database}.{table.name}"
                         self.tables_index[index] = table
 
     def lookup_table(self, index: str, first_match: bool = True):
         matches = fnmatch.filter(list(self.tables_index.keys()), index)
 
         if not matches:
             raise Exception(f"index {index} not found in tables_index")
```

### Comparing `dbxconfig-1.0.6/dbxconfig/_timeslice.py` & `dbxconfig-1.0.7/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.6/dbxconfig/_utils.py` & `dbxconfig-1.0.7/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.6/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.7/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.6
+Version: 1.0.7
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.6/setup.py` & `dbxconfig-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.6",
+    version="1.0.7",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

