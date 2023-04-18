# Comparing `tmp/fastapi_versionizer-0.1.4.tar.gz` & `tmp/fastapi_versionizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastapi_versionizer-0.1.4.tar", last modified: Thu Apr 13 04:12:44 2023, max compression
+gzip compressed data, was "dist/fastapi_versionizer-0.1.5.tar", last modified: Tue Apr 18 15:31:15 2023, max compression
```

## Comparing `fastapi_versionizer-0.1.4.tar` & `fastapi_versionizer-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/
--rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/PKG-INFO
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/
--rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/PKG-INFO
--rw-r--r--   0 alexschimpf   (501) staff       (20)      336 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/SOURCES.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)       26 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/requires.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)       20 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/top_level.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)        1 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/dependency_links.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)     1076 2022-12-22 21:04:28.000000 fastapi_versionizer-0.1.4/LICENSE
--rw-r--r--   0 alexschimpf   (501) staff       (20)     2896 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.4/README.md
--rw-r--r--   0 alexschimpf   (501) staff       (20)     1060 2023-04-13 04:11:39.000000 fastapi_versionizer-0.1.4/setup.py
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/
--rw-r--r--   0 alexschimpf   (501) staff       (20)      101 2022-12-22 21:10:07.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/__init__.py
--rw-r--r--   0 alexschimpf   (501) staff       (20)    10234 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/versionizer.py
--rw-r--r--   0 alexschimpf   (501) staff       (20)        0 2022-12-23 09:34:59.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/py.typed
--rw-r--r--   0 alexschimpf   (501) staff       (20)       38 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/setup.cfg
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-18 15:31:15.000000 fastapi_versionizer-0.1.5/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-18 15:31:15.000000 fastapi_versionizer-0.1.5/PKG-INFO
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-18 15:31:15.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-18 15:31:14.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/PKG-INFO
+-rw-r--r--   0 alexschimpf   (501) staff       (20)      336 2023-04-18 15:31:14.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/SOURCES.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       26 2023-04-18 15:31:14.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/requires.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       20 2023-04-18 15:31:14.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/top_level.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)        1 2023-04-18 15:31:14.000000 fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/dependency_links.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     1076 2022-12-22 21:04:28.000000 fastapi_versionizer-0.1.5/LICENSE
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     2896 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.5/README.md
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     1060 2023-04-18 15:30:58.000000 fastapi_versionizer-0.1.5/setup.py
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-18 15:31:15.000000 fastapi_versionizer-0.1.5/fastapi_versionizer/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)      147 2023-04-18 15:30:13.000000 fastapi_versionizer-0.1.5/fastapi_versionizer/__init__.py
+-rw-r--r--   0 alexschimpf   (501) staff       (20)    10234 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.5/fastapi_versionizer/versionizer.py
+-rw-r--r--   0 alexschimpf   (501) staff       (20)        0 2022-12-23 09:34:59.000000 fastapi_versionizer-0.1.5/fastapi_versionizer/py.typed
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       38 2023-04-18 15:31:15.000000 fastapi_versionizer-0.1.5/setup.cfg
```

### Comparing `fastapi_versionizer-0.1.4/PKG-INFO` & `fastapi_versionizer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_versionizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: API versionizer for FastAPI web applications
 Home-page: https://github.com/alexschimpf/fastapi-versionizer
 Author: Alex Schimpf
 Author-email: aschimpf1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/PKG-INFO` & `fastapi_versionizer-0.1.5/fastapi_versionizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-versionizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: API versionizer for FastAPI web applications
 Home-page: https://github.com/alexschimpf/fastapi-versionizer
 Author: Alex Schimpf
 Author-email: aschimpf1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fastapi_versionizer-0.1.4/LICENSE` & `fastapi_versionizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_versionizer-0.1.4/README.md` & `fastapi_versionizer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_versionizer-0.1.4/setup.py` & `fastapi_versionizer-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='fastapi_versionizer',
-    version='0.1.4',
+    version='0.1.5',
     author='Alex Schimpf',
     author_email='aschimpf1@gmail.com',
     description='API versionizer for FastAPI web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/alexschimpf/fastapi-versionizer',
     package_data={'fastapi_versionizer': ['py.typed']},
```

### Comparing `fastapi_versionizer-0.1.4/fastapi_versionizer/versionizer.py` & `fastapi_versionizer-0.1.5/fastapi_versionizer/versionizer.py`

 * *Files identical despite different names*

