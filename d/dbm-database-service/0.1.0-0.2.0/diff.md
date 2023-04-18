# Comparing `tmp/dbm_database_service-0.1.0.tar.gz` & `tmp/dbm_database_service-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm_database_service-0.1.0.tar", max compression
+gzip compressed data, was "dbm_database_service-0.2.0.tar", max compression
```

## Comparing `dbm_database_service-0.1.0.tar` & `dbm_database_service-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.1.0/dbm_database_service/__init__.py
--rw-r--r--   0        0        0      342 2023-04-12 14:45:46.999428 dbm_database_service-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       14 2023-04-12 14:51:20.937044 dbm_database_service-0.1.0/README.md
--rw-r--r--   0        0        0      312 1970-01-01 00:00:00.000000 dbm_database_service-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.0/dbm_database_service/__init__.py
+-rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.0/dbm_database_service/connectors.py
+-rw-r--r--   0        0        0     3208 2023-04-17 21:00:23.708163 dbm_database_service-0.2.0/dbm_database_service/managers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.0/dbm_database_service/models/__init__.py
+-rw-r--r--   0        0        0     1612 2023-04-17 21:13:25.033005 dbm_database_service-0.2.0/dbm_database_service/models/column.py
+-rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.0/dbm_database_service/models/config.py
+-rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.0/dbm_database_service/models/datatype.py
+-rw-r--r--   0        0        0     1000 2023-04-17 21:13:25.053962 dbm_database_service-0.2.0/dbm_database_service/models/table.py
+-rw-r--r--   0        0        0      655 2023-04-18 08:31:20.784056 dbm_database_service-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3539 2023-04-18 08:25:27.534276 dbm_database_service-0.2.0/README.md
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 dbm_database_service-0.2.0/PKG-INFO
```

