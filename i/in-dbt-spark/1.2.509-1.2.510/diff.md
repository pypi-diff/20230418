# Comparing `tmp/in-dbt-spark-1.2.509.tar.gz` & `tmp/in-dbt-spark-1.2.510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.509.tar", last modified: Mon Apr 10 21:15:53 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.2.510.tar", last modified: Tue Apr 18 18:34:43 2023, max compression
```

## Comparing `in-dbt-spark-1.2.509.tar` & `in-dbt-spark-1.2.510.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.765031 in-dbt-spark-1.2.510/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-18 18:34:43.765031 in-dbt-spark-1.2.510/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.749031 in-dbt-spark-1.2.510/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.749031 in-dbt-spark-1.2.510/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.753031 in-dbt-spark-1.2.510/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.757031 in-dbt-spark-1.2.510/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.749031 in-dbt-spark-1.2.510/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.757031 in-dbt-spark-1.2.510/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.757031 in-dbt-spark-1.2.510/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.757031 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.757031 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.761031 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:34:43.765031 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 18:34:43.000000 in-dbt-spark-1.2.510/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:34:43.765031 in-dbt-spark-1.2.510/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-18 18:34:29.000000 in-dbt-spark-1.2.510/setup.py
```

### Comparing `in-dbt-spark-1.2.509/PKG-INFO` & `in-dbt-spark-1.2.510/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.509
+Version: 1.2.510
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.509 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.510 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.509/README.md` & `in-dbt-spark-1.2.510/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/client.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/models.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,22 @@
     RUNNING = "running"
     BUSY = "busy"
     SHUTTING_DOWN = "shutting_down"
     ERROR = "error"
     DEAD = "dead"
     KILLED = "killed"
     SUCCESS = "success"
+    SUBMITTING = "submitting"
 
 
-SESSION_STATE_NOT_READY = {SessionState.NOT_STARTED, SessionState.STARTING}
+SESSION_STATE_NOT_READY = {
+    SessionState.NOT_STARTED,
+    SessionState.STARTING,
+    SessionState.SUBMITTING,
+}
 SESSION_STATE_FINISHED = {
     SessionState.ERROR,
     SessionState.DEAD,
     SessionState.KILLED,
     SessionState.SUCCESS,
 }
```

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/session.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.2.510/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/spark/column.py` & `in-dbt-spark-1.2.510/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.2.510/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.2.510/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.2.510/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/adapters/spark/session.py` & `in-dbt-spark-1.2.510/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/materializations/validate.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.2.510/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.2.510/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.2.510/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.509
+Version: 1.2.510
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.509 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.510 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.509/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.2.510/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.509/setup.py` & `in-dbt-spark-1.2.510/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.509"
+package_version = "1.2.510"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.16.0",
```

