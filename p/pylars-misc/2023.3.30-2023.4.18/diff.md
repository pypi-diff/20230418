# Comparing `tmp/pylars_misc-2023.3.30.tar.gz` & `tmp/pylars_misc-2023.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylars_misc-2023.3.30.tar", last modified: Thu Mar 30 10:33:06 2023, max compression
+gzip compressed data, was "pylars_misc-2023.4.18.tar", last modified: Tue Apr 18 10:22:51 2023, max compression
```

## Comparing `pylars_misc-2023.3.30.tar` & `pylars_misc-2023.4.18.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:33:06.316187 pylars_misc-2023.3.30/
--rw-r--r--   0 root         (0) root         (0)      229 2023-03-30 10:33:06.314080 pylars_misc-2023.3.30/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      316 2023-03-30 10:26:49.000000 pylars_misc-2023.3.30/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 10:33:06.317290 pylars_misc-2023.3.30/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:33:06.169122 pylars_misc-2023.3.30/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:33:06.213518 pylars_misc-2023.3.30/src/pylars_misc/
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-14 19:18:37.000000 pylars_misc-2023.3.30/src/pylars_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-03-30 10:25:11.000000 pylars_misc-2023.3.30/src/pylars_misc/pylars_misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:33:06.293500 pylars_misc-2023.3.30/src/pylars_misc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      229 2023-03-30 10:33:06.000000 pylars_misc-2023.3.30/src/pylars_misc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      229 2023-03-30 10:33:06.000000 pylars_misc-2023.3.30/src/pylars_misc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 10:33:06.000000 pylars_misc-2023.3.30/src/pylars_misc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-30 10:33:06.000000 pylars_misc-2023.3.30/src/pylars_misc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.381293 pylars_misc-2023.4.18/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.379299 pylars_misc-2023.4.18/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-18 10:22:10.000000 pylars_misc-2023.4.18/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 10:22:51.382295 pylars_misc-2023.4.18/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.250928 pylars_misc-2023.4.18/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.286963 pylars_misc-2023.4.18/src/pylars_misc/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-03-14 19:18:37.000000 pylars_misc-2023.4.18/src/pylars_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-03-30 10:25:11.000000 pylars_misc-2023.4.18/src/pylars_misc/pylars_misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.358972 pylars_misc-2023.4.18/src/pylars_misc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/top_level.txt
```

### Comparing `pylars_misc-2023.3.30/src/pylars_misc/pylars_misc.py` & `pylars_misc-2023.4.18/src/pylars_misc/pylars_misc.py`

 * *Files identical despite different names*

