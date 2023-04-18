# Comparing `tmp/soau-1.0.3.tar.gz` & `tmp/soau-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soau-1.0.3.tar", last modified: Tue Apr 18 17:56:08 2023, max compression
+gzip compressed data, was "soau-1.0.4.tar", last modified: Tue Apr 18 18:01:00 2023, max compression
```

## Comparing `soau-1.0.3.tar` & `soau-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 17:56:08.643041 soau-1.0.3/
--rw-rw-rw-   0        0        0      118 2023-04-18 17:56:08.643041 soau-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-18 17:56:08.643041 soau-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      370 2023-04-18 17:56:05.000000 soau-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:56:08.627440 soau-1.0.3/soau/
--rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.3/soau/__init__.py
--rw-rw-rw-   0        0        0    15224 2023-04-18 17:14:41.000000 soau-1.0.3/soau/client.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:56:08.643041 soau-1.0.3/soau.egg-info/
--rw-rw-rw-   0        0        0      118 2023-04-18 17:56:08.000000 soau-1.0.3/soau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-18 17:56:08.000000 soau-1.0.3/soau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 17:56:08.000000 soau-1.0.3/soau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 17:56:08.000000 soau-1.0.3/soau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 18:01:00.387823 soau-1.0.4/
+-rw-rw-rw-   0        0        0      118 2023-04-18 18:01:00.387823 soau-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 18:01:00.387823 soau-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      472 2023-04-18 18:00:55.000000 soau-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:01:00.372200 soau-1.0.4/soau/
+-rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.4/soau/__init__.py
+-rw-rw-rw-   0        0        0    15224 2023-04-18 17:14:41.000000 soau-1.0.4/soau/client.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:01:00.387823 soau-1.0.4/soau.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-04-18 18:01:00.000000 soau-1.0.4/soau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-18 18:01:00.000000 soau-1.0.4/soau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 18:01:00.000000 soau-1.0.4/soau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-18 18:01:00.000000 soau-1.0.4/soau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 18:01:00.000000 soau-1.0.4/soau.egg-info/top_level.txt
```

### Comparing `soau-1.0.3/soau/client.py` & `soau-1.0.4/soau/client.py`

 * *Files identical despite different names*

