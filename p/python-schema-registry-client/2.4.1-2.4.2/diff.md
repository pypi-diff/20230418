# Comparing `tmp/python-schema-registry-client-2.4.1.tar.gz` & `tmp/python-schema-registry-client-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schema-registry-client-2.4.1.tar", last modified: Thu Sep  8 11:39:05 2022, max compression
+gzip compressed data, was "python-schema-registry-client-2.4.2.tar", last modified: Tue Apr 18 15:04:03 2023, max compression
```

## Comparing `python-schema-registry-client-2.4.1.tar` & `python-schema-registry-client-2.4.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.155738 python-schema-registry-client-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)    14559 2022-09-08 11:39:05.155738 python-schema-registry-client-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10776 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.147738 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14559 2022-09-08 11:39:04.000000 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-09-08 11:39:05.000000 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 11:39:04.000000 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-08 11:39:04.000000 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-08 11:39:04.000000 python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.147738 python-schema-registry-client-2.4.1/schema_registry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.151738 python-schema-registry-client-2.4.1/schema_registry/client/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    55077 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     4701 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.151738 python-schema-registry-client-2.4.1/schema_registry/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/serializers/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/serializers/faust.py
--rw-r--r--   0 runner    (1001) docker     (121)    14841 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/schema_registry/serializers/message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-09-08 11:39:05.155738 python-schema-registry-client-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.147738 python-schema-registry-client-2.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.151738 python-schema-registry-client-2.4.1/tests/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.151738 python-schema-registry-client-2.4.1/tests/client/async_client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4850 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1258 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (121)     9025 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.151738 python-schema-registry-client-2.4.1/tests/client/sync_client/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5798 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3497 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7957 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/client/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:39:05.155738 python-schema-registry-client-2.4.1/tests/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/serializer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8284 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/serializer/test_async_message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9806 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/serializer/test_faust_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/serializer/test_faust_serializer_clean_payload.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7624 2022-09-08 11:38:53.000000 python-schema-registry-client-2.4.1/tests/serializer/test_message_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/faust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/message_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/client/async_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4850 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_http_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/tests/client/sync_client/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_http_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3497 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/tests/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8284 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_async_message_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer_clean_payload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7624 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_message_serializer.py
```

### Comparing `python-schema-registry-client-2.4.1/PKG-INFO` & `python-schema-registry-client-2.4.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,383 +1,406 @@
 Metadata-Version: 2.1
 Name: python-schema-registry-client
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Rest Client to interact against Schema Registry Confluent Server to manage Avro Schemas
 Home-page: https://github.com/marcosschroh/python-schema-registry-client
 Author: Marcos Schroh
 Author-email: schrohm@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-schema-registry-client/#files
-Description: # Python Rest Client Schema Registry
-        
-        [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
-        [![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
-        [![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
-        [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
-        
-        Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
-        
-        ## Requirements
-        
-        python 3.7+
-        
-        ## Installation
-        
-        ```bash
-        pip install python-schema-registry-client
-        ```
-        
-        If you want the `Faust` functionality:
-        
-        ```bash
-        pip install python-schema-registry-client[faust]
-        ```
-        
-        Note that this will automatically add a dependency on the [faust-streaming](https://github.com/faust-streaming/faust) fork of faust. If you want to use the
-        old faust version, simply install it manually and then install `python-schema-registry-client` without the `faust` extra enabled, the functionality will
-        be the same.
-        
-        ## Client API, Serializer, Faust Integration and Schema Server description
-        
-        **Documentation**: [https://marcosschroh.github.io/python-schema-registry-client.io](https://marcosschroh.github.io/python-schema-registry-client)
-        
-        ## Avro Schema Usage
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "type": "record",
-            "namespace": "com.kubertenes",
-            "name": "AvroDeployment",
-            "fields": [
-                {"name": "image", "type": "string"},
-                {"name": "replicas", "type": "int"},
-                {"name": "port", "type": "int"},
-            ],
-        }
-        
-        avro_schema = schema.AvroSchema(deployment_schema)
-        
-        schema_id = client.register("test-deployment", avro_schema)
-        ```
-        
-        or async
-        
-        ```python
-        from schema_registry.client import AsyncSchemaRegistryClient, schema
-        
-        async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "type": "record",
-            "namespace": "com.kubertenes",
-            "name": "AvroDeployment",
-            "fields": [
-                {"name": "image", "type": "string"},
-                {"name": "replicas", "type": "int"},
-                {"name": "port", "type": "int"},
-            ],
-        }
-        
-        avro_schema = schema.AvroSchema(deployment_schema)
-        
-        schema_id = await async_client.register("test-deployment", avro_schema)
-        ```
-        
-        ## JSON Schema Usage
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "definitions" : {
-                "JsonDeployment" : {
-                    "type" : "object",
-                    "required" : ["image", "replicas", "port"],
-                    "properties" : {
-                        "image" :       {"type" : "string"},
-                        "replicas" :    {"type" : "integer"},
-                        "port" :        {"type" : "integer"}
-                    }
-                }
-            },
-            "$ref" : "#/definitions/JsonDeployment"
-        }
-        
-        json_schema = schema.JsonSchema(deployment_schema)
-        
-        schema_id = client.register("test-deployment", json_schema)
-        ```
-        
-        or async
-        
-        ```python
-        from schema_registry.client import AsyncSchemaRegistryClient, schema
-        
-        async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "definitions" : {
-                "JsonDeployment" : {
-                    "type" : "object",
-                    "required" : ["image", "replicas", "port"],
-                    "properties" : {
-                        "image" :       {"type" : "string"},
-                        "replicas" :    {"type" : "integer"},
-                        "port" :        {"type" : "integer"}
-                    }
-                }
-            },
-            "$ref" : "#/definitions/JsonDeployment"
-        }
-        
-        json_schema = schema.JsonSchema(deployment_schema)
-        
-        schema_id = await async_client.register("test-deployment", json_schema)
-        ```
-        
-        ## Usage with dataclasses-avroschema for avro schemas
-        
-        You can generate the `avro schema` directely from a python class using [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema)
-        and use it in the API for `register schemas`, `check versions` and `test compatibility`:
-        
-        ```python
-        import dataclasses
-        
-        from dataclasses_avroschema import AvroModel, types
-        
-        from schema_registry.client import SchemaRegistryClient
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        
-        @dataclasses.dataclass
-        class UserAdvance(AvroModel):
-            name: str
-            age: int
-            pets: typing.List[str] = dataclasses.field(default_factory=lambda: ["dog", "cat"])
-            accounts: typing.Dict[str, int] = dataclasses.field(default_factory=lambda: {"key": 1})
-            has_car: bool = False
-            favorite_colors: types.Enum = types.Enum(["BLUE", "YELLOW", "GREEN"], default="BLUE")
-            country: str = "Argentina"
-            address: str = None
-        
-        # register the schema
-        schema_id = client.register(subject, UserAdvance.avro_schema())
-        
-        print(schema_id)
-        # >>> 12
-        
-        result = client.check_version(subject, UserAdvance.avro_schema())
-        print(result)
-        # >>> SchemaVersion(subject='dataclasses-avroschema-subject-2', schema_id=12, schema=1, version={"type":"record" ...')
-        
-        compatibility = client.test_compatibility(subject, UserAdvance.avro_schema())
-        print(compatibility)
-        
-        # >>> True
-        ```
-        
-        ### Usage with pydantic for json schemas
-        You can generate the json schema directely from a python class using pydantic and use it in the API for register schemas, check versions and test compatibility:
-        
-        ```python
-        import typing
-        
-        from enum import Enum
-        
-        from pydantic import BaseModel
-        
-        from schema_registry.client import SchemaRegistryClient
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        class ColorEnum(str, Enum):
-          BLUE = "BLUE"
-          YELLOW = "YELLOW"
-          GREEN = "GREEN"
-        
-        
-        class UserAdvance(BaseModel):
-            name: str
-            age: int
-            pets: typing.List[str] = ["dog", "cat"]
-            accounts: typing.Dict[str, int] = {"key": 1}
-            has_car: bool = False
-            favorite_colors: ColorEnum = ColorEnum.BLUE
-            country: str = "Argentina"
-            address: str = None
-        
-        # register the schema
-        schema_id = client.register(subject, UserAdvance.schema_json(), schema_type="JSON")
-        
-        print(schema_id)
-        # >>> 12
-        
-        result = client.check_version(subject, UserAdvance.schema_json(), schema_type="JSON")
-        print(result)
-        # >>> SchemaVersion(subject='pydantic-jsonschema-subject', schema_id=12, schema=1, version=<schema_registry.client.schema.JsonSchema object at 0x7f40354550a0>)
-        
-        compatibility = client.test_compatibility(subject, UserAdvance.schema_json(), schema_type="JSON")
-        print(compatibility)
-        
-        # >>> True
-        ```
-        
-        ## Serializers
-        
-        You can use `AvroMessageSerializer` to encode/decode messages in `avro`
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        from schema_registry.serializers import AvroMessageSerializer
-        
-        
-        client = SchemaRegistryClient("http://127.0.0.1:8081")
-        avro_message_serializer = AvroMessageSerializer(client)
-        
-        avro_user_schema = schema.AvroSchema({
-            "type": "record",
-            "namespace": "com.example",
-            "name": "AvroUsers",
-            "fields": [
-                {"name": "first_name", "type": "string"},
-                {"name": "last_name", "type": "string"},
-                {"name": "age", "type": "int"},
-        
-            ],
-        })
-        
-        # We want to encode the user_record with avro_user_schema
-        user_record = {
-            "first_name": "my_first_name",
-            "last_name": "my_last_name",
-            "age": 20,
-        }
-        
-        # Encode the record
-        message_encoded = avro_message_serializer.encode_record_with_schema(
-            "user", avro_user_schema, user_record)
-        
-        print(message_encoded)
-        # >>> b'\x00\x00\x00\x00\x01\x1amy_first_name\x18my_last_name('
-        ```
-        
-        or with `json schemas`
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        from schema_registry.serializers import JsonMessageSerializer
-        
-        
-        client = SchemaRegistryClient("http://127.0.0.1:8081")
-        json_message_serializer = JsonMessageSerializer(client)
-        
-        json_schema = schema.JsonSchema({
-          "definitions" : {
-            "record:python.test.basic.basic" : {
-              "description" : "basic schema for tests",
-              "type" : "object",
-              "required" : [ "number", "name" ],
-              "properties" : {
-                "number" : {
-                  "oneOf" : [ {
-                    "type" : "integer"
-                  }, {
-                    "type" : "null"
-                  } ]
-                },
-                "name" : {
-                  "oneOf" : [ {
-                    "type" : "string"
-                  } ]
-                }
-              }
-            }
-          },
-          "$ref" : "#/definitions/record:python.test.basic.basic"
-        })
-        
-        # Encode the record
-        basic_record = {
-            "number": 10,
-            "name": "a_name",
-        }
-        
-        message_encoded = json_message_serializer.encode_record_with_schema(
-            "basic", json_schema, basic_record)
-        
-        print(message_encoded)
-        # >>> b'\x00\x00\x00\x00\x02{"number": 10, "name": "a_name"}'
-        ```
-        
-        ## When use this library
-        
-        Usually, we have a situation like this:
-        
-        ![Confluent Architecture](docs/img/confluent_architecture.png)
-        
-        So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
-        
-        Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
-        
-        ## Development
-        
-        Install the project and development utilities in edit mode:
-        
-        ```bash
-        pip3 install -e ".[tests,docs,faust]"
-        ```
-        
-        The tests are run against the `Schema Server` using `docker compose`, so you will need
-        `Docker` and `Docker Compose` installed.
-        
-        ```bash
-        ./scripts/test
-        ```
-        
-        You can run tests with arbitrary python version by:
-        
-        ```bash
-        ./scripts/test --python-version 3.x
-        ```
-        
-        All additional args will be passed to pytest, for example:
-        
-        ```bash
-        ./scripts/test ./tests/client/ --maxfail=1 
-        ```
-        
-        Run code linting:
-        
-        ```bash
-        ./scripts/lint
-        ```
-        
-        To perform tests using the python shell you can execute `docker-compose up` and the `schema registry server` 
-        will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        # do some operations with the client...
-        ```
-        
 Keywords: Schema Registry,Python,Avro,Apache,Apache Avro,JSON,JSON Schema
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: faust
 Provides-Extra: tests
+License-File: LICENSE
+
+# Python Rest Client Schema Registry
+
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
+[![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
+[![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
+
+Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
+
+## Requirements
+
+python 3.7+
+
+## Installation
+
+```bash
+pip install python-schema-registry-client
+```
+
+If you want the `Faust` functionality:
+
+```bash
+pip install python-schema-registry-client[faust]
+```
+
+Note that this will automatically add a dependency on the [faust-streaming](https://github.com/faust-streaming/faust) fork of faust. If you want to use the
+old faust version, simply install it manually and then install `python-schema-registry-client` without the `faust` extra enabled, the functionality will
+be the same.
+
+## Client API, Serializer, Faust Integration and Schema Server description
+
+**Documentation**: [https://marcosschroh.github.io/python-schema-registry-client.io](https://marcosschroh.github.io/python-schema-registry-client)
+
+## Avro Schema Usage
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+
+schema_id = client.register("test-deployment", avro_schema)
+```
+
+or async
+
+```python
+from schema_registry.client import AsyncSchemaRegistryClient, schema
+
+async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+
+schema_id = await async_client.register("test-deployment", avro_schema)
+```
+
+## JSON Schema Usage
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "definitions" : {
+        "JsonDeployment" : {
+            "type" : "object",
+            "required" : ["image", "replicas", "port"],
+            "properties" : {
+                "image" :       {"type" : "string"},
+                "replicas" :    {"type" : "integer"},
+                "port" :        {"type" : "integer"}
+            }
+        }
+    },
+    "$ref" : "#/definitions/JsonDeployment"
+}
+
+json_schema = schema.JsonSchema(deployment_schema)
+
+schema_id = client.register("test-deployment", json_schema)
+```
+
+or async
+
+```python
+from schema_registry.client import AsyncSchemaRegistryClient, schema
+
+async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "definitions" : {
+        "JsonDeployment" : {
+            "type" : "object",
+            "required" : ["image", "replicas", "port"],
+            "properties" : {
+                "image" :       {"type" : "string"},
+                "replicas" :    {"type" : "integer"},
+                "port" :        {"type" : "integer"}
+            }
+        }
+    },
+    "$ref" : "#/definitions/JsonDeployment"
+}
+
+json_schema = schema.JsonSchema(deployment_schema)
+
+schema_id = await async_client.register("test-deployment", json_schema)
+```
+
+## Usage with dataclasses-avroschema for avro schemas
+
+You can generate the `avro schema` directely from a python class using [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema)
+and use it in the API for `register schemas`, `check versions` and `test compatibility`:
+
+```python
+import dataclasses
+
+from dataclasses_avroschema import AvroModel, types
+
+from schema_registry.client import SchemaRegistryClient
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+
+@dataclasses.dataclass
+class UserAdvance(AvroModel):
+    name: str
+    age: int
+    pets: typing.List[str] = dataclasses.field(default_factory=lambda: ["dog", "cat"])
+    accounts: typing.Dict[str, int] = dataclasses.field(default_factory=lambda: {"key": 1})
+    has_car: bool = False
+    favorite_colors: types.Enum = types.Enum(["BLUE", "YELLOW", "GREEN"], default="BLUE")
+    country: str = "Argentina"
+    address: str = None
+
+# register the schema
+schema_id = client.register(subject, UserAdvance.avro_schema())
+
+print(schema_id)
+# >>> 12
+
+result = client.check_version(subject, UserAdvance.avro_schema())
+print(result)
+# >>> SchemaVersion(subject='dataclasses-avroschema-subject-2', schema_id=12, schema=1, version={"type":"record" ...')
+
+compatibility = client.test_compatibility(subject, UserAdvance.avro_schema())
+print(compatibility)
+
+# >>> True
+```
+
+### Usage with pydantic for json schemas
+You can generate the json schema directely from a python class using pydantic and use it in the API for register schemas, check versions and test compatibility:
+
+```python
+import typing
+
+from enum import Enum
+
+from pydantic import BaseModel
+
+from schema_registry.client import SchemaRegistryClient
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+class ColorEnum(str, Enum):
+  BLUE = "BLUE"
+  YELLOW = "YELLOW"
+  GREEN = "GREEN"
+
+
+class UserAdvance(BaseModel):
+    name: str
+    age: int
+    pets: typing.List[str] = ["dog", "cat"]
+    accounts: typing.Dict[str, int] = {"key": 1}
+    has_car: bool = False
+    favorite_colors: ColorEnum = ColorEnum.BLUE
+    country: str = "Argentina"
+    address: str = None
+
+# register the schema
+schema_id = client.register(subject, UserAdvance.schema_json(), schema_type="JSON")
+
+print(schema_id)
+# >>> 12
+
+result = client.check_version(subject, UserAdvance.schema_json(), schema_type="JSON")
+print(result)
+# >>> SchemaVersion(subject='pydantic-jsonschema-subject', schema_id=12, schema=1, version=<schema_registry.client.schema.JsonSchema object at 0x7f40354550a0>)
+
+compatibility = client.test_compatibility(subject, UserAdvance.schema_json(), schema_type="JSON")
+print(compatibility)
+
+# >>> True
+```
+
+## Serializers
+
+You can use `AvroMessageSerializer` to encode/decode messages in `avro`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+from schema_registry.serializers import AvroMessageSerializer
+
+
+client = SchemaRegistryClient("http://127.0.0.1:8081")
+avro_message_serializer = AvroMessageSerializer(client)
+
+avro_user_schema = schema.AvroSchema({
+    "type": "record",
+    "namespace": "com.example",
+    "name": "AvroUsers",
+    "fields": [
+        {"name": "first_name", "type": "string"},
+        {"name": "last_name", "type": "string"},
+        {"name": "age", "type": "int"},
+
+    ],
+})
+
+# We want to encode the user_record with avro_user_schema
+user_record = {
+    "first_name": "my_first_name",
+    "last_name": "my_last_name",
+    "age": 20,
+}
+
+# Encode the record
+message_encoded = avro_message_serializer.encode_record_with_schema(
+    "user", avro_user_schema, user_record)
+
+print(message_encoded)
+# >>> b'\x00\x00\x00\x00\x01\x1amy_first_name\x18my_last_name('
+```
+
+or with `json schemas`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+from schema_registry.serializers import JsonMessageSerializer
+
+
+client = SchemaRegistryClient("http://127.0.0.1:8081")
+json_message_serializer = JsonMessageSerializer(client)
+
+json_schema = schema.JsonSchema({
+  "definitions" : {
+    "record:python.test.basic.basic" : {
+      "description" : "basic schema for tests",
+      "type" : "object",
+      "required" : [ "number", "name" ],
+      "properties" : {
+        "number" : {
+          "oneOf" : [ {
+            "type" : "integer"
+          }, {
+            "type" : "null"
+          } ]
+        },
+        "name" : {
+          "oneOf" : [ {
+            "type" : "string"
+          } ]
+        }
+      }
+    }
+  },
+  "$ref" : "#/definitions/record:python.test.basic.basic"
+})
+
+# Encode the record
+basic_record = {
+    "number": 10,
+    "name": "a_name",
+}
+
+message_encoded = json_message_serializer.encode_record_with_schema(
+    "basic", json_schema, basic_record)
+
+print(message_encoded)
+# >>> b'\x00\x00\x00\x00\x02{"number": 10, "name": "a_name"}'
+```
+
+## When use this library
+
+Usually, we have a situation like this:
+
+![Confluent Architecture](docs/img/confluent_architecture.png)
+
+So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
+
+Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
+
+## Development
+
+Install the project and development utilities in edit mode:
+
+```bash
+pip3 install -e ".[tests,docs,faust]"
+```
+
+The tests are run against the `Schema Server` using `docker compose`, so you will need
+`Docker` and `Docker Compose` installed.
+
+```bash
+./scripts/test
+```
+
+You can run tests with arbitrary python version by:
+
+```bash
+./scripts/test --python-version 3.x
+```
+
+All additional args will be passed to pytest, for example:
+
+```bash
+./scripts/test ./tests/client/ --maxfail=1 
+```
+
+Run code linting:
+
+```bash
+./scripts/lint
+```
+
+To perform tests using the python shell you can run the project using `docker-compose`.
+
+1. Build: `docker-compose build --build-arg PYTHON_VERSION=$PYTHON_VERSION`
+2. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+3. Use the python interpreter (get a python shell typing `python` in your command line)
+4. Play with the `schema server`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+# do some operations with the client...
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+client.register("test-deployment", avro_schema)
+# >>>> Out[5]: 1
+```
+
+Then, you can check the schema using your browser going to the url `http://127.0.0.1:8081/schemas/ids/1`
+
+
```

### Comparing `python-schema-registry-client-2.4.1/README.md` & `python-schema-registry-client-2.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -345,17 +345,37 @@
 
 Run code linting:
 
 ```bash
 ./scripts/lint
 ```
 
-To perform tests using the python shell you can execute `docker-compose up` and the `schema registry server` 
-will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+To perform tests using the python shell you can run the project using `docker-compose`.
+
+1. Build: `docker-compose build --build-arg PYTHON_VERSION=$PYTHON_VERSION`
+2. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+3. Use the python interpreter (get a python shell typing `python` in your command line)
+4. Play with the `schema server`
 
 ```python
 from schema_registry.client import SchemaRegistryClient, schema
 
 client = SchemaRegistryClient(url="http://127.0.0.1:8081")
 
 # do some operations with the client...
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+client.register("test-deployment", avro_schema)
+# >>>> Out[5]: 1
 ```
+
+Then, you can check the schema using your browser going to the url `http://127.0.0.1:8081/schemas/ids/1`
```

### Comparing `python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/PKG-INFO` & `python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,383 +1,406 @@
 Metadata-Version: 2.1
 Name: python-schema-registry-client
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Rest Client to interact against Schema Registry Confluent Server to manage Avro Schemas
 Home-page: https://github.com/marcosschroh/python-schema-registry-client
 Author: Marcos Schroh
 Author-email: schrohm@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-schema-registry-client/#files
-Description: # Python Rest Client Schema Registry
-        
-        [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
-        [![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
-        [![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
-        [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
-        
-        Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
-        
-        ## Requirements
-        
-        python 3.7+
-        
-        ## Installation
-        
-        ```bash
-        pip install python-schema-registry-client
-        ```
-        
-        If you want the `Faust` functionality:
-        
-        ```bash
-        pip install python-schema-registry-client[faust]
-        ```
-        
-        Note that this will automatically add a dependency on the [faust-streaming](https://github.com/faust-streaming/faust) fork of faust. If you want to use the
-        old faust version, simply install it manually and then install `python-schema-registry-client` without the `faust` extra enabled, the functionality will
-        be the same.
-        
-        ## Client API, Serializer, Faust Integration and Schema Server description
-        
-        **Documentation**: [https://marcosschroh.github.io/python-schema-registry-client.io](https://marcosschroh.github.io/python-schema-registry-client)
-        
-        ## Avro Schema Usage
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "type": "record",
-            "namespace": "com.kubertenes",
-            "name": "AvroDeployment",
-            "fields": [
-                {"name": "image", "type": "string"},
-                {"name": "replicas", "type": "int"},
-                {"name": "port", "type": "int"},
-            ],
-        }
-        
-        avro_schema = schema.AvroSchema(deployment_schema)
-        
-        schema_id = client.register("test-deployment", avro_schema)
-        ```
-        
-        or async
-        
-        ```python
-        from schema_registry.client import AsyncSchemaRegistryClient, schema
-        
-        async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "type": "record",
-            "namespace": "com.kubertenes",
-            "name": "AvroDeployment",
-            "fields": [
-                {"name": "image", "type": "string"},
-                {"name": "replicas", "type": "int"},
-                {"name": "port", "type": "int"},
-            ],
-        }
-        
-        avro_schema = schema.AvroSchema(deployment_schema)
-        
-        schema_id = await async_client.register("test-deployment", avro_schema)
-        ```
-        
-        ## JSON Schema Usage
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "definitions" : {
-                "JsonDeployment" : {
-                    "type" : "object",
-                    "required" : ["image", "replicas", "port"],
-                    "properties" : {
-                        "image" :       {"type" : "string"},
-                        "replicas" :    {"type" : "integer"},
-                        "port" :        {"type" : "integer"}
-                    }
-                }
-            },
-            "$ref" : "#/definitions/JsonDeployment"
-        }
-        
-        json_schema = schema.JsonSchema(deployment_schema)
-        
-        schema_id = client.register("test-deployment", json_schema)
-        ```
-        
-        or async
-        
-        ```python
-        from schema_registry.client import AsyncSchemaRegistryClient, schema
-        
-        async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        deployment_schema = {
-            "definitions" : {
-                "JsonDeployment" : {
-                    "type" : "object",
-                    "required" : ["image", "replicas", "port"],
-                    "properties" : {
-                        "image" :       {"type" : "string"},
-                        "replicas" :    {"type" : "integer"},
-                        "port" :        {"type" : "integer"}
-                    }
-                }
-            },
-            "$ref" : "#/definitions/JsonDeployment"
-        }
-        
-        json_schema = schema.JsonSchema(deployment_schema)
-        
-        schema_id = await async_client.register("test-deployment", json_schema)
-        ```
-        
-        ## Usage with dataclasses-avroschema for avro schemas
-        
-        You can generate the `avro schema` directely from a python class using [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema)
-        and use it in the API for `register schemas`, `check versions` and `test compatibility`:
-        
-        ```python
-        import dataclasses
-        
-        from dataclasses_avroschema import AvroModel, types
-        
-        from schema_registry.client import SchemaRegistryClient
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        
-        @dataclasses.dataclass
-        class UserAdvance(AvroModel):
-            name: str
-            age: int
-            pets: typing.List[str] = dataclasses.field(default_factory=lambda: ["dog", "cat"])
-            accounts: typing.Dict[str, int] = dataclasses.field(default_factory=lambda: {"key": 1})
-            has_car: bool = False
-            favorite_colors: types.Enum = types.Enum(["BLUE", "YELLOW", "GREEN"], default="BLUE")
-            country: str = "Argentina"
-            address: str = None
-        
-        # register the schema
-        schema_id = client.register(subject, UserAdvance.avro_schema())
-        
-        print(schema_id)
-        # >>> 12
-        
-        result = client.check_version(subject, UserAdvance.avro_schema())
-        print(result)
-        # >>> SchemaVersion(subject='dataclasses-avroschema-subject-2', schema_id=12, schema=1, version={"type":"record" ...')
-        
-        compatibility = client.test_compatibility(subject, UserAdvance.avro_schema())
-        print(compatibility)
-        
-        # >>> True
-        ```
-        
-        ### Usage with pydantic for json schemas
-        You can generate the json schema directely from a python class using pydantic and use it in the API for register schemas, check versions and test compatibility:
-        
-        ```python
-        import typing
-        
-        from enum import Enum
-        
-        from pydantic import BaseModel
-        
-        from schema_registry.client import SchemaRegistryClient
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        class ColorEnum(str, Enum):
-          BLUE = "BLUE"
-          YELLOW = "YELLOW"
-          GREEN = "GREEN"
-        
-        
-        class UserAdvance(BaseModel):
-            name: str
-            age: int
-            pets: typing.List[str] = ["dog", "cat"]
-            accounts: typing.Dict[str, int] = {"key": 1}
-            has_car: bool = False
-            favorite_colors: ColorEnum = ColorEnum.BLUE
-            country: str = "Argentina"
-            address: str = None
-        
-        # register the schema
-        schema_id = client.register(subject, UserAdvance.schema_json(), schema_type="JSON")
-        
-        print(schema_id)
-        # >>> 12
-        
-        result = client.check_version(subject, UserAdvance.schema_json(), schema_type="JSON")
-        print(result)
-        # >>> SchemaVersion(subject='pydantic-jsonschema-subject', schema_id=12, schema=1, version=<schema_registry.client.schema.JsonSchema object at 0x7f40354550a0>)
-        
-        compatibility = client.test_compatibility(subject, UserAdvance.schema_json(), schema_type="JSON")
-        print(compatibility)
-        
-        # >>> True
-        ```
-        
-        ## Serializers
-        
-        You can use `AvroMessageSerializer` to encode/decode messages in `avro`
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        from schema_registry.serializers import AvroMessageSerializer
-        
-        
-        client = SchemaRegistryClient("http://127.0.0.1:8081")
-        avro_message_serializer = AvroMessageSerializer(client)
-        
-        avro_user_schema = schema.AvroSchema({
-            "type": "record",
-            "namespace": "com.example",
-            "name": "AvroUsers",
-            "fields": [
-                {"name": "first_name", "type": "string"},
-                {"name": "last_name", "type": "string"},
-                {"name": "age", "type": "int"},
-        
-            ],
-        })
-        
-        # We want to encode the user_record with avro_user_schema
-        user_record = {
-            "first_name": "my_first_name",
-            "last_name": "my_last_name",
-            "age": 20,
-        }
-        
-        # Encode the record
-        message_encoded = avro_message_serializer.encode_record_with_schema(
-            "user", avro_user_schema, user_record)
-        
-        print(message_encoded)
-        # >>> b'\x00\x00\x00\x00\x01\x1amy_first_name\x18my_last_name('
-        ```
-        
-        or with `json schemas`
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        from schema_registry.serializers import JsonMessageSerializer
-        
-        
-        client = SchemaRegistryClient("http://127.0.0.1:8081")
-        json_message_serializer = JsonMessageSerializer(client)
-        
-        json_schema = schema.JsonSchema({
-          "definitions" : {
-            "record:python.test.basic.basic" : {
-              "description" : "basic schema for tests",
-              "type" : "object",
-              "required" : [ "number", "name" ],
-              "properties" : {
-                "number" : {
-                  "oneOf" : [ {
-                    "type" : "integer"
-                  }, {
-                    "type" : "null"
-                  } ]
-                },
-                "name" : {
-                  "oneOf" : [ {
-                    "type" : "string"
-                  } ]
-                }
-              }
-            }
-          },
-          "$ref" : "#/definitions/record:python.test.basic.basic"
-        })
-        
-        # Encode the record
-        basic_record = {
-            "number": 10,
-            "name": "a_name",
-        }
-        
-        message_encoded = json_message_serializer.encode_record_with_schema(
-            "basic", json_schema, basic_record)
-        
-        print(message_encoded)
-        # >>> b'\x00\x00\x00\x00\x02{"number": 10, "name": "a_name"}'
-        ```
-        
-        ## When use this library
-        
-        Usually, we have a situation like this:
-        
-        ![Confluent Architecture](docs/img/confluent_architecture.png)
-        
-        So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
-        
-        Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
-        
-        ## Development
-        
-        Install the project and development utilities in edit mode:
-        
-        ```bash
-        pip3 install -e ".[tests,docs,faust]"
-        ```
-        
-        The tests are run against the `Schema Server` using `docker compose`, so you will need
-        `Docker` and `Docker Compose` installed.
-        
-        ```bash
-        ./scripts/test
-        ```
-        
-        You can run tests with arbitrary python version by:
-        
-        ```bash
-        ./scripts/test --python-version 3.x
-        ```
-        
-        All additional args will be passed to pytest, for example:
-        
-        ```bash
-        ./scripts/test ./tests/client/ --maxfail=1 
-        ```
-        
-        Run code linting:
-        
-        ```bash
-        ./scripts/lint
-        ```
-        
-        To perform tests using the python shell you can execute `docker-compose up` and the `schema registry server` 
-        will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
-        
-        ```python
-        from schema_registry.client import SchemaRegistryClient, schema
-        
-        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
-        
-        # do some operations with the client...
-        ```
-        
 Keywords: Schema Registry,Python,Avro,Apache,Apache Avro,JSON,JSON Schema
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: faust
 Provides-Extra: tests
+License-File: LICENSE
+
+# Python Rest Client Schema Registry
+
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
+[![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
+[![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
+
+Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
+
+## Requirements
+
+python 3.7+
+
+## Installation
+
+```bash
+pip install python-schema-registry-client
+```
+
+If you want the `Faust` functionality:
+
+```bash
+pip install python-schema-registry-client[faust]
+```
+
+Note that this will automatically add a dependency on the [faust-streaming](https://github.com/faust-streaming/faust) fork of faust. If you want to use the
+old faust version, simply install it manually and then install `python-schema-registry-client` without the `faust` extra enabled, the functionality will
+be the same.
+
+## Client API, Serializer, Faust Integration and Schema Server description
+
+**Documentation**: [https://marcosschroh.github.io/python-schema-registry-client.io](https://marcosschroh.github.io/python-schema-registry-client)
+
+## Avro Schema Usage
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+
+schema_id = client.register("test-deployment", avro_schema)
+```
+
+or async
+
+```python
+from schema_registry.client import AsyncSchemaRegistryClient, schema
+
+async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+
+schema_id = await async_client.register("test-deployment", avro_schema)
+```
+
+## JSON Schema Usage
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "definitions" : {
+        "JsonDeployment" : {
+            "type" : "object",
+            "required" : ["image", "replicas", "port"],
+            "properties" : {
+                "image" :       {"type" : "string"},
+                "replicas" :    {"type" : "integer"},
+                "port" :        {"type" : "integer"}
+            }
+        }
+    },
+    "$ref" : "#/definitions/JsonDeployment"
+}
+
+json_schema = schema.JsonSchema(deployment_schema)
+
+schema_id = client.register("test-deployment", json_schema)
+```
+
+or async
+
+```python
+from schema_registry.client import AsyncSchemaRegistryClient, schema
+
+async_client = AsyncSchemaRegistryClient(url="http://127.0.0.1:8081")
+
+deployment_schema = {
+    "definitions" : {
+        "JsonDeployment" : {
+            "type" : "object",
+            "required" : ["image", "replicas", "port"],
+            "properties" : {
+                "image" :       {"type" : "string"},
+                "replicas" :    {"type" : "integer"},
+                "port" :        {"type" : "integer"}
+            }
+        }
+    },
+    "$ref" : "#/definitions/JsonDeployment"
+}
+
+json_schema = schema.JsonSchema(deployment_schema)
+
+schema_id = await async_client.register("test-deployment", json_schema)
+```
+
+## Usage with dataclasses-avroschema for avro schemas
+
+You can generate the `avro schema` directely from a python class using [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema)
+and use it in the API for `register schemas`, `check versions` and `test compatibility`:
+
+```python
+import dataclasses
+
+from dataclasses_avroschema import AvroModel, types
+
+from schema_registry.client import SchemaRegistryClient
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+
+@dataclasses.dataclass
+class UserAdvance(AvroModel):
+    name: str
+    age: int
+    pets: typing.List[str] = dataclasses.field(default_factory=lambda: ["dog", "cat"])
+    accounts: typing.Dict[str, int] = dataclasses.field(default_factory=lambda: {"key": 1})
+    has_car: bool = False
+    favorite_colors: types.Enum = types.Enum(["BLUE", "YELLOW", "GREEN"], default="BLUE")
+    country: str = "Argentina"
+    address: str = None
+
+# register the schema
+schema_id = client.register(subject, UserAdvance.avro_schema())
+
+print(schema_id)
+# >>> 12
+
+result = client.check_version(subject, UserAdvance.avro_schema())
+print(result)
+# >>> SchemaVersion(subject='dataclasses-avroschema-subject-2', schema_id=12, schema=1, version={"type":"record" ...')
+
+compatibility = client.test_compatibility(subject, UserAdvance.avro_schema())
+print(compatibility)
+
+# >>> True
+```
+
+### Usage with pydantic for json schemas
+You can generate the json schema directely from a python class using pydantic and use it in the API for register schemas, check versions and test compatibility:
+
+```python
+import typing
+
+from enum import Enum
+
+from pydantic import BaseModel
+
+from schema_registry.client import SchemaRegistryClient
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+class ColorEnum(str, Enum):
+  BLUE = "BLUE"
+  YELLOW = "YELLOW"
+  GREEN = "GREEN"
+
+
+class UserAdvance(BaseModel):
+    name: str
+    age: int
+    pets: typing.List[str] = ["dog", "cat"]
+    accounts: typing.Dict[str, int] = {"key": 1}
+    has_car: bool = False
+    favorite_colors: ColorEnum = ColorEnum.BLUE
+    country: str = "Argentina"
+    address: str = None
+
+# register the schema
+schema_id = client.register(subject, UserAdvance.schema_json(), schema_type="JSON")
+
+print(schema_id)
+# >>> 12
+
+result = client.check_version(subject, UserAdvance.schema_json(), schema_type="JSON")
+print(result)
+# >>> SchemaVersion(subject='pydantic-jsonschema-subject', schema_id=12, schema=1, version=<schema_registry.client.schema.JsonSchema object at 0x7f40354550a0>)
+
+compatibility = client.test_compatibility(subject, UserAdvance.schema_json(), schema_type="JSON")
+print(compatibility)
+
+# >>> True
+```
+
+## Serializers
+
+You can use `AvroMessageSerializer` to encode/decode messages in `avro`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+from schema_registry.serializers import AvroMessageSerializer
+
+
+client = SchemaRegistryClient("http://127.0.0.1:8081")
+avro_message_serializer = AvroMessageSerializer(client)
+
+avro_user_schema = schema.AvroSchema({
+    "type": "record",
+    "namespace": "com.example",
+    "name": "AvroUsers",
+    "fields": [
+        {"name": "first_name", "type": "string"},
+        {"name": "last_name", "type": "string"},
+        {"name": "age", "type": "int"},
+
+    ],
+})
+
+# We want to encode the user_record with avro_user_schema
+user_record = {
+    "first_name": "my_first_name",
+    "last_name": "my_last_name",
+    "age": 20,
+}
+
+# Encode the record
+message_encoded = avro_message_serializer.encode_record_with_schema(
+    "user", avro_user_schema, user_record)
+
+print(message_encoded)
+# >>> b'\x00\x00\x00\x00\x01\x1amy_first_name\x18my_last_name('
+```
+
+or with `json schemas`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+from schema_registry.serializers import JsonMessageSerializer
+
+
+client = SchemaRegistryClient("http://127.0.0.1:8081")
+json_message_serializer = JsonMessageSerializer(client)
+
+json_schema = schema.JsonSchema({
+  "definitions" : {
+    "record:python.test.basic.basic" : {
+      "description" : "basic schema for tests",
+      "type" : "object",
+      "required" : [ "number", "name" ],
+      "properties" : {
+        "number" : {
+          "oneOf" : [ {
+            "type" : "integer"
+          }, {
+            "type" : "null"
+          } ]
+        },
+        "name" : {
+          "oneOf" : [ {
+            "type" : "string"
+          } ]
+        }
+      }
+    }
+  },
+  "$ref" : "#/definitions/record:python.test.basic.basic"
+})
+
+# Encode the record
+basic_record = {
+    "number": 10,
+    "name": "a_name",
+}
+
+message_encoded = json_message_serializer.encode_record_with_schema(
+    "basic", json_schema, basic_record)
+
+print(message_encoded)
+# >>> b'\x00\x00\x00\x00\x02{"number": 10, "name": "a_name"}'
+```
+
+## When use this library
+
+Usually, we have a situation like this:
+
+![Confluent Architecture](docs/img/confluent_architecture.png)
+
+So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
+
+Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
+
+## Development
+
+Install the project and development utilities in edit mode:
+
+```bash
+pip3 install -e ".[tests,docs,faust]"
+```
+
+The tests are run against the `Schema Server` using `docker compose`, so you will need
+`Docker` and `Docker Compose` installed.
+
+```bash
+./scripts/test
+```
+
+You can run tests with arbitrary python version by:
+
+```bash
+./scripts/test --python-version 3.x
+```
+
+All additional args will be passed to pytest, for example:
+
+```bash
+./scripts/test ./tests/client/ --maxfail=1 
+```
+
+Run code linting:
+
+```bash
+./scripts/lint
+```
+
+To perform tests using the python shell you can run the project using `docker-compose`.
+
+1. Build: `docker-compose build --build-arg PYTHON_VERSION=$PYTHON_VERSION`
+2. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+3. Use the python interpreter (get a python shell typing `python` in your command line)
+4. Play with the `schema server`
+
+```python
+from schema_registry.client import SchemaRegistryClient, schema
+
+client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+# do some operations with the client...
+deployment_schema = {
+    "type": "record",
+    "namespace": "com.kubertenes",
+    "name": "AvroDeployment",
+    "fields": [
+        {"name": "image", "type": "string"},
+        {"name": "replicas", "type": "int"},
+        {"name": "port", "type": "int"},
+    ],
+}
+
+avro_schema = schema.AvroSchema(deployment_schema)
+client.register("test-deployment", avro_schema)
+# >>>> Out[5]: 1
+```
+
+Then, you can check the schema using your browser going to the url `http://127.0.0.1:8081/schemas/ids/1`
+
+
```

### Comparing `python-schema-registry-client-2.4.1/python_schema_registry_client.egg-info/SOURCES.txt` & `python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 python_schema_registry_client.egg-info/PKG-INFO
 python_schema_registry_client.egg-info/SOURCES.txt
 python_schema_registry_client.egg-info/dependency_links.txt
```

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/client.py` & `python-schema-registry-client-2.4.2/schema_registry/client/client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/paths.py` & `python-schema-registry-client-2.4.2/schema_registry/client/paths.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/schema.py` & `python-schema-registry-client-2.4.2/schema_registry/client/schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/status.py` & `python-schema-registry-client-2.4.2/schema_registry/client/status.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/urls.py` & `python-schema-registry-client-2.4.2/schema_registry/client/urls.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/client/utils.py` & `python-schema-registry-client-2.4.2/schema_registry/client/utils.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/serializers/__init__.py` & `python-schema-registry-client-2.4.2/schema_registry/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/serializers/faust.py` & `python-schema-registry-client-2.4.2/schema_registry/serializers/faust.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/schema_registry/serializers/message_serializer.py` & `python-schema-registry-client-2.4.2/schema_registry/serializers/message_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/setup.py` & `python-schema-registry-client-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """ setup.py for python-schema-registry-client."""
 
 from setuptools import find_packages, setup
 
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 
 requires = [
     "fastavro>=1.4.4",
```

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_http_client.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_compatibility.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_compatibility.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_delete.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_delete.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_getters.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_getters.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_registration.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_registration.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/async_client/test_schema_version.py` & `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_version.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_http_client.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_compatibility.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_compatibility.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_delete.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_delete.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_getters.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_getters.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_registration.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_registration.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/sync_client/test_schema_version.py` & `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_version.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/client/test_urls.py` & `python-schema-registry-client-2.4.2/tests/client/test_urls.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/serializer/test_async_message_serializer.py` & `python-schema-registry-client-2.4.2/tests/serializer/test_async_message_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/serializer/test_faust_serializer.py` & `python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/serializer/test_faust_serializer_clean_payload.py` & `python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer_clean_payload.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.1/tests/serializer/test_message_serializer.py` & `python-schema-registry-client-2.4.2/tests/serializer/test_message_serializer.py`

 * *Files identical despite different names*

