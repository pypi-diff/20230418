# Comparing `tmp/pype-hyperopt-0.2.0.tar.gz` & `tmp/pype-hyperopt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-hyperopt-0.2.0.tar", last modified: Fri Jan 20 12:14:51 2023, max compression
+gzip compressed data, was "pype-hyperopt-0.3.0.tar", last modified: Tue Apr 18 07:35:49 2023, max compression
```

## Comparing `pype-hyperopt-0.2.0.tar` & `pype-hyperopt-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:14:51.943446 pype-hyperopt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-20 12:14:51.943446 pype-hyperopt-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:14:51.943446 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-20 12:14:51.000000 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-20 12:14:51.000000 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:14:51.000000 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-20 12:14:51.000000 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:14:51.000000 pype-hyperopt-0.2.0/pype_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:14:51.943446 pype-hyperopt-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-20 12:11:52.000000 pype-hyperopt-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:49.098370 pype-hyperopt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 07:35:49.098370 pype-hyperopt-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:49.098370 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 07:35:49.000000 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 07:35:49.000000 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:49.000000 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 07:35:49.000000 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:49.000000 pype-hyperopt-0.3.0/pype_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:35:49.098370 pype-hyperopt-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-18 07:32:59.000000 pype-hyperopt-0.3.0/setup.py
```

