# Comparing `tmp/bmgen-2023.4.0b1.tar.gz` & `tmp/bmgen-2023.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmgen-2023.4.0b1.tar", last modified: Mon Apr 17 17:32:47 2023, max compression
+gzip compressed data, was "bmgen-2023.4.0b2.tar", last modified: Tue Apr 18 05:23:05 2023, max compression
```

## Comparing `bmgen-2023.4.0b1.tar` & `bmgen-2023.4.0b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-17 17:32:47.493973 bmgen-2023.4.0b1/
--rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.4.0b1/LICENSE
--rw-rw-r--   0 ever      (1000) ever      (1000)     2013 2023-04-17 17:32:47.493973 bmgen-2023.4.0b1/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)     1675 2023-04-17 17:30:23.000000 bmgen-2023.4.0b1/README.md
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-17 17:32:47.489973 bmgen-2023.4.0b1/bmgen/
--rw-r--r--   0 ever      (1000) ever      (1000)     4965 2023-04-17 17:23:15.000000 bmgen-2023.4.0b1/bmgen/__main__.py
--rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-04-17 17:32:29.000000 bmgen-2023.4.0b1/bmgen/info.py
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-17 17:32:47.493973 bmgen-2023.4.0b1/bmgen.egg-info/
--rw-r--r--   0 ever      (1000) ever      (1000)     2013 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/SOURCES.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/dependency_links.txt
--rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/entry_points.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/requires.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-17 17:32:47.000000 bmgen-2023.4.0b1/bmgen.egg-info/top_level.txt
--rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-04-17 17:32:47.493973 bmgen-2023.4.0b1/setup.cfg
--rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.4.0b1/setup.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/
+-rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.4.0b2/LICENSE
+-rw-rw-r--   0 ever      (1000) ever      (1000)     2013 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/PKG-INFO
+-rw-r--r--   0 ever      (1000) ever      (1000)     1675 2023-04-17 17:30:23.000000 bmgen-2023.4.0b2/README.md
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/bmgen/
+-rw-r--r--   0 ever      (1000) ever      (1000)     4965 2023-04-17 17:23:15.000000 bmgen-2023.4.0b2/bmgen/__main__.py
+-rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-04-18 05:19:41.000000 bmgen-2023.4.0b2/bmgen/info.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/bmgen.egg-info/
+-rw-r--r--   0 ever      (1000) ever      (1000)     2013 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/PKG-INFO
+-rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/SOURCES.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/dependency_links.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/entry_points.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/requires.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 05:23:05.000000 bmgen-2023.4.0b2/bmgen.egg-info/top_level.txt
+-rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-04-18 05:23:05.716219 bmgen-2023.4.0b2/setup.cfg
+-rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.4.0b2/setup.py
```

### Comparing `bmgen-2023.4.0b1/LICENSE` & `bmgen-2023.4.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmgen-2023.4.0b1/PKG-INFO` & `bmgen-2023.4.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmgen
-Version: 2023.4.0b1
+Version: 2023.4.0b2
 Summary: Broken Mouse Studios' build solution
 Home-page: https://git.brokenmouse.studio/bms/bmgen
 Author: bms
 Author-email: bmgen@brokenmouse.studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bmgen-2023.4.0b1/README.md` & `bmgen-2023.4.0b2/README.md`

 * *Files identical despite different names*

### Comparing `bmgen-2023.4.0b1/bmgen/__main__.py` & `bmgen-2023.4.0b2/bmgen/__main__.py`

 * *Files identical despite different names*

### Comparing `bmgen-2023.4.0b1/bmgen.egg-info/PKG-INFO` & `bmgen-2023.4.0b2/bmgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmgen
-Version: 2023.4.0b1
+Version: 2023.4.0b2
 Summary: Broken Mouse Studios' build solution
 Home-page: https://git.brokenmouse.studio/bms/bmgen
 Author: bms
 Author-email: bmgen@brokenmouse.studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bmgen-2023.4.0b1/setup.py` & `bmgen-2023.4.0b2/setup.py`

 * *Files identical despite different names*

