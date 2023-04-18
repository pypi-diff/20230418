# Comparing `tmp/quarter_lib-0.0.5.tar.gz` & `tmp/quarter_lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarter_lib-0.0.5.tar", last modified: Mon Apr 17 17:53:44 2023, max compression
+gzip compressed data, was "quarter_lib-0.0.6.tar", last modified: Tue Apr 18 08:28:47 2023, max compression
```

## Comparing `quarter_lib-0.0.5.tar` & `quarter_lib-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.229812 quarter_lib-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.225813 quarter_lib-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.225813 quarter_lib-0.0.5/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.225813 quarter_lib-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 17:53:44.229812 quarter_lib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 17:53:44.229812 quarter_lib-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.225813 quarter_lib-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.225813 quarter_lib-0.0.5/src/quarter_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/src/quarter_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.229812 quarter_lib-0.0.5/src/quarter_lib/akeyless/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/src/quarter_lib/akeyless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 17:53:36.000000 quarter_lib-0.0.5/src/quarter_lib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:44.229812 quarter_lib-0.0.5/src/quarter_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 17:53:44.000000 quarter_lib-0.0.5/src/quarter_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 17:53:44.000000 quarter_lib-0.0.5/src/quarter_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:53:44.000000 quarter_lib-0.0.5/src/quarter_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:53:44.000000 quarter_lib-0.0.5/src/quarter_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.287395 quarter_lib-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-18 08:28:47.287395 quarter_lib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 08:28:47.287395 quarter_lib-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/src/quarter_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/src/quarter_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/src/quarter_lib/akeyless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/src/quarter_lib/akeyless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/src/quarter_lib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.287395 quarter_lib-0.0.6/src/quarter_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-18 08:28:39.000000 quarter_lib-0.0.6/src/quarter_lib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:28:47.283395 quarter_lib-0.0.6/src/quarter_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-18 08:28:47.000000 quarter_lib-0.0.6/src/quarter_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 08:28:47.000000 quarter_lib-0.0.6/src/quarter_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:28:47.000000 quarter_lib-0.0.6/src/quarter_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:28:47.000000 quarter_lib-0.0.6/src/quarter_lib.egg-info/top_level.txt
```

### Comparing `quarter_lib-0.0.5/.github/scripts/release.py` & `quarter_lib-0.0.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `quarter_lib-0.0.5/.gitignore` & `quarter_lib-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `quarter_lib-0.0.5/src/quarter_lib/akeyless/__init__.py` & `quarter_lib-0.0.6/src/quarter_lib/akeyless/__init__.py`

 * *Files identical despite different names*

