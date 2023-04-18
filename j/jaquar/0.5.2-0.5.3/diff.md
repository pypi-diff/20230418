# Comparing `tmp/jaquar-0.5.2.tar.gz` & `tmp/jaquar-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.5.2.tar", last modified: Tue Apr 18 08:46:27 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.3.tar", last modified: Tue Apr 18 08:51:19 2023, max compression
```

## Comparing `jaquar-0.5.2.tar` & `jaquar-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/
--rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.2/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.2/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.2/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.2/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:46:27.000000 jaquar-0.5.2/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 08:46:26.000000 jaquar-0.5.2/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 08:46:27.000000 jaquar-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 08:46:27.000000 jaquar-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      473 2023-04-18 08:46:23.000000 jaquar-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar/
+-rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.3/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.3/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.3/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.3/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:51:19.000000 jaquar-0.5.3/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:51:19.000000 jaquar-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 08:51:19.000000 jaquar-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      584 2023-04-18 08:51:05.000000 jaquar-0.5.3/setup.py
```

### Comparing `jaquar-0.5.2/jaquar/cli.py` & `jaquar-0.5.3/jaquar/cli.py`

 * *Files identical despite different names*

