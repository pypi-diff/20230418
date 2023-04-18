# Comparing `tmp/stringhandling-0.2.tar.gz` & `tmp/stringhandling-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringhandling-0.2.tar", last modified: Tue Apr 18 13:03:26 2023, max compression
+gzip compressed data, was "stringhandling-0.3.tar", last modified: Tue Apr 18 13:14:58 2023, max compression
```

## Comparing `stringhandling-0.2.tar` & `stringhandling-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:03:26.572615 stringhandling-0.2/
--rw-rw-rw-   0        0        0     1058 2023-04-18 11:14:34.000000 stringhandling-0.2/LICENSE.md
--rw-rw-rw-   0        0        0      208 2023-04-18 13:03:26.572615 stringhandling-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-04-18 13:02:14.000000 stringhandling-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 13:03:26.572615 stringhandling-0.2/setup.cfg
--rw-rw-rw-   0        0        0      303 2023-04-18 13:03:17.000000 stringhandling-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:03:26.510114 stringhandling-0.2/stringhandling/
--rw-rw-rw-   0        0        0       53 2023-04-18 13:01:29.000000 stringhandling-0.2/stringhandling/__init__.y.py
--rw-rw-rw-   0        0        0      691 2023-04-18 12:59:55.000000 stringhandling-0.2/stringhandling/strhandle.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:03:26.556998 stringhandling-0.2/stringhandling.egg-info/
--rw-rw-rw-   0        0        0      208 2023-04-18 13:03:26.000000 stringhandling-0.2/stringhandling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-18 13:03:26.000000 stringhandling-0.2/stringhandling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:03:26.000000 stringhandling-0.2/stringhandling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 13:03:26.000000 stringhandling-0.2/stringhandling.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-18 13:03:26.000000 stringhandling-0.2/stringhandling.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 13:14:58.018103 stringhandling-0.3/
+-rw-rw-rw-   0        0        0     1058 2023-04-18 11:14:34.000000 stringhandling-0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1090 2023-04-18 13:14:58.018103 stringhandling-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-04-18 13:02:14.000000 stringhandling-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:14:58.018103 stringhandling-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-04-18 13:14:39.000000 stringhandling-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:14:57.971225 stringhandling-0.3/stringhandling/
+-rw-rw-rw-   0        0        0       53 2023-04-18 13:01:29.000000 stringhandling-0.3/stringhandling/__init__.y.py
+-rw-rw-rw-   0        0        0      691 2023-04-18 12:59:55.000000 stringhandling-0.3/stringhandling/strhandle.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:14:58.018103 stringhandling-0.3/stringhandling.egg-info/
+-rw-rw-rw-   0        0        0     1090 2023-04-18 13:14:57.000000 stringhandling-0.3/stringhandling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-18 13:14:57.000000 stringhandling-0.3/stringhandling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:14:57.000000 stringhandling-0.3/stringhandling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 13:14:57.000000 stringhandling-0.3/stringhandling.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-04-18 13:14:57.000000 stringhandling-0.3/stringhandling.egg-info/top_level.txt
```

### Comparing `stringhandling-0.2/LICENSE.md` & `stringhandling-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stringhandling-0.2/README.md` & `stringhandling-0.3/README.md`

 * *Files identical despite different names*

### Comparing `stringhandling-0.2/stringhandling/strhandle.py` & `stringhandling-0.3/stringhandling/strhandle.py`

 * *Files identical despite different names*

