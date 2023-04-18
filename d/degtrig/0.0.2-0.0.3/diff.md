# Comparing `tmp/degtrig-0.0.2.tar.gz` & `tmp/degtrig-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degtrig-0.0.2.tar", last modified: Tue Apr 18 10:50:45 2023, max compression
+gzip compressed data, was "degtrig-0.0.3.tar", last modified: Tue Apr 18 10:59:22 2023, max compression
```

## Comparing `degtrig-0.0.2.tar` & `degtrig-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.524823 degtrig-0.0.2/
--rw-rw-rw-   0        0        0     2020 2023-04-18 10:50:45.523513 degtrig-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1398 2023-04-18 10:50:34.000000 degtrig-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.491616 degtrig-0.0.2/degtrig/
--rw-rw-rw-   0        0        0      119 2023-04-18 09:34:28.000000 degtrig-0.0.2/degtrig/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-04-18 10:49:35.000000 degtrig-0.0.2/degtrig/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:50:45.515256 degtrig-0.0.2/degtrig.egg-info/
--rw-rw-rw-   0        0        0     2020 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 10:50:45.000000 degtrig-0.0.2/degtrig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:50:45.524823 degtrig-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-04-18 10:50:40.000000 degtrig-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:59:22.151643 degtrig-0.0.3/
+-rw-rw-rw-   0        0        0     2032 2023-04-18 10:59:22.151643 degtrig-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1410 2023-04-18 10:58:55.000000 degtrig-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:59:22.117861 degtrig-0.0.3/degtrig/
+-rw-rw-rw-   0        0        0      119 2023-04-18 09:34:28.000000 degtrig-0.0.3/degtrig/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-04-18 10:58:09.000000 degtrig-0.0.3/degtrig/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:59:22.144587 degtrig-0.0.3/degtrig.egg-info/
+-rw-rw-rw-   0        0        0     2032 2023-04-18 10:59:21.000000 degtrig-0.0.3/degtrig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-18 10:59:22.000000 degtrig-0.0.3/degtrig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:59:21.000000 degtrig-0.0.3/degtrig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 10:59:21.000000 degtrig-0.0.3/degtrig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:59:22.156654 degtrig-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2023-04-18 10:59:18.000000 degtrig-0.0.3/setup.py
```

### Comparing `degtrig-0.0.2/PKG-INFO` & `degtrig-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-Metadata-Version: 2.1
-Name: degtrig
-Version: 0.0.2
-Summary: Adds all of the trigonometric functions using degrees instead of radians.
-Home-page: https://github.com/abhinav-gg/StupidPipPackages/DegTrig
-Author: Abhinav G
-Author-email: agupta.cam7@gmail.com
-License: MIT
-Keywords: trigonometry,radians,degrees,trig,convert,radians to degrees,degrees to radians,deg,rad,hyperbolic,hyperbolic functions
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # DegTrig
 
 A PyPi module providing all of the trigonometric functions that deal in degrees. No more math and numpy radians confusion!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.2-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import DegTrig to get access to the convert functions:**
 
 ```python
-from degtrig import \*
+from degtrig import *
 ```
 and then use the functions:
 ```python
 sin(30)
 cosh(1)
 asin(1/2)
-atanh(9)
+atanh(0.1)
 cot(60)
+asec(0.9)
 ```
 
 ## Why DegTrig
 
 `math` provides trigonometric functions however the normal functions use radians while the hyperbolic functions use degrees. It's all a little too much to remember! DegTrig provides the answer to this problem by unifying the functions so that they all use degrees (the better unit of rotation).
 
 ## Installation
@@ -65,9 +51,8 @@
 5. Make sure that the script does not have errors or warnings
 6. Create a new Pull Request
 
 ## License
 
 This tool is open source under the [MIT License](https://opensource.org/licenses/MIT) terms.
 
-[[Back To Top]](#DegTrig)
-
+[[Back To Top]](#DegTrig)
```

### Comparing `degtrig-0.0.2/degtrig/main.py` & `degtrig-0.0.3/degtrig/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import math
 pi = math.pi
 
 def sin(deg: float) -> float:
     return math.sin(deg * math.pi / 180)
 
 def cos(deg: float) -> float:
@@ -41,8 +40,20 @@
 def cot(deg: float) -> float:
     return 1 / tan(deg)
 
 def sec(deg: float) -> float:
     return 1 / cos(deg)
 
 def cosec(deg: float) -> float:
-    return 1 / sin(deg)
+    return 1 / sin(deg)
+
+def acot(deg: float) -> float:
+    return 1 / atan(deg)
+
+def asec(deg: float) -> float:
+    return 1 / acos(deg)
+
+def acosec(deg: float) -> float:
+    return 1 / asin(deg)
+
+def radians(deg: float) -> float:
+    return math.radians(deg)
```

### Comparing `degtrig-0.0.2/degtrig.egg-info/PKG-INFO` & `degtrig-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degtrig
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adds all of the trigonometric functions using degrees instead of radians.
 Home-page: https://github.com/abhinav-gg/StupidPipPackages/DegTrig
 Author: Abhinav G
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: trigonometry,radians,degrees,trig,convert,radians to degrees,degrees to radians,deg,rad,hyperbolic,hyperbolic functions
 Platform: UNKNOWN
@@ -13,30 +13,31 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # DegTrig
 
 A PyPi module providing all of the trigonometric functions that deal in degrees. No more math and numpy radians confusion!
 
-![Generic badge](https://img.shields.io/badge/version-0.0.2-green.svg)
+![Generic badge](https://img.shields.io/badge/version-0.0.3-green.svg)
 
 ## How does it work?
 
 **Use import DegTrig to get access to the convert functions:**
 
 ```python
-from degtrig import \*
+from degtrig import *
 ```
 and then use the functions:
 ```python
 sin(30)
 cosh(1)
 asin(1/2)
-atanh(9)
+atanh(0.1)
 cot(60)
+asec(0.9)
 ```
 
 ## Why DegTrig
 
 `math` provides trigonometric functions however the normal functions use radians while the hyperbolic functions use degrees. It's all a little too much to remember! DegTrig provides the answer to this problem by unifying the functions so that they all use degrees (the better unit of rotation).
 
 ## Installation
```

### Comparing `degtrig-0.0.2/setup.py` & `degtrig-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="degtrig",
  
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
  
     # Name of Author
     author="Abhinav G",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
```

