# Comparing `tmp/calculation_mapilio-0.1.8.tar.gz` & `tmp/calculation_mapilio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calculation_mapilio-0.1.8.tar", last modified: Wed Mar 10 15:56:28 2021, max compression
+gzip compressed data, was "dist/calculation_mapilio-0.1.9.tar", last modified: Wed Mar 10 15:58:50 2021, max compression
```

## Comparing `calculation_mapilio-0.1.8.tar` & `calculation_mapilio-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation/
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/area.py
--rw-r--r--   0 runner    (1001) docker     (116)     2842 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/units.py
--rw-r--r--   0 runner    (1001) docker     (116)     8184 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/intersection.py
--rw-r--r--   0 runner    (1001) docker     (116)      220 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     6557 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/distance.py
--rw-r--r--   0 runner    (1001) docker     (116)     2797 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)      949 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/iterator.py
--rw-r--r--   0 runner    (1001) docker     (116)      487 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      686 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      499 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      499 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/calculation_mapilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-10 15:56:28.000000 calculation_mapilio-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2021-03-10 15:56:13.000000 calculation_mapilio-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation/
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/area.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2842 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/units.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8184 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      220 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/util.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6557 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/distance.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2797 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)      949 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      487 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      686 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      499 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      499 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/calculation_mapilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-10 15:58:50.000000 calculation_mapilio-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1215 2021-03-10 15:58:33.000000 calculation_mapilio-0.1.9/setup.py
```

### Comparing `calculation_mapilio-0.1.8/calculation/units.py` & `calculation_mapilio-0.1.9/calculation/units.py`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/calculation/intersection.py` & `calculation_mapilio-0.1.9/calculation/intersection.py`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/calculation/distance.py` & `calculation_mapilio-0.1.9/calculation/distance.py`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/calculation/pixel.py` & `calculation_mapilio-0.1.9/calculation/pixel.py`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/calculation/iterator.py` & `calculation_mapilio-0.1.9/calculation/iterator.py`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/README.md` & `calculation_mapilio-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `calculation_mapilio-0.1.8/setup.py` & `calculation_mapilio-0.1.9/setup.py`

 * *Files identical despite different names*

