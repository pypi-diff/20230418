# Comparing `tmp/thrivve_core-0.0.7.tar.gz` & `tmp/thrivve_core-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-i80w0gv5/thrivve_core-0.0.7.tar", last modified: Mon Apr 17 12:28:39 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-8i158xim/thrivve_core-0.0.8.tar", last modified: Tue Apr 18 12:53:58 2023, max compression
```

## Comparing `thrivve_core-0.0.7.tar` & `thrivve_core-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2307 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-17 12:28:27.000000 thrivve_core-0.0.7/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-17 12:28:39.000000 thrivve_core-0.0.7/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-18 12:53:47.000000 thrivve_core-0.0.8/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-18 12:53:58.000000 thrivve_core-0.0.8/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.0.7/PKG-INFO` & `thrivve_core-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.0.7
+Version: 0.0.8
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.7/setup.py` & `thrivve_core-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.0.7",
+    version="0.0.8",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.0.7/thrivve_core/__init__.py` & `thrivve_core-0.0.8/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.0.8/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.0.8/thrivve_core/app_decorators/handle_auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import wraps
 
 from flask import request
 
-from thrivve_core.helpers.auth import verify_user_token
+from thrivve_core.helpers.auth import verify_user_token_v2
 from thrivve_core.helpers.exceptions import (
     AppValidationError,
     AppMissingAuthError,
 )
-from thrivve_core.helpers.acl_enum import Permission
+# from thrivve_core.helpers.acl_enum import Permission
 
 
 def handle_auth(require_auth, append_auth_args=None, allowed_roles=None, pre_login=False, allowed_permissions=None):
     def factory(func):
         @wraps(func)
         def inner_function(*args, **kws):
             if not require_auth:
@@ -20,15 +20,15 @@
             if "Authorization" not in request.headers:
                 raise AppMissingAuthError("Missing authentication")
 
             token = request.headers["Authorization"]
             if "country_code" not in request.headers and request.endpoint != "health_check":
                 raise AppValidationError("Country Code is Required (c)")
 
-            user = verify_user_token(token=token)
+            user = verify_user_token_v2(token=token)
 
             if not pre_login:
                 if not user.get("is_logged"):
                     raise AppValidationError("Not Logged Token, please complete login process")
 
             if allowed_roles:
                 if user.get("role") not in allowed_roles:
```

### Comparing `thrivve_core-0.0.7/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.0.8/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.0.8/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.0.8/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/base.py` & `thrivve_core-0.0.8/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.0.8/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.0.8/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.0.8/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.0.8/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.0.8/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.0.8/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.0.8/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/auth.py` & `thrivve_core-0.0.8/thrivve_core/helpers/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import requests
 from flask import request
 
 from app.helpers.auth.enums import Language
-from .exceptions import AppValidationError, AppMissingAuthError
+from .exceptions import AppValidationError
 from flask import session
 
 from .. import ThrivveCore
-
+from .micro_fetcher import MicroFetcher
 
 class Auth:
     def __init__(self):
         pass
 
     @staticmethod
     def set_user(user):
@@ -82,7 +82,24 @@
         raise AppValidationError("Error in parsing auth response")
 
     response["data"].update(token=token)
     user = response["data"]
 
     Auth.set_user(user)
     return user
+
+
+def verify_user_token_v2(token):
+
+    results = MicroFetcher(
+        "AUTH_SERVICE"
+    ).from_function(
+        "app.business_logic.auth.authenticate.authenticate"
+    ).with_params(
+        token=token
+    ).fetch()
+
+    results["data"].update(token=token)
+    user = results["data"]
+
+    Auth.set_user(user)
+    return user
```

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/config.py` & `thrivve_core-0.0.8/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.0.8/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.0.8/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/enums.py` & `thrivve_core-0.0.8/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.0.8/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.0.8/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/filters.py` & `thrivve_core-0.0.8/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.0.8/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.0.8/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.0.8/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/log_config.py` & `thrivve_core-0.0.8/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.0.8/thrivve_core/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/notification_center.py` & `thrivve_core-0.0.8/thrivve_core/helpers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/search_function.py` & `thrivve_core-0.0.8/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/service_config.py` & `thrivve_core-0.0.8/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/sql.py` & `thrivve_core-0.0.8/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/time.py` & `thrivve_core-0.0.8/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/topics.py` & `thrivve_core-0.0.8/thrivve_core/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.0.8/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.0.8/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.0.7/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.0.8/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.0.7
+Version: 0.0.8
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.7/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.0.8/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

