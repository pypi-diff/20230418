# Comparing `tmp/jaquar-0.5.6.tar.gz` & `tmp/jaquar-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.5.6.tar", last modified: Tue Apr 18 09:03:00 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.7.tar", last modified: Tue Apr 18 09:11:11 2023, max compression
```

## Comparing `jaquar-0.5.6.tar` & `jaquar-0.5.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/
--rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.6/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.6/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.6/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.6/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 09:03:00.000000 jaquar-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 09:03:00.000000 jaquar-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-04-18 09:02:50.000000 jaquar-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar/
+-rw-rw-rw-   0        0        0     4280 2023-04-18 09:06:12.000000 jaquar-0.5.7/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.7/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.7/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.7/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:11:10.000000 jaquar-0.5.7/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:11:10.000000 jaquar-0.5.7/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:11:10.000000 jaquar-0.5.7/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:11:10.000000 jaquar-0.5.7/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 09:11:11.000000 jaquar-0.5.7/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:11:10.000000 jaquar-0.5.7/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:11:11.000000 jaquar-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:11:11.000000 jaquar-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-18 09:11:08.000000 jaquar-0.5.7/setup.py
```

### Comparing `jaquar-0.5.6/jaquar/cli.py` & `jaquar-0.5.7/jaquar/cli.py`

 * *Files identical despite different names*

