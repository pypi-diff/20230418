# Comparing `tmp/Mensajes-jdjj43-5.0.tar.gz` & `tmp/Mensajes-jdjj43-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-jdjj43-5.0.tar", last modified: Tue Apr 18 03:22:44 2023, max compression
+gzip compressed data, was "Mensajes-jdjj43-6.0.tar", last modified: Tue Apr 18 03:35:45 2023, max compression
```

## Comparing `Mensajes-jdjj43-5.0.tar` & `Mensajes-jdjj43-6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 03:22:44.379880 Mensajes-jdjj43-5.0/
--rw-rw-rw-   0        0        0     1096 2023-04-18 03:05:25.000000 Mensajes-jdjj43-5.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-04-18 03:05:56.000000 Mensajes-jdjj43-5.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-18 03:22:44.350856 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/
--rw-rw-rw-   0        0        0      704 2023-04-18 03:22:44.000000 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-04-18 03:22:44.000000 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 03:22:44.000000 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-18 03:22:44.000000 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 03:22:44.000000 Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      704 2023-04-18 03:22:44.377860 Mensajes-jdjj43-5.0/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-04-18 03:00:56.000000 Mensajes-jdjj43-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 03:22:44.354858 Mensajes-jdjj43-5.0/mensajes/
--rw-rw-rw-   0        0        0       38 2023-03-09 15:09:18.000000 Mensajes-jdjj43-5.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:22:44.365878 Mensajes-jdjj43-5.0/mensajes/hola/
--rw-rw-rw-   0        0        0       45 2023-03-09 13:24:42.000000 Mensajes-jdjj43-5.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      380 2023-04-16 22:35:38.000000 Mensajes-jdjj43-5.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-04-16 22:25:35.000000 Mensajes-jdjj43-5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 03:22:44.380862 Mensajes-jdjj43-5.0/setup.cfg
--rw-rw-rw-   0        0        0      971 2023-04-18 03:21:56.000000 Mensajes-jdjj43-5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:22:44.371880 Mensajes-jdjj43-5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-16 22:38:28.000000 Mensajes-jdjj43-5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      276 2023-04-16 22:37:18.000000 Mensajes-jdjj43-5.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:35:45.469349 Mensajes-jdjj43-6.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-18 03:05:25.000000 Mensajes-jdjj43-6.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-04-18 03:05:56.000000 Mensajes-jdjj43-6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-18 03:35:45.429368 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-04-18 03:35:45.000000 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-18 03:35:45.000000 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:35:45.000000 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 03:35:45.000000 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 03:35:45.000000 Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      704 2023-04-18 03:35:45.467347 Mensajes-jdjj43-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2023-04-18 03:00:56.000000 Mensajes-jdjj43-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 03:35:45.432358 Mensajes-jdjj43-6.0/mensajes/
+-rw-rw-rw-   0        0        0       38 2023-03-09 15:09:18.000000 Mensajes-jdjj43-6.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:35:45.457345 Mensajes-jdjj43-6.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       45 2023-03-09 13:24:42.000000 Mensajes-jdjj43-6.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      391 2023-04-18 03:34:04.000000 Mensajes-jdjj43-6.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-04-16 22:25:35.000000 Mensajes-jdjj43-6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:35:45.470350 Mensajes-jdjj43-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      971 2023-04-18 03:34:09.000000 Mensajes-jdjj43-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:35:45.464348 Mensajes-jdjj43-6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-16 22:38:28.000000 Mensajes-jdjj43-6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-04-16 22:37:18.000000 Mensajes-jdjj43-6.0/tests/test_hola.py
```

### Comparing `Mensajes-jdjj43-5.0/LICENSE` & `Mensajes-jdjj43-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-jdjj43-5.0/Mensajes_jdjj43.egg-info/PKG-INFO` & `Mensajes-jdjj43-6.0/Mensajes_jdjj43.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-jdjj43
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Héctor Costa Guzmán
 Author-email: hola@hektor.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-jdjj43-5.0/PKG-INFO` & `Mensajes-jdjj43-6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-jdjj43
-Version: 5.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Héctor Costa Guzmán
 Author-email: hola@hektor.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-jdjj43-5.0/setup.py` & `Mensajes-jdjj43-6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-jdjj43',
-    version='5.0',
+    version='6.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Héctor Costa Guzmán',
     author_email='hola@hektor.dev',
     url='https://www.hektor.dev',
     license_files=['LICENSE'],
```

