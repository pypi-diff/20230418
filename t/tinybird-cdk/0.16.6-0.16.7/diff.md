# Comparing `tmp/tinybird-cdk-0.16.6.tar.gz` & `tmp/tinybird-cdk-0.16.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.16.6.tar", last modified: Mon Apr 17 07:42:19 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.16.7.tar", last modified: Tue Apr 18 07:53:07 2023, max compression
```

## Comparing `tinybird-cdk-0.16.6.tar` & `tinybird-cdk-0.16.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.523024 tinybird-cdk-0.16.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 07:53:07.523024 tinybird-cdk-0.16.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:53:07.523024 tinybird-cdk-0.16.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.515024 tinybird-cdk-0.16.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.519024 tinybird-cdk-0.16.7/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.519024 tinybird-cdk-0.16.7/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.523024 tinybird-cdk-0.16.7/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 07:52:54.000000 tinybird-cdk-0.16.7/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:53:07.519024 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 07:53:07.000000 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-18 07:53:07.000000 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:53:07.000000 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 07:53:07.000000 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 07:53:07.000000 tinybird-cdk-0.16.7/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.16.6/README.md` & `tinybird-cdk-0.16.7/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/setup.py` & `tinybird-cdk-0.16.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.16.6',
+    version='0.16.7',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.16.6/tests/test_gcp.py` & `tinybird-cdk-0.16.7/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.16.7/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.16.7/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.16.7/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.16.7/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.16.7/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/config.py` & `tinybird-cdk-0.16.7/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connector.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.16.7/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/errors.py` & `tinybird-cdk-0.16.7/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/export.py` & `tinybird-cdk-0.16.7/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/formats.py` & `tinybird-cdk-0.16.7/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/logger.py` & `tinybird-cdk-0.16.7/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/migration.py` & `tinybird-cdk-0.16.7/tinybird_cdk/migration.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 datetime_type_pattern = r"^DateTime(\(('.+')?)?\)?$"
 
 
 class NonSupportedMigrationException(Exception):
     pass
 
 
+def parse_path(sql_query: str) -> Tuple[str, str, str]:
+    path = re.search(
+        r'.*\s+FROM\s+`?([^\s`]+)\.([^\s`]+)\.([^\s`]+)`?', sql_query, re.IGNORECASE).groups()
+    return (path[0], path[1], path[2])
+
+
 def get_migration(tb_schema, bq_schema) -> Tuple[str, List[str]]:
     tb_columns = tb_schema['columns']
     tb_schema_sql = tb_schema['sql_schema']
     tb_columns_sql = tb_schema_sql.split(', ')
     for c, sql, idx in zip(tb_columns, tb_columns_sql, range(len(tb_columns))):
         c['sql'] = sql
         c['index'] = idx
@@ -95,31 +101,7 @@
         if bq_column.name in tb_columns_dict:
             tb_column = tb_columns_dict[bq_column.name]
             final_column_list.append(tb_column['sql'])
         else:
             final_column_list.append(build_column_sql(bq_column))
         columns.append(bq_column.name)
     return (final_column_list, columns)
-
-
-def add_missing_columns_to_sql(query: str, new_columns: List[str]) -> str:
-    sql_parts = query.split('FROM')
-    if len(sql_parts) < 2:
-        sql_parts = query.split('from')
-    query_columns_str = re.sub("SELECT", "", sql_parts[0])
-    query_columns_str = re.sub("select", "", query_columns_str).strip()
-    query_columns = [s.strip() for s in query_columns_str.split(',')]
-
-    def get_column_in_sql(c):
-        column = [ec for ec in query_columns if c in ec]
-        if len(column) > 0:
-            return column[0]
-        return None
-
-    new_column_list = []
-    for column in new_columns:
-        if (column_to_add := get_column_in_sql(column)) is None:
-            column_to_add = column
-        new_column_list.append(column_to_add)
-
-    new_sql = f"SELECT {', '.join(new_column_list)} FROM {sql_parts[1].lstrip()}"
-    return new_sql
```

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/schema.py` & `tinybird-cdk-0.16.7/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.16.7/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.6/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.16.7/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

