# Comparing `tmp/rrb_package-0.1.0.tar.gz` & `tmp/rrb_package-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrb_package-0.1.0.tar", last modified: Tue Apr 18 18:32:39 2023, max compression
+gzip compressed data, was "rrb_package-0.1.1.tar", last modified: Tue Apr 18 18:48:48 2023, max compression
```

## Comparing `rrb_package-0.1.0.tar` & `rrb_package-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:32:39.160743 rrb_package-0.1.0/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      482 2023-04-18 18:32:39.160574 rrb_package-0.1.0/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:23:30.000000 rrb_package-0.1.0/README.md
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:32:39.159573 rrb_package-0.1.0/rrb_package/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 rrb_package-0.1.0/rrb_package/__init__.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       45 2023-04-18 18:30:56.000000 rrb_package-0.1.0/rrb_package/my_module.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:32:39.160343 rrb_package-0.1.0/rrb_package.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      482 2023-04-18 18:32:39.000000 rrb_package-0.1.0/rrb_package.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      207 2023-04-18 18:32:39.000000 rrb_package-0.1.0/rrb_package.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-04-18 18:32:39.000000 rrb_package-0.1.0/rrb_package.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       12 2023-04-18 18:32:39.000000 rrb_package-0.1.0/rrb_package.egg-info/top_level.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-04-18 18:32:39.160802 rrb_package-0.1.0/setup.cfg
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      654 2023-04-18 18:27:03.000000 rrb_package-0.1.0/setup.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:48:48.947558 rrb_package-0.1.1/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     4423 2023-04-18 18:48:48.947366 rrb_package-0.1.1/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     3644 2023-04-18 18:47:34.000000 rrb_package-0.1.1/README.md
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:48:48.946446 rrb_package-0.1.1/rrb_package/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 rrb_package-0.1.1/rrb_package/__init__.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       45 2023-04-18 18:30:56.000000 rrb_package-0.1.1/rrb_package/my_module.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:48:48.947129 rrb_package-0.1.1/rrb_package.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     4423 2023-04-18 18:48:48.000000 rrb_package-0.1.1/rrb_package.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      207 2023-04-18 18:48:48.000000 rrb_package-0.1.1/rrb_package.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-04-18 18:48:48.000000 rrb_package-0.1.1/rrb_package.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       12 2023-04-18 18:48:48.000000 rrb_package-0.1.1/rrb_package.egg-info/top_level.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-04-18 18:48:48.947623 rrb_package-0.1.1/setup.cfg
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      654 2023-04-18 18:47:43.000000 rrb_package-0.1.1/setup.py
```

### Comparing `rrb_package-0.1.0/setup.py` & `rrb_package-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='rrb_package',
-    version='0.1.0',
+    version='0.1.1',
     author='Rahul Bhoyar',
     author_email='rahulbhoyaroffice@gmail.com',
     description='My first pip installabe package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rahulbhoyar1995/rrb_package',
     packages=['rrb_package'],
```

