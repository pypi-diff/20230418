# Comparing `tmp/RNApolis-0.1.0.tar.gz` & `tmp/RNApolis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RNApolis-0.1.0.tar", last modified: Tue Apr  4 15:16:14 2023, max compression
+gzip compressed data, was "RNApolis-0.1.1.tar", last modified: Tue Apr 18 11:56:10 2023, max compression
```

## Comparing `RNApolis-0.1.0.tar` & `RNApolis-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-04 15:16:14.797824 RNApolis-0.1.0/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.1.0/LICENSE
--rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-04-04 15:16:14.797824 RNApolis-0.1.0/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      264 2023-04-04 15:11:51.000000 RNApolis-0.1.0/README.md
--rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.1.0/pyproject.toml
--rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2023-04-04 15:16:14.797824 RNApolis-0.1.0/setup.cfg
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1368 2023-04-04 15:16:07.000000 RNApolis-0.1.0/setup.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-04 15:16:14.794491 RNApolis-0.1.0/src/
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-04 15:16:14.797824 RNApolis-0.1.0/src/RNApolis.egg-info/
--rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      656 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/SOURCES.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/dependency_links.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)      220 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/entry_points.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)       42 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/requires.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2023-04-04 15:16:14.000000 RNApolis-0.1.0/src/RNApolis.egg-info/top_level.txt
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-04 15:16:14.797824 RNApolis-0.1.0/src/rnapolis/
--rw-r--r--   0 tzok      (1000) tzok      (1000)    20766 2023-04-04 15:16:07.000000 RNApolis-0.1.0/src/rnapolis/annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.1.0/src/rnapolis/clashfinder.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    24518 2023-04-04 15:16:07.000000 RNApolis-0.1.0/src/rnapolis/common.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.1.0/src/rnapolis/metareader.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)      961 2023-04-04 15:16:07.000000 RNApolis-0.1.0/src/rnapolis/motif_extractor.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    11905 2023-04-04 15:11:51.000000 RNApolis-0.1.0/src/rnapolis/parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    18293 2023-04-04 15:16:07.000000 RNApolis-0.1.0/src/rnapolis/tertiary.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.1.0/src/rnapolis/transformer.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.1.0/src/rnapolis/util.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-04 15:16:14.797824 RNApolis-0.1.0/tests/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1509 2023-04-04 15:11:51.000000 RNApolis-0.1.0/tests/test_annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     2639 2023-04-04 15:16:07.000000 RNApolis-0.1.0/tests/test_bugfixes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     3635 2023-04-04 15:16:07.000000 RNApolis-0.1.0/tests/test_common.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.1.0/tests/test_metareader.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.1.0/tests/test_parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    15655 2023-04-04 15:16:07.000000 RNApolis-0.1.0/tests/test_quadruplexes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      445 2023-04-04 15:11:51.000000 RNApolis-0.1.0/tests/test_tertiary.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-18 11:56:10.468753 RNApolis-0.1.1/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.1.1/LICENSE
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-04-18 11:56:10.468753 RNApolis-0.1.1/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      264 2023-04-04 15:11:51.000000 RNApolis-0.1.1/README.md
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.1.1/pyproject.toml
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2023-04-18 11:56:10.468753 RNApolis-0.1.1/setup.cfg
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1368 2023-04-18 11:55:24.000000 RNApolis-0.1.1/setup.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-18 11:56:10.465419 RNApolis-0.1.1/src/
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-18 11:56:10.468753 RNApolis-0.1.1/src/RNApolis.egg-info/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      656 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/SOURCES.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/dependency_links.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      220 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/entry_points.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       42 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/requires.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2023-04-18 11:56:10.000000 RNApolis-0.1.1/src/RNApolis.egg-info/top_level.txt
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-18 11:56:10.468753 RNApolis-0.1.1/src/rnapolis/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    20766 2023-04-18 11:45:44.000000 RNApolis-0.1.1/src/rnapolis/annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.1.1/src/rnapolis/clashfinder.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    24518 2023-04-04 15:16:07.000000 RNApolis-0.1.1/src/rnapolis/common.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.1.1/src/rnapolis/metareader.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)      961 2023-04-04 15:16:07.000000 RNApolis-0.1.1/src/rnapolis/motif_extractor.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    11905 2023-04-04 15:11:51.000000 RNApolis-0.1.1/src/rnapolis/parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    18293 2023-04-18 11:45:44.000000 RNApolis-0.1.1/src/rnapolis/tertiary.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.1.1/src/rnapolis/transformer.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.1.1/src/rnapolis/util.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-04-18 11:56:10.468753 RNApolis-0.1.1/tests/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1509 2023-04-04 15:11:51.000000 RNApolis-0.1.1/tests/test_annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     2639 2023-04-04 15:16:07.000000 RNApolis-0.1.1/tests/test_bugfixes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     3635 2023-04-04 15:16:07.000000 RNApolis-0.1.1/tests/test_common.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.1.1/tests/test_metareader.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.1.1/tests/test_parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    15655 2023-04-04 15:16:07.000000 RNApolis-0.1.1/tests/test_quadruplexes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      445 2023-04-04 15:11:51.000000 RNApolis-0.1.1/tests/test_tertiary.py
```

### Comparing `RNApolis-0.1.0/LICENSE` & `RNApolis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/PKG-INFO` & `RNApolis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.1.0/setup.py` & `RNApolis-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="RNApolis",
-    version="0.1.0",
+    version="0.1.1",
     packages=["rnapolis"],
     package_dir={"": "src"},
     author="Tomasz Zok",
     author_email="tomasz.zok@cs.put.poznan.pl",
     description="A Python library containing RNA-related bioinformatics functions and classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `RNApolis-0.1.0/src/RNApolis.egg-info/PKG-INFO` & `RNApolis-0.1.1/src/RNApolis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.1.0/src/RNApolis.egg-info/SOURCES.txt` & `RNApolis-0.1.1/src/RNApolis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/annotator.py` & `RNApolis-0.1.1/src/rnapolis/annotator.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/clashfinder.py` & `RNApolis-0.1.1/src/rnapolis/clashfinder.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/common.py` & `RNApolis-0.1.1/src/rnapolis/common.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/metareader.py` & `RNApolis-0.1.1/src/rnapolis/metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/motif_extractor.py` & `RNApolis-0.1.1/src/rnapolis/motif_extractor.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/parser.py` & `RNApolis-0.1.1/src/rnapolis/parser.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/tertiary.py` & `RNApolis-0.1.1/src/rnapolis/tertiary.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/transformer.py` & `RNApolis-0.1.1/src/rnapolis/transformer.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/src/rnapolis/util.py` & `RNApolis-0.1.1/src/rnapolis/util.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/tests/test_annotator.py` & `RNApolis-0.1.1/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/tests/test_bugfixes.py` & `RNApolis-0.1.1/tests/test_bugfixes.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/tests/test_common.py` & `RNApolis-0.1.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/tests/test_metareader.py` & `RNApolis-0.1.1/tests/test_metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.0/tests/test_quadruplexes.py` & `RNApolis-0.1.1/tests/test_quadruplexes.py`

 * *Files identical despite different names*

