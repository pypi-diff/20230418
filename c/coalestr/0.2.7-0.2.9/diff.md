# Comparing `tmp/coalestr-0.2.7.tar.gz` & `tmp/coalestr-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coalestr-0.2.7.tar", last modified: Wed Feb 22 15:45:07 2023, max compression
+gzip compressed data, was "coalestr-0.2.9.tar", last modified: Wed Feb 22 16:56:43 2023, max compression
```

## Comparing `coalestr-0.2.7.tar` & `coalestr-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 15:45:07.023000 coalestr-0.2.7/
--rw-rw-rw-   0        0        0    35802 2023-02-22 15:29:00.000000 coalestr-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      542 2023-02-22 15:45:07.017000 coalestr-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-02-22 15:29:00.000000 coalestr-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-22 15:45:07.011000 coalestr-0.2.7/coalestr.egg-info/
--rw-rw-rw-   0        0        0      542 2023-02-22 15:45:06.000000 coalestr-0.2.7/coalestr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-02-22 15:45:06.000000 coalestr-0.2.7/coalestr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 15:45:06.000000 coalestr-0.2.7/coalestr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 15:45:06.000000 coalestr-0.2.7/coalestr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-22 15:45:07.021000 coalestr-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-02-22 15:38:31.000000 coalestr-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-22 16:56:43.581000 coalestr-0.2.9/
+-rw-rw-rw-   0        0        0    35802 2023-02-22 16:49:40.000000 coalestr-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      542 2023-02-22 16:56:43.575000 coalestr-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-02-22 16:49:40.000000 coalestr-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-22 16:56:43.526000 coalestr-0.2.9/coalestr/
+-rw-rw-rw-   0        0        0       17 2023-02-22 16:53:06.000000 coalestr-0.2.9/coalestr/__init__.py
+-rw-rw-rw-   0        0        0    47710 2023-02-22 10:43:56.000000 coalestr-0.2.9/coalestr/cs.py
+drwxrwxrwx   0        0        0        0 2023-02-22 16:56:43.569000 coalestr-0.2.9/coalestr.egg-info/
+-rw-rw-rw-   0        0        0      542 2023-02-22 16:56:43.000000 coalestr-0.2.9/coalestr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-02-22 16:56:43.000000 coalestr-0.2.9/coalestr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-22 16:56:43.000000 coalestr-0.2.9/coalestr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-02-22 16:56:43.000000 coalestr-0.2.9/coalestr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-22 16:56:43.579000 coalestr-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-02-22 16:54:39.000000 coalestr-0.2.9/setup.py
```

### Comparing `coalestr-0.2.7/LICENSE` & `coalestr-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coalestr-0.2.7/PKG-INFO` & `coalestr-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coalestr
-Version: 0.2.7
+Version: 0.2.9
 Summary: Short description of coalestr
 Author: Dominic Kwiatkowski
 Author-email: <dkwiatkowski@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `coalestr-0.2.7/coalestr.egg-info/PKG-INFO` & `coalestr-0.2.9/coalestr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coalestr
-Version: 0.2.7
+Version: 0.2.9
 Summary: Short description of coalestr
 Author: Dominic Kwiatkowski
 Author-email: <dkwiatkowski@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `coalestr-0.2.7/setup.py` & `coalestr-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7' 
+VERSION = '0.2.9' 
 DESCRIPTION = 'Short description of coalestr'
 LONG_DESCRIPTION = 'Long description of coalestr'
 
 # Setting up
 setup(
        # the name must match the folder name'
         name="coalestr",
```

