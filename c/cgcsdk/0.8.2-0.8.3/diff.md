# Comparing `tmp/cgcsdk-0.8.2.tar.gz` & `tmp/cgcsdk-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.2.tar", last modified: Tue Apr 18 10:15:47 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.3.tar", last modified: Tue Apr 18 11:04:00 2023, max compression
```

## Comparing `cgcsdk-0.8.2.tar` & `cgcsdk-0.8.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.209233 cgcsdk-0.8.2/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.2/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-04-18 10:15:47.207705 cgcsdk-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:46.974822 cgcsdk-0.8.2/cgc/
--rw-rw-rw-   0        0        0      234 2023-04-18 10:14:24.000000 cgcsdk-0.8.2/cgc/.env
--rw-rw-rw-   0        0        0     3191 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:46.994510 cgcsdk-0.8.2/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.008714 cgcsdk-0.8.2/cgc/commands/auth/
--rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.2/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.2/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.2/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.022916 cgcsdk-0.8.2/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/cgc_cmd_responses.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.038993 cgcsdk-0.8.2/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5189 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.046262 cgcsdk-0.8.2/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3294 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.049496 cgcsdk-0.8.2/cgc/commands/debug/
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.2/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.055140 cgcsdk-0.8.2/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.071364 cgcsdk-0.8.2/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.2/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.2/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.088266 cgcsdk-0.8.2/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7155 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1597 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     1459 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.093997 cgcsdk-0.8.2/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.099847 cgcsdk-0.8.2/cgc/tests/
--rw-rw-rw-   0        0        0   102745 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.126824 cgcsdk-0.8.2/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.2/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.2/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.159157 cgcsdk-0.8.2/cgc/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.2/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.2/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.169024 cgcsdk-0.8.2/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.2/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.185213 cgcsdk-0.8.2/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.2/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.2/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.2/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.2/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.2/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.2/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.2/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.2/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:15:47.205003 cgcsdk-0.8.2/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2387 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 10:15:46.000000 cgcsdk-0.8.2/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 10:15:47.210307 cgcsdk-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.564134 cgcsdk-0.8.3/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-04-18 11:04:00.562138 cgcsdk-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.291920 cgcsdk-0.8.3/cgc/
+-rw-rw-rw-   0        0        0      234 2023-04-18 10:51:28.000000 cgcsdk-0.8.3/cgc/.env
+-rw-rw-rw-   0        0        0     3350 2023-04-18 10:59:49.000000 cgcsdk-0.8.3/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.317490 cgcsdk-0.8.3/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.343277 cgcsdk-0.8.3/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.3/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.3/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.3/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.366148 cgcsdk-0.8.3/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/cgc_cmd_responses.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.384169 cgcsdk-0.8.3/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.3/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.389809 cgcsdk-0.8.3/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.3/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.392716 cgcsdk-0.8.3/cgc/commands/debug/
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.3/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.398564 cgcsdk-0.8.3/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.414921 cgcsdk-0.8.3/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.3/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.3/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.428071 cgcsdk-0.8.3/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7189 2023-04-18 10:58:34.000000 cgcsdk-0.8.3/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.3/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     1499 2023-04-18 10:58:48.000000 cgcsdk-0.8.3/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.434509 cgcsdk-0.8.3/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.439978 cgcsdk-0.8.3/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.3/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.469620 cgcsdk-0.8.3/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.3/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.3/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.509686 cgcsdk-0.8.3/cgc/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.3/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.3/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.519366 cgcsdk-0.8.3/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.3/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.532761 cgcsdk-0.8.3/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.3/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.3/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.3/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.3/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.3/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.3/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.3/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.3/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:04:00.557565 cgcsdk-0.8.3/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2387 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 11:04:00.000000 cgcsdk-0.8.3/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 11:04:00.565134 cgcsdk-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.3/setup.py
```

### Comparing `cgcsdk-0.8.2/PKG-INFO` & `cgcsdk-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.2/cgc/CHANGELOG.md` & `cgcsdk-0.8.3/cgc/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Change Log
 
+## 0.8.3
+
+Release on Apr 18, 2023.
+
+* minor db sdk update
+* added restart optional parameter to client
+
+## 0.8.2
+
+Release on Apr 18, 2023.
+
+* minor bug fixes
+
 ## 0.8.1
 
 Release on Apr 17, 2023.
 
 * cgc db list
 * cgc compute list
 * cgc events APP_NAME
```

### Comparing `cgcsdk-0.8.2/cgc/cgc.py` & `cgcsdk-0.8.3/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.3/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.3/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.3/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.3/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.3/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.3/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.3/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.3/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.3/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.3/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.3/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.3/cgc/commands/compute/compute_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         message += f"Container will be Ready after volumes can be see mounted.\n"
 
     app_url = data["details"]["created_template"]["pod_url"]
     if app_url == "None":
         message += "This app is not exposed via HTTPS\n"
     else:
         message += f"Will be accessible at: {app_url}\n"
-    message += f"App token: {app_token}\nTo monitor the startup status use command: cgc resource list"
+    message += f"App token: {app_token}\nTo monitor the startup status use list command"
 
     return message
 
 
 @key_error_decorator_for_helpers
 def compute_delete_response(data: dict) -> str:
     """Create response string for compute delete command.
```

### Comparing `cgcsdk-0.8.2/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.3/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.3/cgc/commands/db/db_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     default=2,
     help="How much Gi RAM app can use",
 )
 @click.option(
     "-v",
     "--volume",
     "volumes",
-    multiple=False,
+    multiple=True,
     help="Volume name to be mounted with default mount path",
 )
 def db_create(
     entity: str,
     cpu: int,
     memory: int,
     volumes: list[str],
```

### Comparing `cgcsdk-0.8.2/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.8.3/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.3/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.3/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.3/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.3/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/sdk/handlers.py` & `cgcsdk-0.8.3/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/sdk/mongodb.py` & `cgcsdk-0.8.3/cgc/sdk/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,26 +177,26 @@
         # print("collection   : {}.{}".format(d["ns"]["db"], d["ns"]["coll"]))
         # try:
         #     print("doc          : {}".format(d["fullDocument"]))
         # except KeyError:
         #     pass
 
 
-def get_mongo_access(app_name: str, password: str):
+def get_mongo_access(app_name: str, password: str, restart: bool = False):
     global _mongo_access
 
     def init_access():
         global _mongo_access
         _mongo_access = MongoConnector(
             database_name="db",
             hosts=f"{app_name}:27017",
             username="admin",
             password=password,
         )
 
     try:
-        if not isinstance(_mongo_access, MongoConnector):
+        if not isinstance(_mongo_access, MongoConnector) or restart:
             init_access()
     except NameError:
         init_access()
         pass
     return _mongo_access
```

### Comparing `cgcsdk-0.8.2/cgc/sdk/postgresql.py` & `cgcsdk-0.8.3/cgc/sdk/postgresql.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,25 @@
                 print(f"PostgreSQL connection error: {e}")
                 print(f"retrying to connect...")
 
     def get_postgresql_client(self):
         return self._postgresql_client
 
 
-def get_postgresql_access(app_name: str, password: str, database: str = "db"):
+def get_postgresql_access(
+    app_name: str, password: str, database: str = "db", restart: bool = False
+):
     global _postgresql_access
 
     def init_access():
         global _postgresql_access
         _postgresql_access = PostreSQLConnector(
             host=app_name, password=password, database=database
         )
 
     try:
-        if not isinstance(_postgresql_access, PostreSQLConnector):
+        if not isinstance(_postgresql_access, PostreSQLConnector) or restart:
             init_access()
     except NameError:
         init_access()
         pass
     return _postgresql_access
```

### Comparing `cgcsdk-0.8.2/cgc/sdk/redis.py` & `cgcsdk-0.8.3/cgc/sdk/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,25 @@
                 print(f"Redis connection error: {e}")
                 print(f"retrying to connect...")
 
     def get_redis_client(self):
         return self._redis_client
 
 
-def get_redis_access(app_name: str, password: str, decode_responses: bool = False):
+def get_redis_access(
+    app_name: str, password: str, decode_responses: bool = False, restart: bool = False
+):
     global _redis_access
 
     def init_access():
         global _redis_access
         _redis_access = RedisConnector(
             host=app_name, password=password, decode_responses=decode_responses
         )
 
     try:
-        if not isinstance(_redis_access, RedisConnector):
+        if not isinstance(_redis_access, RedisConnector) or restart:
             init_access()
     except NameError:
         init_access()
         pass
     return _redis_access
```

### Comparing `cgcsdk-0.8.2/cgc/server.crt` & `cgcsdk-0.8.3/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/telemetry/basic.py` & `cgcsdk-0.8.3/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/tests/__init__.py` & `cgcsdk-0.8.3/cgc/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1812,15 +1812,15 @@
         "Username: pytest\n"
         "Password: 9bb9c88f8fc14eadba5c5fbdafc06275"
     )
     test_compute_create = (
         "nvidia-pytorch app test1 creation started!\n"
         "Will be accessible at: https://test1.pytest.dev.quantdevlabs.com\n"
         "App token: 1ce03c31ab9c40df8594d97b301eaaea\n"
-        "To monitor the startup status use command: cgc resource list"
+        "To monitor the startup status use command: cgc compute list"
     )
     test_compute_create_no_volume_found = "[33mVolume name not found in namespace.[0m"
     test_compute_delete = "App test1 and its service successfully deleted."
     test_compute_restart = "App test1 has been successfully restarted."
     test_compute_list = get_desired_response_data("test_compute_list.txt")
     test_compute_template_list = "Available templates: tensorflow-jupyter, datascience-jupyter, nvidia-rapids, nvidia-pytorch, nvidia-tensorflow"
     test_tabulate_a_response = get_desired_response_data("test_tabulate_response.txt")
```

### Comparing `cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.3/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.3/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.3/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/tests/responses_tests.py` & `cgcsdk-0.8.3/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/click_group.py` & `cgcsdk-0.8.3/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/config_utils.py` & `cgcsdk-0.8.3/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.3/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.3/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.3/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.3/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.3/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.3/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/message_utils.py` & `cgcsdk-0.8.3/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.3/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/requests_helper.py` & `cgcsdk-0.8.3/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/response_utils.py` & `cgcsdk-0.8.3/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgc/utils/version_control.py` & `cgcsdk-0.8.3/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.3/cgcsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.2/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.3/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.2/setup.py` & `cgcsdk-0.8.3/setup.py`

 * *Files identical despite different names*

