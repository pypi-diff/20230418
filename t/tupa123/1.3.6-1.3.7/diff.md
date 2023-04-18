# Comparing `tmp/tupa123-1.3.6.tar.gz` & `tmp/tupa123-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.6.tar", last modified: Mon Apr 17 21:01:09 2023, max compression
+gzip compressed data, was "tupa123-1.3.7.tar", last modified: Tue Apr 18 11:51:49 2023, max compression
```

## Comparing `tupa123-1.3.6.tar` & `tupa123-1.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.546476 tupa123-1.3.6/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0     7904 2023-04-17 21:01:09.545507 tupa123-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     7428 2023-04-17 21:00:27.000000 tupa123-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 21:01:09.546476 tupa123-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 21:00:39.000000 tupa123-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.534536 tupa123-1.3.6/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.6/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.6/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.543513 tupa123-1.3.6/tupa123.egg-info/
--rw-rw-rw-   0        0        0     7904 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.195545 tupa123-1.3.7/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2345 2023-04-18 11:51:49.195545 tupa123-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-04-18 11:48:41.000000 tupa123-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 11:51:49.195545 tupa123-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-18 11:46:01.000000 tupa123-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.179924 tupa123-1.3.7/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.7/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.7/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:51:49.195545 tupa123-1.3.7/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2345 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 11:51:49.000000 tupa123-1.3.7/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.6/LICENSE.txt` & `tupa123-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.6/setup.py` & `tupa123-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.6',
+    version='1.3.7',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.6/tupa123/tupa123.py` & `tupa123-1.3.7/tupa123/tupa123.py`

 * *Files identical despite different names*

