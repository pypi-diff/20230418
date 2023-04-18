# Comparing `tmp/nparray2pil-0.0.1.tar.gz` & `tmp/nparray2pil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nparray2pil-0.0.1.tar", last modified: Mon Apr 17 12:42:11 2023, max compression
+gzip compressed data, was "nparray2pil-0.0.3.tar", last modified: Tue Apr 18 10:36:39 2023, max compression
```

## Comparing `nparray2pil-0.0.1.tar` & `nparray2pil-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.398545 nparray2pil-0.0.1/
--rw-rw-rw-   0        0        0     1769 2023-04-17 12:42:11.390558 nparray2pil-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-04-17 12:42:01.000000 nparray2pil-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.341138 nparray2pil-0.0.1/nparray2pil/
--rw-rw-rw-   0        0        0       36 2023-04-17 12:08:53.000000 nparray2pil-0.0.1/nparray2pil/__init__.py
--rw-rw-rw-   0        0        0      211 2023-04-17 12:12:04.000000 nparray2pil-0.0.1/nparray2pil/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.382510 nparray2pil-0.0.1/nparray2pil.egg-info/
--rw-rw-rw-   0        0        0     1769 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:42:11.398545 nparray2pil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1496 2023-04-17 12:41:37.000000 nparray2pil-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:36:39.026157 nparray2pil-0.0.3/
+-rw-rw-rw-   0        0        0     1740 2023-04-18 10:36:39.026157 nparray2pil-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2023-04-18 10:36:25.000000 nparray2pil-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:36:38.994158 nparray2pil-0.0.3/nparray2pil/
+-rw-rw-rw-   0        0        0       36 2023-04-17 12:08:53.000000 nparray2pil-0.0.3/nparray2pil/__init__.py
+-rw-rw-rw-   0        0        0      211 2023-04-17 12:12:04.000000 nparray2pil-0.0.3/nparray2pil/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:36:39.018639 nparray2pil-0.0.3/nparray2pil.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-04-18 10:36:38.000000 nparray2pil-0.0.3/nparray2pil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-18 10:36:38.000000 nparray2pil-0.0.3/nparray2pil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:36:38.000000 nparray2pil-0.0.3/nparray2pil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-18 10:36:38.000000 nparray2pil-0.0.3/nparray2pil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 10:36:38.000000 nparray2pil-0.0.3/nparray2pil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:36:39.031591 nparray2pil-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1496 2023-04-18 10:36:28.000000 nparray2pil-0.0.3/setup.py
```

### Comparing `nparray2pil-0.0.1/PKG-INFO` & `nparray2pil-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: nparray2pil
-Version: 0.0.1
+Version: 0.0.3
 Summary: Converts numpy arrays into images.
 Home-page: https://github.com/abhinav-gg/nparray2pil/
 Author: Abhinav G, Oliver Gibson
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: np,array,pil,convertion,convert,opencv,array to pil
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # nparray2pil
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a numpy array into a PIL image.
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import nparray2pil to get access to the convert functions:**
 ```python
 from nparray2pil import convert
 ```
```

### Comparing `nparray2pil-0.0.1/README.md` & `nparray2pil-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # nparray2pil
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a numpy array into a PIL image.
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import nparray2pil to get access to the convert functions:**
 ```python
 from nparray2pil import convert
 ```
```

### Comparing `nparray2pil-0.0.1/nparray2pil.egg-info/PKG-INFO` & `nparray2pil-0.0.3/nparray2pil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: nparray2pil
-Version: 0.0.1
+Version: 0.0.3
 Summary: Converts numpy arrays into images.
 Home-page: https://github.com/abhinav-gg/nparray2pil/
 Author: Abhinav G, Oliver Gibson
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: np,array,pil,convertion,convert,opencv,array to pil
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # nparray2pil
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a numpy array into a PIL image.
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import nparray2pil to get access to the convert functions:**
 ```python
 from nparray2pil import convert
 ```
```

### Comparing `nparray2pil-0.0.1/setup.py` & `nparray2pil-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="nparray2pil",
  
     # version of the module
-    version="0.0.1",
+    version="0.0.3",
  
     # Name of Author
     author="Abhinav G, Oliver Gibson",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
```

