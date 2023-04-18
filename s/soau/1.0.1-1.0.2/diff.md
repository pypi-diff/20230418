# Comparing `tmp/soau-1.0.1.tar.gz` & `tmp/soau-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soau-1.0.1.tar", last modified: Tue Apr 18 17:17:44 2023, max compression
+gzip compressed data, was "soau-1.0.2.tar", last modified: Tue Apr 18 17:54:03 2023, max compression
```

## Comparing `soau-1.0.1.tar` & `soau-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.387044 soau-1.0.1/
--rw-rw-rw-   0        0        0      118 2023-04-18 17:17:44.387044 soau-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-18 17:17:44.390044 soau-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-18 17:13:15.000000 soau-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.369043 soau-1.0.1/soau/
--rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.1/soau/__init__.py
--rw-rw-rw-   0        0        0    15224 2023-04-18 17:14:41.000000 soau-1.0.1/soau/client.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:17:44.385042 soau-1.0.1/soau.egg-info/
--rw-rw-rw-   0        0        0      118 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 17:17:44.000000 soau-1.0.1/soau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 17:54:03.219385 soau-1.0.2/
+-rw-rw-rw-   0        0        0      118 2023-04-18 17:54:03.219401 soau-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 17:54:03.221700 soau-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      430 2023-04-18 17:53:55.000000 soau-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:54:03.201372 soau-1.0.2/soau/
+-rw-rw-rw-   0        0        0      326 2023-04-17 13:09:29.000000 soau-1.0.2/soau/__init__.py
+-rw-rw-rw-   0        0        0    15224 2023-04-18 17:14:41.000000 soau-1.0.2/soau/client.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:54:03.214045 soau-1.0.2/soau.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-04-18 17:54:03.000000 soau-1.0.2/soau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-18 17:54:03.000000 soau-1.0.2/soau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 17:54:03.000000 soau-1.0.2/soau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 17:54:03.000000 soau-1.0.2/soau.egg-info/top_level.txt
```

### Comparing `soau-1.0.1/soau/client.py` & `soau-1.0.2/soau/client.py`

 * *Files identical despite different names*

