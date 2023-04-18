# Comparing `tmp/pype-xgboost-0.2.0.tar.gz` & `tmp/pype-xgboost-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-xgboost-0.2.0.tar", last modified: Fri Jan 20 12:15:37 2023, max compression
+gzip compressed data, was "pype-xgboost-0.3.0.tar", last modified: Tue Apr 18 07:36:21 2023, max compression
```

## Comparing `pype-xgboost-0.2.0.tar` & `pype-xgboost-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:37.537853 pype-xgboost-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-20 12:15:37.537853 pype-xgboost-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:37.537853 pype-xgboost-0.2.0/pype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-20 12:15:37.000000 pype-xgboost-0.2.0/pype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-20 12:15:37.000000 pype-xgboost-0.2.0/pype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:37.000000 pype-xgboost-0.2.0/pype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-20 12:15:37.000000 pype-xgboost-0.2.0/pype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:37.000000 pype-xgboost-0.2.0/pype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:15:37.537853 pype-xgboost-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 12:11:52.000000 pype-xgboost-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:21.802479 pype-xgboost-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 07:36:21.802479 pype-xgboost-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:21.802479 pype-xgboost-0.3.0/pype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 07:36:21.000000 pype-xgboost-0.3.0/pype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-18 07:36:21.000000 pype-xgboost-0.3.0/pype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:21.000000 pype-xgboost-0.3.0/pype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 07:36:21.000000 pype-xgboost-0.3.0/pype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:21.000000 pype-xgboost-0.3.0/pype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:36:21.802479 pype-xgboost-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 07:32:59.000000 pype-xgboost-0.3.0/setup.py
```

