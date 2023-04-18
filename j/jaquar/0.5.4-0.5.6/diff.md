# Comparing `tmp/jaquar-0.5.4.tar.gz` & `tmp/jaquar-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.5.4.tar", last modified: Tue Apr 18 08:54:06 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.6.tar", last modified: Tue Apr 18 09:03:00 2023, max compression
```

## Comparing `jaquar-0.5.4.tar` & `jaquar-0.5.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:06.000000 jaquar-0.5.4/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar/
--rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.4/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar/templates/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar/templates/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:06.000000 jaquar-0.5.4/jaquar/templates/static/css/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.4/jaquar/templates/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:06.000000 jaquar-0.5.4/jaquar/templates/static/js/
--rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.4/jaquar/templates/static/js/scripts.js
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.4/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:54:06.000000 jaquar-0.5.4/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 08:54:05.000000 jaquar-0.5.4/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2023-04-18 08:54:06.000000 jaquar-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 08:54:06.000000 jaquar-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-04-18 08:54:02.000000 jaquar-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/
+-rw-rw-rw-   0        0        0     4280 2023-04-18 08:46:08.000000 jaquar-0.5.6/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar/templates/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar/templates/static/css/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:39.000000 jaquar-0.5.6/jaquar/templates/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar/templates/static/js/
+-rw-rw-rw-   0        0        0        0 2023-04-18 08:36:27.000000 jaquar-0.5.6/jaquar/templates/static/js/scripts.js
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.6/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:03:00.000000 jaquar-0.5.6/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:02:59.000000 jaquar-0.5.6/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 09:03:00.000000 jaquar-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 09:03:00.000000 jaquar-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-04-18 09:02:50.000000 jaquar-0.5.6/setup.py
```

### Comparing `jaquar-0.5.4/jaquar/cli.py` & `jaquar-0.5.6/jaquar/cli.py`

 * *Files identical despite different names*

### Comparing `jaquar-0.5.4/setup.py` & `jaquar-0.5.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jaquar',
-    version='0.5.4',
+    version='0.5.6',
     description='A web framework for python',
     url='http://skillfam.writermint.com',
     license='BSD',
     author='Kipono Japhet',
     packages=find_packages(),
     install_requires=[
         'click',
@@ -15,11 +15,11 @@
         'werkzeug',
     ],
     entry_points='''
         [console_scripts]
         jaquar=jaquar.cli:cli
     ''',
     package_data={
-        'jaquar': ['templates/*'],
+        'jaquar': ['templates/**/*'],
     },
     include_package_data=True,
 )
```

