# Comparing `tmp/ByeByeLogger-2.1.5.tar.gz` & `tmp/ByeByeLogger-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ByeByeLogger-2.1.5.tar", last modified: Fri Apr 14 13:11:46 2023, max compression
+gzip compressed data, was "ByeByeLogger-3.0.0.tar", last modified: Tue Apr 18 04:08:36 2023, max compression
```

## Comparing `ByeByeLogger-2.1.5.tar` & `ByeByeLogger-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.159439 ByeByeLogger-2.1.5/
--rw-rw-rw-   0        0        0      978 2023-04-14 13:11:46.159439 ByeByeLogger-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-14 13:11:46.160442 ByeByeLogger-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-04-14 13:11:43.000000 ByeByeLogger-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.124441 ByeByeLogger-2.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.142438 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/
--rw-rw-rw-   0        0        0      978 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.144441 ByeByeLogger-2.1.5/src/byebyelogger/
--rw-rw-rw-   0        0        0      496 2023-04-14 12:46:34.000000 ByeByeLogger-2.1.5/src/byebyelogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.151441 ByeByeLogger-2.1.5/src/byebyelogger/core/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-04-14 12:54:13.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/datascience.py
--rw-rw-rw-   0        0        0     1898 2023-04-14 12:53:47.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/repository.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.157441 ByeByeLogger-2.1.5/src/byebyelogger/style/
--rw-rw-rw-   0        0        0        0 2023-04-14 11:23:20.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/colorizer.py
--rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.040716 ByeByeLogger-3.0.0/
+-rw-rw-rw-   0        0        0     2714 2023-04-18 04:08:36.040716 ByeByeLogger-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2084 2023-04-18 04:05:33.000000 ByeByeLogger-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 04:08:36.040716 ByeByeLogger-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-04-18 04:08:12.000000 ByeByeLogger-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.016714 ByeByeLogger-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.026716 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/
+-rw-rw-rw-   0        0        0     2714 2023-04-18 04:08:34.000000 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-04-18 04:08:35.000000 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 04:08:34.000000 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 04:08:35.000000 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 04:08:35.000000 ByeByeLogger-3.0.0/src/ByeByeLogger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.030716 ByeByeLogger-3.0.0/src/byebyelogger/
+-rw-rw-rw-   0        0        0      750 2023-04-18 03:28:05.000000 ByeByeLogger-3.0.0/src/byebyelogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.034713 ByeByeLogger-3.0.0/src/byebyelogger/core/
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 ByeByeLogger-3.0.0/src/byebyelogger/core/__init__.py
+-rw-rw-rw-   0        0        0     2712 2023-04-18 03:25:30.000000 ByeByeLogger-3.0.0/src/byebyelogger/core/configuration.py
+-rw-rw-rw-   0        0        0     1304 2023-04-18 02:05:15.000000 ByeByeLogger-3.0.0/src/byebyelogger/core/stack_info.py
+-rw-rw-rw-   0        0        0     2584 2023-04-18 04:07:55.000000 ByeByeLogger-3.0.0/src/byebyelogger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:08:36.038712 ByeByeLogger-3.0.0/src/byebyelogger/style/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:32:48.000000 ByeByeLogger-3.0.0/src/byebyelogger/style/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-04-17 21:26:31.000000 ByeByeLogger-3.0.0/src/byebyelogger/style/color.py
+-rw-rw-rw-   0        0        0      496 2023-04-17 21:34:44.000000 ByeByeLogger-3.0.0/src/byebyelogger/style/format.py
```

### Comparing `ByeByeLogger-2.1.5/setup.py` & `ByeByeLogger-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from setuptools import find_packages, setup
+
 with open("src/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ByeByeLogger",
-    version = "2.1.5",
+    version="3.0.0",
     description="A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aleksa Lukic",
-    classifiers=["License :: OSI Approved :: MIT License",
-                 "Operating System :: OS Independent",
-                 "Programming Language :: Python :: 3.7",
-                 "Programming Language :: Python :: 3.8",
-                 "Programming Language :: Python :: 3.9",
-                 "Programming Language :: Python :: 3.10",
-                 "Programming Language :: Python :: 3.11",
-                ],
-    install_requires=["colorama==0.4.6"],)
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    install_requires=["colorama==0.4.6"],
+)
```

### Comparing `ByeByeLogger-2.1.5/src/byebyelogger/style/colorizer.py` & `ByeByeLogger-3.0.0/src/byebyelogger/style/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import colorama
 from colorama import Fore, Style
+
 colorama.init(autoreset=True)
 
+
 class Color:
     def __init__(self, color: str):
         self.color = color.upper()
-        
+
         if self.color in Fore.__dict__:
             self.wrappercolor = Fore.__dict__[self.color]
         else:
-            raise ValueError(f"Invalid color '{color}'. Choose a valid color from colorama.Fore.")
-    
+            raise ValueError(
+                f"Invalid color '{color}'. Choose a valid color from colorama.Fore."
+            )
+
     def __call__(self, string: str) -> str:
         return f"{self.wrappercolor}{Style.BRIGHT}{string}{Fore.RESET}"
 
 
-
 BLACK = Color("BLACK")
 RED = Color("RED")
 GREEN = Color("GREEN")
 YELLOW = Color("YELLOW")
 BLUE = Color("BLUE")
 MAGENTA = Color("MAGENTA")
 CYAN = Color("CYAN")
```

