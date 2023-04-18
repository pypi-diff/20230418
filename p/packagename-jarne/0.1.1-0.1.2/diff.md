# Comparing `tmp/packagename_jarne-0.1.1.tar.gz` & `tmp/packagename_jarne-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagename_jarne-0.1.1.tar", last modified: Mon Apr 17 08:48:34 2023, max compression
+gzip compressed data, was "packagename_jarne-0.1.2.tar", last modified: Tue Apr 18 07:41:26 2023, max compression
```

## Comparing `packagename_jarne-0.1.1.tar` & `packagename_jarne-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-17 08:45:42.000000 packagename_jarne-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/packagename_jarne.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-17 08:45:42.000000 packagename_jarne-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/packagename_jarne.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/tests/test_PID.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/tests/test_imports.py
```

### Comparing `packagename_jarne-0.1.1/PKG-INFO` & `packagename_jarne-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: packagename_jarne
-Version: 0.1.1
+Version: 0.1.2
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENCE
 
 
 # Python-sphinx-documentation
 
 Template to document code with sphinx.
 install package ```pip install packagename_jarne```
```

### Comparing `packagename_jarne-0.1.1/README.md` & `packagename_jarne-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `packagename_jarne-0.1.1/packagename_jarne.egg-info/PKG-INFO` & `packagename_jarne-0.1.2/packagename_jarne.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: packagename-jarne
-Version: 0.1.1
+Version: 0.1.2
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENCE
 
 
 # Python-sphinx-documentation
 
 Template to document code with sphinx.
 install package ```pip install packagename_jarne```
```

### Comparing `packagename_jarne-0.1.1/setup.py` & `packagename_jarne-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 	'psutil'
 ]
 
 
 
 # What packages are optional?
 EXTRAS = {
-	'docs': [ 'Sphinx==6.1.3', 'sphinx-markdown-builder==0.5.5','sphinx-press-theme', 'twine']
+	'docs': [ 'Sphinx==6.1.3', 'sphinx-markdown-builder==0.5.5','sphinx-press-theme', 'twine',
+          'pytest']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

