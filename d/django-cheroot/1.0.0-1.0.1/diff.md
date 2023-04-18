# Comparing `tmp/django-cheroot-1.0.0.tar.gz` & `tmp/django-cheroot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cheroot-1.0.0.tar", last modified: Sun Apr 16 10:06:06 2023, max compression
+gzip compressed data, was "django-cheroot-1.0.1.tar", last modified: Tue Apr 18 18:32:30 2023, max compression
```

## Comparing `django-cheroot-1.0.0.tar` & `django-cheroot-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:06:06.206467 django-cheroot-1.0.0/
--rw-rw-rw-   0        0        0     1544 2023-04-16 08:25:53.000000 django-cheroot-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1929 2023-04-16 10:06:06.205467 django-cheroot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1118 2023-04-16 10:03:37.000000 django-cheroot-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 10:06:06.194466 django-cheroot-1.0.0/django_cheroot/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:24:33.000000 django-cheroot-1.0.0/django_cheroot/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-16 06:24:33.000000 django-cheroot-1.0.0/django_cheroot/admin.py
--rw-rw-rw-   0        0        0      165 2023-04-16 06:24:34.000000 django-cheroot-1.0.0/django_cheroot/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:06:06.203468 django-cheroot-1.0.0/django_cheroot.egg-info/
--rw-rw-rw-   0        0        0     1929 2023-04-16 10:06:06.000000 django-cheroot-1.0.0/django_cheroot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-16 10:06:06.000000 django-cheroot-1.0.0/django_cheroot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:06:06.000000 django-cheroot-1.0.0/django_cheroot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-16 10:06:06.000000 django-cheroot-1.0.0/django_cheroot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 10:06:06.000000 django-cheroot-1.0.0/django_cheroot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 10:06:06.206467 django-cheroot-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-04-16 08:37:35.000000 django-cheroot-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:32:30.613252 django-cheroot-1.0.1/
+-rw-rw-rw-   0        0        0     1544 2023-04-16 08:25:53.000000 django-cheroot-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2087 2023-04-18 18:32:30.612274 django-cheroot-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2023-04-16 10:08:45.000000 django-cheroot-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 18:32:30.592597 django-cheroot-1.0.1/django_cheroot/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:24:33.000000 django-cheroot-1.0.1/django_cheroot/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-16 06:24:33.000000 django-cheroot-1.0.1/django_cheroot/admin.py
+-rw-rw-rw-   0        0        0      165 2023-04-16 06:24:34.000000 django-cheroot-1.0.1/django_cheroot/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:32:30.604417 django-cheroot-1.0.1/django_cheroot/management/
+-rw-rw-rw-   0        0        0        0 2023-04-18 18:31:28.000000 django-cheroot-1.0.1/django_cheroot/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:32:30.608369 django-cheroot-1.0.1/django_cheroot/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-18 18:31:33.000000 django-cheroot-1.0.1/django_cheroot/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1812 2023-04-16 09:59:06.000000 django-cheroot-1.0.1/django_cheroot/management/commands/cheroot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 18:32:30.602438 django-cheroot-1.0.1/django_cheroot.egg-info/
+-rw-rw-rw-   0        0        0     2087 2023-04-18 18:32:30.000000 django-cheroot-1.0.1/django_cheroot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-04-18 18:32:30.000000 django-cheroot-1.0.1/django_cheroot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 18:32:30.000000 django-cheroot-1.0.1/django_cheroot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-18 18:32:30.000000 django-cheroot-1.0.1/django_cheroot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 18:32:30.000000 django-cheroot-1.0.1/django_cheroot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 18:32:30.613252 django-cheroot-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-04-16 10:44:04.000000 django-cheroot-1.0.1/setup.py
```

### Comparing `django-cheroot-1.0.0/LICENSE` & `django-cheroot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cheroot-1.0.0/PKG-INFO` & `django-cheroot-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cheroot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Cheroot provides a bridge to use Cheroot which is the high-performance, pure-Python HTTP server used by CherryPy
 Home-page: https://github.com/modbender/django-cheroot
 Author: Yashas H R
 Author-email: rameshmamathayashas@gmail.com
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -44,15 +44,18 @@
 ```shell
 python manage.py cheroot
 ```
 
 Default arguments
 
 ```shell
-python manage.py cheroot
+python manage.py cheroot -h 127.0.0.1 -p 8000 -w 40 -t 30 -c 20
+```
+```shell
+python manage.py cheroot --host 127.0.0.1 --port 8000 --maxthreads 40 --minthreads 30 --connections 20
 ```
 
 ## Arguments
 
 | Name                       | Short | Long          | Type | Default   |
 | -------------------------- | ----- | ------------- | ---- | --------- |
 | IP Address                 | -h    | --host        | str  | 127.0.0.1 |
```

### Comparing `django-cheroot-1.0.0/README.md` & `django-cheroot-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 ```shell
 python manage.py cheroot
 ```
 
 Default arguments
 
 ```shell
-python manage.py cheroot
+python manage.py cheroot -h 127.0.0.1 -p 8000 -w 40 -t 30 -c 20
+```
+```shell
+python manage.py cheroot --host 127.0.0.1 --port 8000 --maxthreads 40 --minthreads 30 --connections 20
 ```
 
 ## Arguments
 
 | Name                       | Short | Long          | Type | Default   |
 | -------------------------- | ----- | ------------- | ---- | --------- |
 | IP Address                 | -h    | --host        | str  | 127.0.0.1 |
```

### Comparing `django-cheroot-1.0.0/django_cheroot.egg-info/PKG-INFO` & `django-cheroot-1.0.1/django_cheroot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cheroot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Cheroot provides a bridge to use Cheroot which is the high-performance, pure-Python HTTP server used by CherryPy
 Home-page: https://github.com/modbender/django-cheroot
 Author: Yashas H R
 Author-email: rameshmamathayashas@gmail.com
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -44,15 +44,18 @@
 ```shell
 python manage.py cheroot
 ```
 
 Default arguments
 
 ```shell
-python manage.py cheroot
+python manage.py cheroot -h 127.0.0.1 -p 8000 -w 40 -t 30 -c 20
+```
+```shell
+python manage.py cheroot --host 127.0.0.1 --port 8000 --maxthreads 40 --minthreads 30 --connections 20
 ```
 
 ## Arguments
 
 | Name                       | Short | Long          | Type | Default   |
 | -------------------------- | ----- | ------------- | ---- | --------- |
 | IP Address                 | -h    | --host        | str  | 127.0.0.1 |
```

### Comparing `django-cheroot-1.0.0/setup.py` & `django-cheroot-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 README = open('README.md').read()
 
 setuptools.setup(
     name='django-cheroot',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/modbender/django-cheroot',
     description='Django Cheroot provides a bridge to use Cheroot which is the high-performance, pure-Python HTTP server used by CherryPy',
     long_description=README,
     long_description_content_type='text/markdown',
     author='Yashas H R',
     author_email='rameshmamathayashas@gmail.com',
     install_requires=[
```

