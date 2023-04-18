# Comparing `tmp/ghdtimer-0.1.tar.gz` & `tmp/ghdtimer-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghdtimer-0.1.tar", last modified: Tue Apr 18 00:39:12 2023, max compression
+gzip compressed data, was "ghdtimer-0.11.tar", last modified: Tue Apr 18 00:51:02 2023, max compression
```

## Comparing `ghdtimer-0.1.tar` & `ghdtimer-0.11.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:39:12.878970 ghdtimer-0.1/
--rw-rw-r--   0 ghd       (1000) ghd       (1000)      149 2023-04-18 00:39:12.878970 ghdtimer-0.1/PKG-INFO
-drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:39:12.874970 ghdtimer-0.1/ghdtimer/
--rw-rw-r--   0 ghd       (1000) ghd       (1000)     2116 2023-04-18 00:22:49.000000 ghdtimer-0.1/ghdtimer/ghdtimer.py
--rw-rw-r--   0 ghd       (1000) ghd       (1000)      286 2023-04-18 00:34:35.000000 ghdtimer-0.1/ghdtimer/test_ghdtimer.py
-drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:39:12.878970 ghdtimer-0.1/ghdtimer.egg-info/
--rw-rw-r--   0 ghd       (1000) ghd       (1000)      149 2023-04-18 00:39:12.000000 ghdtimer-0.1/ghdtimer.egg-info/PKG-INFO
--rw-rw-r--   0 ghd       (1000) ghd       (1000)      183 2023-04-18 00:39:12.000000 ghdtimer-0.1/ghdtimer.egg-info/SOURCES.txt
--rw-rw-r--   0 ghd       (1000) ghd       (1000)        1 2023-04-18 00:39:12.000000 ghdtimer-0.1/ghdtimer.egg-info/dependency_links.txt
--rw-rw-r--   0 ghd       (1000) ghd       (1000)        9 2023-04-18 00:39:12.000000 ghdtimer-0.1/ghdtimer.egg-info/top_level.txt
--rw-rw-r--   0 ghd       (1000) ghd       (1000)       38 2023-04-18 00:39:12.878970 ghdtimer-0.1/setup.cfg
--rw-rw-r--   0 ghd       (1000) ghd       (1000)      227 2023-04-18 00:36:26.000000 ghdtimer-0.1/setup.py
+drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:51:02.918419 ghdtimer-0.11/
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      150 2023-04-18 00:51:02.918419 ghdtimer-0.11/PKG-INFO
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      294 2023-04-18 00:50:41.000000 ghdtimer-0.11/README.md
+drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:51:02.918419 ghdtimer-0.11/ghdtimer/
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:48:50.000000 ghdtimer-0.11/ghdtimer/__init__.py
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)     2116 2023-04-18 00:22:49.000000 ghdtimer-0.11/ghdtimer/ghdtimer.py
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      286 2023-04-18 00:34:35.000000 ghdtimer-0.11/ghdtimer/test_ghdtimer.py
+drwxrwxr-x   0 ghd       (1000) ghd       (1000)        0 2023-04-18 00:51:02.918419 ghdtimer-0.11/ghdtimer.egg-info/
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      150 2023-04-18 00:51:02.000000 ghdtimer-0.11/ghdtimer.egg-info/PKG-INFO
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      214 2023-04-18 00:51:02.000000 ghdtimer-0.11/ghdtimer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)        1 2023-04-18 00:51:02.000000 ghdtimer-0.11/ghdtimer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)        9 2023-04-18 00:51:02.000000 ghdtimer-0.11/ghdtimer.egg-info/top_level.txt
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)       38 2023-04-18 00:51:02.918419 ghdtimer-0.11/setup.cfg
+-rw-rw-r--   0 ghd       (1000) ghd       (1000)      228 2023-04-18 00:48:33.000000 ghdtimer-0.11/setup.py
```

### Comparing `ghdtimer-0.1/ghdtimer/ghdtimer.py` & `ghdtimer-0.11/ghdtimer/ghdtimer.py`

 * *Files identical despite different names*

