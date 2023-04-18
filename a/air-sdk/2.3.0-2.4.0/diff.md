# Comparing `tmp/air-sdk-2.3.0.tar.gz` & `tmp/air-sdk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air-sdk-2.3.0.tar", last modified: Thu Oct  6 14:46:35 2022, max compression
+gzip compressed data, was "air-sdk-2.4.0.tar", last modified: Tue Apr 18 15:21:00 2023, max compression
```

## Comparing `air-sdk-2.3.0.tar` & `air-sdk-2.4.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 mrobertson   (502) staff       (20)        0 2022-10-06 14:46:35.342383 air-sdk-2.3.0/
--rw-r--r--   0 mrobertson   (502) staff       (20)    14647 2022-09-30 12:14:05.000000 air-sdk-2.3.0/LICENSE
--rw-r--r--   0 mrobertson   (502) staff       (20)    19758 2022-10-06 14:46:35.341848 air-sdk-2.3.0/PKG-INFO
--rw-r--r--   0 mrobertson   (502) staff       (20)     2450 2022-09-30 12:14:05.000000 air-sdk-2.3.0/README.md
-drwxr-xr-x   0 mrobertson   (502) staff       (20)        0 2022-10-06 14:46:35.289365 air-sdk-2.3.0/air_sdk/
--rw-r--r--   0 mrobertson   (502) staff       (20)      196 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/__init__.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2539 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/account.py
--rw-r--r--   0 mrobertson   (502) staff       (20)    10854 2022-10-06 14:40:42.000000 air-sdk-2.3.0/air_sdk/air_api.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     7903 2022-10-06 14:40:42.000000 air-sdk-2.3.0/air_sdk/air_model.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     1988 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/capacity.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2401 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/demo.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     1800 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/exceptions.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4515 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/image.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2532 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/interface.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2571 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/job.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3732 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/link.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2089 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/login.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2369 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/marketplace.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4068 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/node.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     7426 2022-10-06 14:40:42.000000 air-sdk-2.3.0/air_sdk/organization.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4623 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/permission.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6080 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/service.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     9860 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/simulation.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3350 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/simulation_interface.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6790 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/simulation_node.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2794 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/ssh_key.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3400 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/token.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6106 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/topology.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3474 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/util.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4825 2022-09-30 12:14:05.000000 air-sdk-2.3.0/air_sdk/worker.py
-drwxr-xr-x   0 mrobertson   (502) staff       (20)        0 2022-10-06 14:46:35.296684 air-sdk-2.3.0/air_sdk.egg-info/
--rw-r--r--   0 mrobertson   (502) staff       (20)    19758 2022-10-06 14:46:35.000000 air-sdk-2.3.0/air_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mrobertson   (502) staff       (20)     1141 2022-10-06 14:46:35.000000 air-sdk-2.3.0/air_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mrobertson   (502) staff       (20)        1 2022-10-06 14:46:35.000000 air-sdk-2.3.0/air_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mrobertson   (502) staff       (20)       25 2022-10-06 14:46:35.000000 air-sdk-2.3.0/air_sdk.egg-info/requires.txt
--rw-r--r--   0 mrobertson   (502) staff       (20)       14 2022-10-06 14:46:35.000000 air-sdk-2.3.0/air_sdk.egg-info/top_level.txt
--rw-r--r--   0 mrobertson   (502) staff       (20)      622 2022-10-06 14:41:04.000000 air-sdk-2.3.0/pyproject.toml
--rw-r--r--   0 mrobertson   (502) staff       (20)       38 2022-10-06 14:46:35.342610 air-sdk-2.3.0/setup.cfg
--rw-r--r--   0 mrobertson   (502) staff       (20)      880 2022-10-06 14:41:04.000000 air-sdk-2.3.0/setup.py
-drwxr-xr-x   0 mrobertson   (502) staff       (20)        0 2022-10-06 14:46:35.340166 air-sdk-2.3.0/tests/
--rw-r--r--   0 mrobertson   (502) staff       (20)        0 2022-07-08 13:12:46.000000 air-sdk-2.3.0/tests/__init__.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2122 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/account.py
--rw-r--r--   0 mrobertson   (502) staff       (20)    17120 2022-10-06 14:40:42.000000 air-sdk-2.3.0/tests/air_api.py
--rw-r--r--   0 mrobertson   (502) staff       (20)    12526 2022-10-06 14:40:42.000000 air-sdk-2.3.0/tests/air_model.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2885 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/capacity.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2302 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/demo.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2551 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/exceptions.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4645 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/image.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2421 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/interface.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2290 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/job.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3298 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/link.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     1835 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/login.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2502 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/marketplace.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3993 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/node.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6583 2022-10-06 14:40:42.000000 air-sdk-2.3.0/tests/organization.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3765 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/permission.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6787 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/service.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     9626 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/simulation.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3204 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/simulation_interface.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6535 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/simulation_node.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     2759 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/ssh_key.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     3317 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/token.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     6730 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/topology.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     4538 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/util.py
--rw-r--r--   0 mrobertson   (502) staff       (20)     5959 2022-09-30 12:14:05.000000 air-sdk-2.3.0/tests/worker.py
+drwxr-xr-x   0 nmitchell   (502) staff       (20)        0 2023-04-18 15:21:00.680835 air-sdk-2.4.0/
+-rw-r--r--   0 nmitchell   (502) staff       (20)    14657 2023-04-18 15:16:13.000000 air-sdk-2.4.0/LICENSE
+-rw-r--r--   0 nmitchell   (502) staff       (20)    19768 2023-04-18 15:21:00.680629 air-sdk-2.4.0/PKG-INFO
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2450 2022-12-08 17:34:42.000000 air-sdk-2.4.0/README.md
+drwxr-xr-x   0 nmitchell   (502) staff       (20)        0 2023-04-18 15:21:00.675537 air-sdk-2.4.0/air_sdk/
+-rw-r--r--   0 nmitchell   (502) staff       (20)      201 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/__init__.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2544 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/account.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)    10992 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/air_api.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     7908 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/air_model.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     1993 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/capacity.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2406 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/demo.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     1805 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/exceptions.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     5400 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/image.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2537 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/interface.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2576 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/job.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3737 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/link.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2094 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/login.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2374 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/marketplace.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     4073 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/node.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     7431 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/organization.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     4628 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/permission.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2738 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/resource_budget.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6085 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/service.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     9865 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/simulation.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3355 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/simulation_interface.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6795 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/simulation_node.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2799 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/ssh_key.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3405 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/token.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6111 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/topology.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3479 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/util.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     4830 2023-04-18 15:16:13.000000 air-sdk-2.4.0/air_sdk/worker.py
+drwxr-xr-x   0 nmitchell   (502) staff       (20)        0 2023-04-18 15:21:00.676286 air-sdk-2.4.0/air_sdk.egg-info/
+-rw-r--r--   0 nmitchell   (502) staff       (20)    19768 2023-04-18 15:21:00.000000 air-sdk-2.4.0/air_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nmitchell   (502) staff       (20)     1193 2023-04-18 15:21:00.000000 air-sdk-2.4.0/air_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nmitchell   (502) staff       (20)        1 2023-04-18 15:21:00.000000 air-sdk-2.4.0/air_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nmitchell   (502) staff       (20)       25 2023-04-18 15:21:00.000000 air-sdk-2.4.0/air_sdk.egg-info/requires.txt
+-rw-r--r--   0 nmitchell   (502) staff       (20)       14 2023-04-18 15:21:00.000000 air-sdk-2.4.0/air_sdk.egg-info/top_level.txt
+-rw-r--r--   0 nmitchell   (502) staff       (20)      622 2023-04-18 15:18:40.000000 air-sdk-2.4.0/pyproject.toml
+-rw-r--r--   0 nmitchell   (502) staff       (20)       38 2023-04-18 15:21:00.680879 air-sdk-2.4.0/setup.cfg
+-rw-r--r--   0 nmitchell   (502) staff       (20)      885 2023-04-18 15:18:35.000000 air-sdk-2.4.0/setup.py
+drwxr-xr-x   0 nmitchell   (502) staff       (20)        0 2023-04-18 15:21:00.680371 air-sdk-2.4.0/tests/
+-rw-r--r--   0 nmitchell   (502) staff       (20)        0 2023-01-10 19:31:32.000000 air-sdk-2.4.0/tests/__init__.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2127 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/account.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)    17295 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/air_api.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)    12531 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/air_model.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2890 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/capacity.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2307 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/demo.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2556 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/exceptions.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     5356 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/image.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2426 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/interface.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2295 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/job.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3303 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/link.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     1840 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/login.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2507 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/marketplace.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3998 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/node.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6588 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/organization.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3770 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/permission.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2453 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/resource_budget.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6792 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/service.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     9631 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/simulation.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3209 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/simulation_interface.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6540 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/simulation_node.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     2764 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/ssh_key.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     3322 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/token.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     6735 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/topology.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     4543 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/util.py
+-rw-r--r--   0 nmitchell   (502) staff       (20)     5964 2023-04-18 15:16:13.000000 air-sdk-2.4.0/tests/worker.py
```

### Comparing `air-sdk-2.3.0/LICENSE` & `air-sdk-2.4.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,916 +1,917 @@
 00000000: 5350 4458 2d46 696c 6543 6f70 7972 6967  SPDX-FileCopyrig
 00000010: 6874 5465 7874 3a20 436f 7079 7269 6768  htText: Copyrigh
-00000020: 7420 2863 2920 3230 3232 204e 5649 4449  t (c) 2022 NVIDI
-00000030: 4120 434f 5250 4f52 4154 494f 4e20 2620  A CORPORATION & 
-00000040: 4146 4649 4c49 4154 4553 2e20 416c 6c20  AFFILIATES. All 
-00000050: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-00000060: 0a53 5044 582d 4c69 6365 6e73 652d 4964  .SPDX-License-Id
-00000070: 656e 7469 6669 6572 3a20 4d49 540a 0a43  entifier: MIT..C
-00000080: 6f70 7972 6967 6874 2028 6329 2032 3032  opyright (c) 202
-00000090: 322c 204e 5649 4449 4120 434f 5250 4f52  2, NVIDIA CORPOR
-000000a0: 4154 494f 4e20 2620 4146 4649 4c49 4154  ATION & AFFILIAT
-000000b0: 4553 2e20 416c 6c20 7269 6768 7473 2072  ES. All rights r
-000000c0: 6573 6572 7665 642e 0a0a 5065 726d 6973  eserved...Permis
-000000d0: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
-000000e0: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
-000000f0: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
-00000100: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
-00000110: 610a 636f 7079 206f 6620 7468 6973 2073  a.copy of this s
-00000120: 6f66 7477 6172 6520 616e 6420 6173 736f  oftware and asso
-00000130: 6369 6174 6564 2064 6f63 756d 656e 7461  ciated documenta
-00000140: 7469 6f6e 2066 696c 6573 2028 7468 6520  tion files (the 
-00000150: 2253 6f66 7477 6172 6522 292c 0a74 6f20  "Software"),.to 
-00000160: 6465 616c 2069 6e20 7468 6520 536f 6674  deal in the Soft
-00000170: 7761 7265 2077 6974 686f 7574 2072 6573  ware without res
-00000180: 7472 6963 7469 6f6e 2c20 696e 636c 7564  triction, includ
-00000190: 696e 6720 7769 7468 6f75 7420 6c69 6d69  ing without limi
-000001a0: 7461 7469 6f6e 0a74 6865 2072 6967 6874  tation.the right
-000001b0: 7320 746f 2075 7365 2c20 636f 7079 2c20  s to use, copy, 
-000001c0: 6d6f 6469 6679 2c20 6d65 7267 652c 2070  modify, merge, p
-000001d0: 7562 6c69 7368 2c20 6469 7374 7269 6275  ublish, distribu
-000001e0: 7465 2c20 7375 626c 6963 656e 7365 2c0a  te, sublicense,.
-000001f0: 616e 642f 6f72 2073 656c 6c20 636f 7069  and/or sell copi
-00000200: 6573 206f 6620 7468 6520 536f 6674 7761  es of the Softwa
-00000210: 7265 2c20 616e 6420 746f 2070 6572 6d69  re, and to permi
-00000220: 7420 7065 7273 6f6e 7320 746f 2077 686f  t persons to who
-00000230: 6d20 7468 650a 536f 6674 7761 7265 2069  m the.Software i
-00000240: 7320 6675 726e 6973 6865 6420 746f 2064  s furnished to d
-00000250: 6f20 736f 2c20 7375 626a 6563 7420 746f  o so, subject to
-00000260: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000270: 6f6e 6469 7469 6f6e 733a 0a0a 5468 6520  onditions:..The 
-00000280: 6162 6f76 6520 636f 7079 7269 6768 7420  above copyright 
-00000290: 6e6f 7469 6365 2061 6e64 2074 6869 7320  notice and this 
-000002a0: 7065 726d 6973 7369 6f6e 206e 6f74 6963  permission notic
-000002b0: 6520 7368 616c 6c20 6265 2069 6e63 6c75  e shall be inclu
-000002c0: 6465 6420 696e 0a61 6c6c 2063 6f70 6965  ded in.all copie
-000002d0: 7320 6f72 2073 7562 7374 616e 7469 616c  s or substantial
-000002e0: 2070 6f72 7469 6f6e 7320 6f66 2074 6865   portions of the
-000002f0: 2053 6f66 7477 6172 652e 0a0a 5448 4520   Software...THE 
-00000300: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
-00000310: 4944 4544 2022 4153 2049 5322 2c20 5749  IDED "AS IS", WI
-00000320: 5448 4f55 5420 5741 5252 414e 5459 204f  THOUT WARRANTY O
-00000330: 4620 414e 5920 4b49 4e44 2c20 4558 5052  F ANY KIND, EXPR
-00000340: 4553 5320 4f52 0a49 4d50 4c49 4544 2c20  ESS OR.IMPLIED, 
-00000350: 494e 434c 5544 494e 4720 4255 5420 4e4f  INCLUDING BUT NO
-00000360: 5420 4c49 4d49 5445 4420 544f 2054 4845  T LIMITED TO THE
-00000370: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
-00000380: 4552 4348 414e 5441 4249 4c49 5459 2c0a  ERCHANTABILITY,.
-00000390: 4649 544e 4553 5320 464f 5220 4120 5041  FITNESS FOR A PA
-000003a0: 5254 4943 554c 4152 2050 5552 504f 5345  RTICULAR PURPOSE
-000003b0: 2041 4e44 204e 4f4e 494e 4652 494e 4745   AND NONINFRINGE
-000003c0: 4d45 4e54 2e20 494e 204e 4f20 4556 454e  MENT. IN NO EVEN
-000003d0: 5420 5348 414c 4c0a 5448 4520 4155 5448  T SHALL.THE AUTH
-000003e0: 4f52 5320 4f52 2043 4f50 5952 4947 4854  ORS OR COPYRIGHT
-000003f0: 2048 4f4c 4445 5253 2042 4520 4c49 4142   HOLDERS BE LIAB
-00000400: 4c45 2046 4f52 2041 4e59 2043 4c41 494d  LE FOR ANY CLAIM
-00000410: 2c20 4441 4d41 4745 5320 4f52 204f 5448  , DAMAGES OR OTH
-00000420: 4552 0a4c 4941 4249 4c49 5459 2c20 5748  ER.LIABILITY, WH
-00000430: 4554 4845 5220 494e 2041 4e20 4143 5449  ETHER IN AN ACTI
-00000440: 4f4e 204f 4620 434f 4e54 5241 4354 2c20  ON OF CONTRACT, 
-00000450: 544f 5254 204f 5220 4f54 4845 5257 4953  TORT OR OTHERWIS
-00000460: 452c 2041 5249 5349 4e47 0a46 524f 4d2c  E, ARISING.FROM,
-00000470: 204f 5554 204f 4620 4f52 2049 4e20 434f   OUT OF OR IN CO
-00000480: 4e4e 4543 5449 4f4e 2057 4954 4820 5448  NNECTION WITH TH
-00000490: 4520 534f 4654 5741 5245 204f 5220 5448  E SOFTWARE OR TH
-000004a0: 4520 5553 4520 4f52 204f 5448 4552 0a44  E USE OR OTHER.D
-000004b0: 4541 4c49 4e47 5320 494e 2054 4845 2053  EALINGS IN THE S
-000004c0: 4f46 5457 4152 452e 0a0a 506f 7274 696f  OFTWARE...Portio
-000004d0: 6e73 2070 726f 7669 6465 6420 756e 6465  ns provided unde
-000004e0: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
-000004f0: 7465 726d 733a 0a2d 2d2d 2d2d 2d2d 2d2d  terms:.---------
-00000500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000020: 7420 2863 2920 3230 3232 2d32 3032 3320  t (c) 2022-2023 
+00000030: 4e56 4944 4941 2043 4f52 504f 5241 5449  NVIDIA CORPORATI
+00000040: 4f4e 2026 2041 4646 494c 4941 5445 532e  ON & AFFILIATES.
+00000050: 2041 6c6c 2072 6967 6874 7320 7265 7365   All rights rese
+00000060: 7276 6564 2e0a 5350 4458 2d4c 6963 656e  rved..SPDX-Licen
+00000070: 7365 2d49 6465 6e74 6966 6965 723a 204d  se-Identifier: M
+00000080: 4954 0a0a 436f 7079 7269 6768 7420 2863  IT..Copyright (c
+00000090: 2920 3230 3232 2d32 3032 332c 204e 5649  ) 2022-2023, NVI
+000000a0: 4449 4120 434f 5250 4f52 4154 494f 4e20  DIA CORPORATION 
+000000b0: 2620 4146 4649 4c49 4154 4553 2e20 416c  & AFFILIATES. Al
+000000c0: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
+000000d0: 642e 0a0a 5065 726d 6973 7369 6f6e 2069  d...Permission i
+000000e0: 7320 6865 7265 6279 2067 7261 6e74 6564  s hereby granted
+000000f0: 2c20 6672 6565 206f 6620 6368 6172 6765  , free of charge
+00000100: 2c20 746f 2061 6e79 2070 6572 736f 6e20  , to any person 
+00000110: 6f62 7461 696e 696e 6720 610a 636f 7079  obtaining a.copy
+00000120: 206f 6620 7468 6973 2073 6f66 7477 6172   of this softwar
+00000130: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
+00000140: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
+00000150: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
+00000160: 6172 6522 292c 0a74 6f20 6465 616c 2069  are"),.to deal i
+00000170: 6e20 7468 6520 536f 6674 7761 7265 2077  n the Software w
+00000180: 6974 686f 7574 2072 6573 7472 6963 7469  ithout restricti
+00000190: 6f6e 2c20 696e 636c 7564 696e 6720 7769  on, including wi
+000001a0: 7468 6f75 7420 6c69 6d69 7461 7469 6f6e  thout limitation
+000001b0: 0a74 6865 2072 6967 6874 7320 746f 2075  .the rights to u
+000001c0: 7365 2c20 636f 7079 2c20 6d6f 6469 6679  se, copy, modify
+000001d0: 2c20 6d65 7267 652c 2070 7562 6c69 7368  , merge, publish
+000001e0: 2c20 6469 7374 7269 6275 7465 2c20 7375  , distribute, su
+000001f0: 626c 6963 656e 7365 2c0a 616e 642f 6f72  blicense,.and/or
+00000200: 2073 656c 6c20 636f 7069 6573 206f 6620   sell copies of 
+00000210: 7468 6520 536f 6674 7761 7265 2c20 616e  the Software, an
+00000220: 6420 746f 2070 6572 6d69 7420 7065 7273  d to permit pers
+00000230: 6f6e 7320 746f 2077 686f 6d20 7468 650a  ons to whom the.
+00000240: 536f 6674 7761 7265 2069 7320 6675 726e  Software is furn
+00000250: 6973 6865 6420 746f 2064 6f20 736f 2c20  ished to do so, 
+00000260: 7375 626a 6563 7420 746f 2074 6865 2066  subject to the f
+00000270: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
+00000280: 6f6e 733a 0a0a 5468 6520 6162 6f76 6520  ons:..The above 
+00000290: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
+000002a0: 2061 6e64 2074 6869 7320 7065 726d 6973   and this permis
+000002b0: 7369 6f6e 206e 6f74 6963 6520 7368 616c  sion notice shal
+000002c0: 6c20 6265 2069 6e63 6c75 6465 6420 696e  l be included in
+000002d0: 0a61 6c6c 2063 6f70 6965 7320 6f72 2073  .all copies or s
+000002e0: 7562 7374 616e 7469 616c 2070 6f72 7469  ubstantial porti
+000002f0: 6f6e 7320 6f66 2074 6865 2053 6f66 7477  ons of the Softw
+00000300: 6172 652e 0a0a 5448 4520 534f 4654 5741  are...THE SOFTWA
+00000310: 5245 2049 5320 5052 4f56 4944 4544 2022  RE IS PROVIDED "
+00000320: 4153 2049 5322 2c20 5749 5448 4f55 5420  AS IS", WITHOUT 
+00000330: 5741 5252 414e 5459 204f 4620 414e 5920  WARRANTY OF ANY 
+00000340: 4b49 4e44 2c20 4558 5052 4553 5320 4f52  KIND, EXPRESS OR
+00000350: 0a49 4d50 4c49 4544 2c20 494e 434c 5544  .IMPLIED, INCLUD
+00000360: 494e 4720 4255 5420 4e4f 5420 4c49 4d49  ING BUT NOT LIMI
+00000370: 5445 4420 544f 2054 4845 2057 4152 5241  TED TO THE WARRA
+00000380: 4e54 4945 5320 4f46 204d 4552 4348 414e  NTIES OF MERCHAN
+00000390: 5441 4249 4c49 5459 2c0a 4649 544e 4553  TABILITY,.FITNES
+000003a0: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
+000003b0: 4152 2050 5552 504f 5345 2041 4e44 204e  AR PURPOSE AND N
+000003c0: 4f4e 494e 4652 494e 4745 4d45 4e54 2e20  ONINFRINGEMENT. 
+000003d0: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
+000003e0: 4c0a 5448 4520 4155 5448 4f52 5320 4f52  L.THE AUTHORS OR
+000003f0: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
+00000400: 5253 2042 4520 4c49 4142 4c45 2046 4f52  RS BE LIABLE FOR
+00000410: 2041 4e59 2043 4c41 494d 2c20 4441 4d41   ANY CLAIM, DAMA
+00000420: 4745 5320 4f52 204f 5448 4552 0a4c 4941  GES OR OTHER.LIA
+00000430: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
+00000440: 494e 2041 4e20 4143 5449 4f4e 204f 4620  IN AN ACTION OF 
+00000450: 434f 4e54 5241 4354 2c20 544f 5254 204f  CONTRACT, TORT O
+00000460: 5220 4f54 4845 5257 4953 452c 2041 5249  R OTHERWISE, ARI
+00000470: 5349 4e47 0a46 524f 4d2c 204f 5554 204f  SING.FROM, OUT O
+00000480: 4620 4f52 2049 4e20 434f 4e4e 4543 5449  F OR IN CONNECTI
+00000490: 4f4e 2057 4954 4820 5448 4520 534f 4654  ON WITH THE SOFT
+000004a0: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
+000004b0: 4f52 204f 5448 4552 0a44 4541 4c49 4e47  OR OTHER.DEALING
+000004c0: 5320 494e 2054 4845 2053 4f46 5457 4152  S IN THE SOFTWAR
+000004d0: 452e 0a0a 506f 7274 696f 6e73 2070 726f  E...Portions pro
+000004e0: 7669 6465 6420 756e 6465 7220 7468 6520  vided under the 
+000004f0: 666f 6c6c 6f77 696e 6720 7465 726d 733a  following terms:
+00000500: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
 00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000540: 2d2d 2d2d 2d2d 2d0a 7265 7175 6573 7473  -------.requests
-00000550: 3a0a 436f 7079 7269 6768 7420 3230 3139  :.Copyright 2019
-00000560: 204b 656e 6e65 7468 2052 6569 747a 0a20   Kenneth Reitz. 
-00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000550: 2d0a 7265 7175 6573 7473 3a0a 436f 7079  -.requests:.Copy
+00000560: 7269 6768 7420 3230 3139 204b 656e 6e65  right 2019 Kenne
+00000570: 7468 2052 6569 747a 0a20 2020 2020 2020  th Reitz.       
 00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000590: 4170 6163 6865 204c 6963 656e 7365 0a20  Apache License. 
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 2020 2020 5665 7273 696f            Versio
-000005c0: 6e20 322e 302c 204a 616e 7561 7279 2032  n 2.0, January 2
-000005d0: 3030 340a 2020 2020 2020 2020 2020 2020  004.            
-000005e0: 2020 2020 2020 2020 2020 2020 6874 7470              http
-000005f0: 3a2f 2f77 7777 2e61 7061 6368 652e 6f72  ://www.apache.or
-00000600: 672f 6c69 6365 6e73 6573 2f0a 0a20 2020  g/licenses/..   
-00000610: 5445 524d 5320 414e 4420 434f 4e44 4954  TERMS AND CONDIT
-00000620: 494f 4e53 2046 4f52 2055 5345 2c20 5245  IONS FOR USE, RE
-00000630: 5052 4f44 5543 5449 4f4e 2c20 414e 4420  PRODUCTION, AND 
-00000640: 4449 5354 5249 4255 5449 4f4e 0a0a 2020  DISTRIBUTION..  
-00000650: 2031 2e20 4465 6669 6e69 7469 6f6e 732e   1. Definitions.
-00000660: 0a0a 2020 2020 2020 224c 6963 656e 7365  ..      "License
-00000670: 2220 7368 616c 6c20 6d65 616e 2074 6865  " shall mean the
-00000680: 2074 6572 6d73 2061 6e64 2063 6f6e 6469   terms and condi
-00000690: 7469 6f6e 7320 666f 7220 7573 652c 2072  tions for use, r
-000006a0: 6570 726f 6475 6374 696f 6e2c 0a20 2020  eproduction,.   
-000006b0: 2020 2061 6e64 2064 6973 7472 6962 7574     and distribut
-000006c0: 696f 6e20 6173 2064 6566 696e 6564 2062  ion as defined b
-000006d0: 7920 5365 6374 696f 6e73 2031 2074 6872  y Sections 1 thr
-000006e0: 6f75 6768 2039 206f 6620 7468 6973 2064  ough 9 of this d
-000006f0: 6f63 756d 656e 742e 0a0a 2020 2020 2020  ocument...      
-00000700: 224c 6963 656e 736f 7222 2073 6861 6c6c  "Licensor" shall
-00000710: 206d 6561 6e20 7468 6520 636f 7079 7269   mean the copyri
-00000720: 6768 7420 6f77 6e65 7220 6f72 2065 6e74  ght owner or ent
-00000730: 6974 7920 6175 7468 6f72 697a 6564 2062  ity authorized b
-00000740: 790a 2020 2020 2020 7468 6520 636f 7079  y.      the copy
-00000750: 7269 6768 7420 6f77 6e65 7220 7468 6174  right owner that
-00000760: 2069 7320 6772 616e 7469 6e67 2074 6865   is granting the
-00000770: 204c 6963 656e 7365 2e0a 0a20 2020 2020   License...     
-00000780: 2022 4c65 6761 6c20 456e 7469 7479 2220   "Legal Entity" 
-00000790: 7368 616c 6c20 6d65 616e 2074 6865 2075  shall mean the u
-000007a0: 6e69 6f6e 206f 6620 7468 6520 6163 7469  nion of the acti
-000007b0: 6e67 2065 6e74 6974 7920 616e 6420 616c  ng entity and al
-000007c0: 6c0a 2020 2020 2020 6f74 6865 7220 656e  l.      other en
-000007d0: 7469 7469 6573 2074 6861 7420 636f 6e74  tities that cont
-000007e0: 726f 6c2c 2061 7265 2063 6f6e 7472 6f6c  rol, are control
-000007f0: 6c65 6420 6279 2c20 6f72 2061 7265 2075  led by, or are u
-00000800: 6e64 6572 2063 6f6d 6d6f 6e0a 2020 2020  nder common.    
-00000810: 2020 636f 6e74 726f 6c20 7769 7468 2074    control with t
-00000820: 6861 7420 656e 7469 7479 2e20 466f 7220  hat entity. For 
-00000830: 7468 6520 7075 7270 6f73 6573 206f 6620  the purposes of 
-00000840: 7468 6973 2064 6566 696e 6974 696f 6e2c  this definition,
-00000850: 0a20 2020 2020 2022 636f 6e74 726f 6c22  .      "control"
-00000860: 206d 6561 6e73 2028 6929 2074 6865 2070   means (i) the p
-00000870: 6f77 6572 2c20 6469 7265 6374 206f 7220  ower, direct or 
-00000880: 696e 6469 7265 6374 2c20 746f 2063 6175  indirect, to cau
-00000890: 7365 2074 6865 0a20 2020 2020 2064 6972  se the.      dir
-000008a0: 6563 7469 6f6e 206f 7220 6d61 6e61 6765  ection or manage
-000008b0: 6d65 6e74 206f 6620 7375 6368 2065 6e74  ment of such ent
-000008c0: 6974 792c 2077 6865 7468 6572 2062 7920  ity, whether by 
-000008d0: 636f 6e74 7261 6374 206f 720a 2020 2020  contract or.    
-000008e0: 2020 6f74 6865 7277 6973 652c 206f 7220    otherwise, or 
-000008f0: 2869 6929 206f 776e 6572 7368 6970 206f  (ii) ownership o
-00000900: 6620 6669 6674 7920 7065 7263 656e 7420  f fifty percent 
-00000910: 2835 3025 2920 6f72 206d 6f72 6520 6f66  (50%) or more of
-00000920: 2074 6865 0a20 2020 2020 206f 7574 7374   the.      outst
-00000930: 616e 6469 6e67 2073 6861 7265 732c 206f  anding shares, o
-00000940: 7220 2869 6969 2920 6265 6e65 6669 6369  r (iii) benefici
-00000950: 616c 206f 776e 6572 7368 6970 206f 6620  al ownership of 
-00000960: 7375 6368 2065 6e74 6974 792e 0a0a 2020  such entity...  
-00000970: 2020 2020 2259 6f75 2220 286f 7220 2259      "You" (or "Y
-00000980: 6f75 7222 2920 7368 616c 6c20 6d65 616e  our") shall mean
-00000990: 2061 6e20 696e 6469 7669 6475 616c 206f   an individual o
-000009a0: 7220 4c65 6761 6c20 456e 7469 7479 0a20  r Legal Entity. 
-000009b0: 2020 2020 2065 7865 7263 6973 696e 6720       exercising 
-000009c0: 7065 726d 6973 7369 6f6e 7320 6772 616e  permissions gran
-000009d0: 7465 6420 6279 2074 6869 7320 4c69 6365  ted by this Lice
-000009e0: 6e73 652e 0a0a 2020 2020 2020 2253 6f75  nse...      "Sou
-000009f0: 7263 6522 2066 6f72 6d20 7368 616c 6c20  rce" form shall 
-00000a00: 6d65 616e 2074 6865 2070 7265 6665 7272  mean the preferr
-00000a10: 6564 2066 6f72 6d20 666f 7220 6d61 6b69  ed form for maki
-00000a20: 6e67 206d 6f64 6966 6963 6174 696f 6e73  ng modifications
-00000a30: 2c0a 2020 2020 2020 696e 636c 7564 696e  ,.      includin
-00000a40: 6720 6275 7420 6e6f 7420 6c69 6d69 7465  g but not limite
-00000a50: 6420 746f 2073 6f66 7477 6172 6520 736f  d to software so
-00000a60: 7572 6365 2063 6f64 652c 2064 6f63 756d  urce code, docum
-00000a70: 656e 7461 7469 6f6e 0a20 2020 2020 2073  entation.      s
-00000a80: 6f75 7263 652c 2061 6e64 2063 6f6e 6669  ource, and confi
-00000a90: 6775 7261 7469 6f6e 2066 696c 6573 2e0a  guration files..
-00000aa0: 0a20 2020 2020 2022 4f62 6a65 6374 2220  .      "Object" 
-00000ab0: 666f 726d 2073 6861 6c6c 206d 6561 6e20  form shall mean 
-00000ac0: 616e 7920 666f 726d 2072 6573 756c 7469  any form resulti
-00000ad0: 6e67 2066 726f 6d20 6d65 6368 616e 6963  ng from mechanic
-00000ae0: 616c 0a20 2020 2020 2074 7261 6e73 666f  al.      transfo
-00000af0: 726d 6174 696f 6e20 6f72 2074 7261 6e73  rmation or trans
-00000b00: 6c61 7469 6f6e 206f 6620 6120 536f 7572  lation of a Sour
-00000b10: 6365 2066 6f72 6d2c 2069 6e63 6c75 6469  ce form, includi
-00000b20: 6e67 2062 7574 0a20 2020 2020 206e 6f74  ng but.      not
-00000b30: 206c 696d 6974 6564 2074 6f20 636f 6d70   limited to comp
-00000b40: 696c 6564 206f 626a 6563 7420 636f 6465  iled object code
-00000b50: 2c20 6765 6e65 7261 7465 6420 646f 6375  , generated docu
-00000b60: 6d65 6e74 6174 696f 6e2c 0a20 2020 2020  mentation,.     
-00000b70: 2061 6e64 2063 6f6e 7665 7273 696f 6e73   and conversions
-00000b80: 2074 6f20 6f74 6865 7220 6d65 6469 6120   to other media 
-00000b90: 7479 7065 732e 0a0a 2020 2020 2020 2257  types...      "W
-00000ba0: 6f72 6b22 2073 6861 6c6c 206d 6561 6e20  ork" shall mean 
-00000bb0: 7468 6520 776f 726b 206f 6620 6175 7468  the work of auth
-00000bc0: 6f72 7368 6970 2c20 7768 6574 6865 7220  orship, whether 
-00000bd0: 696e 2053 6f75 7263 6520 6f72 0a20 2020  in Source or.   
-00000be0: 2020 204f 626a 6563 7420 666f 726d 2c20     Object form, 
-00000bf0: 6d61 6465 2061 7661 696c 6162 6c65 2075  made available u
-00000c00: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
-00000c10: 2c20 6173 2069 6e64 6963 6174 6564 2062  , as indicated b
-00000c20: 7920 610a 2020 2020 2020 636f 7079 7269  y a.      copyri
-00000c30: 6768 7420 6e6f 7469 6365 2074 6861 7420  ght notice that 
-00000c40: 6973 2069 6e63 6c75 6465 6420 696e 206f  is included in o
-00000c50: 7220 6174 7461 6368 6564 2074 6f20 7468  r attached to th
-00000c60: 6520 776f 726b 0a20 2020 2020 2028 616e  e work.      (an
-00000c70: 2065 7861 6d70 6c65 2069 7320 7072 6f76   example is prov
-00000c80: 6964 6564 2069 6e20 7468 6520 4170 7065  ided in the Appe
-00000c90: 6e64 6978 2062 656c 6f77 292e 0a0a 2020  ndix below)...  
-00000ca0: 2020 2020 2244 6572 6976 6174 6976 6520      "Derivative 
-00000cb0: 576f 726b 7322 2073 6861 6c6c 206d 6561  Works" shall mea
-00000cc0: 6e20 616e 7920 776f 726b 2c20 7768 6574  n any work, whet
-00000cd0: 6865 7220 696e 2053 6f75 7263 6520 6f72  her in Source or
-00000ce0: 204f 626a 6563 740a 2020 2020 2020 666f   Object.      fo
-00000cf0: 726d 2c20 7468 6174 2069 7320 6261 7365  rm, that is base
-00000d00: 6420 6f6e 2028 6f72 2064 6572 6976 6564  d on (or derived
-00000d10: 2066 726f 6d29 2074 6865 2057 6f72 6b20   from) the Work 
-00000d20: 616e 6420 666f 7220 7768 6963 6820 7468  and for which th
-00000d30: 650a 2020 2020 2020 6564 6974 6f72 6961  e.      editoria
-00000d40: 6c20 7265 7669 7369 6f6e 732c 2061 6e6e  l revisions, ann
-00000d50: 6f74 6174 696f 6e73 2c20 656c 6162 6f72  otations, elabor
-00000d60: 6174 696f 6e73 2c20 6f72 206f 7468 6572  ations, or other
-00000d70: 206d 6f64 6966 6963 6174 696f 6e73 0a20   modifications. 
-00000d80: 2020 2020 2072 6570 7265 7365 6e74 2c20       represent, 
-00000d90: 6173 2061 2077 686f 6c65 2c20 616e 206f  as a whole, an o
-00000da0: 7269 6769 6e61 6c20 776f 726b 206f 6620  riginal work of 
-00000db0: 6175 7468 6f72 7368 6970 2e20 466f 7220  authorship. For 
-00000dc0: 7468 6520 7075 7270 6f73 6573 0a20 2020  the purposes.   
-00000dd0: 2020 206f 6620 7468 6973 204c 6963 656e     of this Licen
-00000de0: 7365 2c20 4465 7269 7661 7469 7665 2057  se, Derivative W
-00000df0: 6f72 6b73 2073 6861 6c6c 206e 6f74 2069  orks shall not i
-00000e00: 6e63 6c75 6465 2077 6f72 6b73 2074 6861  nclude works tha
-00000e10: 7420 7265 6d61 696e 0a20 2020 2020 2073  t remain.      s
-00000e20: 6570 6172 6162 6c65 2066 726f 6d2c 206f  eparable from, o
-00000e30: 7220 6d65 7265 6c79 206c 696e 6b20 286f  r merely link (o
-00000e40: 7220 6269 6e64 2062 7920 6e61 6d65 2920  r bind by name) 
-00000e50: 746f 2074 6865 2069 6e74 6572 6661 6365  to the interface
-00000e60: 7320 6f66 2c0a 2020 2020 2020 7468 6520  s of,.      the 
-00000e70: 576f 726b 2061 6e64 2044 6572 6976 6174  Work and Derivat
-00000e80: 6976 6520 576f 726b 7320 7468 6572 656f  ive Works thereo
-00000e90: 662e 0a0a 2020 2020 2020 2243 6f6e 7472  f...      "Contr
-00000ea0: 6962 7574 696f 6e22 2073 6861 6c6c 206d  ibution" shall m
-00000eb0: 6561 6e20 616e 7920 776f 726b 206f 6620  ean any work of 
-00000ec0: 6175 7468 6f72 7368 6970 2c20 696e 636c  authorship, incl
-00000ed0: 7564 696e 670a 2020 2020 2020 7468 6520  uding.      the 
-00000ee0: 6f72 6967 696e 616c 2076 6572 7369 6f6e  original version
-00000ef0: 206f 6620 7468 6520 576f 726b 2061 6e64   of the Work and
-00000f00: 2061 6e79 206d 6f64 6966 6963 6174 696f   any modificatio
-00000f10: 6e73 206f 7220 6164 6469 7469 6f6e 730a  ns or additions.
-00000f20: 2020 2020 2020 746f 2074 6861 7420 576f        to that Wo
-00000f30: 726b 206f 7220 4465 7269 7661 7469 7665  rk or Derivative
-00000f40: 2057 6f72 6b73 2074 6865 7265 6f66 2c20   Works thereof, 
-00000f50: 7468 6174 2069 7320 696e 7465 6e74 696f  that is intentio
-00000f60: 6e61 6c6c 790a 2020 2020 2020 7375 626d  nally.      subm
-00000f70: 6974 7465 6420 746f 204c 6963 656e 736f  itted to Licenso
-00000f80: 7220 666f 7220 696e 636c 7573 696f 6e20  r for inclusion 
-00000f90: 696e 2074 6865 2057 6f72 6b20 6279 2074  in the Work by t
-00000fa0: 6865 2063 6f70 7972 6967 6874 206f 776e  he copyright own
-00000fb0: 6572 0a20 2020 2020 206f 7220 6279 2061  er.      or by a
-00000fc0: 6e20 696e 6469 7669 6475 616c 206f 7220  n individual or 
-00000fd0: 4c65 6761 6c20 456e 7469 7479 2061 7574  Legal Entity aut
-00000fe0: 686f 7269 7a65 6420 746f 2073 7562 6d69  horized to submi
-00000ff0: 7420 6f6e 2062 6568 616c 6620 6f66 0a20  t on behalf of. 
-00001000: 2020 2020 2074 6865 2063 6f70 7972 6967       the copyrig
-00001010: 6874 206f 776e 6572 2e20 466f 7220 7468  ht owner. For th
-00001020: 6520 7075 7270 6f73 6573 206f 6620 7468  e purposes of th
-00001030: 6973 2064 6566 696e 6974 696f 6e2c 2022  is definition, "
-00001040: 7375 626d 6974 7465 6422 0a20 2020 2020  submitted".     
-00001050: 206d 6561 6e73 2061 6e79 2066 6f72 6d20   means any form 
-00001060: 6f66 2065 6c65 6374 726f 6e69 632c 2076  of electronic, v
-00001070: 6572 6261 6c2c 206f 7220 7772 6974 7465  erbal, or writte
-00001080: 6e20 636f 6d6d 756e 6963 6174 696f 6e20  n communication 
-00001090: 7365 6e74 0a20 2020 2020 2074 6f20 7468  sent.      to th
-000010a0: 6520 4c69 6365 6e73 6f72 206f 7220 6974  e Licensor or it
-000010b0: 7320 7265 7072 6573 656e 7461 7469 7665  s representative
-000010c0: 732c 2069 6e63 6c75 6469 6e67 2062 7574  s, including but
-000010d0: 206e 6f74 206c 696d 6974 6564 2074 6f0a   not limited to.
-000010e0: 2020 2020 2020 636f 6d6d 756e 6963 6174        communicat
-000010f0: 696f 6e20 6f6e 2065 6c65 6374 726f 6e69  ion on electroni
-00001100: 6320 6d61 696c 696e 6720 6c69 7374 732c  c mailing lists,
-00001110: 2073 6f75 7263 6520 636f 6465 2063 6f6e   source code con
-00001120: 7472 6f6c 2073 7973 7465 6d73 2c0a 2020  trol systems,.  
-00001130: 2020 2020 616e 6420 6973 7375 6520 7472      and issue tr
-00001140: 6163 6b69 6e67 2073 7973 7465 6d73 2074  acking systems t
-00001150: 6861 7420 6172 6520 6d61 6e61 6765 6420  hat are managed 
-00001160: 6279 2c20 6f72 206f 6e20 6265 6861 6c66  by, or on behalf
-00001170: 206f 662c 2074 6865 0a20 2020 2020 204c   of, the.      L
-00001180: 6963 656e 736f 7220 666f 7220 7468 6520  icensor for the 
-00001190: 7075 7270 6f73 6520 6f66 2064 6973 6375  purpose of discu
-000011a0: 7373 696e 6720 616e 6420 696d 7072 6f76  ssing and improv
-000011b0: 696e 6720 7468 6520 576f 726b 2c20 6275  ing the Work, bu
-000011c0: 740a 2020 2020 2020 6578 636c 7564 696e  t.      excludin
-000011d0: 6720 636f 6d6d 756e 6963 6174 696f 6e20  g communication 
-000011e0: 7468 6174 2069 7320 636f 6e73 7069 6375  that is conspicu
-000011f0: 6f75 736c 7920 6d61 726b 6564 206f 7220  ously marked or 
-00001200: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
-00001210: 6465 7369 676e 6174 6564 2069 6e20 7772  designated in wr
-00001220: 6974 696e 6720 6279 2074 6865 2063 6f70  iting by the cop
-00001230: 7972 6967 6874 206f 776e 6572 2061 7320  yright owner as 
-00001240: 224e 6f74 2061 2043 6f6e 7472 6962 7574  "Not a Contribut
-00001250: 696f 6e2e 220a 0a20 2020 2020 2022 436f  ion."..      "Co
-00001260: 6e74 7269 6275 746f 7222 2073 6861 6c6c  ntributor" shall
-00001270: 206d 6561 6e20 4c69 6365 6e73 6f72 2061   mean Licensor a
-00001280: 6e64 2061 6e79 2069 6e64 6976 6964 7561  nd any individua
-00001290: 6c20 6f72 204c 6567 616c 2045 6e74 6974  l or Legal Entit
-000012a0: 790a 2020 2020 2020 6f6e 2062 6568 616c  y.      on behal
-000012b0: 6620 6f66 2077 686f 6d20 6120 436f 6e74  f of whom a Cont
-000012c0: 7269 6275 7469 6f6e 2068 6173 2062 6565  ribution has bee
-000012d0: 6e20 7265 6365 6976 6564 2062 7920 4c69  n received by Li
-000012e0: 6365 6e73 6f72 2061 6e64 0a20 2020 2020  censor and.     
-000012f0: 2073 7562 7365 7175 656e 746c 7920 696e   subsequently in
-00001300: 636f 7270 6f72 6174 6564 2077 6974 6869  corporated withi
-00001310: 6e20 7468 6520 576f 726b 2e0a 0a20 2020  n the Work...   
-00001320: 322e 2047 7261 6e74 206f 6620 436f 7079  2. Grant of Copy
-00001330: 7269 6768 7420 4c69 6365 6e73 652e 2053  right License. S
-00001340: 7562 6a65 6374 2074 6f20 7468 6520 7465  ubject to the te
-00001350: 726d 7320 616e 6420 636f 6e64 6974 696f  rms and conditio
-00001360: 6e73 206f 660a 2020 2020 2020 7468 6973  ns of.      this
-00001370: 204c 6963 656e 7365 2c20 6561 6368 2043   License, each C
-00001380: 6f6e 7472 6962 7574 6f72 2068 6572 6562  ontributor hereb
-00001390: 7920 6772 616e 7473 2074 6f20 596f 7520  y grants to You 
-000013a0: 6120 7065 7270 6574 7561 6c2c 0a20 2020  a perpetual,.   
-000013b0: 2020 2077 6f72 6c64 7769 6465 2c20 6e6f     worldwide, no
-000013c0: 6e2d 6578 636c 7573 6976 652c 206e 6f2d  n-exclusive, no-
-000013d0: 6368 6172 6765 2c20 726f 7961 6c74 792d  charge, royalty-
-000013e0: 6672 6565 2c20 6972 7265 766f 6361 626c  free, irrevocabl
-000013f0: 650a 2020 2020 2020 636f 7079 7269 6768  e.      copyrigh
-00001400: 7420 6c69 6365 6e73 6520 746f 2072 6570  t license to rep
-00001410: 726f 6475 6365 2c20 7072 6570 6172 6520  roduce, prepare 
-00001420: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
-00001430: 206f 662c 0a20 2020 2020 2070 7562 6c69   of,.      publi
-00001440: 636c 7920 6469 7370 6c61 792c 2070 7562  cly display, pub
-00001450: 6c69 636c 7920 7065 7266 6f72 6d2c 2073  licly perform, s
-00001460: 7562 6c69 6365 6e73 652c 2061 6e64 2064  ublicense, and d
-00001470: 6973 7472 6962 7574 6520 7468 650a 2020  istribute the.  
-00001480: 2020 2020 576f 726b 2061 6e64 2073 7563      Work and suc
-00001490: 6820 4465 7269 7661 7469 7665 2057 6f72  h Derivative Wor
-000014a0: 6b73 2069 6e20 536f 7572 6365 206f 7220  ks in Source or 
-000014b0: 4f62 6a65 6374 2066 6f72 6d2e 0a0a 2020  Object form...  
-000014c0: 2033 2e20 4772 616e 7420 6f66 2050 6174   3. Grant of Pat
-000014d0: 656e 7420 4c69 6365 6e73 652e 2053 7562  ent License. Sub
-000014e0: 6a65 6374 2074 6f20 7468 6520 7465 726d  ject to the term
-000014f0: 7320 616e 6420 636f 6e64 6974 696f 6e73  s and conditions
-00001500: 206f 660a 2020 2020 2020 7468 6973 204c   of.      this L
-00001510: 6963 656e 7365 2c20 6561 6368 2043 6f6e  icense, each Con
-00001520: 7472 6962 7574 6f72 2068 6572 6562 7920  tributor hereby 
-00001530: 6772 616e 7473 2074 6f20 596f 7520 6120  grants to You a 
-00001540: 7065 7270 6574 7561 6c2c 0a20 2020 2020  perpetual,.     
-00001550: 2077 6f72 6c64 7769 6465 2c20 6e6f 6e2d   worldwide, non-
-00001560: 6578 636c 7573 6976 652c 206e 6f2d 6368  exclusive, no-ch
-00001570: 6172 6765 2c20 726f 7961 6c74 792d 6672  arge, royalty-fr
-00001580: 6565 2c20 6972 7265 766f 6361 626c 650a  ee, irrevocable.
-00001590: 2020 2020 2020 2865 7863 6570 7420 6173        (except as
-000015a0: 2073 7461 7465 6420 696e 2074 6869 7320   stated in this 
-000015b0: 7365 6374 696f 6e29 2070 6174 656e 7420  section) patent 
-000015c0: 6c69 6365 6e73 6520 746f 206d 616b 652c  license to make,
-000015d0: 2068 6176 6520 6d61 6465 2c0a 2020 2020   have made,.    
-000015e0: 2020 7573 652c 206f 6666 6572 2074 6f20    use, offer to 
-000015f0: 7365 6c6c 2c20 7365 6c6c 2c20 696d 706f  sell, sell, impo
-00001600: 7274 2c20 616e 6420 6f74 6865 7277 6973  rt, and otherwis
-00001610: 6520 7472 616e 7366 6572 2074 6865 2057  e transfer the W
-00001620: 6f72 6b2c 0a20 2020 2020 2077 6865 7265  ork,.      where
-00001630: 2073 7563 6820 6c69 6365 6e73 6520 6170   such license ap
-00001640: 706c 6965 7320 6f6e 6c79 2074 6f20 7468  plies only to th
-00001650: 6f73 6520 7061 7465 6e74 2063 6c61 696d  ose patent claim
-00001660: 7320 6c69 6365 6e73 6162 6c65 0a20 2020  s licensable.   
-00001670: 2020 2062 7920 7375 6368 2043 6f6e 7472     by such Contr
-00001680: 6962 7574 6f72 2074 6861 7420 6172 6520  ibutor that are 
-00001690: 6e65 6365 7373 6172 696c 7920 696e 6672  necessarily infr
-000016a0: 696e 6765 6420 6279 2074 6865 6972 0a20  inged by their. 
-000016b0: 2020 2020 2043 6f6e 7472 6962 7574 696f       Contributio
-000016c0: 6e28 7329 2061 6c6f 6e65 206f 7220 6279  n(s) alone or by
-000016d0: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
-000016e0: 7468 6569 7220 436f 6e74 7269 6275 7469  their Contributi
-000016f0: 6f6e 2873 290a 2020 2020 2020 7769 7468  on(s).      with
-00001700: 2074 6865 2057 6f72 6b20 746f 2077 6869   the Work to whi
-00001710: 6368 2073 7563 6820 436f 6e74 7269 6275  ch such Contribu
-00001720: 7469 6f6e 2873 2920 7761 7320 7375 626d  tion(s) was subm
-00001730: 6974 7465 642e 2049 6620 596f 750a 2020  itted. If You.  
-00001740: 2020 2020 696e 7374 6974 7574 6520 7061      institute pa
-00001750: 7465 6e74 206c 6974 6967 6174 696f 6e20  tent litigation 
-00001760: 6167 6169 6e73 7420 616e 7920 656e 7469  against any enti
-00001770: 7479 2028 696e 636c 7564 696e 6720 610a  ty (including a.
-00001780: 2020 2020 2020 6372 6f73 732d 636c 6169        cross-clai
-00001790: 6d20 6f72 2063 6f75 6e74 6572 636c 6169  m or counterclai
-000017a0: 6d20 696e 2061 206c 6177 7375 6974 2920  m in a lawsuit) 
-000017b0: 616c 6c65 6769 6e67 2074 6861 7420 7468  alleging that th
-000017c0: 6520 576f 726b 0a20 2020 2020 206f 7220  e Work.      or 
-000017d0: 6120 436f 6e74 7269 6275 7469 6f6e 2069  a Contribution i
-000017e0: 6e63 6f72 706f 7261 7465 6420 7769 7468  ncorporated with
-000017f0: 696e 2074 6865 2057 6f72 6b20 636f 6e73  in the Work cons
-00001800: 7469 7475 7465 7320 6469 7265 6374 0a20  titutes direct. 
-00001810: 2020 2020 206f 7220 636f 6e74 7269 6275       or contribu
-00001820: 746f 7279 2070 6174 656e 7420 696e 6672  tory patent infr
-00001830: 696e 6765 6d65 6e74 2c20 7468 656e 2061  ingement, then a
-00001840: 6e79 2070 6174 656e 7420 6c69 6365 6e73  ny patent licens
-00001850: 6573 0a20 2020 2020 2067 7261 6e74 6564  es.      granted
-00001860: 2074 6f20 596f 7520 756e 6465 7220 7468   to You under th
-00001870: 6973 204c 6963 656e 7365 2066 6f72 2074  is License for t
-00001880: 6861 7420 576f 726b 2073 6861 6c6c 2074  hat Work shall t
-00001890: 6572 6d69 6e61 7465 0a20 2020 2020 2061  erminate.      a
-000018a0: 7320 6f66 2074 6865 2064 6174 6520 7375  s of the date su
-000018b0: 6368 206c 6974 6967 6174 696f 6e20 6973  ch litigation is
-000018c0: 2066 696c 6564 2e0a 0a20 2020 342e 2052   filed...   4. R
-000018d0: 6564 6973 7472 6962 7574 696f 6e2e 2059  edistribution. Y
-000018e0: 6f75 206d 6179 2072 6570 726f 6475 6365  ou may reproduce
-000018f0: 2061 6e64 2064 6973 7472 6962 7574 6520   and distribute 
-00001900: 636f 7069 6573 206f 6620 7468 650a 2020  copies of the.  
-00001910: 2020 2020 576f 726b 206f 7220 4465 7269      Work or Deri
-00001920: 7661 7469 7665 2057 6f72 6b73 2074 6865  vative Works the
-00001930: 7265 6f66 2069 6e20 616e 7920 6d65 6469  reof in any medi
-00001940: 756d 2c20 7769 7468 206f 7220 7769 7468  um, with or with
-00001950: 6f75 740a 2020 2020 2020 6d6f 6469 6669  out.      modifi
-00001960: 6361 7469 6f6e 732c 2061 6e64 2069 6e20  cations, and in 
-00001970: 536f 7572 6365 206f 7220 4f62 6a65 6374  Source or Object
-00001980: 2066 6f72 6d2c 2070 726f 7669 6465 6420   form, provided 
-00001990: 7468 6174 2059 6f75 0a20 2020 2020 206d  that You.      m
-000019a0: 6565 7420 7468 6520 666f 6c6c 6f77 696e  eet the followin
-000019b0: 6720 636f 6e64 6974 696f 6e73 3a0a 0a20  g conditions:.. 
-000019c0: 2020 2020 2028 6129 2059 6f75 206d 7573       (a) You mus
-000019d0: 7420 6769 7665 2061 6e79 206f 7468 6572  t give any other
-000019e0: 2072 6563 6970 6965 6e74 7320 6f66 2074   recipients of t
-000019f0: 6865 2057 6f72 6b20 6f72 0a20 2020 2020  he Work or.     
-00001a00: 2020 2020 2044 6572 6976 6174 6976 6520       Derivative 
-00001a10: 576f 726b 7320 6120 636f 7079 206f 6620  Works a copy of 
-00001a20: 7468 6973 204c 6963 656e 7365 3b20 616e  this License; an
-00001a30: 640a 0a20 2020 2020 2028 6229 2059 6f75  d..      (b) You
-00001a40: 206d 7573 7420 6361 7573 6520 616e 7920   must cause any 
-00001a50: 6d6f 6469 6669 6564 2066 696c 6573 2074  modified files t
-00001a60: 6f20 6361 7272 7920 7072 6f6d 696e 656e  o carry prominen
-00001a70: 7420 6e6f 7469 6365 730a 2020 2020 2020  t notices.      
-00001a80: 2020 2020 7374 6174 696e 6720 7468 6174      stating that
-00001a90: 2059 6f75 2063 6861 6e67 6564 2074 6865   You changed the
-00001aa0: 2066 696c 6573 3b20 616e 640a 0a20 2020   files; and..   
-00001ab0: 2020 2028 6329 2059 6f75 206d 7573 7420     (c) You must 
-00001ac0: 7265 7461 696e 2c20 696e 2074 6865 2053  retain, in the S
-00001ad0: 6f75 7263 6520 666f 726d 206f 6620 616e  ource form of an
-00001ae0: 7920 4465 7269 7661 7469 7665 2057 6f72  y Derivative Wor
-00001af0: 6b73 0a20 2020 2020 2020 2020 2074 6861  ks.          tha
-00001b00: 7420 596f 7520 6469 7374 7269 6275 7465  t You distribute
-00001b10: 2c20 616c 6c20 636f 7079 7269 6768 742c  , all copyright,
-00001b20: 2070 6174 656e 742c 2074 7261 6465 6d61   patent, tradema
-00001b30: 726b 2c20 616e 640a 2020 2020 2020 2020  rk, and.        
-00001b40: 2020 6174 7472 6962 7574 696f 6e20 6e6f    attribution no
-00001b50: 7469 6365 7320 6672 6f6d 2074 6865 2053  tices from the S
-00001b60: 6f75 7263 6520 666f 726d 206f 6620 7468  ource form of th
-00001b70: 6520 576f 726b 2c0a 2020 2020 2020 2020  e Work,.        
-00001b80: 2020 6578 636c 7564 696e 6720 7468 6f73    excluding thos
-00001b90: 6520 6e6f 7469 6365 7320 7468 6174 2064  e notices that d
-00001ba0: 6f20 6e6f 7420 7065 7274 6169 6e20 746f  o not pertain to
-00001bb0: 2061 6e79 2070 6172 7420 6f66 0a20 2020   any part of.   
-00001bc0: 2020 2020 2020 2074 6865 2044 6572 6976         the Deriv
-00001bd0: 6174 6976 6520 576f 726b 733b 2061 6e64  ative Works; and
-00001be0: 0a0a 2020 2020 2020 2864 2920 4966 2074  ..      (d) If t
-00001bf0: 6865 2057 6f72 6b20 696e 636c 7564 6573  he Work includes
-00001c00: 2061 2022 4e4f 5449 4345 2220 7465 7874   a "NOTICE" text
-00001c10: 2066 696c 6520 6173 2070 6172 7420 6f66   file as part of
-00001c20: 2069 7473 0a20 2020 2020 2020 2020 2064   its.          d
-00001c30: 6973 7472 6962 7574 696f 6e2c 2074 6865  istribution, the
-00001c40: 6e20 616e 7920 4465 7269 7661 7469 7665  n any Derivative
-00001c50: 2057 6f72 6b73 2074 6861 7420 596f 7520   Works that You 
-00001c60: 6469 7374 7269 6275 7465 206d 7573 740a  distribute must.
-00001c70: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00001c80: 6520 6120 7265 6164 6162 6c65 2063 6f70  e a readable cop
-00001c90: 7920 6f66 2074 6865 2061 7474 7269 6275  y of the attribu
-00001ca0: 7469 6f6e 206e 6f74 6963 6573 2063 6f6e  tion notices con
-00001cb0: 7461 696e 6564 0a20 2020 2020 2020 2020  tained.         
-00001cc0: 2077 6974 6869 6e20 7375 6368 204e 4f54   within such NOT
-00001cd0: 4943 4520 6669 6c65 2c20 6578 636c 7564  ICE file, exclud
-00001ce0: 696e 6720 7468 6f73 6520 6e6f 7469 6365  ing those notice
-00001cf0: 7320 7468 6174 2064 6f20 6e6f 740a 2020  s that do not.  
-00001d00: 2020 2020 2020 2020 7065 7274 6169 6e20          pertain 
-00001d10: 746f 2061 6e79 2070 6172 7420 6f66 2074  to any part of t
-00001d20: 6865 2044 6572 6976 6174 6976 6520 576f  he Derivative Wo
-00001d30: 726b 732c 2069 6e20 6174 206c 6561 7374  rks, in at least
-00001d40: 206f 6e65 0a20 2020 2020 2020 2020 206f   one.          o
-00001d50: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
-00001d60: 706c 6163 6573 3a20 7769 7468 696e 2061  places: within a
-00001d70: 204e 4f54 4943 4520 7465 7874 2066 696c   NOTICE text fil
-00001d80: 6520 6469 7374 7269 6275 7465 640a 2020  e distributed.  
-00001d90: 2020 2020 2020 2020 6173 2070 6172 7420          as part 
-00001da0: 6f66 2074 6865 2044 6572 6976 6174 6976  of the Derivativ
-00001db0: 6520 576f 726b 733b 2077 6974 6869 6e20  e Works; within 
-00001dc0: 7468 6520 536f 7572 6365 2066 6f72 6d20  the Source form 
-00001dd0: 6f72 0a20 2020 2020 2020 2020 2064 6f63  or.          doc
-00001de0: 756d 656e 7461 7469 6f6e 2c20 6966 2070  umentation, if p
-00001df0: 726f 7669 6465 6420 616c 6f6e 6720 7769  rovided along wi
-00001e00: 7468 2074 6865 2044 6572 6976 6174 6976  th the Derivativ
-00001e10: 6520 576f 726b 733b 206f 722c 0a20 2020  e Works; or,.   
-00001e20: 2020 2020 2020 2077 6974 6869 6e20 6120         within a 
-00001e30: 6469 7370 6c61 7920 6765 6e65 7261 7465  display generate
-00001e40: 6420 6279 2074 6865 2044 6572 6976 6174  d by the Derivat
-00001e50: 6976 6520 576f 726b 732c 2069 6620 616e  ive Works, if an
-00001e60: 640a 2020 2020 2020 2020 2020 7768 6572  d.          wher
-00001e70: 6576 6572 2073 7563 6820 7468 6972 642d  ever such third-
-00001e80: 7061 7274 7920 6e6f 7469 6365 7320 6e6f  party notices no
-00001e90: 726d 616c 6c79 2061 7070 6561 722e 2054  rmally appear. T
-00001ea0: 6865 2063 6f6e 7465 6e74 730a 2020 2020  he contents.    
-00001eb0: 2020 2020 2020 6f66 2074 6865 204e 4f54        of the NOT
-00001ec0: 4943 4520 6669 6c65 2061 7265 2066 6f72  ICE file are for
-00001ed0: 2069 6e66 6f72 6d61 7469 6f6e 616c 2070   informational p
-00001ee0: 7572 706f 7365 7320 6f6e 6c79 2061 6e64  urposes only and
-00001ef0: 0a20 2020 2020 2020 2020 2064 6f20 6e6f  .          do no
-00001f00: 7420 6d6f 6469 6679 2074 6865 204c 6963  t modify the Lic
-00001f10: 656e 7365 2e20 596f 7520 6d61 7920 6164  ense. You may ad
-00001f20: 6420 596f 7572 206f 776e 2061 7474 7269  d Your own attri
-00001f30: 6275 7469 6f6e 0a20 2020 2020 2020 2020  bution.         
-00001f40: 206e 6f74 6963 6573 2077 6974 6869 6e20   notices within 
-00001f50: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
-00001f60: 2074 6861 7420 596f 7520 6469 7374 7269   that You distri
-00001f70: 6275 7465 2c20 616c 6f6e 6773 6964 650a  bute, alongside.
-00001f80: 2020 2020 2020 2020 2020 6f72 2061 7320            or as 
-00001f90: 616e 2061 6464 656e 6475 6d20 746f 2074  an addendum to t
-00001fa0: 6865 204e 4f54 4943 4520 7465 7874 2066  he NOTICE text f
-00001fb0: 726f 6d20 7468 6520 576f 726b 2c20 7072  rom the Work, pr
-00001fc0: 6f76 6964 6564 0a20 2020 2020 2020 2020  ovided.         
-00001fd0: 2074 6861 7420 7375 6368 2061 6464 6974   that such addit
-00001fe0: 696f 6e61 6c20 6174 7472 6962 7574 696f  ional attributio
-00001ff0: 6e20 6e6f 7469 6365 7320 6361 6e6e 6f74  n notices cannot
-00002000: 2062 6520 636f 6e73 7472 7565 640a 2020   be construed.  
-00002010: 2020 2020 2020 2020 6173 206d 6f64 6966          as modif
-00002020: 7969 6e67 2074 6865 204c 6963 656e 7365  ying the License
-00002030: 2e0a 0a20 2020 2020 2059 6f75 206d 6179  ...      You may
-00002040: 2061 6464 2059 6f75 7220 6f77 6e20 636f   add Your own co
-00002050: 7079 7269 6768 7420 7374 6174 656d 656e  pyright statemen
-00002060: 7420 746f 2059 6f75 7220 6d6f 6469 6669  t to Your modifi
-00002070: 6361 7469 6f6e 7320 616e 640a 2020 2020  cations and.    
-00002080: 2020 6d61 7920 7072 6f76 6964 6520 6164    may provide ad
-00002090: 6469 7469 6f6e 616c 206f 7220 6469 6666  ditional or diff
-000020a0: 6572 656e 7420 6c69 6365 6e73 6520 7465  erent license te
-000020b0: 726d 7320 616e 6420 636f 6e64 6974 696f  rms and conditio
-000020c0: 6e73 0a20 2020 2020 2066 6f72 2075 7365  ns.      for use
-000020d0: 2c20 7265 7072 6f64 7563 7469 6f6e 2c20  , reproduction, 
-000020e0: 6f72 2064 6973 7472 6962 7574 696f 6e20  or distribution 
-000020f0: 6f66 2059 6f75 7220 6d6f 6469 6669 6361  of Your modifica
-00002100: 7469 6f6e 732c 206f 720a 2020 2020 2020  tions, or.      
-00002110: 666f 7220 616e 7920 7375 6368 2044 6572  for any such Der
-00002120: 6976 6174 6976 6520 576f 726b 7320 6173  ivative Works as
-00002130: 2061 2077 686f 6c65 2c20 7072 6f76 6964   a whole, provid
-00002140: 6564 2059 6f75 7220 7573 652c 0a20 2020  ed Your use,.   
-00002150: 2020 2072 6570 726f 6475 6374 696f 6e2c     reproduction,
-00002160: 2061 6e64 2064 6973 7472 6962 7574 696f   and distributio
-00002170: 6e20 6f66 2074 6865 2057 6f72 6b20 6f74  n of the Work ot
-00002180: 6865 7277 6973 6520 636f 6d70 6c69 6573  herwise complies
-00002190: 2077 6974 680a 2020 2020 2020 7468 6520   with.      the 
-000021a0: 636f 6e64 6974 696f 6e73 2073 7461 7465  conditions state
-000021b0: 6420 696e 2074 6869 7320 4c69 6365 6e73  d in this Licens
-000021c0: 652e 0a0a 2020 2035 2e20 5375 626d 6973  e...   5. Submis
-000021d0: 7369 6f6e 206f 6620 436f 6e74 7269 6275  sion of Contribu
-000021e0: 7469 6f6e 732e 2055 6e6c 6573 7320 596f  tions. Unless Yo
-000021f0: 7520 6578 706c 6963 6974 6c79 2073 7461  u explicitly sta
-00002200: 7465 206f 7468 6572 7769 7365 2c0a 2020  te otherwise,.  
-00002210: 2020 2020 616e 7920 436f 6e74 7269 6275      any Contribu
-00002220: 7469 6f6e 2069 6e74 656e 7469 6f6e 616c  tion intentional
-00002230: 6c79 2073 7562 6d69 7474 6564 2066 6f72  ly submitted for
-00002240: 2069 6e63 6c75 7369 6f6e 2069 6e20 7468   inclusion in th
-00002250: 6520 576f 726b 0a20 2020 2020 2062 7920  e Work.      by 
-00002260: 596f 7520 746f 2074 6865 204c 6963 656e  You to the Licen
-00002270: 736f 7220 7368 616c 6c20 6265 2075 6e64  sor shall be und
-00002280: 6572 2074 6865 2074 6572 6d73 2061 6e64  er the terms and
-00002290: 2063 6f6e 6469 7469 6f6e 7320 6f66 0a20   conditions of. 
-000022a0: 2020 2020 2074 6869 7320 4c69 6365 6e73       this Licens
-000022b0: 652c 2077 6974 686f 7574 2061 6e79 2061  e, without any a
-000022c0: 6464 6974 696f 6e61 6c20 7465 726d 7320  dditional terms 
-000022d0: 6f72 2063 6f6e 6469 7469 6f6e 732e 0a20  or conditions.. 
-000022e0: 2020 2020 204e 6f74 7769 7468 7374 616e       Notwithstan
-000022f0: 6469 6e67 2074 6865 2061 626f 7665 2c20  ding the above, 
-00002300: 6e6f 7468 696e 6720 6865 7265 696e 2073  nothing herein s
-00002310: 6861 6c6c 2073 7570 6572 7365 6465 206f  hall supersede o
-00002320: 7220 6d6f 6469 6679 0a20 2020 2020 2074  r modify.      t
-00002330: 6865 2074 6572 6d73 206f 6620 616e 7920  he terms of any 
-00002340: 7365 7061 7261 7465 206c 6963 656e 7365  separate license
-00002350: 2061 6772 6565 6d65 6e74 2079 6f75 206d   agreement you m
-00002360: 6179 2068 6176 6520 6578 6563 7574 6564  ay have executed
-00002370: 0a20 2020 2020 2077 6974 6820 4c69 6365  .      with Lice
-00002380: 6e73 6f72 2072 6567 6172 6469 6e67 2073  nsor regarding s
-00002390: 7563 6820 436f 6e74 7269 6275 7469 6f6e  uch Contribution
-000023a0: 732e 0a0a 2020 2036 2e20 5472 6164 656d  s...   6. Tradem
-000023b0: 6172 6b73 2e20 5468 6973 204c 6963 656e  arks. This Licen
-000023c0: 7365 2064 6f65 7320 6e6f 7420 6772 616e  se does not gran
-000023d0: 7420 7065 726d 6973 7369 6f6e 2074 6f20  t permission to 
-000023e0: 7573 6520 7468 6520 7472 6164 650a 2020  use the trade.  
-000023f0: 2020 2020 6e61 6d65 732c 2074 7261 6465      names, trade
-00002400: 6d61 726b 732c 2073 6572 7669 6365 206d  marks, service m
-00002410: 6172 6b73 2c20 6f72 2070 726f 6475 6374  arks, or product
-00002420: 206e 616d 6573 206f 6620 7468 6520 4c69   names of the Li
-00002430: 6365 6e73 6f72 2c0a 2020 2020 2020 6578  censor,.      ex
-00002440: 6365 7074 2061 7320 7265 7175 6972 6564  cept as required
-00002450: 2066 6f72 2072 6561 736f 6e61 626c 6520   for reasonable 
-00002460: 616e 6420 6375 7374 6f6d 6172 7920 7573  and customary us
-00002470: 6520 696e 2064 6573 6372 6962 696e 6720  e in describing 
-00002480: 7468 650a 2020 2020 2020 6f72 6967 696e  the.      origin
-00002490: 206f 6620 7468 6520 576f 726b 2061 6e64   of the Work and
-000024a0: 2072 6570 726f 6475 6369 6e67 2074 6865   reproducing the
-000024b0: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-000024c0: 4e4f 5449 4345 2066 696c 652e 0a0a 2020  NOTICE file...  
-000024d0: 2037 2e20 4469 7363 6c61 696d 6572 206f   7. Disclaimer o
-000024e0: 6620 5761 7272 616e 7479 2e20 556e 6c65  f Warranty. Unle
-000024f0: 7373 2072 6571 7569 7265 6420 6279 2061  ss required by a
-00002500: 7070 6c69 6361 626c 6520 6c61 7720 6f72  pplicable law or
-00002510: 0a20 2020 2020 2061 6772 6565 6420 746f  .      agreed to
-00002520: 2069 6e20 7772 6974 696e 672c 204c 6963   in writing, Lic
-00002530: 656e 736f 7220 7072 6f76 6964 6573 2074  ensor provides t
-00002540: 6865 2057 6f72 6b20 2861 6e64 2065 6163  he Work (and eac
-00002550: 680a 2020 2020 2020 436f 6e74 7269 6275  h.      Contribu
-00002560: 746f 7220 7072 6f76 6964 6573 2069 7473  tor provides its
-00002570: 2043 6f6e 7472 6962 7574 696f 6e73 2920   Contributions) 
-00002580: 6f6e 2061 6e20 2241 5320 4953 2220 4241  on an "AS IS" BA
-00002590: 5349 532c 0a20 2020 2020 2057 4954 484f  SIS,.      WITHO
-000025a0: 5554 2057 4152 5241 4e54 4945 5320 4f52  UT WARRANTIES OR
-000025b0: 2043 4f4e 4449 5449 4f4e 5320 4f46 2041   CONDITIONS OF A
-000025c0: 4e59 204b 494e 442c 2065 6974 6865 7220  NY KIND, either 
-000025d0: 6578 7072 6573 7320 6f72 0a20 2020 2020  express or.     
-000025e0: 2069 6d70 6c69 6564 2c20 696e 636c 7564   implied, includ
-000025f0: 696e 672c 2077 6974 686f 7574 206c 696d  ing, without lim
-00002600: 6974 6174 696f 6e2c 2061 6e79 2077 6172  itation, any war
-00002610: 7261 6e74 6965 7320 6f72 2063 6f6e 6469  ranties or condi
-00002620: 7469 6f6e 730a 2020 2020 2020 6f66 2054  tions.      of T
-00002630: 4954 4c45 2c20 4e4f 4e2d 494e 4652 494e  ITLE, NON-INFRIN
-00002640: 4745 4d45 4e54 2c20 4d45 5243 4841 4e54  GEMENT, MERCHANT
-00002650: 4142 494c 4954 592c 206f 7220 4649 544e  ABILITY, or FITN
-00002660: 4553 5320 464f 5220 410a 2020 2020 2020  ESS FOR A.      
-00002670: 5041 5254 4943 554c 4152 2050 5552 504f  PARTICULAR PURPO
-00002680: 5345 2e20 596f 7520 6172 6520 736f 6c65  SE. You are sole
-00002690: 6c79 2072 6573 706f 6e73 6962 6c65 2066  ly responsible f
-000026a0: 6f72 2064 6574 6572 6d69 6e69 6e67 2074  or determining t
-000026b0: 6865 0a20 2020 2020 2061 7070 726f 7072  he.      appropr
-000026c0: 6961 7465 6e65 7373 206f 6620 7573 696e  iateness of usin
-000026d0: 6720 6f72 2072 6564 6973 7472 6962 7574  g or redistribut
-000026e0: 696e 6720 7468 6520 576f 726b 2061 6e64  ing the Work and
-000026f0: 2061 7373 756d 6520 616e 790a 2020 2020   assume any.    
-00002700: 2020 7269 736b 7320 6173 736f 6369 6174    risks associat
-00002710: 6564 2077 6974 6820 596f 7572 2065 7865  ed with Your exe
-00002720: 7263 6973 6520 6f66 2070 6572 6d69 7373  rcise of permiss
-00002730: 696f 6e73 2075 6e64 6572 2074 6869 7320  ions under this 
-00002740: 4c69 6365 6e73 652e 0a0a 2020 2038 2e20  License...   8. 
-00002750: 4c69 6d69 7461 7469 6f6e 206f 6620 4c69  Limitation of Li
-00002760: 6162 696c 6974 792e 2049 6e20 6e6f 2065  ability. In no e
-00002770: 7665 6e74 2061 6e64 2075 6e64 6572 206e  vent and under n
-00002780: 6f20 6c65 6761 6c20 7468 656f 7279 2c0a  o legal theory,.
-00002790: 2020 2020 2020 7768 6574 6865 7220 696e        whether in
-000027a0: 2074 6f72 7420 2869 6e63 6c75 6469 6e67   tort (including
-000027b0: 206e 6567 6c69 6765 6e63 6529 2c20 636f   negligence), co
-000027c0: 6e74 7261 6374 2c20 6f72 206f 7468 6572  ntract, or other
-000027d0: 7769 7365 2c0a 2020 2020 2020 756e 6c65  wise,.      unle
-000027e0: 7373 2072 6571 7569 7265 6420 6279 2061  ss required by a
-000027f0: 7070 6c69 6361 626c 6520 6c61 7720 2873  pplicable law (s
-00002800: 7563 6820 6173 2064 656c 6962 6572 6174  uch as deliberat
-00002810: 6520 616e 6420 6772 6f73 736c 790a 2020  e and grossly.  
-00002820: 2020 2020 6e65 676c 6967 656e 7420 6163      negligent ac
-00002830: 7473 2920 6f72 2061 6772 6565 6420 746f  ts) or agreed to
-00002840: 2069 6e20 7772 6974 696e 672c 2073 6861   in writing, sha
-00002850: 6c6c 2061 6e79 2043 6f6e 7472 6962 7574  ll any Contribut
-00002860: 6f72 2062 650a 2020 2020 2020 6c69 6162  or be.      liab
-00002870: 6c65 2074 6f20 596f 7520 666f 7220 6461  le to You for da
-00002880: 6d61 6765 732c 2069 6e63 6c75 6469 6e67  mages, including
-00002890: 2061 6e79 2064 6972 6563 742c 2069 6e64   any direct, ind
-000028a0: 6972 6563 742c 2073 7065 6369 616c 2c0a  irect, special,.
-000028b0: 2020 2020 2020 696e 6369 6465 6e74 616c        incidental
-000028c0: 2c20 6f72 2063 6f6e 7365 7175 656e 7469  , or consequenti
-000028d0: 616c 2064 616d 6167 6573 206f 6620 616e  al damages of an
-000028e0: 7920 6368 6172 6163 7465 7220 6172 6973  y character aris
-000028f0: 696e 6720 6173 2061 0a20 2020 2020 2072  ing as a.      r
-00002900: 6573 756c 7420 6f66 2074 6869 7320 4c69  esult of this Li
-00002910: 6365 6e73 6520 6f72 206f 7574 206f 6620  cense or out of 
-00002920: 7468 6520 7573 6520 6f72 2069 6e61 6269  the use or inabi
-00002930: 6c69 7479 2074 6f20 7573 6520 7468 650a  lity to use the.
-00002940: 2020 2020 2020 576f 726b 2028 696e 636c        Work (incl
-00002950: 7564 696e 6720 6275 7420 6e6f 7420 6c69  uding but not li
-00002960: 6d69 7465 6420 746f 2064 616d 6167 6573  mited to damages
-00002970: 2066 6f72 206c 6f73 7320 6f66 2067 6f6f   for loss of goo
-00002980: 6477 696c 6c2c 0a20 2020 2020 2077 6f72  dwill,.      wor
-00002990: 6b20 7374 6f70 7061 6765 2c20 636f 6d70  k stoppage, comp
-000029a0: 7574 6572 2066 6169 6c75 7265 206f 7220  uter failure or 
-000029b0: 6d61 6c66 756e 6374 696f 6e2c 206f 7220  malfunction, or 
-000029c0: 616e 7920 616e 6420 616c 6c0a 2020 2020  any and all.    
-000029d0: 2020 6f74 6865 7220 636f 6d6d 6572 6369    other commerci
-000029e0: 616c 2064 616d 6167 6573 206f 7220 6c6f  al damages or lo
-000029f0: 7373 6573 292c 2065 7665 6e20 6966 2073  sses), even if s
-00002a00: 7563 6820 436f 6e74 7269 6275 746f 720a  uch Contributor.
-00002a10: 2020 2020 2020 6861 7320 6265 656e 2061        has been a
-00002a20: 6476 6973 6564 206f 6620 7468 6520 706f  dvised of the po
-00002a30: 7373 6962 696c 6974 7920 6f66 2073 7563  ssibility of suc
-00002a40: 6820 6461 6d61 6765 732e 0a0a 2020 2039  h damages...   9
-00002a50: 2e20 4163 6365 7074 696e 6720 5761 7272  . Accepting Warr
-00002a60: 616e 7479 206f 7220 4164 6469 7469 6f6e  anty or Addition
-00002a70: 616c 204c 6961 6269 6c69 7479 2e20 5768  al Liability. Wh
-00002a80: 696c 6520 7265 6469 7374 7269 6275 7469  ile redistributi
-00002a90: 6e67 0a20 2020 2020 2074 6865 2057 6f72  ng.      the Wor
-00002aa0: 6b20 6f72 2044 6572 6976 6174 6976 6520  k or Derivative 
-00002ab0: 576f 726b 7320 7468 6572 656f 662c 2059  Works thereof, Y
-00002ac0: 6f75 206d 6179 2063 686f 6f73 6520 746f  ou may choose to
-00002ad0: 206f 6666 6572 2c0a 2020 2020 2020 616e   offer,.      an
-00002ae0: 6420 6368 6172 6765 2061 2066 6565 2066  d charge a fee f
-00002af0: 6f72 2c20 6163 6365 7074 616e 6365 206f  or, acceptance o
-00002b00: 6620 7375 7070 6f72 742c 2077 6172 7261  f support, warra
-00002b10: 6e74 792c 2069 6e64 656d 6e69 7479 2c0a  nty, indemnity,.
-00002b20: 2020 2020 2020 6f72 206f 7468 6572 206c        or other l
-00002b30: 6961 6269 6c69 7479 206f 626c 6967 6174  iability obligat
-00002b40: 696f 6e73 2061 6e64 2f6f 7220 7269 6768  ions and/or righ
-00002b50: 7473 2063 6f6e 7369 7374 656e 7420 7769  ts consistent wi
-00002b60: 7468 2074 6869 730a 2020 2020 2020 4c69  th this.      Li
-00002b70: 6365 6e73 652e 2048 6f77 6576 6572 2c20  cense. However, 
-00002b80: 696e 2061 6363 6570 7469 6e67 2073 7563  in accepting suc
-00002b90: 6820 6f62 6c69 6761 7469 6f6e 732c 2059  h obligations, Y
-00002ba0: 6f75 206d 6179 2061 6374 206f 6e6c 790a  ou may act only.
-00002bb0: 2020 2020 2020 6f6e 2059 6f75 7220 6f77        on Your ow
-00002bc0: 6e20 6265 6861 6c66 2061 6e64 206f 6e20  n behalf and on 
-00002bd0: 596f 7572 2073 6f6c 6520 7265 7370 6f6e  Your sole respon
-00002be0: 7369 6269 6c69 7479 2c20 6e6f 7420 6f6e  sibility, not on
-00002bf0: 2062 6568 616c 660a 2020 2020 2020 6f66   behalf.      of
-00002c00: 2061 6e79 206f 7468 6572 2043 6f6e 7472   any other Contr
-00002c10: 6962 7574 6f72 2c20 616e 6420 6f6e 6c79  ibutor, and only
-00002c20: 2069 6620 596f 7520 6167 7265 6520 746f   if You agree to
-00002c30: 2069 6e64 656d 6e69 6679 2c0a 2020 2020   indemnify,.    
-00002c40: 2020 6465 6665 6e64 2c20 616e 6420 686f    defend, and ho
-00002c50: 6c64 2065 6163 6820 436f 6e74 7269 6275  ld each Contribu
-00002c60: 746f 7220 6861 726d 6c65 7373 2066 6f72  tor harmless for
-00002c70: 2061 6e79 206c 6961 6269 6c69 7479 0a20   any liability. 
-00002c80: 2020 2020 2069 6e63 7572 7265 6420 6279       incurred by
-00002c90: 2c20 6f72 2063 6c61 696d 7320 6173 7365  , or claims asse
-00002ca0: 7274 6564 2061 6761 696e 7374 2c20 7375  rted against, su
-00002cb0: 6368 2043 6f6e 7472 6962 7574 6f72 2062  ch Contributor b
-00002cc0: 7920 7265 6173 6f6e 0a20 2020 2020 206f  y reason.      o
-00002cd0: 6620 796f 7572 2061 6363 6570 7469 6e67  f your accepting
-00002ce0: 2061 6e79 2073 7563 6820 7761 7272 616e   any such warran
-00002cf0: 7479 206f 7220 6164 6469 7469 6f6e 616c  ty or additional
-00002d00: 206c 6961 6269 6c69 7479 2e0a 2d2d 2d2d   liability..----
-00002d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000590: 2020 2020 2020 2020 2020 4170 6163 6865            Apache
+000005a0: 204c 6963 656e 7365 0a20 2020 2020 2020   License.       
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 2020 2020 5665 7273 696f 6e20 322e 302c      Version 2.0,
+000005d0: 204a 616e 7561 7279 2032 3030 340a 2020   January 2004.  
+000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005f0: 2020 2020 2020 6874 7470 3a2f 2f77 7777        http://www
+00000600: 2e61 7061 6368 652e 6f72 672f 6c69 6365  .apache.org/lice
+00000610: 6e73 6573 2f0a 0a20 2020 5445 524d 5320  nses/..   TERMS 
+00000620: 414e 4420 434f 4e44 4954 494f 4e53 2046  AND CONDITIONS F
+00000630: 4f52 2055 5345 2c20 5245 5052 4f44 5543  OR USE, REPRODUC
+00000640: 5449 4f4e 2c20 414e 4420 4449 5354 5249  TION, AND DISTRI
+00000650: 4255 5449 4f4e 0a0a 2020 2031 2e20 4465  BUTION..   1. De
+00000660: 6669 6e69 7469 6f6e 732e 0a0a 2020 2020  finitions...    
+00000670: 2020 224c 6963 656e 7365 2220 7368 616c    "License" shal
+00000680: 6c20 6d65 616e 2074 6865 2074 6572 6d73  l mean the terms
+00000690: 2061 6e64 2063 6f6e 6469 7469 6f6e 7320   and conditions 
+000006a0: 666f 7220 7573 652c 2072 6570 726f 6475  for use, reprodu
+000006b0: 6374 696f 6e2c 0a20 2020 2020 2061 6e64  ction,.      and
+000006c0: 2064 6973 7472 6962 7574 696f 6e20 6173   distribution as
+000006d0: 2064 6566 696e 6564 2062 7920 5365 6374   defined by Sect
+000006e0: 696f 6e73 2031 2074 6872 6f75 6768 2039  ions 1 through 9
+000006f0: 206f 6620 7468 6973 2064 6f63 756d 656e   of this documen
+00000700: 742e 0a0a 2020 2020 2020 224c 6963 656e  t...      "Licen
+00000710: 736f 7222 2073 6861 6c6c 206d 6561 6e20  sor" shall mean 
+00000720: 7468 6520 636f 7079 7269 6768 7420 6f77  the copyright ow
+00000730: 6e65 7220 6f72 2065 6e74 6974 7920 6175  ner or entity au
+00000740: 7468 6f72 697a 6564 2062 790a 2020 2020  thorized by.    
+00000750: 2020 7468 6520 636f 7079 7269 6768 7420    the copyright 
+00000760: 6f77 6e65 7220 7468 6174 2069 7320 6772  owner that is gr
+00000770: 616e 7469 6e67 2074 6865 204c 6963 656e  anting the Licen
+00000780: 7365 2e0a 0a20 2020 2020 2022 4c65 6761  se...      "Lega
+00000790: 6c20 456e 7469 7479 2220 7368 616c 6c20  l Entity" shall 
+000007a0: 6d65 616e 2074 6865 2075 6e69 6f6e 206f  mean the union o
+000007b0: 6620 7468 6520 6163 7469 6e67 2065 6e74  f the acting ent
+000007c0: 6974 7920 616e 6420 616c 6c0a 2020 2020  ity and all.    
+000007d0: 2020 6f74 6865 7220 656e 7469 7469 6573    other entities
+000007e0: 2074 6861 7420 636f 6e74 726f 6c2c 2061   that control, a
+000007f0: 7265 2063 6f6e 7472 6f6c 6c65 6420 6279  re controlled by
+00000800: 2c20 6f72 2061 7265 2075 6e64 6572 2063  , or are under c
+00000810: 6f6d 6d6f 6e0a 2020 2020 2020 636f 6e74  ommon.      cont
+00000820: 726f 6c20 7769 7468 2074 6861 7420 656e  rol with that en
+00000830: 7469 7479 2e20 466f 7220 7468 6520 7075  tity. For the pu
+00000840: 7270 6f73 6573 206f 6620 7468 6973 2064  rposes of this d
+00000850: 6566 696e 6974 696f 6e2c 0a20 2020 2020  efinition,.     
+00000860: 2022 636f 6e74 726f 6c22 206d 6561 6e73   "control" means
+00000870: 2028 6929 2074 6865 2070 6f77 6572 2c20   (i) the power, 
+00000880: 6469 7265 6374 206f 7220 696e 6469 7265  direct or indire
+00000890: 6374 2c20 746f 2063 6175 7365 2074 6865  ct, to cause the
+000008a0: 0a20 2020 2020 2064 6972 6563 7469 6f6e  .      direction
+000008b0: 206f 7220 6d61 6e61 6765 6d65 6e74 206f   or management o
+000008c0: 6620 7375 6368 2065 6e74 6974 792c 2077  f such entity, w
+000008d0: 6865 7468 6572 2062 7920 636f 6e74 7261  hether by contra
+000008e0: 6374 206f 720a 2020 2020 2020 6f74 6865  ct or.      othe
+000008f0: 7277 6973 652c 206f 7220 2869 6929 206f  rwise, or (ii) o
+00000900: 776e 6572 7368 6970 206f 6620 6669 6674  wnership of fift
+00000910: 7920 7065 7263 656e 7420 2835 3025 2920  y percent (50%) 
+00000920: 6f72 206d 6f72 6520 6f66 2074 6865 0a20  or more of the. 
+00000930: 2020 2020 206f 7574 7374 616e 6469 6e67       outstanding
+00000940: 2073 6861 7265 732c 206f 7220 2869 6969   shares, or (iii
+00000950: 2920 6265 6e65 6669 6369 616c 206f 776e  ) beneficial own
+00000960: 6572 7368 6970 206f 6620 7375 6368 2065  ership of such e
+00000970: 6e74 6974 792e 0a0a 2020 2020 2020 2259  ntity...      "Y
+00000980: 6f75 2220 286f 7220 2259 6f75 7222 2920  ou" (or "Your") 
+00000990: 7368 616c 6c20 6d65 616e 2061 6e20 696e  shall mean an in
+000009a0: 6469 7669 6475 616c 206f 7220 4c65 6761  dividual or Lega
+000009b0: 6c20 456e 7469 7479 0a20 2020 2020 2065  l Entity.      e
+000009c0: 7865 7263 6973 696e 6720 7065 726d 6973  xercising permis
+000009d0: 7369 6f6e 7320 6772 616e 7465 6420 6279  sions granted by
+000009e0: 2074 6869 7320 4c69 6365 6e73 652e 0a0a   this License...
+000009f0: 2020 2020 2020 2253 6f75 7263 6522 2066        "Source" f
+00000a00: 6f72 6d20 7368 616c 6c20 6d65 616e 2074  orm shall mean t
+00000a10: 6865 2070 7265 6665 7272 6564 2066 6f72  he preferred for
+00000a20: 6d20 666f 7220 6d61 6b69 6e67 206d 6f64  m for making mod
+00000a30: 6966 6963 6174 696f 6e73 2c0a 2020 2020  ifications,.    
+00000a40: 2020 696e 636c 7564 696e 6720 6275 7420    including but 
+00000a50: 6e6f 7420 6c69 6d69 7465 6420 746f 2073  not limited to s
+00000a60: 6f66 7477 6172 6520 736f 7572 6365 2063  oftware source c
+00000a70: 6f64 652c 2064 6f63 756d 656e 7461 7469  ode, documentati
+00000a80: 6f6e 0a20 2020 2020 2073 6f75 7263 652c  on.      source,
+00000a90: 2061 6e64 2063 6f6e 6669 6775 7261 7469   and configurati
+00000aa0: 6f6e 2066 696c 6573 2e0a 0a20 2020 2020  on files...     
+00000ab0: 2022 4f62 6a65 6374 2220 666f 726d 2073   "Object" form s
+00000ac0: 6861 6c6c 206d 6561 6e20 616e 7920 666f  hall mean any fo
+00000ad0: 726d 2072 6573 756c 7469 6e67 2066 726f  rm resulting fro
+00000ae0: 6d20 6d65 6368 616e 6963 616c 0a20 2020  m mechanical.   
+00000af0: 2020 2074 7261 6e73 666f 726d 6174 696f     transformatio
+00000b00: 6e20 6f72 2074 7261 6e73 6c61 7469 6f6e  n or translation
+00000b10: 206f 6620 6120 536f 7572 6365 2066 6f72   of a Source for
+00000b20: 6d2c 2069 6e63 6c75 6469 6e67 2062 7574  m, including but
+00000b30: 0a20 2020 2020 206e 6f74 206c 696d 6974  .      not limit
+00000b40: 6564 2074 6f20 636f 6d70 696c 6564 206f  ed to compiled o
+00000b50: 626a 6563 7420 636f 6465 2c20 6765 6e65  bject code, gene
+00000b60: 7261 7465 6420 646f 6375 6d65 6e74 6174  rated documentat
+00000b70: 696f 6e2c 0a20 2020 2020 2061 6e64 2063  ion,.      and c
+00000b80: 6f6e 7665 7273 696f 6e73 2074 6f20 6f74  onversions to ot
+00000b90: 6865 7220 6d65 6469 6120 7479 7065 732e  her media types.
+00000ba0: 0a0a 2020 2020 2020 2257 6f72 6b22 2073  ..      "Work" s
+00000bb0: 6861 6c6c 206d 6561 6e20 7468 6520 776f  hall mean the wo
+00000bc0: 726b 206f 6620 6175 7468 6f72 7368 6970  rk of authorship
+00000bd0: 2c20 7768 6574 6865 7220 696e 2053 6f75  , whether in Sou
+00000be0: 7263 6520 6f72 0a20 2020 2020 204f 626a  rce or.      Obj
+00000bf0: 6563 7420 666f 726d 2c20 6d61 6465 2061  ect form, made a
+00000c00: 7661 696c 6162 6c65 2075 6e64 6572 2074  vailable under t
+00000c10: 6865 204c 6963 656e 7365 2c20 6173 2069  he License, as i
+00000c20: 6e64 6963 6174 6564 2062 7920 610a 2020  ndicated by a.  
+00000c30: 2020 2020 636f 7079 7269 6768 7420 6e6f      copyright no
+00000c40: 7469 6365 2074 6861 7420 6973 2069 6e63  tice that is inc
+00000c50: 6c75 6465 6420 696e 206f 7220 6174 7461  luded in or atta
+00000c60: 6368 6564 2074 6f20 7468 6520 776f 726b  ched to the work
+00000c70: 0a20 2020 2020 2028 616e 2065 7861 6d70  .      (an examp
+00000c80: 6c65 2069 7320 7072 6f76 6964 6564 2069  le is provided i
+00000c90: 6e20 7468 6520 4170 7065 6e64 6978 2062  n the Appendix b
+00000ca0: 656c 6f77 292e 0a0a 2020 2020 2020 2244  elow)...      "D
+00000cb0: 6572 6976 6174 6976 6520 576f 726b 7322  erivative Works"
+00000cc0: 2073 6861 6c6c 206d 6561 6e20 616e 7920   shall mean any 
+00000cd0: 776f 726b 2c20 7768 6574 6865 7220 696e  work, whether in
+00000ce0: 2053 6f75 7263 6520 6f72 204f 626a 6563   Source or Objec
+00000cf0: 740a 2020 2020 2020 666f 726d 2c20 7468  t.      form, th
+00000d00: 6174 2069 7320 6261 7365 6420 6f6e 2028  at is based on (
+00000d10: 6f72 2064 6572 6976 6564 2066 726f 6d29  or derived from)
+00000d20: 2074 6865 2057 6f72 6b20 616e 6420 666f   the Work and fo
+00000d30: 7220 7768 6963 6820 7468 650a 2020 2020  r which the.    
+00000d40: 2020 6564 6974 6f72 6961 6c20 7265 7669    editorial revi
+00000d50: 7369 6f6e 732c 2061 6e6e 6f74 6174 696f  sions, annotatio
+00000d60: 6e73 2c20 656c 6162 6f72 6174 696f 6e73  ns, elaborations
+00000d70: 2c20 6f72 206f 7468 6572 206d 6f64 6966  , or other modif
+00000d80: 6963 6174 696f 6e73 0a20 2020 2020 2072  ications.      r
+00000d90: 6570 7265 7365 6e74 2c20 6173 2061 2077  epresent, as a w
+00000da0: 686f 6c65 2c20 616e 206f 7269 6769 6e61  hole, an origina
+00000db0: 6c20 776f 726b 206f 6620 6175 7468 6f72  l work of author
+00000dc0: 7368 6970 2e20 466f 7220 7468 6520 7075  ship. For the pu
+00000dd0: 7270 6f73 6573 0a20 2020 2020 206f 6620  rposes.      of 
+00000de0: 7468 6973 204c 6963 656e 7365 2c20 4465  this License, De
+00000df0: 7269 7661 7469 7665 2057 6f72 6b73 2073  rivative Works s
+00000e00: 6861 6c6c 206e 6f74 2069 6e63 6c75 6465  hall not include
+00000e10: 2077 6f72 6b73 2074 6861 7420 7265 6d61   works that rema
+00000e20: 696e 0a20 2020 2020 2073 6570 6172 6162  in.      separab
+00000e30: 6c65 2066 726f 6d2c 206f 7220 6d65 7265  le from, or mere
+00000e40: 6c79 206c 696e 6b20 286f 7220 6269 6e64  ly link (or bind
+00000e50: 2062 7920 6e61 6d65 2920 746f 2074 6865   by name) to the
+00000e60: 2069 6e74 6572 6661 6365 7320 6f66 2c0a   interfaces of,.
+00000e70: 2020 2020 2020 7468 6520 576f 726b 2061        the Work a
+00000e80: 6e64 2044 6572 6976 6174 6976 6520 576f  nd Derivative Wo
+00000e90: 726b 7320 7468 6572 656f 662e 0a0a 2020  rks thereof...  
+00000ea0: 2020 2020 2243 6f6e 7472 6962 7574 696f      "Contributio
+00000eb0: 6e22 2073 6861 6c6c 206d 6561 6e20 616e  n" shall mean an
+00000ec0: 7920 776f 726b 206f 6620 6175 7468 6f72  y work of author
+00000ed0: 7368 6970 2c20 696e 636c 7564 696e 670a  ship, including.
+00000ee0: 2020 2020 2020 7468 6520 6f72 6967 696e        the origin
+00000ef0: 616c 2076 6572 7369 6f6e 206f 6620 7468  al version of th
+00000f00: 6520 576f 726b 2061 6e64 2061 6e79 206d  e Work and any m
+00000f10: 6f64 6966 6963 6174 696f 6e73 206f 7220  odifications or 
+00000f20: 6164 6469 7469 6f6e 730a 2020 2020 2020  additions.      
+00000f30: 746f 2074 6861 7420 576f 726b 206f 7220  to that Work or 
+00000f40: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
+00000f50: 2074 6865 7265 6f66 2c20 7468 6174 2069   thereof, that i
+00000f60: 7320 696e 7465 6e74 696f 6e61 6c6c 790a  s intentionally.
+00000f70: 2020 2020 2020 7375 626d 6974 7465 6420        submitted 
+00000f80: 746f 204c 6963 656e 736f 7220 666f 7220  to Licensor for 
+00000f90: 696e 636c 7573 696f 6e20 696e 2074 6865  inclusion in the
+00000fa0: 2057 6f72 6b20 6279 2074 6865 2063 6f70   Work by the cop
+00000fb0: 7972 6967 6874 206f 776e 6572 0a20 2020  yright owner.   
+00000fc0: 2020 206f 7220 6279 2061 6e20 696e 6469     or by an indi
+00000fd0: 7669 6475 616c 206f 7220 4c65 6761 6c20  vidual or Legal 
+00000fe0: 456e 7469 7479 2061 7574 686f 7269 7a65  Entity authorize
+00000ff0: 6420 746f 2073 7562 6d69 7420 6f6e 2062  d to submit on b
+00001000: 6568 616c 6620 6f66 0a20 2020 2020 2074  ehalf of.      t
+00001010: 6865 2063 6f70 7972 6967 6874 206f 776e  he copyright own
+00001020: 6572 2e20 466f 7220 7468 6520 7075 7270  er. For the purp
+00001030: 6f73 6573 206f 6620 7468 6973 2064 6566  oses of this def
+00001040: 696e 6974 696f 6e2c 2022 7375 626d 6974  inition, "submit
+00001050: 7465 6422 0a20 2020 2020 206d 6561 6e73  ted".      means
+00001060: 2061 6e79 2066 6f72 6d20 6f66 2065 6c65   any form of ele
+00001070: 6374 726f 6e69 632c 2076 6572 6261 6c2c  ctronic, verbal,
+00001080: 206f 7220 7772 6974 7465 6e20 636f 6d6d   or written comm
+00001090: 756e 6963 6174 696f 6e20 7365 6e74 0a20  unication sent. 
+000010a0: 2020 2020 2074 6f20 7468 6520 4c69 6365       to the Lice
+000010b0: 6e73 6f72 206f 7220 6974 7320 7265 7072  nsor or its repr
+000010c0: 6573 656e 7461 7469 7665 732c 2069 6e63  esentatives, inc
+000010d0: 6c75 6469 6e67 2062 7574 206e 6f74 206c  luding but not l
+000010e0: 696d 6974 6564 2074 6f0a 2020 2020 2020  imited to.      
+000010f0: 636f 6d6d 756e 6963 6174 696f 6e20 6f6e  communication on
+00001100: 2065 6c65 6374 726f 6e69 6320 6d61 696c   electronic mail
+00001110: 696e 6720 6c69 7374 732c 2073 6f75 7263  ing lists, sourc
+00001120: 6520 636f 6465 2063 6f6e 7472 6f6c 2073  e code control s
+00001130: 7973 7465 6d73 2c0a 2020 2020 2020 616e  ystems,.      an
+00001140: 6420 6973 7375 6520 7472 6163 6b69 6e67  d issue tracking
+00001150: 2073 7973 7465 6d73 2074 6861 7420 6172   systems that ar
+00001160: 6520 6d61 6e61 6765 6420 6279 2c20 6f72  e managed by, or
+00001170: 206f 6e20 6265 6861 6c66 206f 662c 2074   on behalf of, t
+00001180: 6865 0a20 2020 2020 204c 6963 656e 736f  he.      Licenso
+00001190: 7220 666f 7220 7468 6520 7075 7270 6f73  r for the purpos
+000011a0: 6520 6f66 2064 6973 6375 7373 696e 6720  e of discussing 
+000011b0: 616e 6420 696d 7072 6f76 696e 6720 7468  and improving th
+000011c0: 6520 576f 726b 2c20 6275 740a 2020 2020  e Work, but.    
+000011d0: 2020 6578 636c 7564 696e 6720 636f 6d6d    excluding comm
+000011e0: 756e 6963 6174 696f 6e20 7468 6174 2069  unication that i
+000011f0: 7320 636f 6e73 7069 6375 6f75 736c 7920  s conspicuously 
+00001200: 6d61 726b 6564 206f 7220 6f74 6865 7277  marked or otherw
+00001210: 6973 650a 2020 2020 2020 6465 7369 676e  ise.      design
+00001220: 6174 6564 2069 6e20 7772 6974 696e 6720  ated in writing 
+00001230: 6279 2074 6865 2063 6f70 7972 6967 6874  by the copyright
+00001240: 206f 776e 6572 2061 7320 224e 6f74 2061   owner as "Not a
+00001250: 2043 6f6e 7472 6962 7574 696f 6e2e 220a   Contribution.".
+00001260: 0a20 2020 2020 2022 436f 6e74 7269 6275  .      "Contribu
+00001270: 746f 7222 2073 6861 6c6c 206d 6561 6e20  tor" shall mean 
+00001280: 4c69 6365 6e73 6f72 2061 6e64 2061 6e79  Licensor and any
+00001290: 2069 6e64 6976 6964 7561 6c20 6f72 204c   individual or L
+000012a0: 6567 616c 2045 6e74 6974 790a 2020 2020  egal Entity.    
+000012b0: 2020 6f6e 2062 6568 616c 6620 6f66 2077    on behalf of w
+000012c0: 686f 6d20 6120 436f 6e74 7269 6275 7469  hom a Contributi
+000012d0: 6f6e 2068 6173 2062 6565 6e20 7265 6365  on has been rece
+000012e0: 6976 6564 2062 7920 4c69 6365 6e73 6f72  ived by Licensor
+000012f0: 2061 6e64 0a20 2020 2020 2073 7562 7365   and.      subse
+00001300: 7175 656e 746c 7920 696e 636f 7270 6f72  quently incorpor
+00001310: 6174 6564 2077 6974 6869 6e20 7468 6520  ated within the 
+00001320: 576f 726b 2e0a 0a20 2020 322e 2047 7261  Work...   2. Gra
+00001330: 6e74 206f 6620 436f 7079 7269 6768 7420  nt of Copyright 
+00001340: 4c69 6365 6e73 652e 2053 7562 6a65 6374  License. Subject
+00001350: 2074 6f20 7468 6520 7465 726d 7320 616e   to the terms an
+00001360: 6420 636f 6e64 6974 696f 6e73 206f 660a  d conditions of.
+00001370: 2020 2020 2020 7468 6973 204c 6963 656e        this Licen
+00001380: 7365 2c20 6561 6368 2043 6f6e 7472 6962  se, each Contrib
+00001390: 7574 6f72 2068 6572 6562 7920 6772 616e  utor hereby gran
+000013a0: 7473 2074 6f20 596f 7520 6120 7065 7270  ts to You a perp
+000013b0: 6574 7561 6c2c 0a20 2020 2020 2077 6f72  etual,.      wor
+000013c0: 6c64 7769 6465 2c20 6e6f 6e2d 6578 636c  ldwide, non-excl
+000013d0: 7573 6976 652c 206e 6f2d 6368 6172 6765  usive, no-charge
+000013e0: 2c20 726f 7961 6c74 792d 6672 6565 2c20  , royalty-free, 
+000013f0: 6972 7265 766f 6361 626c 650a 2020 2020  irrevocable.    
+00001400: 2020 636f 7079 7269 6768 7420 6c69 6365    copyright lice
+00001410: 6e73 6520 746f 2072 6570 726f 6475 6365  nse to reproduce
+00001420: 2c20 7072 6570 6172 6520 4465 7269 7661  , prepare Deriva
+00001430: 7469 7665 2057 6f72 6b73 206f 662c 0a20  tive Works of,. 
+00001440: 2020 2020 2070 7562 6c69 636c 7920 6469       publicly di
+00001450: 7370 6c61 792c 2070 7562 6c69 636c 7920  splay, publicly 
+00001460: 7065 7266 6f72 6d2c 2073 7562 6c69 6365  perform, sublice
+00001470: 6e73 652c 2061 6e64 2064 6973 7472 6962  nse, and distrib
+00001480: 7574 6520 7468 650a 2020 2020 2020 576f  ute the.      Wo
+00001490: 726b 2061 6e64 2073 7563 6820 4465 7269  rk and such Deri
+000014a0: 7661 7469 7665 2057 6f72 6b73 2069 6e20  vative Works in 
+000014b0: 536f 7572 6365 206f 7220 4f62 6a65 6374  Source or Object
+000014c0: 2066 6f72 6d2e 0a0a 2020 2033 2e20 4772   form...   3. Gr
+000014d0: 616e 7420 6f66 2050 6174 656e 7420 4c69  ant of Patent Li
+000014e0: 6365 6e73 652e 2053 7562 6a65 6374 2074  cense. Subject t
+000014f0: 6f20 7468 6520 7465 726d 7320 616e 6420  o the terms and 
+00001500: 636f 6e64 6974 696f 6e73 206f 660a 2020  conditions of.  
+00001510: 2020 2020 7468 6973 204c 6963 656e 7365      this License
+00001520: 2c20 6561 6368 2043 6f6e 7472 6962 7574  , each Contribut
+00001530: 6f72 2068 6572 6562 7920 6772 616e 7473  or hereby grants
+00001540: 2074 6f20 596f 7520 6120 7065 7270 6574   to You a perpet
+00001550: 7561 6c2c 0a20 2020 2020 2077 6f72 6c64  ual,.      world
+00001560: 7769 6465 2c20 6e6f 6e2d 6578 636c 7573  wide, non-exclus
+00001570: 6976 652c 206e 6f2d 6368 6172 6765 2c20  ive, no-charge, 
+00001580: 726f 7961 6c74 792d 6672 6565 2c20 6972  royalty-free, ir
+00001590: 7265 766f 6361 626c 650a 2020 2020 2020  revocable.      
+000015a0: 2865 7863 6570 7420 6173 2073 7461 7465  (except as state
+000015b0: 6420 696e 2074 6869 7320 7365 6374 696f  d in this sectio
+000015c0: 6e29 2070 6174 656e 7420 6c69 6365 6e73  n) patent licens
+000015d0: 6520 746f 206d 616b 652c 2068 6176 6520  e to make, have 
+000015e0: 6d61 6465 2c0a 2020 2020 2020 7573 652c  made,.      use,
+000015f0: 206f 6666 6572 2074 6f20 7365 6c6c 2c20   offer to sell, 
+00001600: 7365 6c6c 2c20 696d 706f 7274 2c20 616e  sell, import, an
+00001610: 6420 6f74 6865 7277 6973 6520 7472 616e  d otherwise tran
+00001620: 7366 6572 2074 6865 2057 6f72 6b2c 0a20  sfer the Work,. 
+00001630: 2020 2020 2077 6865 7265 2073 7563 6820       where such 
+00001640: 6c69 6365 6e73 6520 6170 706c 6965 7320  license applies 
+00001650: 6f6e 6c79 2074 6f20 7468 6f73 6520 7061  only to those pa
+00001660: 7465 6e74 2063 6c61 696d 7320 6c69 6365  tent claims lice
+00001670: 6e73 6162 6c65 0a20 2020 2020 2062 7920  nsable.      by 
+00001680: 7375 6368 2043 6f6e 7472 6962 7574 6f72  such Contributor
+00001690: 2074 6861 7420 6172 6520 6e65 6365 7373   that are necess
+000016a0: 6172 696c 7920 696e 6672 696e 6765 6420  arily infringed 
+000016b0: 6279 2074 6865 6972 0a20 2020 2020 2043  by their.      C
+000016c0: 6f6e 7472 6962 7574 696f 6e28 7329 2061  ontribution(s) a
+000016d0: 6c6f 6e65 206f 7220 6279 2063 6f6d 6269  lone or by combi
+000016e0: 6e61 7469 6f6e 206f 6620 7468 6569 7220  nation of their 
+000016f0: 436f 6e74 7269 6275 7469 6f6e 2873 290a  Contribution(s).
+00001700: 2020 2020 2020 7769 7468 2074 6865 2057        with the W
+00001710: 6f72 6b20 746f 2077 6869 6368 2073 7563  ork to which suc
+00001720: 6820 436f 6e74 7269 6275 7469 6f6e 2873  h Contribution(s
+00001730: 2920 7761 7320 7375 626d 6974 7465 642e  ) was submitted.
+00001740: 2049 6620 596f 750a 2020 2020 2020 696e   If You.      in
+00001750: 7374 6974 7574 6520 7061 7465 6e74 206c  stitute patent l
+00001760: 6974 6967 6174 696f 6e20 6167 6169 6e73  itigation agains
+00001770: 7420 616e 7920 656e 7469 7479 2028 696e  t any entity (in
+00001780: 636c 7564 696e 6720 610a 2020 2020 2020  cluding a.      
+00001790: 6372 6f73 732d 636c 6169 6d20 6f72 2063  cross-claim or c
+000017a0: 6f75 6e74 6572 636c 6169 6d20 696e 2061  ounterclaim in a
+000017b0: 206c 6177 7375 6974 2920 616c 6c65 6769   lawsuit) allegi
+000017c0: 6e67 2074 6861 7420 7468 6520 576f 726b  ng that the Work
+000017d0: 0a20 2020 2020 206f 7220 6120 436f 6e74  .      or a Cont
+000017e0: 7269 6275 7469 6f6e 2069 6e63 6f72 706f  ribution incorpo
+000017f0: 7261 7465 6420 7769 7468 696e 2074 6865  rated within the
+00001800: 2057 6f72 6b20 636f 6e73 7469 7475 7465   Work constitute
+00001810: 7320 6469 7265 6374 0a20 2020 2020 206f  s direct.      o
+00001820: 7220 636f 6e74 7269 6275 746f 7279 2070  r contributory p
+00001830: 6174 656e 7420 696e 6672 696e 6765 6d65  atent infringeme
+00001840: 6e74 2c20 7468 656e 2061 6e79 2070 6174  nt, then any pat
+00001850: 656e 7420 6c69 6365 6e73 6573 0a20 2020  ent licenses.   
+00001860: 2020 2067 7261 6e74 6564 2074 6f20 596f     granted to Yo
+00001870: 7520 756e 6465 7220 7468 6973 204c 6963  u under this Lic
+00001880: 656e 7365 2066 6f72 2074 6861 7420 576f  ense for that Wo
+00001890: 726b 2073 6861 6c6c 2074 6572 6d69 6e61  rk shall termina
+000018a0: 7465 0a20 2020 2020 2061 7320 6f66 2074  te.      as of t
+000018b0: 6865 2064 6174 6520 7375 6368 206c 6974  he date such lit
+000018c0: 6967 6174 696f 6e20 6973 2066 696c 6564  igation is filed
+000018d0: 2e0a 0a20 2020 342e 2052 6564 6973 7472  ...   4. Redistr
+000018e0: 6962 7574 696f 6e2e 2059 6f75 206d 6179  ibution. You may
+000018f0: 2072 6570 726f 6475 6365 2061 6e64 2064   reproduce and d
+00001900: 6973 7472 6962 7574 6520 636f 7069 6573  istribute copies
+00001910: 206f 6620 7468 650a 2020 2020 2020 576f   of the.      Wo
+00001920: 726b 206f 7220 4465 7269 7661 7469 7665  rk or Derivative
+00001930: 2057 6f72 6b73 2074 6865 7265 6f66 2069   Works thereof i
+00001940: 6e20 616e 7920 6d65 6469 756d 2c20 7769  n any medium, wi
+00001950: 7468 206f 7220 7769 7468 6f75 740a 2020  th or without.  
+00001960: 2020 2020 6d6f 6469 6669 6361 7469 6f6e      modification
+00001970: 732c 2061 6e64 2069 6e20 536f 7572 6365  s, and in Source
+00001980: 206f 7220 4f62 6a65 6374 2066 6f72 6d2c   or Object form,
+00001990: 2070 726f 7669 6465 6420 7468 6174 2059   provided that Y
+000019a0: 6f75 0a20 2020 2020 206d 6565 7420 7468  ou.      meet th
+000019b0: 6520 666f 6c6c 6f77 696e 6720 636f 6e64  e following cond
+000019c0: 6974 696f 6e73 3a0a 0a20 2020 2020 2028  itions:..      (
+000019d0: 6129 2059 6f75 206d 7573 7420 6769 7665  a) You must give
+000019e0: 2061 6e79 206f 7468 6572 2072 6563 6970   any other recip
+000019f0: 6965 6e74 7320 6f66 2074 6865 2057 6f72  ients of the Wor
+00001a00: 6b20 6f72 0a20 2020 2020 2020 2020 2044  k or.          D
+00001a10: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+00001a20: 6120 636f 7079 206f 6620 7468 6973 204c  a copy of this L
+00001a30: 6963 656e 7365 3b20 616e 640a 0a20 2020  icense; and..   
+00001a40: 2020 2028 6229 2059 6f75 206d 7573 7420     (b) You must 
+00001a50: 6361 7573 6520 616e 7920 6d6f 6469 6669  cause any modifi
+00001a60: 6564 2066 696c 6573 2074 6f20 6361 7272  ed files to carr
+00001a70: 7920 7072 6f6d 696e 656e 7420 6e6f 7469  y prominent noti
+00001a80: 6365 730a 2020 2020 2020 2020 2020 7374  ces.          st
+00001a90: 6174 696e 6720 7468 6174 2059 6f75 2063  ating that You c
+00001aa0: 6861 6e67 6564 2074 6865 2066 696c 6573  hanged the files
+00001ab0: 3b20 616e 640a 0a20 2020 2020 2028 6329  ; and..      (c)
+00001ac0: 2059 6f75 206d 7573 7420 7265 7461 696e   You must retain
+00001ad0: 2c20 696e 2074 6865 2053 6f75 7263 6520  , in the Source 
+00001ae0: 666f 726d 206f 6620 616e 7920 4465 7269  form of any Deri
+00001af0: 7661 7469 7665 2057 6f72 6b73 0a20 2020  vative Works.   
+00001b00: 2020 2020 2020 2074 6861 7420 596f 7520         that You 
+00001b10: 6469 7374 7269 6275 7465 2c20 616c 6c20  distribute, all 
+00001b20: 636f 7079 7269 6768 742c 2070 6174 656e  copyright, paten
+00001b30: 742c 2074 7261 6465 6d61 726b 2c20 616e  t, trademark, an
+00001b40: 640a 2020 2020 2020 2020 2020 6174 7472  d.          attr
+00001b50: 6962 7574 696f 6e20 6e6f 7469 6365 7320  ibution notices 
+00001b60: 6672 6f6d 2074 6865 2053 6f75 7263 6520  from the Source 
+00001b70: 666f 726d 206f 6620 7468 6520 576f 726b  form of the Work
+00001b80: 2c0a 2020 2020 2020 2020 2020 6578 636c  ,.          excl
+00001b90: 7564 696e 6720 7468 6f73 6520 6e6f 7469  uding those noti
+00001ba0: 6365 7320 7468 6174 2064 6f20 6e6f 7420  ces that do not 
+00001bb0: 7065 7274 6169 6e20 746f 2061 6e79 2070  pertain to any p
+00001bc0: 6172 7420 6f66 0a20 2020 2020 2020 2020  art of.         
+00001bd0: 2074 6865 2044 6572 6976 6174 6976 6520   the Derivative 
+00001be0: 576f 726b 733b 2061 6e64 0a0a 2020 2020  Works; and..    
+00001bf0: 2020 2864 2920 4966 2074 6865 2057 6f72    (d) If the Wor
+00001c00: 6b20 696e 636c 7564 6573 2061 2022 4e4f  k includes a "NO
+00001c10: 5449 4345 2220 7465 7874 2066 696c 6520  TICE" text file 
+00001c20: 6173 2070 6172 7420 6f66 2069 7473 0a20  as part of its. 
+00001c30: 2020 2020 2020 2020 2064 6973 7472 6962           distrib
+00001c40: 7574 696f 6e2c 2074 6865 6e20 616e 7920  ution, then any 
+00001c50: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
+00001c60: 2074 6861 7420 596f 7520 6469 7374 7269   that You distri
+00001c70: 6275 7465 206d 7573 740a 2020 2020 2020  bute must.      
+00001c80: 2020 2020 696e 636c 7564 6520 6120 7265      include a re
+00001c90: 6164 6162 6c65 2063 6f70 7920 6f66 2074  adable copy of t
+00001ca0: 6865 2061 7474 7269 6275 7469 6f6e 206e  he attribution n
+00001cb0: 6f74 6963 6573 2063 6f6e 7461 696e 6564  otices contained
+00001cc0: 0a20 2020 2020 2020 2020 2077 6974 6869  .          withi
+00001cd0: 6e20 7375 6368 204e 4f54 4943 4520 6669  n such NOTICE fi
+00001ce0: 6c65 2c20 6578 636c 7564 696e 6720 7468  le, excluding th
+00001cf0: 6f73 6520 6e6f 7469 6365 7320 7468 6174  ose notices that
+00001d00: 2064 6f20 6e6f 740a 2020 2020 2020 2020   do not.        
+00001d10: 2020 7065 7274 6169 6e20 746f 2061 6e79    pertain to any
+00001d20: 2070 6172 7420 6f66 2074 6865 2044 6572   part of the Der
+00001d30: 6976 6174 6976 6520 576f 726b 732c 2069  ivative Works, i
+00001d40: 6e20 6174 206c 6561 7374 206f 6e65 0a20  n at least one. 
+00001d50: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00001d60: 666f 6c6c 6f77 696e 6720 706c 6163 6573  following places
+00001d70: 3a20 7769 7468 696e 2061 204e 4f54 4943  : within a NOTIC
+00001d80: 4520 7465 7874 2066 696c 6520 6469 7374  E text file dist
+00001d90: 7269 6275 7465 640a 2020 2020 2020 2020  ributed.        
+00001da0: 2020 6173 2070 6172 7420 6f66 2074 6865    as part of the
+00001db0: 2044 6572 6976 6174 6976 6520 576f 726b   Derivative Work
+00001dc0: 733b 2077 6974 6869 6e20 7468 6520 536f  s; within the So
+00001dd0: 7572 6365 2066 6f72 6d20 6f72 0a20 2020  urce form or.   
+00001de0: 2020 2020 2020 2064 6f63 756d 656e 7461         documenta
+00001df0: 7469 6f6e 2c20 6966 2070 726f 7669 6465  tion, if provide
+00001e00: 6420 616c 6f6e 6720 7769 7468 2074 6865  d along with the
+00001e10: 2044 6572 6976 6174 6976 6520 576f 726b   Derivative Work
+00001e20: 733b 206f 722c 0a20 2020 2020 2020 2020  s; or,.         
+00001e30: 2077 6974 6869 6e20 6120 6469 7370 6c61   within a displa
+00001e40: 7920 6765 6e65 7261 7465 6420 6279 2074  y generated by t
+00001e50: 6865 2044 6572 6976 6174 6976 6520 576f  he Derivative Wo
+00001e60: 726b 732c 2069 6620 616e 640a 2020 2020  rks, if and.    
+00001e70: 2020 2020 2020 7768 6572 6576 6572 2073        wherever s
+00001e80: 7563 6820 7468 6972 642d 7061 7274 7920  uch third-party 
+00001e90: 6e6f 7469 6365 7320 6e6f 726d 616c 6c79  notices normally
+00001ea0: 2061 7070 6561 722e 2054 6865 2063 6f6e   appear. The con
+00001eb0: 7465 6e74 730a 2020 2020 2020 2020 2020  tents.          
+00001ec0: 6f66 2074 6865 204e 4f54 4943 4520 6669  of the NOTICE fi
+00001ed0: 6c65 2061 7265 2066 6f72 2069 6e66 6f72  le are for infor
+00001ee0: 6d61 7469 6f6e 616c 2070 7572 706f 7365  mational purpose
+00001ef0: 7320 6f6e 6c79 2061 6e64 0a20 2020 2020  s only and.     
+00001f00: 2020 2020 2064 6f20 6e6f 7420 6d6f 6469       do not modi
+00001f10: 6679 2074 6865 204c 6963 656e 7365 2e20  fy the License. 
+00001f20: 596f 7520 6d61 7920 6164 6420 596f 7572  You may add Your
+00001f30: 206f 776e 2061 7474 7269 6275 7469 6f6e   own attribution
+00001f40: 0a20 2020 2020 2020 2020 206e 6f74 6963  .          notic
+00001f50: 6573 2077 6974 6869 6e20 4465 7269 7661  es within Deriva
+00001f60: 7469 7665 2057 6f72 6b73 2074 6861 7420  tive Works that 
+00001f70: 596f 7520 6469 7374 7269 6275 7465 2c20  You distribute, 
+00001f80: 616c 6f6e 6773 6964 650a 2020 2020 2020  alongside.      
+00001f90: 2020 2020 6f72 2061 7320 616e 2061 6464      or as an add
+00001fa0: 656e 6475 6d20 746f 2074 6865 204e 4f54  endum to the NOT
+00001fb0: 4943 4520 7465 7874 2066 726f 6d20 7468  ICE text from th
+00001fc0: 6520 576f 726b 2c20 7072 6f76 6964 6564  e Work, provided
+00001fd0: 0a20 2020 2020 2020 2020 2074 6861 7420  .          that 
+00001fe0: 7375 6368 2061 6464 6974 696f 6e61 6c20  such additional 
+00001ff0: 6174 7472 6962 7574 696f 6e20 6e6f 7469  attribution noti
+00002000: 6365 7320 6361 6e6e 6f74 2062 6520 636f  ces cannot be co
+00002010: 6e73 7472 7565 640a 2020 2020 2020 2020  nstrued.        
+00002020: 2020 6173 206d 6f64 6966 7969 6e67 2074    as modifying t
+00002030: 6865 204c 6963 656e 7365 2e0a 0a20 2020  he License...   
+00002040: 2020 2059 6f75 206d 6179 2061 6464 2059     You may add Y
+00002050: 6f75 7220 6f77 6e20 636f 7079 7269 6768  our own copyrigh
+00002060: 7420 7374 6174 656d 656e 7420 746f 2059  t statement to Y
+00002070: 6f75 7220 6d6f 6469 6669 6361 7469 6f6e  our modification
+00002080: 7320 616e 640a 2020 2020 2020 6d61 7920  s and.      may 
+00002090: 7072 6f76 6964 6520 6164 6469 7469 6f6e  provide addition
+000020a0: 616c 206f 7220 6469 6666 6572 656e 7420  al or different 
+000020b0: 6c69 6365 6e73 6520 7465 726d 7320 616e  license terms an
+000020c0: 6420 636f 6e64 6974 696f 6e73 0a20 2020  d conditions.   
+000020d0: 2020 2066 6f72 2075 7365 2c20 7265 7072     for use, repr
+000020e0: 6f64 7563 7469 6f6e 2c20 6f72 2064 6973  oduction, or dis
+000020f0: 7472 6962 7574 696f 6e20 6f66 2059 6f75  tribution of You
+00002100: 7220 6d6f 6469 6669 6361 7469 6f6e 732c  r modifications,
+00002110: 206f 720a 2020 2020 2020 666f 7220 616e   or.      for an
+00002120: 7920 7375 6368 2044 6572 6976 6174 6976  y such Derivativ
+00002130: 6520 576f 726b 7320 6173 2061 2077 686f  e Works as a who
+00002140: 6c65 2c20 7072 6f76 6964 6564 2059 6f75  le, provided You
+00002150: 7220 7573 652c 0a20 2020 2020 2072 6570  r use,.      rep
+00002160: 726f 6475 6374 696f 6e2c 2061 6e64 2064  roduction, and d
+00002170: 6973 7472 6962 7574 696f 6e20 6f66 2074  istribution of t
+00002180: 6865 2057 6f72 6b20 6f74 6865 7277 6973  he Work otherwis
+00002190: 6520 636f 6d70 6c69 6573 2077 6974 680a  e complies with.
+000021a0: 2020 2020 2020 7468 6520 636f 6e64 6974        the condit
+000021b0: 696f 6e73 2073 7461 7465 6420 696e 2074  ions stated in t
+000021c0: 6869 7320 4c69 6365 6e73 652e 0a0a 2020  his License...  
+000021d0: 2035 2e20 5375 626d 6973 7369 6f6e 206f   5. Submission o
+000021e0: 6620 436f 6e74 7269 6275 7469 6f6e 732e  f Contributions.
+000021f0: 2055 6e6c 6573 7320 596f 7520 6578 706c   Unless You expl
+00002200: 6963 6974 6c79 2073 7461 7465 206f 7468  icitly state oth
+00002210: 6572 7769 7365 2c0a 2020 2020 2020 616e  erwise,.      an
+00002220: 7920 436f 6e74 7269 6275 7469 6f6e 2069  y Contribution i
+00002230: 6e74 656e 7469 6f6e 616c 6c79 2073 7562  ntentionally sub
+00002240: 6d69 7474 6564 2066 6f72 2069 6e63 6c75  mitted for inclu
+00002250: 7369 6f6e 2069 6e20 7468 6520 576f 726b  sion in the Work
+00002260: 0a20 2020 2020 2062 7920 596f 7520 746f  .      by You to
+00002270: 2074 6865 204c 6963 656e 736f 7220 7368   the Licensor sh
+00002280: 616c 6c20 6265 2075 6e64 6572 2074 6865  all be under the
+00002290: 2074 6572 6d73 2061 6e64 2063 6f6e 6469   terms and condi
+000022a0: 7469 6f6e 7320 6f66 0a20 2020 2020 2074  tions of.      t
+000022b0: 6869 7320 4c69 6365 6e73 652c 2077 6974  his License, wit
+000022c0: 686f 7574 2061 6e79 2061 6464 6974 696f  hout any additio
+000022d0: 6e61 6c20 7465 726d 7320 6f72 2063 6f6e  nal terms or con
+000022e0: 6469 7469 6f6e 732e 0a20 2020 2020 204e  ditions..      N
+000022f0: 6f74 7769 7468 7374 616e 6469 6e67 2074  otwithstanding t
+00002300: 6865 2061 626f 7665 2c20 6e6f 7468 696e  he above, nothin
+00002310: 6720 6865 7265 696e 2073 6861 6c6c 2073  g herein shall s
+00002320: 7570 6572 7365 6465 206f 7220 6d6f 6469  upersede or modi
+00002330: 6679 0a20 2020 2020 2074 6865 2074 6572  fy.      the ter
+00002340: 6d73 206f 6620 616e 7920 7365 7061 7261  ms of any separa
+00002350: 7465 206c 6963 656e 7365 2061 6772 6565  te license agree
+00002360: 6d65 6e74 2079 6f75 206d 6179 2068 6176  ment you may hav
+00002370: 6520 6578 6563 7574 6564 0a20 2020 2020  e executed.     
+00002380: 2077 6974 6820 4c69 6365 6e73 6f72 2072   with Licensor r
+00002390: 6567 6172 6469 6e67 2073 7563 6820 436f  egarding such Co
+000023a0: 6e74 7269 6275 7469 6f6e 732e 0a0a 2020  ntributions...  
+000023b0: 2036 2e20 5472 6164 656d 6172 6b73 2e20   6. Trademarks. 
+000023c0: 5468 6973 204c 6963 656e 7365 2064 6f65  This License doe
+000023d0: 7320 6e6f 7420 6772 616e 7420 7065 726d  s not grant perm
+000023e0: 6973 7369 6f6e 2074 6f20 7573 6520 7468  ission to use th
+000023f0: 6520 7472 6164 650a 2020 2020 2020 6e61  e trade.      na
+00002400: 6d65 732c 2074 7261 6465 6d61 726b 732c  mes, trademarks,
+00002410: 2073 6572 7669 6365 206d 6172 6b73 2c20   service marks, 
+00002420: 6f72 2070 726f 6475 6374 206e 616d 6573  or product names
+00002430: 206f 6620 7468 6520 4c69 6365 6e73 6f72   of the Licensor
+00002440: 2c0a 2020 2020 2020 6578 6365 7074 2061  ,.      except a
+00002450: 7320 7265 7175 6972 6564 2066 6f72 2072  s required for r
+00002460: 6561 736f 6e61 626c 6520 616e 6420 6375  easonable and cu
+00002470: 7374 6f6d 6172 7920 7573 6520 696e 2064  stomary use in d
+00002480: 6573 6372 6962 696e 6720 7468 650a 2020  escribing the.  
+00002490: 2020 2020 6f72 6967 696e 206f 6620 7468      origin of th
+000024a0: 6520 576f 726b 2061 6e64 2072 6570 726f  e Work and repro
+000024b0: 6475 6369 6e67 2074 6865 2063 6f6e 7465  ducing the conte
+000024c0: 6e74 206f 6620 7468 6520 4e4f 5449 4345  nt of the NOTICE
+000024d0: 2066 696c 652e 0a0a 2020 2037 2e20 4469   file...   7. Di
+000024e0: 7363 6c61 696d 6572 206f 6620 5761 7272  sclaimer of Warr
+000024f0: 616e 7479 2e20 556e 6c65 7373 2072 6571  anty. Unless req
+00002500: 7569 7265 6420 6279 2061 7070 6c69 6361  uired by applica
+00002510: 626c 6520 6c61 7720 6f72 0a20 2020 2020  ble law or.     
+00002520: 2061 6772 6565 6420 746f 2069 6e20 7772   agreed to in wr
+00002530: 6974 696e 672c 204c 6963 656e 736f 7220  iting, Licensor 
+00002540: 7072 6f76 6964 6573 2074 6865 2057 6f72  provides the Wor
+00002550: 6b20 2861 6e64 2065 6163 680a 2020 2020  k (and each.    
+00002560: 2020 436f 6e74 7269 6275 746f 7220 7072    Contributor pr
+00002570: 6f76 6964 6573 2069 7473 2043 6f6e 7472  ovides its Contr
+00002580: 6962 7574 696f 6e73 2920 6f6e 2061 6e20  ibutions) on an 
+00002590: 2241 5320 4953 2220 4241 5349 532c 0a20  "AS IS" BASIS,. 
+000025a0: 2020 2020 2057 4954 484f 5554 2057 4152       WITHOUT WAR
+000025b0: 5241 4e54 4945 5320 4f52 2043 4f4e 4449  RANTIES OR CONDI
+000025c0: 5449 4f4e 5320 4f46 2041 4e59 204b 494e  TIONS OF ANY KIN
+000025d0: 442c 2065 6974 6865 7220 6578 7072 6573  D, either expres
+000025e0: 7320 6f72 0a20 2020 2020 2069 6d70 6c69  s or.      impli
+000025f0: 6564 2c20 696e 636c 7564 696e 672c 2077  ed, including, w
+00002600: 6974 686f 7574 206c 696d 6974 6174 696f  ithout limitatio
+00002610: 6e2c 2061 6e79 2077 6172 7261 6e74 6965  n, any warrantie
+00002620: 7320 6f72 2063 6f6e 6469 7469 6f6e 730a  s or conditions.
+00002630: 2020 2020 2020 6f66 2054 4954 4c45 2c20        of TITLE, 
+00002640: 4e4f 4e2d 494e 4652 494e 4745 4d45 4e54  NON-INFRINGEMENT
+00002650: 2c20 4d45 5243 4841 4e54 4142 494c 4954  , MERCHANTABILIT
+00002660: 592c 206f 7220 4649 544e 4553 5320 464f  Y, or FITNESS FO
+00002670: 5220 410a 2020 2020 2020 5041 5254 4943  R A.      PARTIC
+00002680: 554c 4152 2050 5552 504f 5345 2e20 596f  ULAR PURPOSE. Yo
+00002690: 7520 6172 6520 736f 6c65 6c79 2072 6573  u are solely res
+000026a0: 706f 6e73 6962 6c65 2066 6f72 2064 6574  ponsible for det
+000026b0: 6572 6d69 6e69 6e67 2074 6865 0a20 2020  ermining the.   
+000026c0: 2020 2061 7070 726f 7072 6961 7465 6e65     appropriatene
+000026d0: 7373 206f 6620 7573 696e 6720 6f72 2072  ss of using or r
+000026e0: 6564 6973 7472 6962 7574 696e 6720 7468  edistributing th
+000026f0: 6520 576f 726b 2061 6e64 2061 7373 756d  e Work and assum
+00002700: 6520 616e 790a 2020 2020 2020 7269 736b  e any.      risk
+00002710: 7320 6173 736f 6369 6174 6564 2077 6974  s associated wit
+00002720: 6820 596f 7572 2065 7865 7263 6973 6520  h Your exercise 
+00002730: 6f66 2070 6572 6d69 7373 696f 6e73 2075  of permissions u
+00002740: 6e64 6572 2074 6869 7320 4c69 6365 6e73  nder this Licens
+00002750: 652e 0a0a 2020 2038 2e20 4c69 6d69 7461  e...   8. Limita
+00002760: 7469 6f6e 206f 6620 4c69 6162 696c 6974  tion of Liabilit
+00002770: 792e 2049 6e20 6e6f 2065 7665 6e74 2061  y. In no event a
+00002780: 6e64 2075 6e64 6572 206e 6f20 6c65 6761  nd under no lega
+00002790: 6c20 7468 656f 7279 2c0a 2020 2020 2020  l theory,.      
+000027a0: 7768 6574 6865 7220 696e 2074 6f72 7420  whether in tort 
+000027b0: 2869 6e63 6c75 6469 6e67 206e 6567 6c69  (including negli
+000027c0: 6765 6e63 6529 2c20 636f 6e74 7261 6374  gence), contract
+000027d0: 2c20 6f72 206f 7468 6572 7769 7365 2c0a  , or otherwise,.
+000027e0: 2020 2020 2020 756e 6c65 7373 2072 6571        unless req
+000027f0: 7569 7265 6420 6279 2061 7070 6c69 6361  uired by applica
+00002800: 626c 6520 6c61 7720 2873 7563 6820 6173  ble law (such as
+00002810: 2064 656c 6962 6572 6174 6520 616e 6420   deliberate and 
+00002820: 6772 6f73 736c 790a 2020 2020 2020 6e65  grossly.      ne
+00002830: 676c 6967 656e 7420 6163 7473 2920 6f72  gligent acts) or
+00002840: 2061 6772 6565 6420 746f 2069 6e20 7772   agreed to in wr
+00002850: 6974 696e 672c 2073 6861 6c6c 2061 6e79  iting, shall any
+00002860: 2043 6f6e 7472 6962 7574 6f72 2062 650a   Contributor be.
+00002870: 2020 2020 2020 6c69 6162 6c65 2074 6f20        liable to 
+00002880: 596f 7520 666f 7220 6461 6d61 6765 732c  You for damages,
+00002890: 2069 6e63 6c75 6469 6e67 2061 6e79 2064   including any d
+000028a0: 6972 6563 742c 2069 6e64 6972 6563 742c  irect, indirect,
+000028b0: 2073 7065 6369 616c 2c0a 2020 2020 2020   special,.      
+000028c0: 696e 6369 6465 6e74 616c 2c20 6f72 2063  incidental, or c
+000028d0: 6f6e 7365 7175 656e 7469 616c 2064 616d  onsequential dam
+000028e0: 6167 6573 206f 6620 616e 7920 6368 6172  ages of any char
+000028f0: 6163 7465 7220 6172 6973 696e 6720 6173  acter arising as
+00002900: 2061 0a20 2020 2020 2072 6573 756c 7420   a.      result 
+00002910: 6f66 2074 6869 7320 4c69 6365 6e73 6520  of this License 
+00002920: 6f72 206f 7574 206f 6620 7468 6520 7573  or out of the us
+00002930: 6520 6f72 2069 6e61 6269 6c69 7479 2074  e or inability t
+00002940: 6f20 7573 6520 7468 650a 2020 2020 2020  o use the.      
+00002950: 576f 726b 2028 696e 636c 7564 696e 6720  Work (including 
+00002960: 6275 7420 6e6f 7420 6c69 6d69 7465 6420  but not limited 
+00002970: 746f 2064 616d 6167 6573 2066 6f72 206c  to damages for l
+00002980: 6f73 7320 6f66 2067 6f6f 6477 696c 6c2c  oss of goodwill,
+00002990: 0a20 2020 2020 2077 6f72 6b20 7374 6f70  .      work stop
+000029a0: 7061 6765 2c20 636f 6d70 7574 6572 2066  page, computer f
+000029b0: 6169 6c75 7265 206f 7220 6d61 6c66 756e  ailure or malfun
+000029c0: 6374 696f 6e2c 206f 7220 616e 7920 616e  ction, or any an
+000029d0: 6420 616c 6c0a 2020 2020 2020 6f74 6865  d all.      othe
+000029e0: 7220 636f 6d6d 6572 6369 616c 2064 616d  r commercial dam
+000029f0: 6167 6573 206f 7220 6c6f 7373 6573 292c  ages or losses),
+00002a00: 2065 7665 6e20 6966 2073 7563 6820 436f   even if such Co
+00002a10: 6e74 7269 6275 746f 720a 2020 2020 2020  ntributor.      
+00002a20: 6861 7320 6265 656e 2061 6476 6973 6564  has been advised
+00002a30: 206f 6620 7468 6520 706f 7373 6962 696c   of the possibil
+00002a40: 6974 7920 6f66 2073 7563 6820 6461 6d61  ity of such dama
+00002a50: 6765 732e 0a0a 2020 2039 2e20 4163 6365  ges...   9. Acce
+00002a60: 7074 696e 6720 5761 7272 616e 7479 206f  pting Warranty o
+00002a70: 7220 4164 6469 7469 6f6e 616c 204c 6961  r Additional Lia
+00002a80: 6269 6c69 7479 2e20 5768 696c 6520 7265  bility. While re
+00002a90: 6469 7374 7269 6275 7469 6e67 0a20 2020  distributing.   
+00002aa0: 2020 2074 6865 2057 6f72 6b20 6f72 2044     the Work or D
+00002ab0: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+00002ac0: 7468 6572 656f 662c 2059 6f75 206d 6179  thereof, You may
+00002ad0: 2063 686f 6f73 6520 746f 206f 6666 6572   choose to offer
+00002ae0: 2c0a 2020 2020 2020 616e 6420 6368 6172  ,.      and char
+00002af0: 6765 2061 2066 6565 2066 6f72 2c20 6163  ge a fee for, ac
+00002b00: 6365 7074 616e 6365 206f 6620 7375 7070  ceptance of supp
+00002b10: 6f72 742c 2077 6172 7261 6e74 792c 2069  ort, warranty, i
+00002b20: 6e64 656d 6e69 7479 2c0a 2020 2020 2020  ndemnity,.      
+00002b30: 6f72 206f 7468 6572 206c 6961 6269 6c69  or other liabili
+00002b40: 7479 206f 626c 6967 6174 696f 6e73 2061  ty obligations a
+00002b50: 6e64 2f6f 7220 7269 6768 7473 2063 6f6e  nd/or rights con
+00002b60: 7369 7374 656e 7420 7769 7468 2074 6869  sistent with thi
+00002b70: 730a 2020 2020 2020 4c69 6365 6e73 652e  s.      License.
+00002b80: 2048 6f77 6576 6572 2c20 696e 2061 6363   However, in acc
+00002b90: 6570 7469 6e67 2073 7563 6820 6f62 6c69  epting such obli
+00002ba0: 6761 7469 6f6e 732c 2059 6f75 206d 6179  gations, You may
+00002bb0: 2061 6374 206f 6e6c 790a 2020 2020 2020   act only.      
+00002bc0: 6f6e 2059 6f75 7220 6f77 6e20 6265 6861  on Your own beha
+00002bd0: 6c66 2061 6e64 206f 6e20 596f 7572 2073  lf and on Your s
+00002be0: 6f6c 6520 7265 7370 6f6e 7369 6269 6c69  ole responsibili
+00002bf0: 7479 2c20 6e6f 7420 6f6e 2062 6568 616c  ty, not on behal
+00002c00: 660a 2020 2020 2020 6f66 2061 6e79 206f  f.      of any o
+00002c10: 7468 6572 2043 6f6e 7472 6962 7574 6f72  ther Contributor
+00002c20: 2c20 616e 6420 6f6e 6c79 2069 6620 596f  , and only if Yo
+00002c30: 7520 6167 7265 6520 746f 2069 6e64 656d  u agree to indem
+00002c40: 6e69 6679 2c0a 2020 2020 2020 6465 6665  nify,.      defe
+00002c50: 6e64 2c20 616e 6420 686f 6c64 2065 6163  nd, and hold eac
+00002c60: 6820 436f 6e74 7269 6275 746f 7220 6861  h Contributor ha
+00002c70: 726d 6c65 7373 2066 6f72 2061 6e79 206c  rmless for any l
+00002c80: 6961 6269 6c69 7479 0a20 2020 2020 2069  iability.      i
+00002c90: 6e63 7572 7265 6420 6279 2c20 6f72 2063  ncurred by, or c
+00002ca0: 6c61 696d 7320 6173 7365 7274 6564 2061  laims asserted a
+00002cb0: 6761 696e 7374 2c20 7375 6368 2043 6f6e  gainst, such Con
+00002cc0: 7472 6962 7574 6f72 2062 7920 7265 6173  tributor by reas
+00002cd0: 6f6e 0a20 2020 2020 206f 6620 796f 7572  on.      of your
+00002ce0: 2061 6363 6570 7469 6e67 2061 6e79 2073   accepting any s
+00002cf0: 7563 6820 7761 7272 616e 7479 206f 7220  uch warranty or 
+00002d00: 6164 6469 7469 6f6e 616c 206c 6961 6269  additional liabi
+00002d10: 6c69 7479 2e0a 2d2d 2d2d 2d2d 2d2d 2d2d  lity..----------
 00002d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a70 7974  ------------.pyt
-00002d60: 686f 6e2d 6461 7465 7574 696c 0a43 6f70  hon-dateutil.Cop
-00002d70: 7972 6967 6874 2032 3031 372d 2050 6175  yright 2017- Pau
-00002d80: 6c20 4761 6e73 736c 6520 3c70 6175 6c40  l Ganssle <paul@
-00002d90: 6761 6e73 736c 652e 696f 3e0a 436f 7079  ganssle.io>.Copy
-00002da0: 7269 6768 7420 3230 3137 2d20 6461 7465  right 2017- date
-00002db0: 7574 696c 2063 6f6e 7472 6962 7574 6f72  util contributor
-00002dc0: 7320 2873 6565 2068 7474 7073 3a2f 2f67  s (see https://g
-00002dd0: 6974 6875 622e 636f 6d2f 6461 7465 7574  ithub.com/dateut
-00002de0: 696c 2f64 6174 6575 7469 6c2f 626c 6f62  il/dateutil/blob
-00002df0: 2f6d 6173 7465 722f 4155 5448 4f52 532e  /master/AUTHORS.
-00002e00: 6d64 290a 0a20 2020 4c69 6365 6e73 6564  md)..   Licensed
-00002e10: 2075 6e64 6572 2074 6865 2041 7061 6368   under the Apach
-00002e20: 6520 4c69 6365 6e73 652c 2056 6572 7369  e License, Versi
-00002e30: 6f6e 2032 2e30 2028 7468 6520 224c 6963  on 2.0 (the "Lic
-00002e40: 656e 7365 2229 3b0a 2020 2079 6f75 206d  ense");.   you m
-00002e50: 6179 206e 6f74 2075 7365 2074 6869 7320  ay not use this 
-00002e60: 6669 6c65 2065 7863 6570 7420 696e 2063  file except in c
-00002e70: 6f6d 706c 6961 6e63 6520 7769 7468 2074  ompliance with t
-00002e80: 6865 204c 6963 656e 7365 2e0a 2020 2059  he License..   Y
-00002e90: 6f75 206d 6179 206f 6274 6169 6e20 6120  ou may obtain a 
-00002ea0: 636f 7079 206f 6620 7468 6520 4c69 6365  copy of the Lice
-00002eb0: 6e73 6520 6174 0a0a 2020 2020 2020 2068  nse at..       h
-00002ec0: 7474 703a 2f2f 7777 772e 6170 6163 6865  ttp://www.apache
-00002ed0: 2e6f 7267 2f6c 6963 656e 7365 732f 4c49  .org/licenses/LI
-00002ee0: 4345 4e53 452d 322e 300a 0a20 2020 556e  CENSE-2.0..   Un
-00002ef0: 6c65 7373 2072 6571 7569 7265 6420 6279  less required by
-00002f00: 2061 7070 6c69 6361 626c 6520 6c61 7720   applicable law 
-00002f10: 6f72 2061 6772 6565 6420 746f 2069 6e20  or agreed to in 
-00002f20: 7772 6974 696e 672c 2073 6f66 7477 6172  writing, softwar
-00002f30: 650a 2020 2064 6973 7472 6962 7574 6564  e.   distributed
-00002f40: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
-00002f50: 7365 2069 7320 6469 7374 7269 6275 7465  se is distribute
-00002f60: 6420 6f6e 2061 6e20 2241 5320 4953 2220  d on an "AS IS" 
-00002f70: 4241 5349 532c 0a20 2020 5749 5448 4f55  BASIS,.   WITHOU
-00002f80: 5420 5741 5252 414e 5449 4553 204f 5220  T WARRANTIES OR 
-00002f90: 434f 4e44 4954 494f 4e53 204f 4620 414e  CONDITIONS OF AN
-00002fa0: 5920 4b49 4e44 2c20 6569 7468 6572 2065  Y KIND, either e
-00002fb0: 7870 7265 7373 206f 7220 696d 706c 6965  xpress or implie
-00002fc0: 642e 0a20 2020 5365 6520 7468 6520 4c69  d..   See the Li
-00002fd0: 6365 6e73 6520 666f 7220 7468 6520 7370  cense for the sp
-00002fe0: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
-00002ff0: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
-00003000: 7369 6f6e 7320 616e 640a 2020 206c 696d  sions and.   lim
-00003010: 6974 6174 696f 6e73 2075 6e64 6572 2074  itations under t
-00003020: 6865 204c 6963 656e 7365 2e0a 0a54 6865  he License...The
-00003030: 2061 626f 7665 206c 6963 656e 7365 2061   above license a
-00003040: 7070 6c69 6573 2074 6f20 616c 6c20 636f  pplies to all co
-00003050: 6e74 7269 6275 7469 6f6e 7320 6166 7465  ntributions afte
-00003060: 7220 3230 3137 2d31 322d 3031 2c20 6173  r 2017-12-01, as
-00003070: 2077 656c 6c20 6173 0a61 6c6c 2063 6f6e   well as.all con
-00003080: 7472 6962 7574 696f 6e73 2074 6861 7420  tributions that 
-00003090: 6861 7665 2062 6565 6e20 7265 2d6c 6963  have been re-lic
-000030a0: 656e 7365 6420 2873 6565 2041 5554 484f  ensed (see AUTHO
-000030b0: 5253 2066 696c 6520 666f 7220 7468 6520  RS file for the 
-000030c0: 6c69 7374 206f 660a 636f 6e74 7269 6275  list of.contribu
-000030d0: 746f 7273 2077 686f 2068 6176 6520 7265  tors who have re
-000030e0: 2d6c 6963 656e 7365 6420 7468 6569 7220  -licensed their 
-000030f0: 636f 6465 292e 0a2d 2d2d 2d2d 2d2d 2d2d  code)..---------
-00003100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d60: 2d2d 2d2d 2d2d 0a70 7974 686f 6e2d 6461  ------.python-da
+00002d70: 7465 7574 696c 0a43 6f70 7972 6967 6874  teutil.Copyright
+00002d80: 2032 3031 372d 2050 6175 6c20 4761 6e73   2017- Paul Gans
+00002d90: 736c 6520 3c70 6175 6c40 6761 6e73 736c  sle <paul@ganssl
+00002da0: 652e 696f 3e0a 436f 7079 7269 6768 7420  e.io>.Copyright 
+00002db0: 3230 3137 2d20 6461 7465 7574 696c 2063  2017- dateutil c
+00002dc0: 6f6e 7472 6962 7574 6f72 7320 2873 6565  ontributors (see
+00002dd0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002de0: 636f 6d2f 6461 7465 7574 696c 2f64 6174  com/dateutil/dat
+00002df0: 6575 7469 6c2f 626c 6f62 2f6d 6173 7465  eutil/blob/maste
+00002e00: 722f 4155 5448 4f52 532e 6d64 290a 0a20  r/AUTHORS.md).. 
+00002e10: 2020 4c69 6365 6e73 6564 2075 6e64 6572    Licensed under
+00002e20: 2074 6865 2041 7061 6368 6520 4c69 6365   the Apache Lice
+00002e30: 6e73 652c 2056 6572 7369 6f6e 2032 2e30  nse, Version 2.0
+00002e40: 2028 7468 6520 224c 6963 656e 7365 2229   (the "License")
+00002e50: 3b0a 2020 2079 6f75 206d 6179 206e 6f74  ;.   you may not
+00002e60: 2075 7365 2074 6869 7320 6669 6c65 2065   use this file e
+00002e70: 7863 6570 7420 696e 2063 6f6d 706c 6961  xcept in complia
+00002e80: 6e63 6520 7769 7468 2074 6865 204c 6963  nce with the Lic
+00002e90: 656e 7365 2e0a 2020 2059 6f75 206d 6179  ense..   You may
+00002ea0: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+00002eb0: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+00002ec0: 0a0a 2020 2020 2020 2068 7474 703a 2f2f  ..       http://
+00002ed0: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+00002ee0: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00002ef0: 322e 300a 0a20 2020 556e 6c65 7373 2072  2.0..   Unless r
+00002f00: 6571 7569 7265 6420 6279 2061 7070 6c69  equired by appli
+00002f10: 6361 626c 6520 6c61 7720 6f72 2061 6772  cable law or agr
+00002f20: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
+00002f30: 672c 2073 6f66 7477 6172 650a 2020 2064  g, software.   d
+00002f40: 6973 7472 6962 7574 6564 2075 6e64 6572  istributed under
+00002f50: 2074 6865 204c 6963 656e 7365 2069 7320   the License is 
+00002f60: 6469 7374 7269 6275 7465 6420 6f6e 2061  distributed on a
+00002f70: 6e20 2241 5320 4953 2220 4241 5349 532c  n "AS IS" BASIS,
+00002f80: 0a20 2020 5749 5448 4f55 5420 5741 5252  .   WITHOUT WARR
+00002f90: 414e 5449 4553 204f 5220 434f 4e44 4954  ANTIES OR CONDIT
+00002fa0: 494f 4e53 204f 4620 414e 5920 4b49 4e44  IONS OF ANY KIND
+00002fb0: 2c20 6569 7468 6572 2065 7870 7265 7373  , either express
+00002fc0: 206f 7220 696d 706c 6965 642e 0a20 2020   or implied..   
+00002fd0: 5365 6520 7468 6520 4c69 6365 6e73 6520  See the License 
+00002fe0: 666f 7220 7468 6520 7370 6563 6966 6963  for the specific
+00002ff0: 206c 616e 6775 6167 6520 676f 7665 726e   language govern
+00003000: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
+00003010: 616e 640a 2020 206c 696d 6974 6174 696f  and.   limitatio
+00003020: 6e73 2075 6e64 6572 2074 6865 204c 6963  ns under the Lic
+00003030: 656e 7365 2e0a 0a54 6865 2061 626f 7665  ense...The above
+00003040: 206c 6963 656e 7365 2061 7070 6c69 6573   license applies
+00003050: 2074 6f20 616c 6c20 636f 6e74 7269 6275   to all contribu
+00003060: 7469 6f6e 7320 6166 7465 7220 3230 3137  tions after 2017
+00003070: 2d31 322d 3031 2c20 6173 2077 656c 6c20  -12-01, as well 
+00003080: 6173 0a61 6c6c 2063 6f6e 7472 6962 7574  as.all contribut
+00003090: 696f 6e73 2074 6861 7420 6861 7665 2062  ions that have b
+000030a0: 6565 6e20 7265 2d6c 6963 656e 7365 6420  een re-licensed 
+000030b0: 2873 6565 2041 5554 484f 5253 2066 696c  (see AUTHORS fil
+000030c0: 6520 666f 7220 7468 6520 6c69 7374 206f  e for the list o
+000030d0: 660a 636f 6e74 7269 6275 746f 7273 2077  f.contributors w
+000030e0: 686f 2068 6176 6520 7265 2d6c 6963 656e  ho have re-licen
+000030f0: 7365 6420 7468 6569 7220 636f 6465 292e  sed their code).
+00003100: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
 00003110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003140: 2d2d 2d2d 2d2d 2d0a 6461 7465 7574 696c  -------.dateutil
-00003150: 202d 2045 7874 656e 7369 6f6e 7320 746f   - Extensions to
-00003160: 2074 6865 2073 7461 6e64 6172 6420 5079   the standard Py
-00003170: 7468 6f6e 2064 6174 6574 696d 6520 6d6f  thon datetime mo
-00003180: 6475 6c65 2e0a 0a43 6f70 7972 6967 6874  dule...Copyright
-00003190: 2028 6329 2032 3030 332d 3230 3131 202d   (c) 2003-2011 -
-000031a0: 2047 7573 7461 766f 204e 6965 6d65 7965   Gustavo Niemeye
-000031b0: 7220 3c67 7573 7461 766f 406e 6965 6d65  r <gustavo@nieme
-000031c0: 7965 722e 6e65 743e 0a43 6f70 7972 6967  yer.net>.Copyrig
-000031d0: 6874 2028 6329 2032 3031 322d 3230 3134  ht (c) 2012-2014
-000031e0: 202d 2054 6f6d 6920 5069 6576 696c c3a4   - Tomi Pievil..
-000031f0: 696e 656e 203c 746f 6d69 2e70 6965 7669  inen <tomi.pievi
-00003200: 6c61 696e 656e 4069 6b69 2e66 693e 0a43  lainen@iki.fi>.C
-00003210: 6f70 7972 6967 6874 2028 6329 2032 3031  opyright (c) 201
-00003220: 342d 3230 3136 202d 2059 6172 6f6e 2064  4-2016 - Yaron d
-00003230: 6520 4c65 6575 7720 3c6d 6540 6a61 726f  e Leeuw <me@jaro
-00003240: 6e64 6c2e 6e65 743e 0a43 6f70 7972 6967  ndl.net>.Copyrig
-00003250: 6874 2028 6329 2032 3031 352d 2020 2020  ht (c) 2015-    
-00003260: 202d 2050 6175 6c20 4761 6e73 736c 6520   - Paul Ganssle 
-00003270: 3c70 6175 6c40 6761 6e73 736c 652e 696f  <paul@ganssle.io
-00003280: 3e0a 436f 7079 7269 6768 7420 2863 2920  >.Copyright (c) 
-00003290: 3230 3135 2d20 2020 2020 2d20 6461 7465  2015-     - date
-000032a0: 7574 696c 2063 6f6e 7472 6962 7574 6f72  util contributor
-000032b0: 7320 2873 6565 2041 5554 484f 5253 2066  s (see AUTHORS f
-000032c0: 696c 6529 0a0a 416c 6c20 7269 6768 7473  ile)..All rights
-000032d0: 2072 6573 6572 7665 642e 0a0a 5265 6469   reserved...Redi
-000032e0: 7374 7269 6275 7469 6f6e 2061 6e64 2075  stribution and u
-000032f0: 7365 2069 6e20 736f 7572 6365 2061 6e64  se in source and
-00003300: 2062 696e 6172 7920 666f 726d 732c 2077   binary forms, w
-00003310: 6974 6820 6f72 2077 6974 686f 7574 0a6d  ith or without.m
-00003320: 6f64 6966 6963 6174 696f 6e2c 2061 7265  odification, are
-00003330: 2070 6572 6d69 7474 6564 2070 726f 7669   permitted provi
-00003340: 6465 6420 7468 6174 2074 6865 2066 6f6c  ded that the fol
-00003350: 6c6f 7769 6e67 2063 6f6e 6469 7469 6f6e  lowing condition
-00003360: 7320 6172 6520 6d65 743a 0a0a 2020 2020  s are met:..    
-00003370: 2a20 5265 6469 7374 7269 6275 7469 6f6e  * Redistribution
-00003380: 7320 6f66 2073 6f75 7263 6520 636f 6465  s of source code
-00003390: 206d 7573 7420 7265 7461 696e 2074 6865   must retain the
-000033a0: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
-000033b0: 206e 6f74 6963 652c 0a20 2020 2020 2074   notice,.      t
-000033c0: 6869 7320 6c69 7374 206f 6620 636f 6e64  his list of cond
-000033d0: 6974 696f 6e73 2061 6e64 2074 6865 2066  itions and the f
-000033e0: 6f6c 6c6f 7769 6e67 2064 6973 636c 6169  ollowing disclai
-000033f0: 6d65 722e 0a20 2020 202a 2052 6564 6973  mer..    * Redis
-00003400: 7472 6962 7574 696f 6e73 2069 6e20 6269  tributions in bi
-00003410: 6e61 7279 2066 6f72 6d20 6d75 7374 2072  nary form must r
-00003420: 6570 726f 6475 6365 2074 6865 2061 626f  eproduce the abo
-00003430: 7665 2063 6f70 7972 6967 6874 206e 6f74  ve copyright not
-00003440: 6963 652c 0a20 2020 2020 2074 6869 7320  ice,.      this 
-00003450: 6c69 7374 206f 6620 636f 6e64 6974 696f  list of conditio
-00003460: 6e73 2061 6e64 2074 6865 2066 6f6c 6c6f  ns and the follo
-00003470: 7769 6e67 2064 6973 636c 6169 6d65 7220  wing disclaimer 
-00003480: 696e 2074 6865 2064 6f63 756d 656e 7461  in the documenta
-00003490: 7469 6f6e 0a20 2020 2020 2061 6e64 2f6f  tion.      and/o
-000034a0: 7220 6f74 6865 7220 6d61 7465 7269 616c  r other material
-000034b0: 7320 7072 6f76 6964 6564 2077 6974 6820  s provided with 
-000034c0: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
-000034d0: 2e0a 2020 2020 2a20 4e65 6974 6865 7220  ..    * Neither 
-000034e0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-000034f0: 636f 7079 7269 6768 7420 686f 6c64 6572  copyright holder
-00003500: 206e 6f72 2074 6865 206e 616d 6573 206f   nor the names o
-00003510: 6620 6974 730a 2020 2020 2020 636f 6e74  f its.      cont
-00003520: 7269 6275 746f 7273 206d 6179 2062 6520  ributors may be 
-00003530: 7573 6564 2074 6f20 656e 646f 7273 6520  used to endorse 
-00003540: 6f72 2070 726f 6d6f 7465 2070 726f 6475  or promote produ
-00003550: 6374 7320 6465 7269 7665 6420 6672 6f6d  cts derived from
-00003560: 0a20 2020 2020 2074 6869 7320 736f 6674  .      this soft
-00003570: 7761 7265 2077 6974 686f 7574 2073 7065  ware without spe
-00003580: 6369 6669 6320 7072 696f 7220 7772 6974  cific prior writ
-00003590: 7465 6e20 7065 726d 6973 7369 6f6e 2e0a  ten permission..
-000035a0: 0a54 4849 5320 534f 4654 5741 5245 2049  .THIS SOFTWARE I
-000035b0: 5320 5052 4f56 4944 4544 2042 5920 5448  S PROVIDED BY TH
-000035c0: 4520 434f 5059 5249 4748 5420 484f 4c44  E COPYRIGHT HOLD
-000035d0: 4552 5320 414e 4420 434f 4e54 5249 4255  ERS AND CONTRIBU
-000035e0: 544f 5253 0a22 4153 2049 5322 2041 4e44  TORS."AS IS" AND
-000035f0: 2041 4e59 2045 5850 5245 5353 204f 5220   ANY EXPRESS OR 
-00003600: 494d 504c 4945 4420 5741 5252 414e 5449  IMPLIED WARRANTI
-00003610: 4553 2c20 494e 434c 5544 494e 472c 2042  ES, INCLUDING, B
-00003620: 5554 204e 4f54 0a4c 494d 4954 4544 2054  UT NOT.LIMITED T
-00003630: 4f2c 2054 4845 2049 4d50 4c49 4544 2057  O, THE IMPLIED W
-00003640: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
-00003650: 4348 414e 5441 4249 4c49 5459 2041 4e44  CHANTABILITY AND
-00003660: 2046 4954 4e45 5353 2046 4f52 0a41 2050   FITNESS FOR.A P
-00003670: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
-00003680: 4520 4152 4520 4449 5343 4c41 494d 4544  E ARE DISCLAIMED
-00003690: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
-000036a0: 414c 4c20 5448 4520 434f 5059 5249 4748  ALL THE COPYRIGH
-000036b0: 5420 4f57 4e45 5220 4f52 0a43 4f4e 5452  T OWNER OR.CONTR
-000036c0: 4942 5554 4f52 5320 4245 204c 4941 424c  IBUTORS BE LIABL
-000036d0: 4520 464f 5220 414e 5920 4449 5245 4354  E FOR ANY DIRECT
-000036e0: 2c20 494e 4449 5245 4354 2c20 494e 4349  , INDIRECT, INCI
-000036f0: 4445 4e54 414c 2c20 5350 4543 4941 4c2c  DENTAL, SPECIAL,
-00003700: 0a45 5845 4d50 4c41 5259 2c20 4f52 2043  .EXEMPLARY, OR C
-00003710: 4f4e 5345 5155 454e 5449 414c 2044 414d  ONSEQUENTIAL DAM
-00003720: 4147 4553 2028 494e 434c 5544 494e 472c  AGES (INCLUDING,
-00003730: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
-00003740: 2054 4f2c 0a50 524f 4355 5245 4d45 4e54   TO,.PROCUREMENT
-00003750: 204f 4620 5355 4253 5449 5455 5445 2047   OF SUBSTITUTE G
-00003760: 4f4f 4453 204f 5220 5345 5256 4943 4553  OODS OR SERVICES
-00003770: 3b20 4c4f 5353 204f 4620 5553 452c 2044  ; LOSS OF USE, D
-00003780: 4154 412c 204f 520a 5052 4f46 4954 533b  ATA, OR.PROFITS;
-00003790: 204f 5220 4255 5349 4e45 5353 2049 4e54   OR BUSINESS INT
-000037a0: 4552 5255 5054 494f 4e29 2048 4f57 4556  ERRUPTION) HOWEV
-000037b0: 4552 2043 4155 5345 4420 414e 4420 4f4e  ER CAUSED AND ON
-000037c0: 2041 4e59 2054 4845 4f52 5920 4f46 0a4c   ANY THEORY OF.L
-000037d0: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
-000037e0: 5220 494e 2043 4f4e 5452 4143 542c 2053  R IN CONTRACT, S
-000037f0: 5452 4943 5420 4c49 4142 494c 4954 592c  TRICT LIABILITY,
-00003800: 204f 5220 544f 5254 2028 494e 434c 5544   OR TORT (INCLUD
-00003810: 494e 470a 4e45 474c 4947 454e 4345 204f  ING.NEGLIGENCE O
-00003820: 5220 4f54 4845 5257 4953 4529 2041 5249  R OTHERWISE) ARI
-00003830: 5349 4e47 2049 4e20 414e 5920 5741 5920  SING IN ANY WAY 
-00003840: 4f55 5420 4f46 2054 4845 2055 5345 204f  OUT OF THE USE O
-00003850: 4620 5448 4953 0a53 4f46 5457 4152 452c  F THIS.SOFTWARE,
-00003860: 2045 5645 4e20 4946 2041 4456 4953 4544   EVEN IF ADVISED
-00003870: 204f 4620 5448 4520 504f 5353 4942 494c   OF THE POSSIBIL
-00003880: 4954 5920 4f46 2053 5543 4820 4441 4d41  ITY OF SUCH DAMA
-00003890: 4745 2e0a 0a54 6865 2061 626f 7665 2042  GE...The above B
-000038a0: 5344 204c 6963 656e 7365 2041 7070 6c69  SD License Appli
-000038b0: 6573 2074 6f20 616c 6c20 636f 6465 2c20  es to all code, 
-000038c0: 6576 656e 2074 6861 7420 616c 736f 2063  even that also c
-000038d0: 6f76 6572 6564 2062 7920 4170 6163 6865  overed by Apache
-000038e0: 2032 2e30 2e0a 2d2d 2d2d 2d2d 2d2d 2d2d   2.0..----------
+00003140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003150: 2d0a 6461 7465 7574 696c 202d 2045 7874  -.dateutil - Ext
+00003160: 656e 7369 6f6e 7320 746f 2074 6865 2073  ensions to the s
+00003170: 7461 6e64 6172 6420 5079 7468 6f6e 2064  tandard Python d
+00003180: 6174 6574 696d 6520 6d6f 6475 6c65 2e0a  atetime module..
+00003190: 0a43 6f70 7972 6967 6874 2028 6329 2032  .Copyright (c) 2
+000031a0: 3030 332d 3230 3131 202d 2047 7573 7461  003-2011 - Gusta
+000031b0: 766f 204e 6965 6d65 7965 7220 3c67 7573  vo Niemeyer <gus
+000031c0: 7461 766f 406e 6965 6d65 7965 722e 6e65  tavo@niemeyer.ne
+000031d0: 743e 0a43 6f70 7972 6967 6874 2028 6329  t>.Copyright (c)
+000031e0: 2032 3031 322d 3230 3134 202d 2054 6f6d   2012-2014 - Tom
+000031f0: 6920 5069 6576 696c c3a4 696e 656e 203c  i Pievil..inen <
+00003200: 746f 6d69 2e70 6965 7669 6c61 696e 656e  tomi.pievilainen
+00003210: 4069 6b69 2e66 693e 0a43 6f70 7972 6967  @iki.fi>.Copyrig
+00003220: 6874 2028 6329 2032 3031 342d 3230 3136  ht (c) 2014-2016
+00003230: 202d 2059 6172 6f6e 2064 6520 4c65 6575   - Yaron de Leeu
+00003240: 7720 3c6d 6540 6a61 726f 6e64 6c2e 6e65  w <me@jarondl.ne
+00003250: 743e 0a43 6f70 7972 6967 6874 2028 6329  t>.Copyright (c)
+00003260: 2032 3031 352d 2020 2020 202d 2050 6175   2015-     - Pau
+00003270: 6c20 4761 6e73 736c 6520 3c70 6175 6c40  l Ganssle <paul@
+00003280: 6761 6e73 736c 652e 696f 3e0a 436f 7079  ganssle.io>.Copy
+00003290: 7269 6768 7420 2863 2920 3230 3135 2d20  right (c) 2015- 
+000032a0: 2020 2020 2d20 6461 7465 7574 696c 2063      - dateutil c
+000032b0: 6f6e 7472 6962 7574 6f72 7320 2873 6565  ontributors (see
+000032c0: 2041 5554 484f 5253 2066 696c 6529 0a0a   AUTHORS file)..
+000032d0: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
+000032e0: 7665 642e 0a0a 5265 6469 7374 7269 6275  ved...Redistribu
+000032f0: 7469 6f6e 2061 6e64 2075 7365 2069 6e20  tion and use in 
+00003300: 736f 7572 6365 2061 6e64 2062 696e 6172  source and binar
+00003310: 7920 666f 726d 732c 2077 6974 6820 6f72  y forms, with or
+00003320: 2077 6974 686f 7574 0a6d 6f64 6966 6963   without.modific
+00003330: 6174 696f 6e2c 2061 7265 2070 6572 6d69  ation, are permi
+00003340: 7474 6564 2070 726f 7669 6465 6420 7468  tted provided th
+00003350: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
+00003360: 2063 6f6e 6469 7469 6f6e 7320 6172 6520   conditions are 
+00003370: 6d65 743a 0a0a 2020 2020 2a20 5265 6469  met:..    * Redi
+00003380: 7374 7269 6275 7469 6f6e 7320 6f66 2073  stributions of s
+00003390: 6f75 7263 6520 636f 6465 206d 7573 7420  ource code must 
+000033a0: 7265 7461 696e 2074 6865 2061 626f 7665  retain the above
+000033b0: 2063 6f70 7972 6967 6874 206e 6f74 6963   copyright notic
+000033c0: 652c 0a20 2020 2020 2074 6869 7320 6c69  e,.      this li
+000033d0: 7374 206f 6620 636f 6e64 6974 696f 6e73  st of conditions
+000033e0: 2061 6e64 2074 6865 2066 6f6c 6c6f 7769   and the followi
+000033f0: 6e67 2064 6973 636c 6169 6d65 722e 0a20  ng disclaimer.. 
+00003400: 2020 202a 2052 6564 6973 7472 6962 7574     * Redistribut
+00003410: 696f 6e73 2069 6e20 6269 6e61 7279 2066  ions in binary f
+00003420: 6f72 6d20 6d75 7374 2072 6570 726f 6475  orm must reprodu
+00003430: 6365 2074 6865 2061 626f 7665 2063 6f70  ce the above cop
+00003440: 7972 6967 6874 206e 6f74 6963 652c 0a20  yright notice,. 
+00003450: 2020 2020 2074 6869 7320 6c69 7374 206f       this list o
+00003460: 6620 636f 6e64 6974 696f 6e73 2061 6e64  f conditions and
+00003470: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+00003480: 6973 636c 6169 6d65 7220 696e 2074 6865  isclaimer in the
+00003490: 2064 6f63 756d 656e 7461 7469 6f6e 0a20   documentation. 
+000034a0: 2020 2020 2061 6e64 2f6f 7220 6f74 6865       and/or othe
+000034b0: 7220 6d61 7465 7269 616c 7320 7072 6f76  r materials prov
+000034c0: 6964 6564 2077 6974 6820 7468 6520 6469  ided with the di
+000034d0: 7374 7269 6275 7469 6f6e 2e0a 2020 2020  stribution..    
+000034e0: 2a20 4e65 6974 6865 7220 7468 6520 6e61  * Neither the na
+000034f0: 6d65 206f 6620 7468 6520 636f 7079 7269  me of the copyri
+00003500: 6768 7420 686f 6c64 6572 206e 6f72 2074  ght holder nor t
+00003510: 6865 206e 616d 6573 206f 6620 6974 730a  he names of its.
+00003520: 2020 2020 2020 636f 6e74 7269 6275 746f        contributo
+00003530: 7273 206d 6179 2062 6520 7573 6564 2074  rs may be used t
+00003540: 6f20 656e 646f 7273 6520 6f72 2070 726f  o endorse or pro
+00003550: 6d6f 7465 2070 726f 6475 6374 7320 6465  mote products de
+00003560: 7269 7665 6420 6672 6f6d 0a20 2020 2020  rived from.     
+00003570: 2074 6869 7320 736f 6674 7761 7265 2077   this software w
+00003580: 6974 686f 7574 2073 7065 6369 6669 6320  ithout specific 
+00003590: 7072 696f 7220 7772 6974 7465 6e20 7065  prior written pe
+000035a0: 726d 6973 7369 6f6e 2e0a 0a54 4849 5320  rmission...THIS 
+000035b0: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
+000035c0: 4944 4544 2042 5920 5448 4520 434f 5059  IDED BY THE COPY
+000035d0: 5249 4748 5420 484f 4c44 4552 5320 414e  RIGHT HOLDERS AN
+000035e0: 4420 434f 4e54 5249 4255 544f 5253 0a22  D CONTRIBUTORS."
+000035f0: 4153 2049 5322 2041 4e44 2041 4e59 2045  AS IS" AND ANY E
+00003600: 5850 5245 5353 204f 5220 494d 504c 4945  XPRESS OR IMPLIE
+00003610: 4420 5741 5252 414e 5449 4553 2c20 494e  D WARRANTIES, IN
+00003620: 434c 5544 494e 472c 2042 5554 204e 4f54  CLUDING, BUT NOT
+00003630: 0a4c 494d 4954 4544 2054 4f2c 2054 4845  .LIMITED TO, THE
+00003640: 2049 4d50 4c49 4544 2057 4152 5241 4e54   IMPLIED WARRANT
+00003650: 4945 5320 4f46 204d 4552 4348 414e 5441  IES OF MERCHANTA
+00003660: 4249 4c49 5459 2041 4e44 2046 4954 4e45  BILITY AND FITNE
+00003670: 5353 2046 4f52 0a41 2050 4152 5449 4355  SS FOR.A PARTICU
+00003680: 4c41 5220 5055 5250 4f53 4520 4152 4520  LAR PURPOSE ARE 
+00003690: 4449 5343 4c41 494d 4544 2e20 494e 204e  DISCLAIMED. IN N
+000036a0: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
+000036b0: 4520 434f 5059 5249 4748 5420 4f57 4e45  E COPYRIGHT OWNE
+000036c0: 5220 4f52 0a43 4f4e 5452 4942 5554 4f52  R OR.CONTRIBUTOR
+000036d0: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
+000036e0: 414e 5920 4449 5245 4354 2c20 494e 4449  ANY DIRECT, INDI
+000036f0: 5245 4354 2c20 494e 4349 4445 4e54 414c  RECT, INCIDENTAL
+00003700: 2c20 5350 4543 4941 4c2c 0a45 5845 4d50  , SPECIAL,.EXEMP
+00003710: 4c41 5259 2c20 4f52 2043 4f4e 5345 5155  LARY, OR CONSEQU
+00003720: 454e 5449 414c 2044 414d 4147 4553 2028  ENTIAL DAMAGES (
+00003730: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
+00003740: 4f54 204c 494d 4954 4544 2054 4f2c 0a50  OT LIMITED TO,.P
+00003750: 524f 4355 5245 4d45 4e54 204f 4620 5355  ROCUREMENT OF SU
+00003760: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
+00003770: 5220 5345 5256 4943 4553 3b20 4c4f 5353  R SERVICES; LOSS
+00003780: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
+00003790: 520a 5052 4f46 4954 533b 204f 5220 4255  R.PROFITS; OR BU
+000037a0: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
+000037b0: 494f 4e29 2048 4f57 4556 4552 2043 4155  ION) HOWEVER CAU
+000037c0: 5345 4420 414e 4420 4f4e 2041 4e59 2054  SED AND ON ANY T
+000037d0: 4845 4f52 5920 4f46 0a4c 4941 4249 4c49  HEORY OF.LIABILI
+000037e0: 5459 2c20 5748 4554 4845 5220 494e 2043  TY, WHETHER IN C
+000037f0: 4f4e 5452 4143 542c 2053 5452 4943 5420  ONTRACT, STRICT 
+00003800: 4c49 4142 494c 4954 592c 204f 5220 544f  LIABILITY, OR TO
+00003810: 5254 2028 494e 434c 5544 494e 470a 4e45  RT (INCLUDING.NE
+00003820: 474c 4947 454e 4345 204f 5220 4f54 4845  GLIGENCE OR OTHE
+00003830: 5257 4953 4529 2041 5249 5349 4e47 2049  RWISE) ARISING I
+00003840: 4e20 414e 5920 5741 5920 4f55 5420 4f46  N ANY WAY OUT OF
+00003850: 2054 4845 2055 5345 204f 4620 5448 4953   THE USE OF THIS
+00003860: 0a53 4f46 5457 4152 452c 2045 5645 4e20  .SOFTWARE, EVEN 
+00003870: 4946 2041 4456 4953 4544 204f 4620 5448  IF ADVISED OF TH
+00003880: 4520 504f 5353 4942 494c 4954 5920 4f46  E POSSIBILITY OF
+00003890: 2053 5543 4820 4441 4d41 4745 2e0a 0a54   SUCH DAMAGE...T
+000038a0: 6865 2061 626f 7665 2042 5344 204c 6963  he above BSD Lic
+000038b0: 656e 7365 2041 7070 6c69 6573 2074 6f20  ense Applies to 
+000038c0: 616c 6c20 636f 6465 2c20 6576 656e 2074  all code, even t
+000038d0: 6861 7420 616c 736f 2063 6f76 6572 6564  hat also covered
+000038e0: 2062 7920 4170 6163 6865 2032 2e30 2e0a   by Apache 2.0..
 000038f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003930: 2d2d 2d2d 2d2d 0a                        ------.
+00003930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003940: 0a                                       .
```

### Comparing `air-sdk-2.3.0/PKG-INFO` & `air-sdk-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: air-sdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python SDK for interacting with NVIDIA Air
 Home-page: https://github.com/NVIDIA/air_sdk
 Author: Mike Robertson
 Author-email: Mike Robertson <mrobertson@nvidia.com>
-License: SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+License: SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
         SPDX-License-Identifier: MIT
         
-        Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+        Copyright (c) 2022-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a
         copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense,
         and/or sell copies of the Software, and to permit persons to whom the
         Software is furnished to do so, subject to the following conditions:
```

### Comparing `air-sdk-2.3.0/README.md` & `air-sdk-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `air-sdk-2.3.0/air_sdk/account.py` & `air-sdk-2.4.0/air_sdk/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Account module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/air_api.py` & `air-sdk-2.4.0/air_sdk/air_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 NVIDIA Air API module
 """
 #pylint: disable=too-many-public-methods
 
@@ -24,14 +24,15 @@
 from .job import JobApi
 from .link import LinkApi
 from .login import LoginApi
 from .marketplace import MarketplaceApi
 from .node import NodeApi
 from .organization import OrganizationApi
 from .permission import PermissionApi
+from .resource_budget import ResourceBudgetApi
 from .service import ServiceApi
 from .ssh_key import SSHKeyApi
 from .simulation import SimulationApi
 from .simulation_interface import SimulationInterfaceApi
 from .simulation_node import SimulationNodeApi
 from .token import TokenApi
 from .topology import TopologyApi
@@ -132,14 +133,18 @@
         return self.permissions
 
     @property
     def permissions(self):
         return PermissionApi(self)
 
     @property
+    def resource_budgets(self):
+        return ResourceBudgetApi(self)
+
+    @property
     @util.deprecated('AirApi.services')
     def service(self):
         return self.services
 
     @property
     def services(self):
         return ServiceApi(self)
```

### Comparing `air-sdk-2.3.0/air_sdk/air_model.py` & `air-sdk-2.4.0/air_sdk/air_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Base classes for AIR object models
 """
 from datetime import date, datetime
 import json
```

### Comparing `air-sdk-2.3.0/air_sdk/capacity.py` & `air-sdk-2.4.0/air_sdk/capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Capacity module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/demo.py` & `air-sdk-2.4.0/air_sdk/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Demo module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/exceptions.py` & `air-sdk-2.4.0/air_sdk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Custom exceptions for the AIR SDK
 """
 class AirError(Exception):
     """
```

### Comparing `air-sdk-2.3.0/air_sdk/image.py` & `air-sdk-2.4.0/air_sdk/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Image module
 """
 
 from . import util
@@ -28,14 +28,40 @@
     ### update
     Update the image with the provided data
 
     Arguments:
         kwargs (dict, optional): All optional keyword arguments are applied as key/value
                 pairs in the request's JSON payload
     """
+    def copy(self, organization):
+        """
+        Make a copy of the image in another organization
+
+        Arguments:
+            organization (str | `Organization`): `Organization` or ID
+
+        Returns:
+        [`Image`](/docs/image)
+
+        Raises:
+        [`AirUnexpectedResposne`](/docs/exceptions) - Copy failed
+
+        Example:
+        ```
+        >>> image = air.images.get('33d8a377-ef0a-4a0d-ac2a-076e32678e18')
+        >>> target_org = air.organizations.get('b0e47509-4099-4e24-b96f-d1278d431f46')
+        >>> image.copy(target_org)
+        <Image cumulus-vx-5.4.0 3dadd54d-583c-432e-9383-a2b0b1d7f551>
+        ```
+        """
+        url = f'{self._api.url}{self.id}/copy/'
+        res = self._api.client.post(url, json={'organization': organization})
+        util.raise_if_invalid_response(res, status_code=201)
+        return Image(self._api, **res.json())
+
     def upload(self, filename):
         """
         Upload an image file
 
         Arguments:
             filename (str): Absolute path to the local image
```

### Comparing `air-sdk-2.3.0/air_sdk/interface.py` & `air-sdk-2.4.0/air_sdk/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Interface module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/job.py` & `air-sdk-2.4.0/air_sdk/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Job module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/link.py` & `air-sdk-2.4.0/air_sdk/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Link module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/login.py` & `air-sdk-2.4.0/air_sdk/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Login module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/marketplace.py` & `air-sdk-2.4.0/air_sdk/marketplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Marketplace Demo module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/node.py` & `air-sdk-2.4.0/air_sdk/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Node module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/organization.py` & `air-sdk-2.4.0/air_sdk/organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Organization module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/permission.py` & `air-sdk-2.4.0/air_sdk/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Permission module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/service.py` & `air-sdk-2.4.0/air_sdk/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Service module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/simulation.py` & `air-sdk-2.4.0/air_sdk/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Simulation module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/simulation_interface.py` & `air-sdk-2.4.0/air_sdk/simulation_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 SimulationInterface module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/simulation_node.py` & `air-sdk-2.4.0/air_sdk/simulation_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 SimulationNode module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/ssh_key.py` & `air-sdk-2.4.0/air_sdk/ssh_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 SSH Key module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/token.py` & `air-sdk-2.4.0/air_sdk/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Token module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk/topology.py` & `air-sdk-2.4.0/air_sdk/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Topology module
 """
 
 import io
```

### Comparing `air-sdk-2.3.0/air_sdk/util.py` & `air-sdk-2.4.0/air_sdk/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Helper utils
 """
 
 import datetime
```

### Comparing `air-sdk-2.3.0/air_sdk/worker.py` & `air-sdk-2.4.0/air_sdk/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Worker module
 """
 
 from . import util
```

### Comparing `air-sdk-2.3.0/air_sdk.egg-info/PKG-INFO` & `air-sdk-2.4.0/air_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: air-sdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python SDK for interacting with NVIDIA Air
 Home-page: https://github.com/NVIDIA/air_sdk
 Author: Mike Robertson
 Author-email: Mike Robertson <mrobertson@nvidia.com>
-License: SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+License: SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
         SPDX-License-Identifier: MIT
         
-        Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+        Copyright (c) 2022-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a
         copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense,
         and/or sell copies of the Software, and to permit persons to whom the
         Software is furnished to do so, subject to the following conditions:
```

### Comparing `air-sdk-2.3.0/air_sdk.egg-info/SOURCES.txt` & `air-sdk-2.4.0/air_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 air_sdk/job.py
 air_sdk/link.py
 air_sdk/login.py
 air_sdk/marketplace.py
 air_sdk/node.py
 air_sdk/organization.py
 air_sdk/permission.py
+air_sdk/resource_budget.py
 air_sdk/service.py
 air_sdk/simulation.py
 air_sdk/simulation_interface.py
 air_sdk/simulation_node.py
 air_sdk/ssh_key.py
 air_sdk/token.py
 air_sdk/topology.py
@@ -44,14 +45,15 @@
 tests/job.py
 tests/link.py
 tests/login.py
 tests/marketplace.py
 tests/node.py
 tests/organization.py
 tests/permission.py
+tests/resource_budget.py
 tests/service.py
 tests/simulation.py
 tests/simulation_interface.py
 tests/simulation_node.py
 tests/ssh_key.py
 tests/token.py
 tests/topology.py
```

### Comparing `air-sdk-2.3.0/pyproject.toml` & `air-sdk-2.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "air-sdk"
-version = "2.3.0"
+version = "2.4.0"
 authors = [
   { name="Mike Robertson", email="mrobertson@nvidia.com" },
 ]
 description = "Python SDK for interacting with NVIDIA Air"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `air-sdk-2.3.0/setup.py` & `air-sdk-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """ Setup script """
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     LONG_DESCRIPTION = fh.read()
 
 setuptools.setup(
     name='air-sdk',
-    version='2.3.0',
+    version='2.4.0',
     author='Mike Robertson',
     author_email='mrobertson@nvidia.com',
     description='Python SDK for interacting with NVIDIA Air',
     license='MIT',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/NVIDIA/air_sdk',
```

### Comparing `air-sdk-2.3.0/tests/account.py` & `air-sdk-2.4.0/tests/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for account.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/air_api.py` & `air-sdk-2.4.0/tests/air_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for air_api.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,protected-access
 #pylint: disable=arguments-differ,unused-argument,no-member,too-many-public-methods
@@ -26,14 +26,15 @@
 from ..air_sdk.job import JobApi
 from ..air_sdk.link import LinkApi
 from ..air_sdk.login import LoginApi
 from ..air_sdk.marketplace import MarketplaceApi
 from ..air_sdk.node import NodeApi
 from ..air_sdk.organization import OrganizationApi
 from ..air_sdk.permission import PermissionApi
+from ..air_sdk.resource_budget import ResourceBudgetApi
 from ..air_sdk.service import ServiceApi
 from ..air_sdk.ssh_key import SSHKeyApi
 from ..air_sdk.simulation import SimulationApi
 from ..air_sdk.simulation_interface import SimulationInterfaceApi
 from ..air_sdk.simulation_node import SimulationNodeApi
 from ..air_sdk.token import TokenApi
 from ..air_sdk.topology import TopologyApi
@@ -130,14 +131,17 @@
 
     def test_permission(self):
         self.assertIsInstance(self.api.permission, PermissionApi)
 
     def test_permissions(self):
         self.assertIsInstance(self.api.permissions, PermissionApi)
 
+    def test_resource_budgets(self):
+        self.assertIsInstance(self.api.resource_budgets, ResourceBudgetApi)
+
     def test_service(self):
         self.assertIsInstance(self.api.service, ServiceApi)
 
     def test_services(self):
         self.assertIsInstance(self.api.services, ServiceApi)
 
     def test_simulation(self):
```

### Comparing `air-sdk-2.3.0/tests/air_model.py` & `air-sdk-2.4.0/tests/air_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for air_model.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 #pylint: disable=too-many-public-methods,duplicate-code,protected-access
```

### Comparing `air-sdk-2.3.0/tests/capacity.py` & `air-sdk-2.4.0/tests/capacity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for capacity.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/demo.py` & `air-sdk-2.4.0/tests/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for demo.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/exceptions.py` & `air-sdk-2.4.0/tests/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for exceptions.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
```

### Comparing `air-sdk-2.3.0/tests/image.py` & `air-sdk-2.4.0/tests/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for image.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
-from ..air_sdk import image
+from ..air_sdk import image, organization
 
 class TestImage(TestCase):
     def setUp(self):
         self.mock_api = MagicMock()
         self.model = image.Image(self.mock_api)
         self.model.id = 'abc123'
         self.model.name = 'ubuntu'
+        self.org1 = organization.Organization(self.mock_api, id='xyz456', name='NVIDIA')
 
     def test_init_(self):
         self.assertTrue(self.model._deletable)
         self.assertTrue(self.model._updatable)
 
     def test_repr(self):
         self.assertEqual(str(self.model), f'<Image {self.model.name} {self.model.id}>')
 
     def test_repr_deleted(self):
         self.model._deleted = True
         self.assertTrue('Deleted Object' in str(self.model))
 
+    @patch('air_sdk.air_sdk.util.raise_if_invalid_response')
+    def test_copy(self, mock_raise):
+        new_id = 'def456'
+        mock_post = self.mock_api.client.post
+        mock_post.return_value.json.return_value = {'id': new_id, 'name': 'new-image'}
+        res = self.model.copy(self.org1)
+        mock_post.assert_called_once_with(f'{self.mock_api.url}{self.model.id}/copy/',
+                                          json={'organization': self.org1})
+        mock_raise.assert_called_once_with(self.mock_api.client.post.return_value, status_code=201)
+        self.assertEqual(res.id, new_id)
+
     @patch('builtins.open')
     @patch('air_sdk.air_sdk.util.raise_if_invalid_response')
     def test_upload(self, mock_raise, mock_open):
         self.model.upload('myfile')
         mock_put = self.mock_api.client.put
         mock_put.assert_called_with(f'{self.mock_api.url}{self.model.id}/upload/',
                                     data=mock_open.return_value.__enter__.return_value)
```

### Comparing `air-sdk-2.3.0/tests/interface.py` & `air-sdk-2.4.0/tests/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for interface.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/job.py` & `air-sdk-2.4.0/tests/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for job.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/link.py` & `air-sdk-2.4.0/tests/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for link.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/login.py` & `air-sdk-2.4.0/tests/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for login.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/marketplace.py` & `air-sdk-2.4.0/tests/marketplace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for marketplace.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/node.py` & `air-sdk-2.4.0/tests/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for node.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/organization.py` & `air-sdk-2.4.0/tests/organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for organization.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,protected-access
 from copy import deepcopy
```

### Comparing `air-sdk-2.3.0/tests/permission.py` & `air-sdk-2.4.0/tests/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for permission.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/service.py` & `air-sdk-2.4.0/tests/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for service.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/simulation.py` & `air-sdk-2.4.0/tests/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for simulation.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,duplicate-code,unused-argument
 import datetime as dt
```

### Comparing `air-sdk-2.3.0/tests/simulation_interface.py` & `air-sdk-2.4.0/tests/simulation_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for simulation_interface.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/simulation_node.py` & `air-sdk-2.4.0/tests/simulation_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for simulation_node.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/ssh_key.py` & `air-sdk-2.4.0/tests/ssh_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for ssh_key.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/token.py` & `air-sdk-2.4.0/tests/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for token.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

### Comparing `air-sdk-2.3.0/tests/topology.py` & `air-sdk-2.4.0/tests/topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for topology.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,unused-argument
 import io
```

### Comparing `air-sdk-2.3.0/tests/util.py` & `air-sdk-2.4.0/tests/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for util.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring,no-self-use,unused-argument
```

### Comparing `air-sdk-2.3.0/tests/worker.py` & `air-sdk-2.4.0/tests/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-FileCopyrightText: Copyright (c) 2022-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 # SPDX-License-Identifier: MIT
 
 """
 Tests for worker.py
 """
 #pylint: disable=missing-function-docstring,missing-class-docstring
 from unittest import TestCase
```

