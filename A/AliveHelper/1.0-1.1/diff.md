# Comparing `tmp/AliveHelper-1.0.tar.gz` & `tmp/AliveHelper-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AliveHelper-1.0.tar", last modified: Tue Apr 18 08:32:40 2023, max compression
+gzip compressed data, was "AliveHelper-1.1.tar", last modified: Tue Apr 18 08:36:00 2023, max compression
```

## Comparing `AliveHelper-1.0.tar` & `AliveHelper-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:32:40.834210 AliveHelper-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:32:40.834210 AliveHelper-1.0/AliveHelper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:32:30.000000 AliveHelper-1.0/AliveHelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 08:32:30.000000 AliveHelper-1.0/AliveHelper/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:32:40.834210 AliveHelper-1.0/AliveHelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:32:40.000000 AliveHelper-1.0/AliveHelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 08:32:40.834210 AliveHelper-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:32:40.834210 AliveHelper-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 08:32:30.000000 AliveHelper-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:36:00.943019 AliveHelper-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:36:00.939019 AliveHelper-1.1/AliveHelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:35:50.000000 AliveHelper-1.1/AliveHelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 08:35:50.000000 AliveHelper-1.1/AliveHelper/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:36:00.943019 AliveHelper-1.1/AliveHelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:36:00.000000 AliveHelper-1.1/AliveHelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 08:36:00.943019 AliveHelper-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:36:00.943019 AliveHelper-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 08:35:50.000000 AliveHelper-1.1/setup.py
```

