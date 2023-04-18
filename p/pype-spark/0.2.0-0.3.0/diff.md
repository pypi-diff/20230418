# Comparing `tmp/pype-spark-0.2.0.tar.gz` & `tmp/pype-spark-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-spark-0.2.0.tar", last modified: Fri Jan 20 12:15:19 2023, max compression
+gzip compressed data, was "pype-spark-0.3.0.tar", last modified: Tue Apr 18 07:36:08 2023, max compression
```

## Comparing `pype-spark-0.2.0.tar` & `pype-spark-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:19.416928 pype-spark-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-20 12:15:19.416928 pype-spark-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:19.416928 pype-spark-0.2.0/pype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-20 12:15:19.000000 pype-spark-0.2.0/pype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-20 12:15:19.000000 pype-spark-0.2.0/pype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:19.000000 pype-spark-0.2.0/pype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-20 12:15:19.000000 pype-spark-0.2.0/pype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:19.000000 pype-spark-0.2.0/pype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:15:19.416928 pype-spark-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-20 12:11:52.000000 pype-spark-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:08.774438 pype-spark-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 07:36:08.774438 pype-spark-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:08.774438 pype-spark-0.3.0/pype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 07:36:08.000000 pype-spark-0.3.0/pype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 07:36:08.000000 pype-spark-0.3.0/pype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:08.000000 pype-spark-0.3.0/pype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-18 07:36:08.000000 pype-spark-0.3.0/pype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:08.000000 pype-spark-0.3.0/pype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:36:08.774438 pype-spark-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 07:32:59.000000 pype-spark-0.3.0/setup.py
```

