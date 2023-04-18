# Comparing `tmp/HassWS-0.0.2.tar.gz` & `tmp/HassWS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HassWS-0.0.2.tar", last modified: Tue Apr 18 08:54:30 2023, max compression
+gzip compressed data, was "HassWS-0.0.3.tar", last modified: Tue Apr 18 09:10:48 2023, max compression
```

## Comparing `HassWS-0.0.2.tar` & `HassWS-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:54:30.294545 HassWS-0.0.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)       50 2023-04-18 08:54:30.294545 HassWS-0.0.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      531 2023-04-18 08:54:20.000000 HassWS-0.0.2/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 08:54:30.294545 HassWS-0.0.2/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:54:30.294545 HassWS-0.0.2/src/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:54:30.294545 HassWS-0.0.2/src/HassWS/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2675 2023-04-18 07:08:23.000000 HassWS-0.0.2/src/HassWS/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:54:30.294545 HassWS-0.0.2/src/HassWS.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)       50 2023-04-18 08:54:30.000000 HassWS-0.0.2/src/HassWS.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      206 2023-04-18 08:54:30.000000 HassWS-0.0.2/src/HassWS.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 08:54:30.000000 HassWS-0.0.2/src/HassWS.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 08:54:30.000000 HassWS-0.0.2/src/HassWS.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 08:54:30.000000 HassWS-0.0.2/src/HassWS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 09:10:40.000000 HassWS-0.0.3/.github/workflows/python-publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/HassWS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:10:48.000000 HassWS-0.0.3/HassWS.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-18 09:10:48.643017 HassWS-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 09:10:40.000000 HassWS-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 09:10:40.000000 HassWS-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 09:10:48.643017 HassWS-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:48.643017 HassWS-0.0.3/src/HassWS/
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-18 09:10:40.000000 HassWS-0.0.3/src/HassWS/__init__.py
```

### Comparing `HassWS-0.0.2/src/HassWS/__init__.py` & `HassWS-0.0.3/src/HassWS/__init__.py`

 * *Files identical despite different names*

