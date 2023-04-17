# Comparing `tmp/pollev-history-compiler-1.0.0.tar.gz` & `tmp/pollev-history-compiler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollev-history-compiler-1.0.0.tar", last modified: Mon Apr 17 23:33:44 2023, max compression
+gzip compressed data, was "pollev-history-compiler-1.0.1.tar", last modified: Mon Apr 17 23:39:09 2023, max compression
```

## Comparing `pollev-history-compiler-1.0.0.tar` & `pollev-history-compiler-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 23:33:44.390927 pollev-history-compiler-1.0.0/
--rw-rw-rw-   0        0        0     1911 2023-04-17 23:33:44.389918 pollev-history-compiler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2023-04-17 23:33:27.000000 pollev-history-compiler-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 23:33:44.386403 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/
--rw-rw-rw-   0        0        0     1911 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 23:33:44.000000 pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 23:33:44.387911 pollev-history-compiler-1.0.0/pollev_tools/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:46:25.000000 pollev-history-compiler-1.0.0/pollev_tools/__init__.py
--rw-rw-rw-   0        0        0    26266 2023-04-17 23:22:21.000000 pollev-history-compiler-1.0.0/pollev_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-04-17 23:33:44.388923 pollev-history-compiler-1.0.0/resources/
--rw-rw-rw-   0        0        0      567 2023-04-16 17:02:01.000000 pollev-history-compiler-1.0.0/resources/config.ini
--rw-rw-rw-   0        0        0      424 2023-04-17 23:31:29.000000 pollev-history-compiler-1.0.0/resources/html-styles.css
--rw-rw-rw-   0        0        0       42 2023-04-17 23:33:44.390927 pollev-history-compiler-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1251 2023-04-17 23:23:14.000000 pollev-history-compiler-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.756001 pollev-history-compiler-1.0.1/
+-rw-rw-rw-   0        0        0     1898 2023-04-17 23:39:09.755000 pollev-history-compiler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2023-04-17 23:35:47.000000 pollev-history-compiler-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.751003 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/
+-rw-rw-rw-   0        0        0     1898 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.753003 pollev-history-compiler-1.0.1/pollev_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:46:25.000000 pollev-history-compiler-1.0.1/pollev_tools/__init__.py
+-rw-rw-rw-   0        0        0    26266 2023-04-17 23:22:21.000000 pollev-history-compiler-1.0.1/pollev_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.754001 pollev-history-compiler-1.0.1/resources/
+-rw-rw-rw-   0        0        0      567 2023-04-16 17:02:01.000000 pollev-history-compiler-1.0.1/resources/config.ini
+-rw-rw-rw-   0        0        0      424 2023-04-17 23:31:29.000000 pollev-history-compiler-1.0.1/resources/html-styles.css
+-rw-rw-rw-   0        0        0       42 2023-04-17 23:39:09.756001 pollev-history-compiler-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2023-04-17 23:37:10.000000 pollev-history-compiler-1.0.1/setup.py
```

### Comparing `pollev-history-compiler-1.0.0/PKG-INFO` & `pollev-history-compiler-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -18,24 +18,20 @@
 Have you ever wanted to compile your Poll Everywhere history into a more usable form?
 This project allows you to use a script to load it into almost any form you want!
 You can filter by presenter, and use different types of encodings so that you can load polls with almost any data in them.
 Right now most of the support is for `Multiple choice` type polls.
 
 ## Installation
 There are two approaches to the installation of this package/script.
-1) 
-
 Clone the repository, and within the root folder run:
 
 ```
 pip install .
 ```
 
-2)
-
 Install the package from PyPI:
 
 ```
 pip install pollev-history-compiler
 ```
 
 ## Usage
```

### Comparing `pollev-history-compiler-1.0.0/README.md` & `pollev-history-compiler-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 Have you ever wanted to compile your Poll Everywhere history into a more usable form?
 This project allows you to use a script to load it into almost any form you want!
 You can filter by presenter, and use different types of encodings so that you can load polls with almost any data in them.
 Right now most of the support is for `Multiple choice` type polls.
 
 ## Installation
 There are two approaches to the installation of this package/script.
-1) 
-
 Clone the repository, and within the root folder run:
 
 ```
 pip install .
 ```
 
-2)
-
 Install the package from PyPI:
 
 ```
 pip install pollev-history-compiler
 ```
 
 ## Usage
```

### Comparing `pollev-history-compiler-1.0.0/pollev_history_compiler.egg-info/PKG-INFO` & `pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -18,24 +18,20 @@
 Have you ever wanted to compile your Poll Everywhere history into a more usable form?
 This project allows you to use a script to load it into almost any form you want!
 You can filter by presenter, and use different types of encodings so that you can load polls with almost any data in them.
 Right now most of the support is for `Multiple choice` type polls.
 
 ## Installation
 There are two approaches to the installation of this package/script.
-1) 
-
 Clone the repository, and within the root folder run:
 
 ```
 pip install .
 ```
 
-2)
-
 Install the package from PyPI:
 
 ```
 pip install pollev-history-compiler
 ```
 
 ## Usage
```

### Comparing `pollev-history-compiler-1.0.0/pollev_tools/reader.py` & `pollev-history-compiler-1.0.1/pollev_tools/reader.py`

 * *Files identical despite different names*

### Comparing `pollev-history-compiler-1.0.0/resources/config.ini` & `pollev-history-compiler-1.0.1/resources/config.ini`

 * *Files identical despite different names*

### Comparing `pollev-history-compiler-1.0.0/setup.py` & `pollev-history-compiler-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pollev-history-compiler",
-    version="1.0.0",
+    version="1.0.1",
     author="Tony Abou Zeidan",
     author_email="tony.azp25@gmail.com",
     description="A script for the compilation of PollEverywhere history CSV files into more usable forms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tony-zeidan/PollEvHistoryCompiler",
     packages=find_packages(),
```

