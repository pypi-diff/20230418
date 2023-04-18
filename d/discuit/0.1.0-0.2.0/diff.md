# Comparing `tmp/discuit-0.1.0.tar.gz` & `tmp/discuit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discuit-0.1.0.tar", last modified: Mon Apr 17 17:59:43 2023, max compression
+gzip compressed data, was "discuit-0.2.0.tar", last modified: Tue Apr 18 07:29:07 2023, max compression
```

## Comparing `discuit-0.1.0.tar` & `discuit-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-17 17:59:43.307787 discuit-0.1.0/
--rw-r--r--   0 doerte     (501) staff       (20)      454 2023-02-25 18:49:41.000000 discuit-0.1.0/CITATION.cff
--rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.1.0/LICENSE
--rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.1.0/MANIFEST.in
--rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.1.0/NOTICE
--rw-r--r--   0 doerte     (501) staff       (20)     7802 2023-04-17 17:59:43.307908 discuit-0.1.0/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)     6720 2023-04-04 13:50:29.000000 discuit-0.1.0/README.md
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-17 17:59:43.306128 discuit-0.1.0/discuit/
--rw-r--r--   0 doerte     (501) staff       (20)      192 2023-02-24 12:59:01.000000 discuit-0.1.0/discuit/__init__.py
--rw-r--r--   0 doerte     (501) staff       (20)    16733 2023-04-17 14:46:16.000000 discuit-0.1.0/discuit/run_discuit.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-17 17:59:43.307377 discuit-0.1.0/discuit.egg-info/
--rw-r--r--   0 doerte     (501) staff       (20)     7802 2023-04-17 17:59:43.000000 discuit-0.1.0/discuit.egg-info/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)      334 2023-04-17 17:59:43.000000 discuit-0.1.0/discuit.egg-info/SOURCES.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-04-17 17:59:43.000000 discuit-0.1.0/discuit.egg-info/dependency_links.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.1.0/discuit.egg-info/not-zip-safe
--rw-r--r--   0 doerte     (501) staff       (20)      276 2023-04-17 17:59:43.000000 discuit-0.1.0/discuit.egg-info/requires.txt
--rw-r--r--   0 doerte     (501) staff       (20)        8 2023-04-17 17:59:43.000000 discuit-0.1.0/discuit.egg-info/top_level.txt
--rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.1.0/pyproject.toml
--rw-r--r--   0 doerte     (501) staff       (20)     1897 2023-04-17 17:59:43.308380 discuit-0.1.0/setup.cfg
--rw-r--r--   0 doerte     (501) staff       (20)       87 2023-02-15 15:09:44.000000 discuit-0.1.0/setup.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-17 17:59:43.307519 discuit-0.1.0/tests/
--rw-r--r--   0 doerte     (501) staff       (20)      343 2023-02-24 12:59:25.000000 discuit-0.1.0/tests/test_my_module.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604421 discuit-0.2.0/
+-rw-r--r--   0 doerte     (501) staff       (20)      454 2023-02-25 18:49:41.000000 discuit-0.2.0/CITATION.cff
+-rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.2.0/LICENSE
+-rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.2.0/MANIFEST.in
+-rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.2.0/NOTICE
+-rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:29:07.604507 discuit-0.2.0/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)     6801 2023-04-18 07:21:17.000000 discuit-0.2.0/README.md
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.602930 discuit-0.2.0/discuit/
+-rw-r--r--   0 doerte     (501) staff       (20)      192 2023-02-24 12:59:01.000000 discuit-0.2.0/discuit/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)    16746 2023-04-18 06:56:27.000000 discuit-0.2.0/discuit/run_discuit.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604066 discuit-0.2.0/discuit.egg-info/
+-rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)      334 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/SOURCES.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/dependency_links.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.2.0/discuit.egg-info/not-zip-safe
+-rw-r--r--   0 doerte     (501) staff       (20)      276 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/requires.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        8 2023-04-18 07:29:07.000000 discuit-0.2.0/discuit.egg-info/top_level.txt
+-rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.2.0/pyproject.toml
+-rw-r--r--   0 doerte     (501) staff       (20)     1897 2023-04-18 07:29:07.604899 discuit-0.2.0/setup.cfg
+-rw-r--r--   0 doerte     (501) staff       (20)       87 2023-02-15 15:09:44.000000 discuit-0.2.0/setup.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:29:07.604190 discuit-0.2.0/tests/
+-rw-r--r--   0 doerte     (501) staff       (20)      343 2023-02-24 12:59:25.000000 discuit-0.2.0/tests/test_my_module.py
```

### Comparing `discuit-0.1.0/LICENSE` & `discuit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discuit-0.1.0/PKG-INFO` & `discuit-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
@@ -58,15 +58,21 @@
 
 In the future, this will be integrated in an GUI. 
 
 The project setup is documented in [project_setup.md](project_setup.md).
 
 ## Installation
 
-To install discuit from GitHub repository, do:
+Discuit is available on PyPI!
+
+```bash
+pip install discuit
+```
+
+Or install the latest development version directly from GitHub:
 
 ```console
 git clone git@github.com:doerte/discuit-project.git
 cd discuit-project
 python3 -m pip install .
 ```
```

### Comparing `discuit-0.1.0/README.md` & `discuit-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,21 @@
 
 In the future, this will be integrated in an GUI. 
 
 The project setup is documented in [project_setup.md](project_setup.md).
 
 ## Installation
 
-To install discuit from GitHub repository, do:
+Discuit is available on PyPI!
+
+```bash
+pip install discuit
+```
+
+Or install the latest development version directly from GitHub:
 
 ```console
 git clone git@github.com:doerte/discuit-project.git
 cd discuit-project
 python3 -m pip install .
 ```
```

### Comparing `discuit-0.1.0/discuit/run_discuit.py` & `discuit-0.2.0/discuit/run_discuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TODO: maybe include more than 1 absolute variable? maybe all categorical variables can be absolute?
-# TODO: stop if silhouette score is too low. Exit with error message.
+# TODO: consider stopping if silhouette score is too low. Exit with error message.
 # pylint: disable-msg=too-many-locals
 
 import argparse
 import pathlib
 import sys
 from typing import List
 import pandas as pd
```

### Comparing `discuit-0.1.0/discuit.egg-info/PKG-INFO` & `discuit-0.2.0/discuit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
@@ -58,15 +58,21 @@
 
 In the future, this will be integrated in an GUI. 
 
 The project setup is documented in [project_setup.md](project_setup.md).
 
 ## Installation
 
-To install discuit from GitHub repository, do:
+Discuit is available on PyPI!
+
+```bash
+pip install discuit
+```
+
+Or install the latest development version directly from GitHub:
 
 ```console
 git clone git@github.com:doerte/discuit-project.git
 cd discuit-project
 python3 -m pip install .
 ```
```

### Comparing `discuit-0.1.0/setup.cfg` & `discuit-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = clustering
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = discuit
 project_urls = 
 	Bug Tracker = https://github.com/doerte/discuit-project/issues
 url = https://github.com/doerte/discuit-project
-version = 0.1.0
+version = 0.2.0
 
 [options]
 zip_safe = False
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires =
```

