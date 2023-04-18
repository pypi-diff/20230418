# Comparing `tmp/FtoC-0.0.1.tar.gz` & `tmp/FtoC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FtoC-0.0.1.tar", last modified: Tue Apr 18 10:27:25 2023, max compression
+gzip compressed data, was "FtoC-0.0.2.tar", last modified: Tue Apr 18 10:29:56 2023, max compression
```

## Comparing `FtoC-0.0.1.tar` & `FtoC-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:27:25.517046 FtoC-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:27:25.484210 FtoC-0.0.1/FtoC/
--rw-rw-rw-   0        0        0      123 2023-04-18 10:20:46.000000 FtoC-0.0.1/FtoC/__init__.py
--rw-rw-rw-   0        0        0      245 2023-04-18 09:02:57.000000 FtoC-0.0.1/FtoC/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:27:25.509012 FtoC-0.0.1/FtoC.egg-info/
--rw-rw-rw-   0        0        0     1736 2023-04-18 10:27:25.000000 FtoC-0.0.1/FtoC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-18 10:27:25.000000 FtoC-0.0.1/FtoC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:27:25.000000 FtoC-0.0.1/FtoC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 10:27:25.000000 FtoC-0.0.1/FtoC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1736 2023-04-18 10:27:25.517046 FtoC-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-04-18 10:27:18.000000 FtoC-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 10:27:25.517046 FtoC-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-04-18 10:22:25.000000 FtoC-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.944390 FtoC-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.919927 FtoC-0.0.2/FtoC/
+-rw-rw-rw-   0        0        0      123 2023-04-18 10:20:46.000000 FtoC-0.0.2/FtoC/__init__.py
+-rw-rw-rw-   0        0        0      245 2023-04-18 09:02:57.000000 FtoC-0.0.2/FtoC/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:29:56.938367 FtoC-0.0.2/FtoC.egg-info/
+-rw-rw-rw-   0        0        0     1750 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 10:29:56.000000 FtoC-0.0.2/FtoC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1750 2023-04-18 10:29:56.944390 FtoC-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-04-18 10:27:18.000000 FtoC-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:29:56.944390 FtoC-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-18 10:29:52.000000 FtoC-0.0.2/setup.py
```

### Comparing `FtoC-0.0.1/FtoC.egg-info/PKG-INFO` & `FtoC-0.0.2/FtoC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: FtoC
-Version: 0.0.1
-Summary: Converts numpy arrays into images.
+Version: 0.0.2
+Summary: Converts temperatures from farenheit to celsius.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/FtoC
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: faren,farenheit,temp,temperature,degrees,degrees c,degrees f,celsius,c,f,ftoc
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FtoC-0.0.1/PKG-INFO` & `FtoC-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: FtoC
-Version: 0.0.1
-Summary: Converts numpy arrays into images.
+Version: 0.0.2
+Summary: Converts temperatures from farenheit to celsius.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/FtoC
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: faren,farenheit,temp,temperature,degrees,degrees c,degrees f,celsius,c,f,ftoc
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FtoC-0.0.1/README.md` & `FtoC-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FtoC-0.0.1/setup.py` & `FtoC-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="FtoC",
  
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
  
     # Name of Author
     author="Abhinav G",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
  
     # #Small Description about module
-    description="Converts numpy arrays into images.",
+    description="Converts temperatures from farenheit to celsius.",
  
     # long_description=long_description,
  
     # Specifying that we are using markdown file for description
     long_description=long_description,
     long_description_content_type="text/markdown",
```

