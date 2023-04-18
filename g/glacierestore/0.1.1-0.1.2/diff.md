# Comparing `tmp/glacierestore-0.1.1.tar.gz` & `tmp/glacierestore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacierestore-0.1.1.tar", last modified: Tue Apr 18 05:54:58 2023, max compression
+gzip compressed data, was "glacierestore-0.1.2.tar", last modified: Tue Apr 18 05:59:15 2023, max compression
```

## Comparing `glacierestore-0.1.1.tar` & `glacierestore-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 05:54:58.768861 glacierestore-0.1.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1076 2023-04-18 05:13:45.000000 glacierestore-0.1.1/LICENSE.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-04-18 05:54:58.768861 glacierestore-0.1.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      481 2023-04-18 05:44:23.000000 glacierestore-0.1.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 05:54:58.768861 glacierestore-0.1.1/glacierestore.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-04-18 05:54:58.000000 glacierestore-0.1.1/glacierestore.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      178 2023-04-18 05:54:58.000000 glacierestore-0.1.1/glacierestore.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-18 05:54:58.000000 glacierestore-0.1.1/glacierestore.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-18 05:54:58.000000 glacierestore-0.1.1/glacierestore.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-04-18 05:54:58.768861 glacierestore-0.1.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3843 2023-04-18 05:51:44.000000 glacierestore-0.1.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 05:59:15.809363 glacierestore-0.1.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1076 2023-04-18 05:13:45.000000 glacierestore-0.1.2/LICENSE.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-04-18 05:59:15.809363 glacierestore-0.1.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      481 2023-04-18 05:44:23.000000 glacierestore-0.1.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 05:59:15.809363 glacierestore-0.1.2/glacierestore.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-04-18 05:59:15.000000 glacierestore-0.1.2/glacierestore.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      178 2023-04-18 05:59:15.000000 glacierestore-0.1.2/glacierestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-18 05:59:15.000000 glacierestore-0.1.2/glacierestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-18 05:59:15.000000 glacierestore-0.1.2/glacierestore.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-04-18 05:59:15.809363 glacierestore-0.1.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3843 2023-04-18 05:59:13.000000 glacierestore-0.1.2/setup.py
```

### Comparing `glacierestore-0.1.1/LICENSE.txt` & `glacierestore-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glacierestore-0.1.1/PKG-INFO` & `glacierestore-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glacierestore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy to restore objects from AWS Glacier to AWS S3 in bulk
 Home-page: https://github.com/nwcd-samples/glacierestore.git
 Author: barry.xu
 Author-email: friendship-119@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `glacierestore-0.1.1/glacierestore.egg-info/PKG-INFO` & `glacierestore-0.1.2/glacierestore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glacierestore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy to restore objects from AWS Glacier to AWS S3 in bulk
 Home-page: https://github.com/nwcd-samples/glacierestore.git
 Author: barry.xu
 Author-email: friendship-119@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `glacierestore-0.1.1/setup.py` & `glacierestore-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Package meta-data.
 NAME = 'glacierestore'
 DESCRIPTION = 'Easy to restore objects from AWS Glacier to AWS S3 in bulk'
 URL = 'https://github.com/nwcd-samples/glacierestore.git'
 EMAIL = 'friendship-119@163.com'
 AUTHOR = 'barry.xu'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

