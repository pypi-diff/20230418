# Comparing `tmp/pype-mlflow-0.2.0.tar.gz` & `tmp/pype-mlflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-mlflow-0.2.0.tar", last modified: Fri Jan 20 12:15:01 2023, max compression
+gzip compressed data, was "pype-mlflow-0.3.0.tar", last modified: Tue Apr 18 07:35:55 2023, max compression
```

## Comparing `pype-mlflow-0.2.0.tar` & `pype-mlflow-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:01.055873 pype-mlflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-20 12:15:01.051873 pype-mlflow-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:01.051873 pype-mlflow-0.2.0/pype_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-20 12:15:01.000000 pype-mlflow-0.2.0/pype_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-20 12:15:01.000000 pype-mlflow-0.2.0/pype_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:01.000000 pype-mlflow-0.2.0/pype_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-20 12:15:01.000000 pype-mlflow-0.2.0/pype_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:01.000000 pype-mlflow-0.2.0/pype_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:15:01.055873 pype-mlflow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-20 12:11:52.000000 pype-mlflow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:55.586393 pype-mlflow-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 07:35:55.586393 pype-mlflow-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:55.586393 pype-mlflow-0.3.0/pype_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 07:35:55.000000 pype-mlflow-0.3.0/pype_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 07:35:55.000000 pype-mlflow-0.3.0/pype_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:55.000000 pype-mlflow-0.3.0/pype_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 07:35:55.000000 pype-mlflow-0.3.0/pype_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:55.000000 pype-mlflow-0.3.0/pype_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:35:55.586393 pype-mlflow-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-18 07:32:59.000000 pype-mlflow-0.3.0/setup.py
```

