# Comparing `tmp/jaquar-0.6.1.tar.gz` & `tmp/jaquar-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.6.1.tar", last modified: Tue Apr 18 09:30:05 2023, max compression
+gzip compressed data, was "dist\jaquar-0.6.2.tar", last modified: Tue Apr 18 09:36:33 2023, max compression
```

## Comparing `jaquar-0.6.1.tar` & `jaquar-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/
--rw-rw-rw-   0        0        0     3680 2023-04-18 09:29:34.000000 jaquar-0.6.1/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.6.1/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.6.1/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.1/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:30:05.000000 jaquar-0.6.1/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:30:04.000000 jaquar-0.6.1/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 09:30:05.000000 jaquar-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 09:30:05.000000 jaquar-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-18 09:29:53.000000 jaquar-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/jaquar/
+-rw-rw-rw-   0        0        0     3680 2023-04-18 09:29:34.000000 jaquar-0.6.2/jaquar/cli.py
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.2/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:36:33.000000 jaquar-0.6.2/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      235 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:36:32.000000 jaquar-0.6.2/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2023-04-18 09:34:44.000000 jaquar-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:36:33.000000 jaquar-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:36:33.000000 jaquar-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-18 09:36:30.000000 jaquar-0.6.2/setup.py
```

### Comparing `jaquar-0.6.1/jaquar/cli.py` & `jaquar-0.6.2/jaquar/cli.py`

 * *Files identical despite different names*

