# Comparing `tmp/tada-qq-2.3.0.tar.gz` & `tmp/tada-qq-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tada-qq-2.3.0.tar", last modified: Tue Jul  5 01:40:21 2022, max compression
+gzip compressed data, was "tada-qq-2.3.1.tar", last modified: Mon Apr 17 22:26:49 2023, max compression
```

## Comparing `tada-qq-2.3.0.tar` & `tada-qq-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.196886 tada-qq-2.3.0/
--rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2021-07-22 08:49:31.000000 tada-qq-2.3.0/LICENSE
--rw-r--r--   0 aalobaid   (501) staff       (20)      754 2022-07-05 01:40:21.196334 tada-qq-2.3.0/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)      954 2022-07-05 01:31:38.000000 tada-qq-2.3.0/README.md
--rw-r--r--   0 aalobaid   (501) staff       (20)       38 2022-07-05 01:40:21.197041 tada-qq-2.3.0/setup.cfg
--rw-r--r--   0 aalobaid   (501) staff       (20)     1208 2022-07-05 01:36:14.000000 tada-qq-2.3.0/setup.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.183478 tada-qq-2.3.0/tada_qq.egg-info/
--rw-r--r--   0 aalobaid   (501) staff       (20)      754 2022-07-05 01:40:21.000000 tada-qq-2.3.0/tada_qq.egg-info/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)      468 2022-07-05 01:40:21.000000 tada-qq-2.3.0/tada_qq.egg-info/SOURCES.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)        1 2022-07-05 01:40:21.000000 tada-qq-2.3.0/tada_qq.egg-info/dependency_links.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)       24 2022-07-05 01:40:21.000000 tada-qq-2.3.0/tada_qq.egg-info/requires.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)        7 2022-07-05 01:40:21.000000 tada-qq-2.3.0/tada_qq.egg-info/top_level.txt
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.179381 tada-qq-2.3.0/tadaqq/
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.185674 tada-qq-2.3.0/tadaqq/clus/
--rw-r--r--   0 aalobaid   (501) staff       (20)       56 2022-04-01 06:29:26.000000 tada-qq-2.3.0/tadaqq/clus/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     4652 2022-06-18 09:03:26.000000 tada-qq-2.3.0/tadaqq/clus/clusterer.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      610 2022-04-01 06:04:15.000000 tada-qq-2.3.0/tadaqq/clus/pmap.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.190429 tada-qq-2.3.0/tadaqq/qq/
--rw-r--r--   0 aalobaid   (501) staff       (20)       20 2022-03-22 06:15:47.000000 tada-qq-2.3.0/tadaqq/qq/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      530 2022-03-21 06:22:06.000000 tada-qq-2.3.0/tadaqq/qq/dist.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     1935 2022-03-28 06:23:20.000000 tada-qq-2.3.0/tadaqq/qq/err.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     1960 2022-03-21 06:22:06.000000 tada-qq-2.3.0/tadaqq/qq/hist.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     9419 2022-07-05 01:23:53.000000 tada-qq-2.3.0/tadaqq/qq/qqe.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.192285 tada-qq-2.3.0/tadaqq/slabel/
--rw-r--r--   0 aalobaid   (501) staff       (20)       27 2022-03-22 06:59:39.000000 tada-qq-2.3.0/tadaqq/slabel/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     9575 2022-07-04 23:08:59.000000 tada-qq-2.3.0/tadaqq/slabel/slabel.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.194063 tada-qq-2.3.0/tadaqq/slabmer/
--rw-r--r--   0 aalobaid   (501) staff       (20)       29 2022-04-01 06:55:48.000000 tada-qq-2.3.0/tadaqq/slabmer/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)     6289 2022-07-04 23:11:15.000000 tada-qq-2.3.0/tadaqq/slabmer/slabmer.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2022-07-05 01:40:21.195126 tada-qq-2.3.0/tadaqq/util/
--rw-r--r--   0 aalobaid   (501) staff       (20)     3670 2022-04-01 05:46:22.000000 tada-qq-2.3.0/tadaqq/util/__init__.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.705268 tada-qq-2.3.1/
+-rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2021-07-22 08:49:31.000000 tada-qq-2.3.1/LICENSE
+-rw-r--r--   0 aalobaid   (501) staff       (20)      839 2023-04-17 22:26:49.704555 tada-qq-2.3.1/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1039 2023-04-15 21:40:20.000000 tada-qq-2.3.1/README.md
+-rw-r--r--   0 aalobaid   (501) staff       (20)       38 2023-04-17 22:26:49.705491 tada-qq-2.3.1/setup.cfg
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1208 2023-04-17 22:26:15.000000 tada-qq-2.3.1/setup.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.674987 tada-qq-2.3.1/tada_qq.egg-info/
+-rw-r--r--   0 aalobaid   (501) staff       (20)      839 2023-04-17 22:26:49.000000 tada-qq-2.3.1/tada_qq.egg-info/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)      468 2023-04-17 22:26:49.000000 tada-qq-2.3.1/tada_qq.egg-info/SOURCES.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)        1 2023-04-17 22:26:49.000000 tada-qq-2.3.1/tada_qq.egg-info/dependency_links.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)       24 2023-04-17 22:26:49.000000 tada-qq-2.3.1/tada_qq.egg-info/requires.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)        7 2023-04-17 22:26:49.000000 tada-qq-2.3.1/tada_qq.egg-info/top_level.txt
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.659177 tada-qq-2.3.1/tadaqq/
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.679842 tada-qq-2.3.1/tadaqq/clus/
+-rw-r--r--   0 aalobaid   (501) staff       (20)       56 2022-04-01 06:29:26.000000 tada-qq-2.3.1/tadaqq/clus/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     4652 2022-06-18 09:03:26.000000 tada-qq-2.3.1/tadaqq/clus/clusterer.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      610 2022-04-01 06:04:15.000000 tada-qq-2.3.1/tadaqq/clus/pmap.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.691066 tada-qq-2.3.1/tadaqq/qq/
+-rw-r--r--   0 aalobaid   (501) staff       (20)       20 2022-03-22 06:15:47.000000 tada-qq-2.3.1/tadaqq/qq/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      530 2022-03-21 06:22:06.000000 tada-qq-2.3.1/tadaqq/qq/dist.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1935 2022-03-28 06:23:20.000000 tada-qq-2.3.1/tadaqq/qq/err.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1960 2022-03-21 06:22:06.000000 tada-qq-2.3.1/tadaqq/qq/hist.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     9419 2022-07-05 01:23:53.000000 tada-qq-2.3.1/tadaqq/qq/qqe.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.693604 tada-qq-2.3.1/tadaqq/slabel/
+-rw-r--r--   0 aalobaid   (501) staff       (20)       27 2022-03-22 06:59:39.000000 tada-qq-2.3.1/tadaqq/slabel/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     9575 2022-07-04 23:08:59.000000 tada-qq-2.3.1/tadaqq/slabel/slabel.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.698410 tada-qq-2.3.1/tadaqq/slabmer/
+-rw-r--r--   0 aalobaid   (501) staff       (20)       29 2022-04-01 06:55:48.000000 tada-qq-2.3.1/tadaqq/slabmer/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     6289 2022-07-04 23:11:15.000000 tada-qq-2.3.1/tadaqq/slabmer/slabmer.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2023-04-17 22:26:49.702193 tada-qq-2.3.1/tadaqq/util/
+-rw-r--r--   0 aalobaid   (501) staff       (20)     3670 2022-04-01 05:46:22.000000 tada-qq-2.3.1/tadaqq/util/__init__.py
```

### Comparing `tada-qq-2.3.0/LICENSE` & `tada-qq-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/PKG-INFO` & `tada-qq-2.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tada-qq
-Version: 2.3.0
+Version: 2.3.1
 Summary: Quantile Quantile Plot with Linear Approximation, Clustering, and Semantic Labelling of Numeric Columns
 Home-page: https://github.com/oeg-upm/tada-qq
 Author: Ahmad Alobaid
 Author-email: aalobaid@fi.upm.es
 License: Apache2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -17,12 +17,18 @@
 
 
 
 
 TADA (TAbular Data Annotator) for numeric column. It focuses on distributions to label numeric columns in tabular data.
 
 
+
 # To publish
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+# Funding
+This work was funded partially by EIT Digital under the WOODS project.
+
+
```

### Comparing `tada-qq-2.3.0/README.md` & `tada-qq-2.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,17 @@
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 
 TADA (TAbular Data Annotator) for numeric column. It focuses on distributions to label numeric columns in tabular data.
 
 
+
 # To publish
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
-```
+```
+
+# Funding
+This work was funded partially by EIT Digital under the WOODS project.
+
```

### Comparing `tada-qq-2.3.0/setup.py` & `tada-qq-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     lines = README.split('\n')
     desc_lines = [line for line in lines if line[:2] != "[!"]
     README = "\n".join(desc_lines)
     README += "\n"
 # This call to setup() does all the work
 setup(
     name="tada-qq",
-    version="2.3.0",
+    version="2.3.1",
     description=description,
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/oeg-upm/tada-qq",
     author="Ahmad Alobaid",
     author_email="aalobaid@fi.upm.es",
     license="Apache2",
```

### Comparing `tada-qq-2.3.0/tada_qq.egg-info/PKG-INFO` & `tada-qq-2.3.1/tada_qq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tada-qq
-Version: 2.3.0
+Version: 2.3.1
 Summary: Quantile Quantile Plot with Linear Approximation, Clustering, and Semantic Labelling of Numeric Columns
 Home-page: https://github.com/oeg-upm/tada-qq
 Author: Ahmad Alobaid
 Author-email: aalobaid@fi.upm.es
 License: Apache2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -17,12 +17,18 @@
 
 
 
 
 TADA (TAbular Data Annotator) for numeric column. It focuses on distributions to label numeric columns in tabular data.
 
 
+
 # To publish
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+# Funding
+This work was funded partially by EIT Digital under the WOODS project.
+
+
```

### Comparing `tada-qq-2.3.0/tadaqq/clus/clusterer.py` & `tada-qq-2.3.1/tadaqq/clus/clusterer.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/clus/pmap.py` & `tada-qq-2.3.1/tadaqq/clus/pmap.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/qq/dist.py` & `tada-qq-2.3.1/tadaqq/qq/dist.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/qq/err.py` & `tada-qq-2.3.1/tadaqq/qq/err.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/qq/hist.py` & `tada-qq-2.3.1/tadaqq/qq/hist.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/qq/qqe.py` & `tada-qq-2.3.1/tadaqq/qq/qqe.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/slabel/slabel.py` & `tada-qq-2.3.1/tadaqq/slabel/slabel.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/slabmer/slabmer.py` & `tada-qq-2.3.1/tadaqq/slabmer/slabmer.py`

 * *Files identical despite different names*

### Comparing `tada-qq-2.3.0/tadaqq/util/__init__.py` & `tada-qq-2.3.1/tadaqq/util/__init__.py`

 * *Files identical despite different names*

