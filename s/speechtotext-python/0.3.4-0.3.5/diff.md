# Comparing `tmp/speechtotext-python-0.3.4.tar.gz` & `tmp/speechtotext-python-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.4.tar", last modified: Mon Apr 17 15:30:09 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.5.tar", last modified: Tue Apr 18 08:11:47 2023, max compression
```

## Comparing `speechtotext-python-0.3.4.tar` & `speechtotext-python-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4066 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3458 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6399 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3458 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6399 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/tests/test_imports.py
```

### Comparing `speechtotext-python-0.3.4/LICENSE` & `speechtotext-python-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.4/PKG-INFO` & `speechtotext-python-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.4/setup.py` & `speechtotext-python-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	'deepgram-sdk', 'azure-cognitiveservices-speech', 
 	'speechmatics-python==1.6.4', 'pydub'
 ]
 
 # What packages are optional?
 EXTRAS = {
 	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
-			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine']
+			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'pytest']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

### Comparing `speechtotext-python-0.3.4/speechtotext/datasets.py` & `speechtotext-python-0.3.5/speechtotext/datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.4/speechtotext/functions.py` & `speechtotext-python-0.3.5/speechtotext/functions.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.4/speechtotext_python.egg-info/PKG-INFO` & `speechtotext-python-0.3.5/speechtotext_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

