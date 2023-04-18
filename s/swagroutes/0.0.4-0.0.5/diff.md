# Comparing `tmp/swagroutes-0.0.4.tar.gz` & `tmp/swagroutes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagroutes-0.0.4.tar", last modified: Tue Apr 18 19:28:22 2023, max compression
+gzip compressed data, was "swagroutes-0.0.5.tar", last modified: Tue Apr 18 19:44:40 2023, max compression
```

## Comparing `swagroutes-0.0.4.tar` & `swagroutes-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:28:22.246863 swagroutes-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 19:28:11.000000 swagroutes-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:28:22.242863 swagroutes-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 19:28:11.000000 swagroutes-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:28:22.246863 swagroutes-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 19:28:11.000000 swagroutes-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:28:22.242863 swagroutes-0.0.4/swagroutes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:28:11.000000 swagroutes-0.0.4/swagroutes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 19:28:11.000000 swagroutes-0.0.4/swagroutes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 19:28:11.000000 swagroutes-0.0.4/swagroutes/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-18 19:28:11.000000 swagroutes-0.0.4/swagroutes/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:28:22.242863 swagroutes-0.0.4/swagroutes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 19:28:22.000000 swagroutes-0.0.4/swagroutes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:28:22.242863 swagroutes-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:28:11.000000 swagroutes-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-18 19:28:11.000000 swagroutes-0.0.4/tests/test_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:44:40.277453 swagroutes-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 19:44:28.000000 swagroutes-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:44:40.277453 swagroutes-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 19:44:28.000000 swagroutes-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:44:40.277453 swagroutes-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 19:44:28.000000 swagroutes-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:44:40.277453 swagroutes-0.0.5/swagroutes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:44:28.000000 swagroutes-0.0.5/swagroutes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 19:44:28.000000 swagroutes-0.0.5/swagroutes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 19:44:28.000000 swagroutes-0.0.5/swagroutes/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-18 19:44:28.000000 swagroutes-0.0.5/swagroutes/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:44:40.277453 swagroutes-0.0.5/swagroutes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 19:44:40.000000 swagroutes-0.0.5/swagroutes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:44:40.277453 swagroutes-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:44:28.000000 swagroutes-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-18 19:44:28.000000 swagroutes-0.0.5/tests/test_extractor.py
```

### Comparing `swagroutes-0.0.4/LICENSE` & `swagroutes-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.4/PKG-INFO` & `swagroutes-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagroutes
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to fetch the details of assets hosted on AWS.
 Home-page: https://github.com/amalmurali47/swagroutes
 Author: Amal Murali
 Author-email: amalmurali47@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swagroutes-0.0.4/README.md` & `swagroutes-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.4/setup.py` & `swagroutes-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.4/swagroutes/cli.py` & `swagroutes-0.0.5/swagroutes/cli.py`

 * *Files identical despite different names*

### Comparing `swagroutes-0.0.4/swagroutes.egg-info/PKG-INFO` & `swagroutes-0.0.5/swagroutes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagroutes
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to fetch the details of assets hosted on AWS.
 Home-page: https://github.com/amalmurali47/swagroutes
 Author: Amal Murali
 Author-email: amalmurali47@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swagroutes-0.0.4/tests/test_extractor.py` & `swagroutes-0.0.5/tests/test_extractor.py`

 * *Files identical despite different names*

