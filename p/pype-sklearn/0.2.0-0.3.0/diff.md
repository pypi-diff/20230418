# Comparing `tmp/pype-sklearn-0.2.0.tar.gz` & `tmp/pype-sklearn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-sklearn-0.2.0.tar", last modified: Fri Jan 20 12:15:10 2023, max compression
+gzip compressed data, was "pype-sklearn-0.3.0.tar", last modified: Tue Apr 18 07:36:02 2023, max compression
```

## Comparing `pype-sklearn-0.2.0.tar` & `pype-sklearn-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:10.168417 pype-sklearn-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-20 12:15:10.168417 pype-sklearn-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:10.168417 pype-sklearn-0.2.0/pype_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-20 12:15:10.000000 pype-sklearn-0.2.0/pype_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-20 12:15:10.000000 pype-sklearn-0.2.0/pype_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:10.000000 pype-sklearn-0.2.0/pype_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-20 12:15:10.000000 pype-sklearn-0.2.0/pype_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:10.000000 pype-sklearn-0.2.0/pype_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:15:10.168417 pype-sklearn-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-20 12:11:52.000000 pype-sklearn-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:02.098415 pype-sklearn-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 07:36:02.098415 pype-sklearn-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:02.098415 pype-sklearn-0.3.0/pype_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 07:36:02.000000 pype-sklearn-0.3.0/pype_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-18 07:36:02.000000 pype-sklearn-0.3.0/pype_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:02.000000 pype-sklearn-0.3.0/pype_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-18 07:36:02.000000 pype-sklearn-0.3.0/pype_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:02.000000 pype-sklearn-0.3.0/pype_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:36:02.098415 pype-sklearn-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-18 07:32:59.000000 pype-sklearn-0.3.0/setup.py
```

