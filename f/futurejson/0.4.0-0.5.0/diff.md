# Comparing `tmp/futurejson-0.4.0.tar.gz` & `tmp/futurejson-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futurejson-0.4.0.tar", last modified: Mon Apr 17 22:19:38 2023, max compression
+gzip compressed data, was "futurejson-0.5.0.tar", last modified: Mon Apr 17 22:28:31 2023, max compression
```

## Comparing `futurejson-0.4.0.tar` & `futurejson-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:19:38.663710 futurejson-0.4.0/
--rw-rw-rw-   0        0        0     1201 2023-04-17 22:19:38.663710 futurejson-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-04-17 21:47:24.000000 futurejson-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:19:38.661711 futurejson-0.4.0/futurejson.egg-info/
--rw-rw-rw-   0        0        0     1201 2023-04-17 22:19:38.000000 futurejson-0.4.0/futurejson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-17 22:19:38.000000 futurejson-0.4.0/futurejson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:19:38.000000 futurejson-0.4.0/futurejson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 22:19:38.000000 futurejson-0.4.0/futurejson.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:19:38.000000 futurejson-0.4.0/futurejson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 22:19:38.664709 futurejson-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-04-17 22:19:13.000000 futurejson-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:28:31.456925 futurejson-0.5.0/
+-rw-rw-rw-   0        0        0     1201 2023-04-17 22:28:31.455925 futurejson-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-04-17 21:47:24.000000 futurejson-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:28:31.454926 futurejson-0.5.0/futurejson.egg-info/
+-rw-rw-rw-   0        0        0     1201 2023-04-17 22:28:31.000000 futurejson-0.5.0/futurejson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-04-17 22:28:31.000000 futurejson-0.5.0/futurejson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:28:31.000000 futurejson-0.5.0/futurejson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 22:28:31.000000 futurejson-0.5.0/futurejson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 22:28:31.000000 futurejson-0.5.0/futurejson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12191 2023-04-17 22:27:48.000000 futurejson-0.5.0/futurejson.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:28:31.456925 futurejson-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-04-17 22:27:16.000000 futurejson-0.5.0/setup.py
```

### Comparing `futurejson-0.4.0/PKG-INFO` & `futurejson-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futurejson
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pure-python FutureJSON implementation
 Author: Andrew
 Author-email: andrew@systemacor.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `futurejson-0.4.0/futurejson.egg-info/PKG-INFO` & `futurejson-0.5.0/futurejson.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futurejson
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pure-python FutureJSON implementation
 Author: Andrew
 Author-email: andrew@systemacor.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `futurejson-0.4.0/setup.py` & `futurejson-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='futurejson',
-    version='0.4.0',
+    version='0.5.0',
     author='Andrew',
     author_email='andrew@systemacor.net',
     description='Pure-python FutureJSON implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'requests',
```

