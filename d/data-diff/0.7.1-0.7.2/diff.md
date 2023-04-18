# Comparing `tmp/data_diff-0.7.1.tar.gz` & `tmp/data_diff-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.1.tar", max compression
+gzip compressed data, was "data_diff-0.7.2.tar", max compression
```

## Comparing `data_diff-0.7.1.tar` & `data_diff-0.7.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.1/LICENSE
--rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.1/README.md
--rw-r--r--   0        0        0     8419 2023-04-03 18:06:26.931396 data_diff-0.7.1/data_diff/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-03 18:06:26.931499 data_diff-0.7.1/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.1/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0     9235 2023-04-14 15:23:33.906694 data_diff-0.7.1/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     8746 2023-04-14 15:23:33.906807 data_diff-0.7.1/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.1/data_diff/config.py
--rw-r--r--   0        0        0      483 2023-04-03 18:06:26.931645 data_diff-0.7.1/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1343 2023-04-03 18:06:26.931693 data_diff-0.7.1/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      164 2023-04-03 18:06:26.931735 data_diff-0.7.1/data_diff/databases/base.py
--rw-r--r--   0        0        0      247 2023-04-03 18:06:26.931779 data_diff-0.7.1/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931823 data_diff-0.7.1/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931868 data_diff-0.7.1/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.931912 data_diff-0.7.1/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      226 2023-04-03 18:06:26.931970 data_diff-0.7.1/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932016 data_diff-0.7.1/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      265 2023-04-03 18:06:26.932063 data_diff-0.7.1/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932105 data_diff-0.7.1/data_diff/databases/presto.py
--rw-r--r--   0        0        0      247 2023-04-03 18:06:26.932150 data_diff-0.7.1/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      254 2023-04-03 18:06:26.932199 data_diff-0.7.1/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      226 2023-04-03 18:06:26.932247 data_diff-0.7.1/data_diff/databases/trino.py
--rw-r--r--   0        0        0      240 2023-04-03 18:06:26.932292 data_diff-0.7.1/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    13473 2023-04-14 23:37:25.350943 data_diff-0.7.1/data_diff/dbt.py
--rw-r--r--   0        0        0    13249 2023-04-14 15:23:33.907122 data_diff-0.7.1/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14366 2023-04-03 18:06:26.932528 data_diff-0.7.1/data_diff/diff_tables.py
--rw-r--r--   0        0        0     8557 2023-04-03 18:06:26.932606 data_diff-0.7.1/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.1/data_diff/info_tree.py
--rw-r--r--   0        0        0    14718 2023-04-03 18:06:26.932755 data_diff-0.7.1/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.1/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.1/data_diff/parse_time.py
--rw-r--r--   0        0        0     1384 2023-04-03 18:06:26.932946 data_diff-0.7.1/data_diff/query_utils.py
--rw-r--r--   0        0        0     1818 2023-04-03 18:06:26.933026 data_diff-0.7.1/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0    10834 2023-04-03 18:06:26.933122 data_diff-0.7.1/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.1/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.1/data_diff/tracking.py
--rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.1/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-04-15 23:11:48.035454 data_diff-0.7.1/data_diff/version.py
--rwxr-xr-x   0        0        0     2708 2023-04-15 23:11:48.035634 data_diff-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 data_diff-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.2/README.md
+-rw-r--r--   0        0        0     8419 2023-04-03 18:06:26.931396 data_diff-0.7.2/data_diff/__init__.py
+-rw-r--r--   0        0        0    15796 2023-04-03 18:06:26.931499 data_diff-0.7.2/data_diff/__main__.py
+-rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.2/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0     9235 2023-04-14 15:23:33.906694 data_diff-0.7.2/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0     8746 2023-04-14 15:23:33.906807 data_diff-0.7.2/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.2/data_diff/config.py
+-rw-r--r--   0        0        0      483 2023-04-03 18:06:26.931645 data_diff-0.7.2/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1343 2023-04-03 18:06:26.931693 data_diff-0.7.2/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      164 2023-04-03 18:06:26.931735 data_diff-0.7.2/data_diff/databases/base.py
+-rw-r--r--   0        0        0      247 2023-04-03 18:06:26.931779 data_diff-0.7.2/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931823 data_diff-0.7.2/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931868 data_diff-0.7.2/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      233 2023-04-03 18:06:26.931912 data_diff-0.7.2/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      226 2023-04-03 18:06:26.931970 data_diff-0.7.2/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932016 data_diff-0.7.2/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      265 2023-04-03 18:06:26.932063 data_diff-0.7.2/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932105 data_diff-0.7.2/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      247 2023-04-03 18:06:26.932150 data_diff-0.7.2/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      254 2023-04-03 18:06:26.932199 data_diff-0.7.2/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      226 2023-04-03 18:06:26.932247 data_diff-0.7.2/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      240 2023-04-03 18:06:26.932292 data_diff-0.7.2/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    13473 2023-04-14 23:37:25.350943 data_diff-0.7.2/data_diff/dbt.py
+-rw-r--r--   0        0        0    13346 2023-04-18 20:40:59.490092 data_diff-0.7.2/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14366 2023-04-03 18:06:26.932528 data_diff-0.7.2/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     8557 2023-04-03 18:06:26.932606 data_diff-0.7.2/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.2/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14718 2023-04-03 18:06:26.932755 data_diff-0.7.2/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.2/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.2/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1384 2023-04-03 18:06:26.932946 data_diff-0.7.2/data_diff/query_utils.py
+-rw-r--r--   0        0        0     1818 2023-04-03 18:06:26.933026 data_diff-0.7.2/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0    10834 2023-04-03 18:06:26.933122 data_diff-0.7.2/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.2/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.2/data_diff/tracking.py
+-rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.2/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-04-18 20:40:59.490257 data_diff-0.7.2/data_diff/version.py
+-rwxr-xr-x   0        0        0     2708 2023-04-18 20:40:59.490498 data_diff-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 data_diff-0.7.2/PKG-INFO
```

### Comparing `data_diff-0.7.1/LICENSE` & `data_diff-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/README.md` & `data_diff-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/__init__.py` & `data_diff-0.7.2/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/__main__.py` & `data_diff-0.7.2/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/cloud/data_source.py` & `data_diff-0.7.2/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/cloud/datafold_api.py` & `data_diff-0.7.2/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/config.py` & `data_diff-0.7.2/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/databases/_connect.py` & `data_diff-0.7.2/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/dbt.py` & `data_diff-0.7.2/data_diff/dbt.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/dbt_parser.py` & `data_diff-0.7.2/data_diff/dbt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
                 "user": credentials.get("user"),
                 "account": credentials.get("account"),
                 "database": credentials.get("database"),
                 "warehouse": credentials.get("warehouse"),
                 "role": credentials.get("role"),
                 "schema": credentials.get("schema"),
                 "insecure_mode": credentials.get("insecure_mode", False),
+                "client_session_keep_alive": credentials.get("client_session_keep_alive", False)
             }
             self.threads = credentials.get("threads")
             self.requires_upper = True
 
             if credentials.get("private_key_path") is not None:
                 if credentials.get("password") is not None:
                     raise Exception("Cannot use password and key at the same time")
```

### Comparing `data_diff-0.7.1/data_diff/diff_tables.py` & `data_diff-0.7.2/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/hashdiff_tables.py` & `data_diff-0.7.2/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/info_tree.py` & `data_diff-0.7.2/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/joindiff_tables.py` & `data_diff-0.7.2/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/lexicographic_space.py` & `data_diff-0.7.2/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/parse_time.py` & `data_diff-0.7.2/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/query_utils.py` & `data_diff-0.7.2/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/sqeleton/repl.py` & `data_diff-0.7.2/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/table_segment.py` & `data_diff-0.7.2/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/thread_utils.py` & `data_diff-0.7.2/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/tracking.py` & `data_diff-0.7.2/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/data_diff/utils.py` & `data_diff-0.7.2/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.1/pyproject.toml` & `data_diff-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.1"
+version = "0.7.2"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
```

### Comparing `data_diff-0.7.1/PKG-INFO` & `data_diff-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.1
+Version: 0.7.2
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

