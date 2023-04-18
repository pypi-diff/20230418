# Comparing `tmp/django-mapper-1.1.1.tar.gz` & `tmp/django-mapper-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.1.tar", last modified: Mon Apr 17 09:20:31 2023, max compression
+gzip compressed data, was "django-mapper-1.1.2.tar", last modified: Tue Apr 18 05:33:48 2023, max compression
```

## Comparing `django-mapper-1.1.1.tar` & `django-mapper-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 09:20:31.658364 django-mapper-1.1.1/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.1/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.1/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2808 2023-04-17 09:18:20.000000 django-mapper-1.1.1/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-17 09:20:31.658364 django-mapper-1.1.1/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-17 09:18:34.000000 django-mapper-1.1.1/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:33:48.243018 django-mapper-1.1.2/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.2/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.2/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     2805 2023-04-18 05:10:47.000000 django-mapper-1.1.2/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:33:48.243018 django-mapper-1.1.2/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-18 05:33:48.000000 django-mapper-1.1.2/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-18 05:33:48.243018 django-mapper-1.1.2/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-18 05:33:02.000000 django-mapper-1.1.2/setup.py
```

### Comparing `django-mapper-1.1.1/PKG-INFO` & `django-mapper-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.1
+Version: 1.1.2
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.1/django_mapper/mapper.py` & `django-mapper-1.1.2/django_mapper/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
             to_field = mapping.get('to_field')
             
             from_field = mapping.get('from_field')
             default_value = mapping.get('default_value')
 
             compute_method = mapping.get('compute_method')
 
-            if to_field and compute_method:
+            if from_field and compute_method:
                 raise ValueError("Both from_field and compute_field should be provided at same time, because it's conflicting")
 
-            if to_field:
+            if from_field:
                 try:
                     value = self.get_value(data, from_field)
                     mapped_data = self.set_value(mapped_data, to_field, value)
                 except KeyError:
                     if default_value is not None:
                         mapped_data = self.set_value(mapped_data, to_field, default_value)
 
             elif compute_method:
-                value = compute_method(value, data)
+                value = compute_method(data)
                 mapped_data = self.set_value(mapped_data, to_field, value)
             else:
                 raise ValueError("from_field or compute_method should be provided")
 
         if self.target_model:
             instance = self.create_instance(self.target_model, mapped_data)
             self.logger.info(f"Created instance of {self.target_model.__name__}")
```

### Comparing `django-mapper-1.1.1/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.2/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.1
+Version: 1.1.2
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.1/setup.py` & `django-mapper-1.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.1',
+    version='1.1.2',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

