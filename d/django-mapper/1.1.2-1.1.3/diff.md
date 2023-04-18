# Comparing `tmp/django-mapper-1.1.2.tar.gz` & `tmp/django-mapper-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.2.tar", last modified: Tue Apr 18 05:33:48 2023, max compression
+gzip compressed data, was "django-mapper-1.1.3.tar", last modified: Tue Apr 18 05:46:00 2023, max compression
```

## Comparing `django-mapper-1.1.2.tar` & `django-mapper-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:33:48.243018 django-mapper-1.1.2/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.2/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.2/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2805 2023-04-18 05:10:47.000000 django-mapper-1.1.2/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-18 05:33:48.243018 django-mapper-1.1.2/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-18 05:33:02.000000 django-mapper-1.1.2/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:46:00.863100 django-mapper-1.1.3/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.3/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.3/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     2805 2023-04-18 05:10:47.000000 django-mapper-1.1.3/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-18 05:46:00.863100 django-mapper-1.1.3/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-18 05:44:16.000000 django-mapper-1.1.3/setup.py
```

### Comparing `django-mapper-1.1.2/PKG-INFO` & `django-mapper-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.2/django_mapper/mapper.py` & `django-mapper-1.1.3/django_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mapper-1.1.2/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.3/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.2/setup.py` & `django-mapper-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.2',
+    version='1.1.3',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

