# Comparing `tmp/soau-1.0.0.tar.gz` & `tmp/soau-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soau-1.0.0.tar", last modified: Mon Apr 17 16:15:55 2023, max compression
+gzip compressed data, was "soau-1.0.1.tar", last modified: Tue Apr 18 17:17:44 2023, max compression
```

## Comparing `soau-1.0.0.tar` & `soau-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:15:55.515926 soau-1.0.0/
--rw-rw-rw-   0        0        0      118 2023-04-17 16:15:55.515926 soau-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 16:15:55.515926 soau-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-17 16:14:21.000000 soau-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:15:55.484663 soau-1.0.0/soau/
--rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.0/soau/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-04-17 14:52:04.000000 soau-1.0.0/soau/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:15:55.515926 soau-1.0.0/soau.egg-info/
--rw-rw-rw-   0        0        0      118 2023-04-17 16:15:55.000000 soau-1.0.0/soau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-17 16:15:55.000000 soau-1.0.0/soau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:15:55.000000 soau-1.0.0/soau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-17 16:15:55.000000 soau-1.0.0/soau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.387044 soau-1.0.1/
+-rw-rw-rw-   0        0        0      118 2023-04-18 17:17:44.387044 soau-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 17:17:44.390044 soau-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-04-18 17:13:15.000000 soau-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.369043 soau-1.0.1/soau/
+-rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.1/soau/__init__.py
+-rw-rw-rw-   0        0        0    15224 2023-04-18 17:14:41.000000 soau-1.0.1/soau/client.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.385042 soau-1.0.1/soau.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/top_level.txt
```

