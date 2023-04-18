# Comparing `tmp/FtoC-0.0.2.tar.gz` & `tmp/FtoC-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FtoC-0.0.2.tar", last modified: Tue Apr 18 10:29:56 2023, max compression
+gzip compressed data, was "FtoC-0.0.3.tar", last modified: Tue Apr 18 10:34:01 2023, max compression
```

## Comparing `FtoC-0.0.2.tar` & `FtoC-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.944390 FtoC-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.919927 FtoC-0.0.2/FtoC/
--rw-rw-rw-   0        0        0      123 2023-04-18 10:20:46.000000 FtoC-0.0.2/FtoC/__init__.py
--rw-rw-rw-   0        0        0      245 2023-04-18 09:02:57.000000 FtoC-0.0.2/FtoC/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.938367 FtoC-0.0.2/FtoC.egg-info/
--rw-rw-rw-   0        0        0     1750 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1750 2023-04-18 10:29:56.944390 FtoC-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-04-18 10:27:18.000000 FtoC-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 10:29:56.944390 FtoC-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1468 2023-04-18 10:29:52.000000 FtoC-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:34:01.205079 FtoC-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:34:01.164504 FtoC-0.0.3/FtoC/
+-rw-rw-rw-   0        0        0      123 2023-04-18 10:20:46.000000 FtoC-0.0.3/FtoC/__init__.py
+-rw-rw-rw-   0        0        0      245 2023-04-18 09:02:57.000000 FtoC-0.0.3/FtoC/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:34:01.189070 FtoC-0.0.3/FtoC.egg-info/
+-rw-rw-rw-   0        0        0     1730 2023-04-18 10:34:00.000000 FtoC-0.0.3/FtoC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-18 10:34:01.000000 FtoC-0.0.3/FtoC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:34:00.000000 FtoC-0.0.3/FtoC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 10:34:00.000000 FtoC-0.0.3/FtoC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1730 2023-04-18 10:34:01.197084 FtoC-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-04-18 10:33:23.000000 FtoC-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:34:01.206298 FtoC-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-18 10:32:05.000000 FtoC-0.0.3/setup.py
```

### Comparing `FtoC-0.0.2/FtoC.egg-info/PKG-INFO` & `FtoC-0.0.3/FtoC.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: FtoC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converts temperatures from farenheit to celsius.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/FtoC
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: faren,farenheit,temp,temperature,degrees,degrees c,degrees f,celsius,c,f,ftoc
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # FtoC
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a temperature from farenheit to celsius!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import FtoC to get access to the convert functions:**
 ```python
 from FtoC import convert
 ```
```

### Comparing `FtoC-0.0.2/PKG-INFO` & `FtoC-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: FtoC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converts temperatures from farenheit to celsius.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/FtoC
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: faren,farenheit,temp,temperature,degrees,degrees c,degrees f,celsius,c,f,ftoc
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # FtoC
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a temperature from farenheit to celsius!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import FtoC to get access to the convert functions:**
 ```python
 from FtoC import convert
 ```
```

### Comparing `FtoC-0.0.2/README.md` & `FtoC-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # FtoC
 
-A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
+A PyPi module allowing the user to convert a temperature from farenheit to celsius!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import FtoC to get access to the convert functions:**
 ```python
 from FtoC import convert
 ```
```

### Comparing `FtoC-0.0.2/setup.py` & `FtoC-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="FtoC",
  
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
  
     # Name of Author
     author="Abhinav G",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
```

