# Comparing `tmp/AliveHelper-1.3.tar.gz` & `tmp/AliveHelper-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AliveHelper-1.3.tar", last modified: Tue Apr 18 09:06:34 2023, max compression
+gzip compressed data, was "AliveHelper-1.4.tar", last modified: Tue Apr 18 09:13:31 2023, max compression
```

## Comparing `AliveHelper-1.3.tar` & `AliveHelper-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:06:34.272461 AliveHelper-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:06:34.272461 AliveHelper-1.3/AliveHelper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:06:22.000000 AliveHelper-1.3/AliveHelper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:06:34.272461 AliveHelper-1.3/AliveHelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 09:06:34.000000 AliveHelper-1.3/AliveHelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 09:06:34.000000 AliveHelper-1.3/AliveHelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:06:34.000000 AliveHelper-1.3/AliveHelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 09:06:34.000000 AliveHelper-1.3/AliveHelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 09:06:34.000000 AliveHelper-1.3/AliveHelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 09:06:34.272461 AliveHelper-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:06:34.272461 AliveHelper-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 09:06:22.000000 AliveHelper-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:13:31.852483 AliveHelper-1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:13:31.852483 AliveHelper-1.4/AliveHelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:13:22.000000 AliveHelper-1.4/AliveHelper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:13:31.852483 AliveHelper-1.4/AliveHelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 09:13:31.000000 AliveHelper-1.4/AliveHelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 09:13:31.000000 AliveHelper-1.4/AliveHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:13:31.000000 AliveHelper-1.4/AliveHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 09:13:31.000000 AliveHelper-1.4/AliveHelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 09:13:31.000000 AliveHelper-1.4/AliveHelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 09:13:31.852483 AliveHelper-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:13:31.852483 AliveHelper-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 09:13:22.000000 AliveHelper-1.4/setup.py
```

