# Comparing `tmp/fwdviewpy-0.1.2.tar.gz` & `tmp/fwdviewpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.2.tar", last modified: Mon Apr 17 18:41:11 2023, max compression
+gzip compressed data, was "fwdviewpy-0.1.3.tar", last modified: Tue Apr 18 09:28:27 2023, max compression
```

## Comparing `fwdviewpy-0.1.2.tar` & `fwdviewpy-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:41:11.108738 fwdviewpy-0.1.2/
--rw-rw-rw-   0        0        0      465 2023-04-17 18:41:11.103735 fwdviewpy-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 18:41:11.069354 fwdviewpy-0.1.2/fwdviewpy/
--rw-rw-rw-   0        0        0    10482 2023-04-17 15:48:31.000000 fwdviewpy-0.1.2/fwdviewpy/fwdviewpy.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:41:11.099736 fwdviewpy-0.1.2/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      465 2023-04-17 18:41:10.000000 fwdviewpy-0.1.2/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-17 18:41:10.000000 fwdviewpy-0.1.2/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:41:10.000000 fwdviewpy-0.1.2/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 18:41:10.000000 fwdviewpy-0.1.2/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 18:41:10.000000 fwdviewpy-0.1.2/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 18:41:11.109737 fwdviewpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      619 2023-04-17 18:40:18.000000 fwdviewpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:28:27.162554 fwdviewpy-0.1.3/
+-rw-rw-rw-   0        0        0      623 2023-04-18 09:28:27.158557 fwdviewpy-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 09:28:27.129395 fwdviewpy-0.1.3/fwdviewpy/
+-rw-rw-rw-   0        0        0      111 2023-04-18 09:23:00.000000 fwdviewpy-0.1.3/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    10482 2023-04-17 15:48:31.000000 fwdviewpy-0.1.3/fwdviewpy/fwdviewpy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:28:27.154565 fwdviewpy-0.1.3/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-04-18 09:28:27.000000 fwdviewpy-0.1.3/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-18 09:28:27.000000 fwdviewpy-0.1.3/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:28:27.000000 fwdviewpy-0.1.3/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 09:28:27.000000 fwdviewpy-0.1.3/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 09:28:27.000000 fwdviewpy-0.1.3/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:28:27.163552 fwdviewpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-04-18 09:28:20.000000 fwdviewpy-0.1.3/setup.py
```

### Comparing `fwdviewpy-0.1.2/fwdviewpy/fwdviewpy.py` & `fwdviewpy-0.1.3/fwdviewpy/fwdviewpy.py`

 * *Files identical despite different names*

### Comparing `fwdviewpy-0.1.2/setup.py` & `fwdviewpy-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from setuptools import setup
 
 setup(
     name='fwdviewpy',
-    version='0.1.2',
-    description='Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.',
+    version='0.1.3',
+    description='Python package developed by FWD View - The Data Transformation Specialists.',
+    long_description='Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.',
     packages=['fwdviewpy'],
+    author='Cameron Bose & Ryan Springett',
+    author_email="cameron.bose@fwdview.com",
+
     install_requires=[
         'requests'
     ],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
```

