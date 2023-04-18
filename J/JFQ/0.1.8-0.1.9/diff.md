# Comparing `tmp/JFQ-0.1.8.tar.gz` & `tmp/JFQ-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JFQ-0.1.8.tar", last modified: Thu Mar  2 09:36:30 2023, max compression
+gzip compressed data, was "JFQ-0.1.9.tar", last modified: Sun Mar 12 11:18:27 2023, max compression
```

## Comparing `JFQ-0.1.8.tar` & `JFQ-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.256219 JFQ-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.171706 JFQ-0.1.8/JFQ/
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.192705 JFQ-0.1.8/JFQ/BBG/
--rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.8/JFQ/BBG/__init__.py
--rw-rw-rw-   0        0        0    42038 2023-03-01 10:24:24.000000 JFQ-0.1.8/JFQ/BBG/core.py
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.245221 JFQ-0.1.8/JFQ/HELPERS/
--rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.8/JFQ/HELPERS/__init__.py
--rw-rw-rw-   0        0        0     1907 2023-03-01 10:14:48.000000 JFQ-0.1.8/JFQ/HELPERS/general.py
--rw-rw-rw-   0        0        0     5144 2023-03-01 10:24:24.000000 JFQ-0.1.8/JFQ/HELPERS/misc.py
--rw-rw-rw-   0        0        0     5059 2023-02-27 11:29:10.000000 JFQ-0.1.8/JFQ/HELPERS/pandas_ext.py
--rw-rw-rw-   0        0        0     2350 2023-03-01 10:14:48.000000 JFQ-0.1.8/JFQ/HELPERS/plotly_ext.py
--rw-rw-rw-   0        0        0        0 2023-02-27 08:37:32.000000 JFQ-0.1.8/JFQ/HELPERS/stats.py
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.251221 JFQ-0.1.8/JFQ/TREE/
--rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.8/JFQ/TREE/__init__.py
--rw-rw-rw-   0        0        0    16444 2023-02-27 08:49:30.000000 JFQ-0.1.8/JFQ/TREE/core.py
--rw-rw-rw-   0        0        0       97 2023-02-27 11:35:13.000000 JFQ-0.1.8/JFQ/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-02 09:36:30.187707 JFQ-0.1.8/JFQ.egg-info/
--rw-rw-rw-   0        0        0      648 2023-03-02 09:36:30.000000 JFQ-0.1.8/JFQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-03-02 09:36:30.000000 JFQ-0.1.8/JFQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 09:36:30.000000 JFQ-0.1.8/JFQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-02 09:36:30.000000 JFQ-0.1.8/JFQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-02 09:36:30.000000 JFQ-0.1.8/JFQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-03-02 09:36:30.256219 JFQ-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       41 2022-05-20 20:34:26.000000 JFQ-0.1.8/README.md
--rw-rw-rw-   0        0        0    37621 2022-05-08 14:20:47.000000 JFQ-0.1.8/licence.txt
--rw-rw-rw-   0        0        0       86 2023-03-02 09:36:30.259221 JFQ-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-03-02 09:33:16.000000 JFQ-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.180933 JFQ-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.108936 JFQ-0.1.9/JFQ/
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.127934 JFQ-0.1.9/JFQ/BBG/
+-rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.9/JFQ/BBG/__init__.py
+-rw-rw-rw-   0        0        0    42038 2023-03-01 10:24:24.000000 JFQ-0.1.9/JFQ/BBG/core.py
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.171938 JFQ-0.1.9/JFQ/HELPERS/
+-rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.9/JFQ/HELPERS/__init__.py
+-rw-rw-rw-   0        0        0     1907 2023-03-01 10:14:48.000000 JFQ-0.1.9/JFQ/HELPERS/general.py
+-rw-rw-rw-   0        0        0     5144 2023-03-01 10:24:24.000000 JFQ-0.1.9/JFQ/HELPERS/misc.py
+-rw-rw-rw-   0        0        0     5059 2023-02-27 11:29:10.000000 JFQ-0.1.9/JFQ/HELPERS/pandas_ext.py
+-rw-rw-rw-   0        0        0     4493 2023-03-12 11:11:10.000000 JFQ-0.1.9/JFQ/HELPERS/plotly_ext.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 08:37:32.000000 JFQ-0.1.9/JFQ/HELPERS/stats.py
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.176936 JFQ-0.1.9/JFQ/TREE/
+-rw-rw-rw-   0        0        0        2 2023-02-27 08:00:57.000000 JFQ-0.1.9/JFQ/TREE/__init__.py
+-rw-rw-rw-   0        0        0    16444 2023-02-27 08:49:30.000000 JFQ-0.1.9/JFQ/TREE/core.py
+-rw-rw-rw-   0        0        0       97 2023-02-27 11:35:13.000000 JFQ-0.1.9/JFQ/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-12 11:18:27.123934 JFQ-0.1.9/JFQ.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-03-12 11:18:27.000000 JFQ-0.1.9/JFQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-03-12 11:18:27.000000 JFQ-0.1.9/JFQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-12 11:18:27.000000 JFQ-0.1.9/JFQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-03-12 11:18:27.000000 JFQ-0.1.9/JFQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-03-12 11:18:27.000000 JFQ-0.1.9/JFQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-03-12 11:18:27.181934 JFQ-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2022-05-20 20:34:26.000000 JFQ-0.1.9/README.md
+-rw-rw-rw-   0        0        0    37621 2022-05-08 14:20:47.000000 JFQ-0.1.9/licence.txt
+-rw-rw-rw-   0        0        0       86 2023-03-12 11:18:27.184935 JFQ-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-03-12 10:16:24.000000 JFQ-0.1.9/setup.py
```

### Comparing `JFQ-0.1.8/JFQ/BBG/core.py` & `JFQ-0.1.9/JFQ/BBG/core.py`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/JFQ/HELPERS/general.py` & `JFQ-0.1.9/JFQ/HELPERS/general.py`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/JFQ/HELPERS/misc.py` & `JFQ-0.1.9/JFQ/HELPERS/misc.py`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/JFQ/HELPERS/pandas_ext.py` & `JFQ-0.1.9/JFQ/HELPERS/pandas_ext.py`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/JFQ/TREE/core.py` & `JFQ-0.1.9/JFQ/TREE/core.py`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/JFQ.egg-info/PKG-INFO` & `JFQ-0.1.9/JFQ.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFQ
-Version: 0.1.8
+Version: 0.1.9
 Summary: various utilities
 Home-page: 
 Author: 
 Author-email: 
 License: GNU2L
 Keywords: openAPI
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `JFQ-0.1.8/PKG-INFO` & `JFQ-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JFQ
-Version: 0.1.8
+Version: 0.1.9
 Summary: various utilities
 Home-page: 
 Author: 
 Author-email: 
 License: GNU2L
 Keywords: openAPI
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `JFQ-0.1.8/licence.txt` & `JFQ-0.1.9/licence.txt`

 * *Files identical despite different names*

### Comparing `JFQ-0.1.8/setup.py` & `JFQ-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='JFQ',  # should match the package folder
     packages=setuptools.find_packages(),  # should match the package folder
-    version='v0.1.8',  # important for updates
+    version='v0.1.9',  # important for updates
     license='GNU2L',  # should match your chosen license
     description='various utilities',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='',
     author_email='',
     url='', #removed github url
```

