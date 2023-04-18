# Comparing `tmp/macrometa-source-postgres-0.0.41.tar.gz` & `tmp/macrometa-source-postgres-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.41.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.42.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.41.tar` & `macrometa-source-postgres-0.0.42.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/LICENSE
--rw-r--r--   0        0        0    35130 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28921 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3650 2023-04-17 09:51:45.643133 macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-04-17 09:51:45.891137 macrometa-source-postgres-0.0.41/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.41/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.41/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/LICENSE
+-rw-r--r--   0        0        0    35130 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28921 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-04-18 02:51:35.807317 macrometa-source-postgres-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.42/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.42/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.41/LICENSE` & `macrometa-source-postgres-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.41/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 import psycopg2.extras
 from singer import metadata
 
 import macrometa_source_postgres.connection as postgres
 from macrometa_source_postgres.sync_strategies.common import should_sync_column
 
 
-def fetch_view(conn_info, stream, desired_columns, md_map):
+def fetch_view(conn_info, stream, desired_columns, md_map, limit=10):
     schema_name = md_map.get(()).get('schema-name')
     escaped_columns = map(postgres.prepare_columns_sql, desired_columns)
     samples = []
     with postgres.connect(conn_info) as conn:
         with conn.cursor(cursor_factory=psycopg2.extras.DictCursor, name='macrometa_cursor') as cur:
             cur.itersize = postgres.CURSOR_ITER_SIZE
             select_sql = f"SELECT {','.join(escaped_columns)} FROM " \
-                         f"{postgres.fully_qualified_table_name(schema_name, stream['table_name'])}"
+                         f"{postgres.fully_qualified_table_name(schema_name, stream['table_name'])} LIMIT {limit}"
             cur.execute(select_sql)
             for rec in cur:
                 rec_msg = postgres.selected_row_to_singer_message(stream, rec, None, desired_columns, None, md_map)
                 samples.append(rec_msg.record)
     return samples
 
 
-def fetch_table(conn_info, stream, desired_columns, md_map):
+def fetch_table(conn_info, stream, desired_columns, md_map, limit=10):
     schema_name = md_map.get(()).get('schema-name')
     escaped_columns = map(partial(postgres.prepare_columns_for_select_sql, md_map=md_map), desired_columns)
     samples = []
     with postgres.connect(conn_info) as conn:
         with conn.cursor(cursor_factory=psycopg2.extras.DictCursor, name='macrometa_cursor') as cur:
             cur.itersize = postgres.CURSOR_ITER_SIZE
             fq_table_name = postgres.fully_qualified_table_name(schema_name, stream['table_name'])
             select_sql = f"""SELECT {','.join(escaped_columns)}, xmin::text::bigint
                               FROM {fq_table_name}
-                             ORDER BY xmin::text ASC"""
+                             ORDER BY xmin::text ASC LIMIT {limit}"""
             cur.execute(select_sql)
             for rec in cur:
                 rec = rec[:-1]
                 rec_msg = postgres.selected_row_to_singer_message(stream, rec, None, desired_columns, None, md_map)
                 samples.append(rec_msg.record)
     return samples
```

### Comparing `macrometa-source-postgres-0.0.41/pyproject.toml` & `macrometa-source-postgres-0.0.42/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.41'
+version='0.0.42'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.41/setup.py` & `macrometa-source-postgres-0.0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.41',
+    'version': '0.0.42',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.41/PKG-INFO` & `macrometa-source-postgres-0.0.42/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.41
+Version: 0.0.42
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

