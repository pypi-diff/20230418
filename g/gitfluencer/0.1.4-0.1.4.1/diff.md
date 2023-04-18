# Comparing `tmp/gitfluencer-0.1.4.tar.gz` & `tmp/gitfluencer-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfluencer-0.1.4.tar", last modified: Tue Apr 18 09:33:48 2023, max compression
+gzip compressed data, was "gitfluencer-0.1.4.1.tar", last modified: Tue Apr 18 09:39:51 2023, max compression
```

## Comparing `gitfluencer-0.1.4.tar` & `gitfluencer-0.1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.4/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/gitfluencer/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.4/gitfluencer/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2751 2023-04-18 09:33:16.000000 gitfluencer-0.1.4/gitfluencer/app.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/gitfluencer.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 09:33:48.508625 gitfluencer-0.1.4/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 09:33:32.000000 gitfluencer-0.1.4/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:39:51.557884 gitfluencer-0.1.4.1/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1773 2023-04-18 09:39:51.557884 gitfluencer-0.1.4.1/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.4.1/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:39:51.557884 gitfluencer-0.1.4.1/gitfluencer/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.4.1/gitfluencer/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2751 2023-04-18 09:33:16.000000 gitfluencer-0.1.4.1/gitfluencer/app.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:39:51.557884 gitfluencer-0.1.4.1/gitfluencer.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1773 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 09:39:51.000000 gitfluencer-0.1.4.1/gitfluencer.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 09:39:51.557884 gitfluencer-0.1.4.1/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     1319 2023-04-18 09:39:31.000000 gitfluencer-0.1.4.1/setup.py
```

### Comparing `gitfluencer-0.1.4/README.md` & `gitfluencer-0.1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gitfluencer-0.1.4/gitfluencer/app.py` & `gitfluencer-0.1.4.1/gitfluencer/app.py`

 * *Files identical despite different names*

