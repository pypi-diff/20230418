# Comparing `tmp/cs-nds-0.2.0.tar.gz` & `tmp/cs-nds-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-nds-0.2.0.tar", last modified: Sun Mar 19 20:59:21 2023, max compression
+gzip compressed data, was "cs-nds-0.3.0.tar", last modified: Tue Apr 18 09:26:34 2023, max compression
```

## Comparing `cs-nds-0.2.0.tar` & `cs-nds-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-03-19 20:59:21.492670 cs-nds-0.2.0/
--rw-r--r--   0 alex      (1000) wheel      (998)    35149 2023-03-19 20:03:06.000000 cs-nds-0.2.0/LICENSE
--rw-r--r--   0 alex      (1000) wheel      (998)     1342 2023-03-19 20:59:21.492670 cs-nds-0.2.0/PKG-INFO
--rw-r--r--   0 alex      (1000) wheel      (998)      705 2023-03-19 20:56:23.000000 cs-nds-0.2.0/README.md
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-03-19 20:59:21.492670 cs-nds-0.2.0/cs_nds/
--rw-r--r--   0 alex      (1000) wheel      (998)       83 2023-03-19 20:58:39.000000 cs-nds-0.2.0/cs_nds/__init__.py
--rw-r--r--   0 alex      (1000) wheel      (998)      988 2023-03-19 20:58:30.000000 cs-nds-0.2.0/cs_nds/dynarray.py
--rw-r--r--   0 alex      (1000) wheel      (998)      346 2023-03-19 20:05:10.000000 cs-nds-0.2.0/cs_nds/queue.py
--rw-r--r--   0 alex      (1000) wheel      (998)      901 2023-03-19 20:05:44.000000 cs-nds-0.2.0/cs_nds/stack.py
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-03-19 20:59:21.492670 cs-nds-0.2.0/cs_nds.egg-info/
--rw-r--r--   0 alex      (1000) wheel      (998)     1342 2023-03-19 20:59:21.000000 cs-nds-0.2.0/cs_nds.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) wheel      (998)      216 2023-03-19 20:59:21.000000 cs-nds-0.2.0/cs_nds.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) wheel      (998)        1 2023-03-19 20:59:21.000000 cs-nds-0.2.0/cs_nds.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) wheel      (998)        7 2023-03-19 20:59:21.000000 cs-nds-0.2.0/cs_nds.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) wheel      (998)       38 2023-03-19 20:59:21.492670 cs-nds-0.2.0/setup.cfg
--rw-r--r--   0 alex      (1000) wheel      (998)      984 2023-03-19 20:59:19.000000 cs-nds-0.2.0/setup.py
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.455708 cs-nds-0.3.0/
+-rw-r--r--   0 alex      (1000) wheel      (998)    35149 2023-03-19 20:03:06.000000 cs-nds-0.3.0/LICENSE
+-rw-r--r--   0 alex      (1000) wheel      (998)     1623 2023-04-18 09:26:34.452375 cs-nds-0.3.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) wheel      (998)      935 2023-04-18 09:21:32.000000 cs-nds-0.3.0/README.md
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.452375 cs-nds-0.3.0/cs_nds/
+-rw-r--r--   0 alex      (1000) wheel      (998)      112 2023-04-18 08:56:46.000000 cs-nds-0.3.0/cs_nds/__init__.py
+-rw-r--r--   0 alex      (1000) wheel      (998)     1018 2023-04-18 09:04:08.000000 cs-nds-0.3.0/cs_nds/bintree.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      995 2023-04-18 09:13:54.000000 cs-nds-0.3.0/cs_nds/dynarray.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      346 2023-03-19 20:05:10.000000 cs-nds-0.3.0/cs_nds/queue.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      902 2023-04-18 09:16:48.000000 cs-nds-0.3.0/cs_nds/stack.py
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.452375 cs-nds-0.3.0/cs_nds.egg-info/
+-rw-r--r--   0 alex      (1000) wheel      (998)     1623 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) wheel      (998)      234 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)        1 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)        7 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)       38 2023-04-18 09:26:34.455708 cs-nds-0.3.0/setup.cfg
+-rw-r--r--   0 alex      (1000) wheel      (998)     1034 2023-04-18 09:18:49.000000 cs-nds-0.3.0/setup.py
```

### Comparing `cs-nds-0.2.0/LICENSE` & `cs-nds-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs-nds-0.2.0/PKG-INFO` & `cs-nds-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cs-nds
-Version: 0.2.0
+Version: 0.3.0
 Summary: Often used things for Computer Science classes
 Home-page: https://github.com/alexcoder04/cs_nds
 Author: alexcoder04
 Author-email: alexcoder04@protonmail.com
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Computer Science Niedersachsen
 
@@ -28,13 +29,28 @@
 **Disclaimer:**
 Although I try to give my best to provide a useful tool,
 I cannot guarantee it always working correctly and being
 up-to-date with the latest specifications.
 
 If you encounter a problem, please open an [issue](https://github.com/alexcoder04/cs_nds/issues).
 
+## Installation
+
+This package is available over `pip`:
+
+```sh
+pip install cs-nds
+```
+
+To use it in your code, just import it:
+
+```python
+import cs_nds
+```
+
 ## Data Structures
 
- - `Stack` ("Stapel")
- - `Queue` ("(Warte-)Schlange")
- - `DynArray` ("Dynamische Reihung")
+ - `Stack` ("Stapel" / stack)
+ - `Queue` ("(Warte-)Schlange" / queue)
+ - `DynArray` ("Dynamische Reihung" / dynamic array)
+ - `BinTree` ("Binärbaum" / binary tree)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cs-nds-0.2.0/cs_nds/dynarray.py` & `cs-nds-0.3.0/cs_nds/dynarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     pass
 
 class DynArray:
     def __init__(self):
         self.__data = []
 
     def append(self, element: any) -> None:
-        self.__data.append()
+        self.__data.append(element)
 
     def delete(self, index: int) -> None:
         del self.__data[index]
 
     def insertAT(self, index: int, element: any) -> None:
         self.__data.insert(index, element)
```

### Comparing `cs-nds-0.2.0/cs_nds/stack.py` & `cs-nds-0.3.0/cs_nds/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,7 +37,8 @@
 
     @classmethod
     def from_elements(cls, *args: any) -> Stack:
         s = cls()
         for el in args:
             s.push(el)
         return s
+
```

### Comparing `cs-nds-0.2.0/cs_nds.egg-info/PKG-INFO` & `cs-nds-0.3.0/cs_nds.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cs-nds
-Version: 0.2.0
+Version: 0.3.0
 Summary: Often used things for Computer Science classes
 Home-page: https://github.com/alexcoder04/cs_nds
 Author: alexcoder04
 Author-email: alexcoder04@protonmail.com
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Computer Science Niedersachsen
 
@@ -28,13 +29,28 @@
 **Disclaimer:**
 Although I try to give my best to provide a useful tool,
 I cannot guarantee it always working correctly and being
 up-to-date with the latest specifications.
 
 If you encounter a problem, please open an [issue](https://github.com/alexcoder04/cs_nds/issues).
 
+## Installation
+
+This package is available over `pip`:
+
+```sh
+pip install cs-nds
+```
+
+To use it in your code, just import it:
+
+```python
+import cs_nds
+```
+
 ## Data Structures
 
- - `Stack` ("Stapel")
- - `Queue` ("(Warte-)Schlange")
- - `DynArray` ("Dynamische Reihung")
+ - `Stack` ("Stapel" / stack)
+ - `Queue` ("(Warte-)Schlange" / queue)
+ - `DynArray` ("Dynamische Reihung" / dynamic array)
+ - `BinTree` ("Binärbaum" / binary tree)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cs-nds-0.2.0/setup.py` & `cs-nds-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 from setuptools import setup, find_packages
 
 from codecs import open
 from os import path
 
 HERE = path.abspath(path.dirname(__file__))
 
-with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
+with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="cs-nds",
-    version="0.2.0",
+    version="0.3.0",
     description="Often used things for Computer Science classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexcoder04/cs_nds",
     author="alexcoder04",
     author_email="alexcoder04@protonmail.com",
     classifiers=[
         "Intended Audience :: Education",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     packages=["cs_nds"],
     install_requires=[]
 )
```

