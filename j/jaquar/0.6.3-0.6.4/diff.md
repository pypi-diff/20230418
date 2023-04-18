# Comparing `tmp/jaquar-0.6.3.tar.gz` & `tmp/jaquar-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.6.3.tar", last modified: Tue Apr 18 09:40:56 2023, max compression
+gzip compressed data, was "dist\jaquar-0.6.4.tar", last modified: Tue Apr 18 09:43:36 2023, max compression
```

## Comparing `jaquar-0.6.3.tar` & `jaquar-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/jaquar/
--rw-rw-rw-   0        0        0     3688 2023-04-18 09:39:38.000000 jaquar-0.6.3/jaquar/cli.py
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.3/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:56.000000 jaquar-0.6.3/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      235 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:40:55.000000 jaquar-0.6.3/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2023-04-18 09:34:44.000000 jaquar-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 09:40:56.000000 jaquar-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 09:40:56.000000 jaquar-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-04-18 09:40:34.000000 jaquar-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:43:36.000000 jaquar-0.6.4/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar/
+-rw-rw-rw-   0        0        0     3688 2023-04-18 09:39:38.000000 jaquar-0.6.4/jaquar/cli.py
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.6.4/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      235 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:43:36.000000 jaquar-0.6.4/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2023-04-18 09:34:44.000000 jaquar-0.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:43:36.000000 jaquar-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:43:36.000000 jaquar-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-04-18 09:43:18.000000 jaquar-0.6.4/setup.py
```

### Comparing `jaquar-0.6.3/jaquar/cli.py` & `jaquar-0.6.4/jaquar/cli.py`

 * *Files identical despite different names*

