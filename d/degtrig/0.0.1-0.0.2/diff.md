# Comparing `tmp/degtrig-0.0.1.tar.gz` & `tmp/degtrig-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degtrig-0.0.1.tar", last modified: Tue Apr 18 10:44:44 2023, max compression
+gzip compressed data, was "degtrig-0.0.2.tar", last modified: Tue Apr 18 10:50:45 2023, max compression
```

## Comparing `degtrig-0.0.1.tar` & `degtrig-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:44:44.105658 degtrig-0.0.1/
--rw-rw-rw-   0        0        0     2011 2023-04-18 10:44:44.104635 degtrig-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2023-04-18 10:41:39.000000 degtrig-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:44:44.073698 degtrig-0.0.1/degtrig/
--rw-rw-rw-   0        0        0      119 2023-04-18 09:34:28.000000 degtrig-0.0.1/degtrig/__init__.py
--rw-rw-rw-   0        0        0      873 2023-04-18 10:10:05.000000 degtrig-0.0.1/degtrig/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:44:44.097121 degtrig-0.0.1/degtrig.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-04-18 10:44:43.000000 degtrig-0.0.1/degtrig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-18 10:44:43.000000 degtrig-0.0.1/degtrig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:44:43.000000 degtrig-0.0.1/degtrig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 10:44:43.000000 degtrig-0.0.1/degtrig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:44:44.105658 degtrig-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-04-18 10:44:25.000000 degtrig-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.524823 degtrig-0.0.2/
+-rw-rw-rw-   0        0        0     2020 2023-04-18 10:50:45.523513 degtrig-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1398 2023-04-18 10:50:34.000000 degtrig-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.491616 degtrig-0.0.2/degtrig/
+-rw-rw-rw-   0        0        0      119 2023-04-18 09:34:28.000000 degtrig-0.0.2/degtrig/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-04-18 10:49:35.000000 degtrig-0.0.2/degtrig/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.515256 degtrig-0.0.2/degtrig.egg-info/
+-rw-rw-rw-   0        0        0     2020 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:50:45.524823 degtrig-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2023-04-18 10:50:40.000000 degtrig-0.0.2/setup.py
```

### Comparing `degtrig-0.0.1/PKG-INFO` & `degtrig-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degtrig
-Version: 0.0.1
+Version: 0.0.2
 Summary: Adds all of the trigonometric functions using degrees instead of radians.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/DegTrig
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: trigonometry,radians,degrees,trig,convert,radians to degrees,degrees to radians,deg,rad,hyperbolic,hyperbolic functions
 Platform: UNKNOWN
@@ -13,29 +13,30 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # DegTrig
 
 A PyPi module providing all of the trigonometric functions that deal in degrees. No more math and numpy radians confusion!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.2-green.svg)
 
 ## How does it work?
 
 **Use import DegTrig to get access to the convert functions:**
 
 ```python
 from degtrig import \*
 ```
 and then use the functions:
 ```python
 sin(30)
 cosh(1)
 asin(1/2)
 atanh(9)
+cot(60)
 ```
 
 ## Why DegTrig
 
 `math` provides trigonometric functions however the normal functions use radians while the hyperbolic functions use degrees. It's all a little too much to remember! DegTrig provides the answer to this problem by unifying the functions so that they all use degrees (the better unit of rotation).
 
 ## Installation
```

### Comparing `degtrig-0.0.1/README.md` & `degtrig-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # DegTrig
 
 A PyPi module providing all of the trigonometric functions that deal in degrees. No more math and numpy radians confusion!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.2-green.svg)
 
 ## How does it work?
 
 **Use import DegTrig to get access to the convert functions:**
 
 ```python
 from degtrig import \*
 ```
 and then use the functions:
 ```python
 sin(30)
 cosh(1)
 asin(1/2)
 atanh(9)
+cot(60)
 ```
 
 ## Why DegTrig
 
 `math` provides trigonometric functions however the normal functions use radians while the hyperbolic functions use degrees. It's all a little too much to remember! DegTrig provides the answer to this problem by unifying the functions so that they all use degrees (the better unit of rotation).
 
 ## Installation
```

### Comparing `degtrig-0.0.1/degtrig/main.py` & `degtrig-0.0.2/degtrig/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,8 +32,17 @@
 def asinh(ratio: float) -> float:
     return math.asinh(ratio)
 
 def acosh(ratio: float) -> float:
     return math.acosh(ratio)
 
 def atanh(ratio: float) -> float:
-    return math.atanh(ratio)
+    return math.atanh(ratio)
+
+def cot(deg: float) -> float:
+    return 1 / tan(deg)
+
+def sec(deg: float) -> float:
+    return 1 / cos(deg)
+
+def cosec(deg: float) -> float:
+    return 1 / sin(deg)
```

### Comparing `degtrig-0.0.1/degtrig.egg-info/PKG-INFO` & `degtrig-0.0.2/degtrig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degtrig
-Version: 0.0.1
+Version: 0.0.2
 Summary: Adds all of the trigonometric functions using degrees instead of radians.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/DegTrig
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: trigonometry,radians,degrees,trig,convert,radians to degrees,degrees to radians,deg,rad,hyperbolic,hyperbolic functions
 Platform: UNKNOWN
@@ -13,29 +13,30 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # DegTrig
 
 A PyPi module providing all of the trigonometric functions that deal in degrees. No more math and numpy radians confusion!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.2-green.svg)
 
 ## How does it work?
 
 **Use import DegTrig to get access to the convert functions:**
 
 ```python
 from degtrig import \*
 ```
 and then use the functions:
 ```python
 sin(30)
 cosh(1)
 asin(1/2)
 atanh(9)
+cot(60)
 ```
 
 ## Why DegTrig
 
 `math` provides trigonometric functions however the normal functions use radians while the hyperbolic functions use degrees. It's all a little too much to remember! DegTrig provides the answer to this problem by unifying the functions so that they all use degrees (the better unit of rotation).
 
 ## Installation
```

### Comparing `degtrig-0.0.1/setup.py` & `degtrig-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="degtrig",
  
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
  
     # Name of Author
     author="Abhinav G",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
```

