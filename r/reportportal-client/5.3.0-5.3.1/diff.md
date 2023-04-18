# Comparing `tmp/reportportal-client-5.3.0.tar.gz` & `tmp/reportportal-client-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportportal-client-5.3.0.tar", last modified: Tue Mar 28 08:52:23 2023, max compression
+gzip compressed data, was "reportportal-client-5.3.1.tar", last modified: Tue Apr 18 12:53:00 2023, max compression
```

## Comparing `reportportal-client-5.3.0.tar` & `reportportal-client-5.3.1.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/rp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/rp_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/rp_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/rp_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/item_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_base_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/items/rp_log_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_log_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_log_items/rp_log_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client/items/rp_test_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_test_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_base_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_child_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_root_test_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/reportportal_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/logs/log_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/reportportal_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/services/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/reportportal_client/static/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/static/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/static/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/static/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/reportportal_client/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/reportportal_client/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.658364 reportportal-client-5.3.0/reportportal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-28 08:52:23.000000 reportportal-client-5.3.0/reportportal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-28 08:52:23.000000 reportportal-client-5.3.0/reportportal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 08:52:23.000000 reportportal-client-5.3.0/reportportal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-28 08:52:23.000000 reportportal-client-5.3.0/reportportal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 08:52:23.000000 reportportal-client-5.3.0/reportportal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 08:52:23.662364 reportportal-client-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-28 08:52:20.000000 reportportal-client-5.3.0/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client/_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/item_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_base_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/rp_log_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_base_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_child_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_root_test_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/logs/log_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/reportportal_client/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/steps/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.0/CONTRIBUTING.rst` & `reportportal-client-5.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/LICENSE.md` & `reportportal-client-5.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/__init__.py` & `reportportal-client-5.3.1/reportportal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/_local/__init__.py` & `reportportal-client-5.3.1/reportportal_client/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/client.py` & `reportportal-client-5.3.1/reportportal_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         self.session.mount('http://', HTTPAdapter(
             max_retries=retry_strategy, pool_maxsize=max_pool_size))
         self.session.headers['Authorization'] = 'bearer {0}'.format(self.token)
 
         self._log_manager = LogManager(
             self.endpoint, self.session, self.api_v2, self.launch_id,
             self.project, max_entry_number=log_batch_size,
-            max_payload_size=log_batch_payload_size)
+            max_payload_size=log_batch_payload_size,
+            verify_ssl=self.verify_ssl)
 
     def finish_launch(self,
                       end_time,
                       status=None,
                       attributes=None,
                       **kwargs):
         """Finish launch.
```

### Comparing `reportportal-client-5.3.0/reportportal_client/core/__init__.py` & `reportportal-client-5.3.1/reportportal_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/rp_file.py` & `reportportal-client-5.3.1/reportportal_client/core/rp_file.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/rp_issues.py` & `reportportal-client-5.3.1/reportportal_client/core/rp_issues.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/rp_requests.py` & `reportportal-client-5.3.1/reportportal_client/core/rp_requests.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/rp_responses.py` & `reportportal-client-5.3.1/reportportal_client/core/rp_responses.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/test_manager.py` & `reportportal-client-5.3.1/reportportal_client/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/core/worker.py` & `reportportal-client-5.3.1/reportportal_client/core/worker.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/errors.py` & `reportportal-client-5.3.1/reportportal_client/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/helpers.py` & `reportportal-client-5.3.1/reportportal_client/helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/__init__.py` & `reportportal-client-5.3.1/reportportal_client/items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/item_weight.py` & `reportportal-client-5.3.1/reportportal_client/items/item_weight.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_base_item.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_base_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_log_items/__init__.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_log_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_log_items/rp_log_item.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_log_items/rp_log_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_test_items/__init__.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_base_test_item.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_base_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_child_test_item.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_child_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/items/rp_test_items/rp_root_test_item.py` & `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_root_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/logs/__init__.py` & `reportportal-client-5.3.1/reportportal_client/logs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,16 @@
             msg = self.format(record)
         except (KeyboardInterrupt, SystemExit):
             raise
         except Exception:
             self.handleError(record)
 
         log_level = self._get_rp_log_level(record.levelno)
-        if self.rp_client:
-            rp_client = self.rp_client
-        else:
+        rp_client = self.rp_client
+        if not rp_client:
             rp_client = current()
         if rp_client:
             rp_client.log(
                 timestamp(),
                 msg,
                 level=log_level,
                 attachment=record.__dict__.get('attachment', None),
```

### Comparing `reportportal-client-5.3.0/reportportal_client/logs/log_manager.py` & `reportportal-client-5.3.1/reportportal_client/logs/log_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,23 @@
     RPRequestLog
 )
 from reportportal_client.core.worker import APIWorker
 from reportportal_client.static.defines import NOT_FOUND
 
 logger = logging.getLogger(__name__)
 
+MAX_LOG_BATCH_SIZE = 20
 MAX_LOG_BATCH_PAYLOAD_SIZE = 65000000
 
 
 class LogManager(object):
     """Manager of the log items."""
 
     def __init__(self, rp_url, session, api_version, launch_id, project_name,
-                 max_entry_number=20, verify_ssl=True,
+                 max_entry_number=MAX_LOG_BATCH_SIZE, verify_ssl=True,
                  max_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE):
         """Initialize instance attributes.
 
         :param rp_url:           Report portal URL
         :param session:          HTTP Session object
         :param api_version:      RP API version
         :param launch_id:        Parent launch UUID
```

### Comparing `reportportal-client-5.3.0/reportportal_client/services/__init__.py` & `reportportal-client-5.3.1/reportportal_client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/services/statistics.py` & `reportportal-client-5.3.1/reportportal_client/services/statistics.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 import logging
-import os
 from platform import python_version
-from uuid import uuid4
 
 import requests
 from pkg_resources import get_distribution
 
-from .constants import CLIENT_INFO, ENDPOINT, CLIENT_ID_PROPERTY
+from .client_id import get_client_id
+from .constants import CLIENT_INFO, ENDPOINT
 
 logger = logging.getLogger(__name__)
 
 ID, KEY = CLIENT_INFO.split(':')
 
 
 def _get_client_info():
@@ -41,54 +40,14 @@
     """Get current platform basic info, e.g.: 'Python 3.6.1'.
 
     :return: str represents the current platform, e.g.: 'Python 3.6.1'
     """
     return 'Python ' + python_version()
 
 
-def _load_properties(filepath, sep='=', comment_str='#'):
-    """Read the file passed as parameter as a properties file.
-
-    :param filepath: path to property file
-    :param sep: separator string between key and value
-    :param comment_str: a string which designate comment line
-    :return: property file as Dict
-    """
-    result = {}
-    with open(filepath, "rt") as f:
-        for line in f:
-            s_line = line.strip()
-            if s_line and not s_line.startswith(comment_str):
-                sep_idx = s_line.index(sep)
-                key = s_line[0:sep_idx]
-                value = s_line[sep_idx + 1:]
-                result[key.rstrip()] = value.lstrip()
-    return result
-
-
-def _get_client_id():
-    """Get client ID.
-
-    :return: str represents the client ID
-    """
-    rp_folder = os.path.expanduser('~/.rp')
-    rp_properties = os.path.join(rp_folder, 'rp.properties')
-    client_id = None
-    if os.path.exists(rp_properties):
-        config = _load_properties(rp_properties)
-        client_id = config.get(CLIENT_ID_PROPERTY)
-    if not client_id:
-        if not os.path.exists(rp_folder):
-            os.mkdir(rp_folder)
-        client_id = str(uuid4())
-        with open(rp_properties, 'a') as f:
-            f.write('\n' + CLIENT_ID_PROPERTY + '=' + client_id + '\n')
-    return client_id
-
-
 def send_event(event_name, agent_name, agent_version):
     """Send an event to statistics service.
 
      Use client and agent versions with their names.
 
     :param event_name: Event name to be used
     :param agent_name: Name of the agent that uses the client
@@ -105,15 +64,15 @@
 
     if agent_name:
         params['agent_name'] = agent_name
     if agent_version:
         params['agent_version'] = agent_version
 
     payload = {
-        'client_id': _get_client_id(),
+        'client_id': get_client_id(),
         'events': [{
             'name': event_name,
             'params': params
         }]
     }
     headers = {'User-Agent': 'python-requests'}
     params = {
```

### Comparing `reportportal-client-5.3.0/reportportal_client/static/__init__.py` & `reportportal-client-5.3.1/reportportal_client/static/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/static/abstract.py` & `reportportal-client-5.3.1/reportportal_client/static/abstract.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/static/defines.py` & `reportportal-client-5.3.1/reportportal_client/static/defines.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/static/errors.py` & `reportportal-client-5.3.1/reportportal_client/static/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client/steps/__init__.py` & `reportportal-client-5.3.1/reportportal_client/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/reportportal_client.egg-info/SOURCES.txt` & `reportportal-client-5.3.1/reportportal_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 reportportal_client/__init__.py
 reportportal_client/client.py
+reportportal_client/client.pyi
 reportportal_client/errors.py
 reportportal_client/helpers.py
+reportportal_client/helpers.pyi
 reportportal_client.egg-info/PKG-INFO
 reportportal_client.egg-info/SOURCES.txt
 reportportal_client.egg-info/dependency_links.txt
 reportportal_client.egg-info/requires.txt
 reportportal_client.egg-info/top_level.txt
 reportportal_client/_local/__init__.py
 reportportal_client/core/__init__.py
@@ -31,17 +33,20 @@
 reportportal_client/items/rp_test_items/__init__.py
 reportportal_client/items/rp_test_items/rp_base_test_item.py
 reportportal_client/items/rp_test_items/rp_child_test_item.py
 reportportal_client/items/rp_test_items/rp_root_test_item.py
 reportportal_client/logs/__init__.py
 reportportal_client/logs/log_manager.py
 reportportal_client/services/__init__.py
+reportportal_client/services/client_id.py
 reportportal_client/services/constants.py
 reportportal_client/services/statistics.py
 reportportal_client/static/__init__.py
 reportportal_client/static/abstract.py
 reportportal_client/static/defines.py
 reportportal_client/static/errors.py
 reportportal_client/steps/__init__.py
+reportportal_client/steps/__init__.pyi
 tests/test_client.py
+tests/test_client_id.py
 tests/test_helpers.py
 tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.0/setup.py` & `reportportal-client-5.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Config for setup package client Python."""
 
 import os
+
 from setuptools import setup, find_packages
 
-__version__ = '5.3.0'
+__version__ = '5.3.1'
+
+TYPE_STUBS = ['*.pyi']
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
@@ -15,18 +18,23 @@
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name='reportportal-client',
     packages=find_packages(exclude=('tests', 'tests.*')),
+    package_data={
+        'reportportal_client': TYPE_STUBS,
+        'reportportal_client.steps': TYPE_STUBS
+    },
     version=__version__,
     description='Python client for Report Portal v5.',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
+    author='Report Portal Team',
     author_email='support@reportportal.io',
     url='https://github.com/reportportal/client-Python',
     download_url=('https://github.com/reportportal/client-Python/'
                   'tarball/%s' % __version__),
     license='Apache 2.0.',
     keywords=['testing', 'reporting', 'reportportal', 'client'],
     classifiers=[
```

### Comparing `reportportal-client-5.3.0/tests/test_client.py` & `reportportal-client-5.3.1/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import pytest
 from requests import Response
 from requests.exceptions import ReadTimeout
 from six.moves import mock
 
 from reportportal_client.helpers import timestamp
+from reportportal_client import RPClient
 
 
 def connection_error(*args, **kwargs):
     raise ReadTimeout()
 
 
 def response_error(*args, **kwargs):
@@ -114,7 +115,27 @@
 
     def get_call(*args, **kwargs):
         return response
 
     rp_client.session.get.side_effect = get_call
 
     assert rp_client.get_launch_ui_url() == expected_url
+
+
+@mock.patch('reportportal_client.client.getenv')
+@mock.patch('reportportal_client.client.send_event')
+def test_skip_analytics(send_event, getenv):
+    getenv.return_value = '1'
+    client = RPClient('http://endpoint', 'project', 'token')
+    client.session = mock.Mock()
+    client.start_launch('Test Launch', timestamp())
+    assert mock.call('start_launch', None, None) not in send_event.mock_calls
+
+
+@mock.patch('reportportal_client.client.getenv')
+@mock.patch('reportportal_client.client.send_event')
+def test_analytics(send_event, getenv):
+    getenv.return_value = ''
+    client = RPClient('http://endpoint', 'project', 'token')
+    client.session = mock.Mock()
+    client.start_launch('Test Launch', timestamp())
+    assert mock.call('start_launch', None, None) in send_event.mock_calls
```

### Comparing `reportportal-client-5.3.0/tests/test_helpers.py` & `reportportal-client-5.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.0/tests/test_statistics.py` & `reportportal-client-5.3.1/tests/test_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,22 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 from requests.exceptions import RequestException
 # noinspection PyUnresolvedReferences
 from six.moves import mock
 
-from reportportal_client.services.constants import ENDPOINT, CLIENT_INFO, \
-    CLIENT_ID_PROPERTY
+from reportportal_client.services.constants import ENDPOINT, CLIENT_INFO
 from reportportal_client.services.statistics import send_event
 
 EVENT_NAME = 'start_launch'
 
 
-@mock.patch('reportportal_client.services.statistics.uuid4',
-            mock.Mock(return_value=555))
-@mock.patch('reportportal_client.services.statistics._load_properties',
-            mock.Mock(return_value={CLIENT_ID_PROPERTY: '555'}))
+@mock.patch('reportportal_client.services.statistics.get_client_id',
+            mock.Mock(return_value='555'))
 @mock.patch('reportportal_client.services.statistics.requests.post')
 @mock.patch('reportportal_client.services.statistics.get_distribution')
 @mock.patch('reportportal_client.services.statistics.python_version',
             mock.Mock(return_value='3.6.6'))
 def test_send_event(mocked_distribution, mocked_requests):
     """Test functionality of the send_event() function.
 
@@ -62,16 +59,16 @@
     expected_params = {'measurement_id': mid, 'api_secret': key}
     send_event(EVENT_NAME, agent_name, agent_version)
     mocked_requests.assert_called_with(
         url=ENDPOINT, json=expected_data, headers=expected_headers,
         params=expected_params)
 
 
-@mock.patch('reportportal_client.services.statistics.uuid4',
-            mock.Mock(return_value=555))
+@mock.patch('reportportal_client.services.statistics.get_client_id',
+            mock.Mock(return_value='555'))
 @mock.patch('reportportal_client.services.statistics.requests.post',
             mock.Mock(side_effect=RequestException))
 @mock.patch('reportportal_client.services.statistics.get_distribution',
             mock.Mock())
 def test_send_event_raises():
     """Test that the send_event() does not raise exceptions."""
     send_event(EVENT_NAME, 'pytest-reportportal', '5.0.5')
@@ -92,9 +89,11 @@
     mocked_distribution.return_value.version = expected_cl_version
     mocked_distribution.return_value.project_name = expected_cl_name
 
     send_event(EVENT_NAME, agent_name, agent_version)
     send_event(EVENT_NAME, agent_name, agent_version)
     args_list = mocked_requests.call_args_list
 
-    assert args_list[0][1]['json']['client_id'] == \
-           args_list[1][1]['json']['client_id']
+    result1 = args_list[0][1]['json']['client_id']
+    result2 = args_list[1][1]['json']['client_id']
+
+    assert result1 == result2
```

