# Comparing `tmp/cgcsdk-0.8.0.tar.gz` & `tmp/cgcsdk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.0.tar", last modified: Fri Apr 14 14:29:17 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.1.tar", last modified: Tue Apr 18 09:57:57 2023, max compression
```

## Comparing `cgcsdk-0.8.0.tar` & `cgcsdk-0.8.1.tar`

### file list

```diff
@@ -1,93 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.576294 cgcsdk-0.8.0/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-04-14 14:29:17.574677 cgcsdk-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.314630 cgcsdk-0.8.0/cgc/
--rw-rw-rw-   0        0        0      234 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/.env
--rw-rw-rw-   0        0        0     3021 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      435 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/__init__.py
--rw-rw-rw-   0        0        0     1253 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.323543 cgcsdk-0.8.0/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.334739 cgcsdk-0.8.0/cgc/commands/auth/
--rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.343461 cgcsdk-0.8.0/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     1353 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/cgc_cmd_responses.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.372502 cgcsdk-0.8.0/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4275 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      883 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5189 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.379463 cgcsdk-0.8.0/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     2592 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.386932 cgcsdk-0.8.0/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.393573 cgcsdk-0.8.0/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     4413 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.412750 cgcsdk-0.8.0/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/config.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.420110 cgcsdk-0.8.0/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3187 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.429987 cgcsdk-0.8.0/cgc/tests/
--rw-rw-rw-   0        0        0   102745 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.470327 cgcsdk-0.8.0/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.512619 cgcsdk-0.8.0/cgc/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.526651 cgcsdk-0.8.0/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.0/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.546520 cgcsdk-0.8.0/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.0/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.0/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.0/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.0/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2958 2023-03-08 10:41:28.000000 cgcsdk-0.8.0/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.570329 cgcsdk-0.8.0/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2320 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       94 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:29:17.576800 cgcsdk-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2061 2023-02-15 12:56:02.000000 cgcsdk-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.267872 cgcsdk-0.8.1/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-04-18 09:57:57.266869 cgcsdk-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.046969 cgcsdk-0.8.1/cgc/
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/.env
+-rw-rw-rw-   0        0        0     3191 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.058110 cgcsdk-0.8.1/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.071635 cgcsdk-0.8.1/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.1/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.1/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.1/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.084606 cgcsdk-0.8.1/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/cgc_cmd_responses.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.100783 cgcsdk-0.8.1/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5189 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.105288 cgcsdk-0.8.1/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3294 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.109030 cgcsdk-0.8.1/cgc/commands/debug/
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.1/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.115384 cgcsdk-0.8.1/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.131097 cgcsdk-0.8.1/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.1/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.1/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.148227 cgcsdk-0.8.1/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7155 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1597 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     1459 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.154892 cgcsdk-0.8.1/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.162141 cgcsdk-0.8.1/cgc/tests/
+-rw-rw-rw-   0        0        0   102745 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.190240 cgcsdk-0.8.1/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.1/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.1/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.221537 cgcsdk-0.8.1/cgc/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.1/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.1/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.231635 cgcsdk-0.8.1/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.1/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.243452 cgcsdk-0.8.1/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.1/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.1/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.1/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.1/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.1/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.1/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.1/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.1/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:57:57.263537 cgcsdk-0.8.1/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2387 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       94 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 09:57:56.000000 cgcsdk-0.8.1/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:57:57.269005 cgcsdk-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2061 2023-02-15 12:56:02.000000 cgcsdk-0.8.1/setup.py
```

### Comparing `cgcsdk-0.8.0/PKG-INFO` & `cgcsdk-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.0/cgc/CHANGELOG.md` & `cgcsdk-0.8.1/cgc/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Change Log
 
+## 0.8.1
+
+Release on Apr 17, 2023.
+
+* cgc db list
+* cgc compute list
+* cgc events APP_NAME
+* package cgc.sdk for management of databases templates inside user namespace
+
 ## 0.8.0
 
 Release on Apr 14, 2023.
 
 * cgc db - new commands for managing databases
 * cgc compute - refactor commands for compute template management
 * cgc resource - new command to control db and compute resources
```

### Comparing `cgcsdk-0.8.0/cgc/cgc.py` & `cgcsdk-0.8.1/cgc/cgc.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 from cgc.commands.billing.billing_cmd import billing_group
 from cgc.commands.db.db_cmd import db_group
 from cgc.commands.resource.resource_cmd import resource_group
 from cgc.commands.auth.auth_cmd import (
     api_keys_group,
     auth_register,
 )
+
 from cgc.commands.debug.debug_cmd import debug_group
-from cgc.commands.cgc_cmd import cgc_rm, cgc_status, sending_telemetry_permission
-from cgc.utils.version_control import check_version, get_version
+from cgc.commands.cgc_cmd import (
+    cgc_rm,
+    cgc_status,
+    sending_telemetry_permission,
+    resource_events,
+)
+from cgc.utils.version_control import check_version, _get_version
 from cgc.utils.click_group import CustomGroup
 
 
 @click.group(cls=CustomGroup)
-@click.version_option(get_version())
+@click.version_option(_get_version())
 def cli():
     """CGC application developed by Comtegra S.A."""
     check_version()
 
 
+cli.add_command(debug_group)
 cli.add_command(auth_register)
 cli.add_command(api_keys_group)
 cli.add_command(volume_group)
 cli.add_command(compute_group)
 cli.add_command(db_group)
+cli.add_command(cgc_rm)
+cli.add_command(resource_events)
 cli.add_command(resource_group)
 cli.add_command(billing_group)
-cli.add_command(cgc_rm)
 cli.add_command(cgc_status)
-cli.add_command(debug_group)
 cli.add_command(sending_telemetry_permission)
 
 
 if __name__ == "__main__" or __name__ == "cgc.cgc":
     cli()
 else:
     raise Exception("This program is not intended for importing!")
```

### Comparing `cgcsdk-0.8.0/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.1/cgc/commands/auth/auth_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cgc.utils.prepare_headers import get_url_and_prepare_headers_register
 from cgc.utils.cryptography import rsa_crypto
 from cgc.utils.click_group import CustomCommand, CustomGroup
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 
 
-@click.group("api-keys", cls=CustomGroup)
+@click.group("api-keys", cls=CustomGroup, hidden=True)
 def api_keys_group():
     """
     Management of API keys.
     """
     pass
```

### Comparing `cgcsdk-0.8.0/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.1/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.1/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.1/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.1/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.1/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.1/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.1/cgc/commands/cgc_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 import click
+import json
+
 from cgc.commands.cgc_cmd_responses import cgc_status_response
 from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.click_group import CustomCommand
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.telemetry.basic import telemetry_permission_set
+from cgc.commands.compute.compute_responses import compute_logs_response
 
 
 @click.command("rm", cls=CustomCommand)
 @click.argument("name", type=click.STRING)
 def cgc_rm(name: str):
     """
     Delete an app in user namespace
     """
     resource_delete(name)
 
 
+@click.command("events", cls=CustomCommand)
+@click.argument("app_name", type=click.STRING)
+def resource_events(app_name: str):
+    """Get events of given app"""
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/get_pod_events"
+    metric = "resource.events"
+    __payload = {"name": app_name}
+    __res = call_api(
+        request=EndpointTypes.get,
+        url=url,
+        headers=headers,
+        data=json.dumps(__payload),
+    )
+    click.echo(
+        compute_logs_response(retrieve_and_validate_response_send_metric(__res, metric))
+    )
+
+
 @click.command("status", cls=CustomCommand)
 def cgc_status():
     """Lists available and used resources"""
     api_url, headers = get_api_url_and_prepare_headers()
     url = f"{api_url}/v1/api/resource/status"
     metric = "resource.status"
     __res = call_api(
```

### Comparing `cgcsdk-0.8.0/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.1/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.1/cgc/commands/compute/compute_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import json
 import click
 
 from cgc.commands.compute.compute_models import EntityList, GPUsList
 from cgc.commands.compute.compute_responses import (
     compute_create_filebrowser_response,
     compute_create_response,
+    compute_list_response,
 )
 from cgc.commands.compute.compute_utills import compute_create_payload
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.commands.resource.resource_cmd import resource_delete
 
 
 @click.group(name="compute", cls=CustomGroup)
-@click.option("--debug", "debug", is_flag=True, default=False, hidden=True)
-@click.pass_context
-def compute_group(ctx, debug):
+def compute_group():
     """
     Management of compute resources.
     """
-    ctx.ensure_object(dict)
-    ctx.obj["DEBUG"] = debug
 
 
 @click.group(name="filebrowser", cls=CustomGroup)
 def filebrowser_group():
     """
     Management of filebrowser.
     """
@@ -159,7 +156,31 @@
     :param name: name of app to delete
     :type name: str
     """
     resource_delete(name)
 
 
 compute_group.add_command(filebrowser_group)
+
+
+@compute_group.command("list", cls=CustomCommand)
+@click.option(
+    "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
+)
+def resource_list(detailed: bool):
+    """
+    List all apps for user namespace.
+    """
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/list?resource_type=compute"
+    metric = "compute.list"
+    __res = call_api(
+        request=EndpointTypes.get,
+        url=url,
+        headers=headers,
+    )
+    table = compute_list_response(
+        detailed,
+        retrieve_and_validate_response_send_metric(__res, metric),
+    )
+
+    click.echo(table)
```

### Comparing `cgcsdk-0.8.0/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.1/cgc/commands/compute/compute_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,28 @@
     :type Enum: str
     """
 
     NVIDIA_TENSORFLOW = "nvidia-tensorflow"
     NVIDIA_RAPIDS = "nvidia-rapids"
     NVIDIA_PYTORCH = "nvidia-pytorch"
     NVIDIA_TRITON = "nvidia-triton"
+    NGINX = "nginx"
 
 
 class DatabasesList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
     """
 
     MONGODB = "mongodb"
     POSTGRESQL = "postgresql"
     REDIS = "redis"
+    # MINIO = "minio"
 
 
 class GPUsList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
```

### Comparing `cgcsdk-0.8.0/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.1/cgc/commands/compute/compute_responses.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,17 +93,17 @@
     message = f"{entity} app {name} creation started!\n"
     if volumes:
         message += f" Volumes to mount: {volumes}\n"
         message += f"Container will be Ready after volumes can be see mounted.\n"
 
     app_url = data["details"]["created_template"]["pod_url"]
     if app_url == "None":
-        message += f"Will be accessible at: {app_url}\n"
-    else:
         message += "This app is not exposed via HTTPS\n"
+    else:
+        message += f"Will be accessible at: {app_url}\n"
     message += f"App token: {app_token}\nTo monitor the startup status use command: cgc resource list"
 
     return message
 
 
 @key_error_decorator_for_helpers
 def compute_delete_response(data: dict) -> str:
```

### Comparing `cgcsdk-0.8.0/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.1/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.1/cgc/commands/db/db_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import click
 
+from cgc.commands.compute.compute_responses import compute_list_response
 from cgc.commands.compute.compute_models import DatabasesList
 from cgc.commands.compute.compute_responses import compute_create_response
 from cgc.commands.compute.compute_utills import compute_create_payload
 from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
@@ -94,7 +95,31 @@
     """
     Delete an app from user namespace.
     \f
     :param name: name of app to delete
     :type name: str
     """
     resource_delete(name)
+
+
+@db_group.command("list", cls=CustomCommand)
+@click.option(
+    "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
+)
+def resource_list(detailed: bool):
+    """
+    List all apps for user namespace.
+    """
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/list?resource_type=db"
+    metric = "db.list"
+    __res = call_api(
+        request=EndpointTypes.get,
+        url=url,
+        headers=headers,
+    )
+    table = compute_list_response(
+        detailed,
+        retrieve_and_validate_response_send_metric(__res, metric),
+    )
+
+    click.echo(table)
```

### Comparing `cgcsdk-0.8.0/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.8.1/cgc/commands/resource/resource_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import click
 import json
 
 from cgc.commands.compute.compute_models import EntityList, DatabasesList
 from cgc.commands.compute.compute_responses import (
     template_list_response,
     template_get_start_path_response,
-    compute_logs_response,
     compute_restart_response,
     compute_delete_response,
-    compute_list_response,
 )
 
 from cgc.commands.compute.compute_utills import compute_delete_payload
 
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 
 
-@click.group(name="resource", cls=CustomGroup)
+@click.group(name="resource", cls=CustomGroup, hidden=True)
 def resource_group():
     """
     Management of templates.
     """
 
 
 @resource_group.command("list_templates", cls=CustomCommand)
@@ -36,38 +34,14 @@
     click.echo(
         template_list_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@resource_group.command("list", cls=CustomCommand)
-@click.option(
-    "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
-)
-def resource_list(detailed: bool):
-    """
-    List all apps for user namespace.
-    """
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/list"
-    metric = "resource.list"
-    __res = call_api(
-        request=EndpointTypes.get,
-        url=url,
-        headers=headers,
-    )
-    table = compute_list_response(
-        detailed,
-        retrieve_and_validate_response_send_metric(__res, metric),
-    )
-
-    click.echo(table)
-
-
 @resource_group.command("get_start_path", cls=CustomCommand)
 @click.argument(
     "template", type=click.Choice([*EntityList.get_list(), *DatabasesList.get_list()])
 )
 def template_get_start_path(template: str):
     """Displays start path of specified template"""
     api_url, headers = get_api_url_and_prepare_headers()
@@ -77,33 +51,14 @@
     click.echo(
         template_get_start_path_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@resource_group.command("logs", cls=CustomCommand)
-@click.argument("app_name", type=click.STRING)
-def compute_logs(app_name: str):
-    """Get logs of given app"""
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/get_pod_events"
-    metric = "resource.logs"
-    __payload = {"name": app_name}
-    __res = call_api(
-        request=EndpointTypes.get,
-        url=url,
-        headers=headers,
-        data=json.dumps(__payload),
-    )
-    click.echo(
-        compute_logs_response(retrieve_and_validate_response_send_metric(__res, metric))
-    )
-
-
 @resource_group.command("restart", cls=CustomCommand)
 @click.argument("name", type=click.STRING)
 def compute_restart(name: str):
     """Restarts the specified app"""
     api_url, headers = get_api_url_and_prepare_headers()
     url = f"{api_url}/v1/api/resource/restart"
     metric = "resource.restart"
```

### Comparing `cgcsdk-0.8.0/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.1/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.1/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.1/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.1/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/server.crt` & `cgcsdk-0.8.1/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/telemetry/basic.py` & `cgcsdk-0.8.1/cgc/telemetry/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     :return: TELEMETRY_PERMISSION value
     :rtype: bool
     """
     while True:
         permission = input(
             "We would like to make your experience with CGC even better! :)\n\
-            We would like to know which commands are utilized most often and if they have finished properly. Nothing else is collected. Only raw numbers.\n\
+We would like to know which commands are utilized most often and if they have finished properly. Nothing else is collected. Only raw numbers.\n\
 Would you agree to send us these numbers? (YES/no) [YES]: \n"
         )
         if permission.lower() in ["yes", "no", ""]:
             break
     permission = True if permission == "" or permission == "yes" else False
 
     f = open(file=ENV_FILE_PATH, mode="r")
```

### Comparing `cgcsdk-0.8.0/cgc/tests/__init__.py` & `cgcsdk-0.8.1/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.1/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.1/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.1/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/tests/responses_tests.py` & `cgcsdk-0.8.1/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/click_group.py` & `cgcsdk-0.8.1/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/config_utils.py` & `cgcsdk-0.8.1/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.1/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.1/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.1/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.1/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.1/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.1/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/message_utils.py` & `cgcsdk-0.8.1/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.1/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/requests_helper.py` & `cgcsdk-0.8.1/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/response_utils.py` & `cgcsdk-0.8.1/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.0/cgc/utils/version_control.py` & `cgcsdk-0.8.1/cgc/utils/version_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,10 +70,10 @@
         and server_major == MAJOR_VERSION
         and server_minor > MINOR_VERSION
     ):
         click.echo(prepare_warning_message(OUTDATED_MINOR))
         print_compare_versions(server_version, client_version)
 
 
-def get_version():
+def _get_version():
     """Returns version of cgcsdk."""
     return f"{RELEASE}.{MAJOR_VERSION}.{MINOR_VERSION}"
```

### Comparing `cgcsdk-0.8.0/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.1/cgcsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.0/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.1/cgcsdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 cgc/commands/compute/__init__.py
 cgc/commands/compute/compute_cmd.py
 cgc/commands/compute/compute_models.py
 cgc/commands/compute/compute_responses.py
 cgc/commands/compute/compute_utills.py
 cgc/commands/db/__init__.py
 cgc/commands/db/db_cmd.py
-cgc/commands/debug/__init__.py
 cgc/commands/debug/debug_cmd.py
 cgc/commands/resource/__init__.py
 cgc/commands/resource/resource_cmd.py
 cgc/commands/volume/__init__.py
 cgc/commands/volume/data_model.py
 cgc/commands/volume/volume_cmd.py
 cgc/commands/volume/volume_responses.py
 cgc/commands/volume/volume_utils.py
+cgc/sdk/__init__.py
+cgc/sdk/handlers.py
+cgc/sdk/mongodb.py
+cgc/sdk/postgresql.py
+cgc/sdk/redis.py
 cgc/telemetry/__init__.py
 cgc/telemetry/basic.py
 cgc/tests/__init__.py
 cgc/tests/responses_tests.py
 cgc/tests/desired_responses/test_billing_invoice.txt
 cgc/tests/desired_responses/test_billing_status.txt
 cgc/tests/desired_responses/test_billing_stop_events_compute.txt
```

### Comparing `cgcsdk-0.8.0/setup.py` & `cgcsdk-0.8.1/setup.py`

 * *Files identical despite different names*

