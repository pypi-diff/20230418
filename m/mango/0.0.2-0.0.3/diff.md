# Comparing `tmp/mango-0.0.2.tar.gz` & `tmp/mango-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-0.0.2.tar", last modified: Wed Apr 12 13:41:11 2023, max compression
+gzip compressed data, was "mango-0.0.3.tar", last modified: Tue Apr 18 12:58:01 2023, max compression
```

## Comparing `mango-0.0.2.tar` & `mango-0.0.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-12 13:41:07.000000 mango-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 13:41:07.000000 mango-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 13:41:11.225054 mango-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 13:41:07.000000 mango-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.205054 mango-0.0.2/mango/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 13:41:07.000000 mango-0.0.2/mango/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/email_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/google_cloud_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/config/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 13:41:07.000000 mango-0.0.2/mango/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-12 13:41:07.000000 mango-0.0.2/mango/config/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/data/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 13:41:07.000000 mango-0.0.2/mango/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-12 13:41:07.000000 mango-0.0.2/mango/data/ts_dataset.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-12 13:41:07.000000 mango-0.0.2/mango/images/images_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/models/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/neural_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 13:41:07.000000 mango-0.0.2/mango/plots/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/processing_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 13:41:07.000000 mango-0.0.2/mango/schemas/location.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/table/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/pytups_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/pytups_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/table_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/mango/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/mango/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/json_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_bad_type.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_bad_value.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_good.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_arcgis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_processing_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.205054 mango-0.0.2/mango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:41:11.225054 mango-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 13:41:07.000000 mango-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-18 12:57:56.000000 mango-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 12:57:56.000000 mango-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 12:58:01.119768 mango-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 12:57:56.000000 mango-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 12:57:56.000000 mango-0.0.3/mango/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/email_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/google_cloud_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 12:57:56.000000 mango-0.0.3/mango/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-18 12:57:56.000000 mango-0.0.3/mango/config/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 12:57:56.000000 mango-0.0.3/mango/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-18 12:57:56.000000 mango-0.0.3/mango/data/ts_dataset.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-18 12:57:56.000000 mango-0.0.3/mango/images/images_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/neural_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-18 12:57:56.000000 mango-0.0.3/mango/plots/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/processing_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 12:57:56.000000 mango-0.0.3/mango/schemas/location.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/pytups_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/pytups_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/mango/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/mango/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/json_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_bad_type.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_bad_value.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_good.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_arcgis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_processing_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:58:01.119768 mango-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 12:57:56.000000 mango-0.0.3/setup.py
```

### Comparing `mango-0.0.2/LICENSE` & `mango-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/PKG-INFO` & `mango-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.2/mango/clients/arcgis.py` & `mango-0.0.3/mango/clients/arcgis.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/clients/email_downloader.py` & `mango-0.0.3/mango/clients/email_downloader.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/clients/email_sender.py` & `mango-0.0.3/mango/clients/email_sender.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/clients/google_cloud_storage.py` & `mango-0.0.3/mango/clients/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/config/base_config.py` & `mango-0.0.3/mango/config/base_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/data/ts_dataset.pkl` & `mango-0.0.3/mango/data/ts_dataset.pkl`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/images/images_functions.py` & `mango-0.0.3/mango/images/images_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/logging/chrono.py` & `mango-0.0.3/mango/logging/chrono.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,53 +35,62 @@
         self.start_time[name] = None
         self.end[name] = None
 
     def start(self, name, silent=True):
         """
         Method to start a chrono
 
-        :param name: name of the chrono
+        :param str name: name of the chrono
+        :param bool silent: if the chrono should be silent. True by default
         """
         self.new(name)
         self.start_time[name] = time.time()
         if not silent:
             self.logger.info(f"Operation {name} starts")
 
-    def stop(self, name: str):
+    def stop(self, name: str, report: bool = True):
         """
         Method to stop a chrono and get back its duration
 
-        :param name: name of the chrono
+        :param str name: name of the chrono
+        :param bool report: if the chrono should be reported. True by default
         :return: the time elapsed for the specific chrono
         :rtype: float
         """
         self.end[name] = time.time()
         duration = self.end[name] - self.start_time[name]
-        if not self.silent:
+        if not self.silent or report:
             self.logger.info(
                 f"Operation {name} took: {round(duration, self.precision)} seconds"
             )
         return duration
 
-    def stop_all(self):
+    def stop_all(self, report: bool = True):
         """
         Method to stop all chronos and get back a dict with their durations
+
+        :param bool report: if the chronos should be reported. True by default
+        :return: a dict with the name of the chronos as key and the durations as value
+        :rtype: dict
         """
         durations = dict()
         for name in self.start_time.keys():
             if self.end[name] is None:
-                durations[name] = self.stop(name)
+                durations[name] = self.stop(name, report)
 
         return durations
 
     def report(self, name: str, message: str = None):
         """
         Method to report the time of a chrono and get back its duration
 
-        :param name: name of the chrono
+        :param str name: name of the chrono
+        :param str message: additional message to display in the log
+        :return: the time elapsed for the specific chrono
+        :rtype: float
         """
 
         if self.end[name] is not None:
             msg = f"Operation {name} took: {round(self.end[name] - self.start_time[name], self.precision)} seconds"
             if message is not None:
                 msg = f"{msg}. {message}"
 
@@ -100,27 +109,30 @@
             self.logger.info(msg)
 
             return duration
 
     def report_all(self):
         """
         Method to report the time of all chronos and get back a dict with all the durations
+
+        :return: a dict with the name of the chronos as key and the durations as value
+        :rtype: dict
         """
         durations = dict()
         for name in self.start_time.keys():
             durations[name] = self.report(name)
         return durations
 
     def __call__(self, func: callable, *args, **kwargs):
         """
-        Method to decorate a function
+        Method to use the chrono as a callable with a function inside
 
         :param func: function to decorate
         :param args: arguments to pass to the function
         :param kwargs: keyword arguments to pass to the function
         :return: the result of the function
         """
         self.start(func.__name__)
         result = func(*args, **kwargs)
-        self.stop(func.__name__)
+        self.stop(func.__name__, False)
         self.report(func.__name__)
         return result
```

### Comparing `mango-0.0.2/mango/logging/decorators.py` & `mango-0.0.3/mango/logging/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/logging/logger.py` & `mango-0.0.3/mango/logging/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,32 +4,37 @@
 LOG_FORMAT = "%(asctime)s: %(levelname)s %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def get_basic_logger(
     console=True,
     log_file=None,
-    log_level=logging.DEBUG,
+    log_level=logging.INFO,
     log_format=LOG_FORMAT,
     date_format=DATE_FORMAT,
-    logger_name="root"
+    logger_name="root",
+    clear=True
 ):
     """
     Create a basic logger to log messages in console and/or file.
 
     :param console: bool output log in python console.
     :param log_file: str path of the file where to write the log.
     :param log_level: minimal level of log to show (logging.DEBUG, INFO, WARNING...)
     :param log_format: str format of log messages
     :param date_format: str format of datetime
     :param logger_name: str name of the logger. Default is root.
+    :param clear: clear previous handlers for this logger.
     :return: the logger
     """
     logger = logging.getLogger(logger_name)
 
+    if clear:
+        logger.handlers.clear()
+
     if console:
         console_handler = logging.StreamHandler()
         console_handler.setFormatter(logging.Formatter(log_format, date_format))
         logger.addHandler(console_handler)
 
     if log_file is not None:
         file_handler = logging.FileHandler(log_file)
```

### Comparing `mango-0.0.2/mango/models/neural_networks.py` & `mango-0.0.3/mango/models/neural_networks.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/plots/plots.py` & `mango-0.0.3/mango/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/processing/__init__.py` & `mango-0.0.3/mango/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/processing/date_functions.py` & `mango-0.0.3/mango/processing/date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/processing/file_functions.py` & `mango-0.0.3/mango/processing/file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/processing/object_functions.py` & `mango-0.0.3/mango/processing/object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/processing/processing_time_series.py` & `mango-0.0.3/mango/processing/processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/shared/const.py` & `mango-0.0.3/mango/shared/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/shared/decorators.py` & `mango-0.0.3/mango/shared/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/table/pytups_table.py` & `mango-0.0.3/mango/table/pytups_table.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/table/pytups_tools.py` & `mango-0.0.3/mango/table/pytups_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/table/table_tools.py` & `mango-0.0.3/mango/table/table_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/const.py` & `mango-0.0.3/mango/tests/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/data/json_dataset.json` & `mango-0.0.3/mango/tests/data/json_dataset.json`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/data/test.xlsx` & `mango-0.0.3/mango/tests/data/test.xlsx`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_arcgis_client.py` & `mango-0.0.3/mango/tests/test_arcgis_client.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_config.py` & `mango-0.0.3/mango/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_date_functions.py` & `mango-0.0.3/mango/tests/test_date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_file_functions.py` & `mango-0.0.3/mango/tests/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_images.py` & `mango-0.0.3/mango/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_logging.py` & `mango-0.0.3/mango/tests/test_logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def test_chrono_class(self):
         chrono = Chrono("first test", silent=True)
         time.sleep(0.1)
         chrono.report_all()
         chrono.start("second test")
         time.sleep(0.1)
-        chrono.stop_all()
+        chrono.stop_all(False)
         chrono.report_all()
         with open(normalize_path("./data/temp.log"), "r") as f:
             lines = f.readlines()
             self.assertEqual(len(lines), 3)
             self.assertIn("first test", lines[0])
             self.assertIn("INFO", lines[0])
             self.assertIn("running", lines[0])
@@ -55,14 +55,45 @@
             self.assertIn("INFO", lines[1])
             self.assertIn("took", lines[1])
 
             self.assertIn("second test", lines[2])
             self.assertIn("INFO", lines[2])
             self.assertIn("took", lines[2])
 
+    def test_chrono_class_stop_report(self):
+        chrono = Chrono("first test", silent=True)
+        time.sleep(0.1)
+        chrono.report_all()
+        chrono.start("second test")
+        time.sleep(0.1)
+        chrono.stop_all(True)
+        chrono.report_all()
+        with open(normalize_path("./data/temp.log"), "r") as f:
+            lines = f.readlines()
+            self.assertEqual(len(lines), 5)
+            self.assertIn("first test", lines[0])
+            self.assertIn("INFO", lines[0])
+            self.assertIn("running", lines[0])
+
+            self.assertIn("first test", lines[1])
+            self.assertIn("INFO", lines[1])
+            self.assertIn("took", lines[1])
+
+            self.assertIn("second test", lines[2])
+            self.assertIn("INFO", lines[2])
+            self.assertIn("took", lines[2])
+
+            self.assertIn("first test", lines[3])
+            self.assertIn("INFO", lines[3])
+            self.assertIn("took", lines[3])
+
+            self.assertIn("second test", lines[4])
+            self.assertIn("INFO", lines[4])
+            self.assertIn("took", lines[4])
+
     def test_chrono_not_silent(self):
         chrono = Chrono("first test", silent=False)
         time.sleep(0.1)
         chrono.start("second test")
         time.sleep(0.1)
         chrono.stop_all()
         with open(normalize_path("./data/temp.log"), "r") as f:
@@ -76,15 +107,15 @@
             self.assertIn("second test", lines[1])
             self.assertIn("INFO", lines[1])
             self.assertIn("took", lines[1])
 
     def test_chrono_callable(self):
         chrono = Chrono("first test", silent=True)
         chrono(time.sleep, 0.1)
-        chrono.stop_all()
+        chrono.stop_all(False)
         chrono.report_all()
         with open(normalize_path("./data/temp.log"), "r") as f:
             lines = f.readlines()
             self.assertEqual(len(lines), 3)
             self.assertIn("sleep", lines[0])
             self.assertIn("INFO", lines[0])
             self.assertIn("took", lines[0])
@@ -98,15 +129,15 @@
             self.assertIn("took", lines[2])
 
     def test_chrono_report_custom(self):
         chrono = Chrono("first test", silent=True)
         time.sleep(0.1)
         chrono.report("first test", "custom message")
         time.sleep(0.1)
-        chrono.stop_all()
+        chrono.stop_all(False)
         chrono.report_all()
         with open(normalize_path("./data/temp.log"), "r") as f:
             lines = f.readlines()
             self.assertEqual(len(lines), 2)
             self.assertIn("first test", lines[0])
             self.assertIn("INFO", lines[0])
             self.assertIn("elapsed", lines[0])
```

### Comparing `mango-0.0.2/mango/tests/test_models.py` & `mango-0.0.3/mango/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_object_functions.py` & `mango-0.0.3/mango/tests/test_object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_processing_time_series.py` & `mango-0.0.3/mango/tests/test_processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_table.py` & `mango-0.0.3/mango/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_tools.py` & `mango-0.0.3/mango/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango/tests/test_validation.py` & `mango-0.0.3/mango/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/mango.egg-info/PKG-INFO` & `mango-0.0.3/mango.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.2/mango.egg-info/SOURCES.txt` & `mango-0.0.3/mango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-0.0.2/setup.py` & `mango-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "xlsxwriter",
     ],
 }
 
 
 setuptools.setup(
     name="mango",
-    version="0.0.2",
+    version="0.0.3",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Library with a collection of useful classes and methods to DRY",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/mango",
     packages=setuptools.find_packages(),
     classifiers=[
```

