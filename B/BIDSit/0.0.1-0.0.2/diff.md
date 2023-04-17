# Comparing `tmp/BIDSit-0.0.1.tar.gz` & `tmp/BIDSit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.1.tar", last modified: Mon Apr 17 23:04:24 2023, max compression
+gzip compressed data, was "BIDSit-0.0.2.tar", last modified: Mon Apr 17 23:29:04 2023, max compression
```

## Comparing `BIDSit-0.0.1.tar` & `BIDSit-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:04:24.064368 BIDSit-0.0.1/
--rw-r--r--   0 labmanager   (501) staff       (20)     1112 2023-04-17 23:04:24.063975 BIDSit-0.0.1/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      661 2023-04-17 22:35:50.000000 BIDSit-0.0.1/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-17 23:04:24.064506 BIDSit-0.0.1/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2363 2023-04-17 23:03:47.000000 BIDSit-0.0.1/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:04:24.058977 BIDSit-0.0.1/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:04:24.061374 BIDSit-0.0.1/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)    49384 2023-04-17 22:19:22.000000 BIDSit-0.0.1/src/BIDSit/BIDSit.py
--rw-r--r--   0 labmanager   (501) staff       (20)    21664 2023-04-17 22:02:10.000000 BIDSit-0.0.1/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.1/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-17 22:34:10.000000 BIDSit-0.0.1/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:04:24.063478 BIDSit-0.0.1/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1112 2023-04-17 23:04:23.000000 BIDSit-0.0.1/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      280 2023-04-17 23:04:23.000000 BIDSit-0.0.1/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-17 23:04:23.000000 BIDSit-0.0.1/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       39 2023-04-17 23:04:23.000000 BIDSit-0.0.1/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-17 23:04:23.000000 BIDSit-0.0.1/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.957500 BIDSit-0.0.2/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1115 2023-04-17 23:29:04.957118 BIDSit-0.0.2/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      664 2023-04-17 23:17:11.000000 BIDSit-0.0.2/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-17 23:29:04.957625 BIDSit-0.0.2/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2421 2023-04-17 23:21:54.000000 BIDSit-0.0.2/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.951182 BIDSit-0.0.2/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.954551 BIDSit-0.0.2/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)    49238 2023-04-17 23:14:31.000000 BIDSit-0.0.2/src/BIDSit/BIDSit.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    21664 2023-04-17 22:02:10.000000 BIDSit-0.0.2/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.2/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-17 23:27:35.000000 BIDSit-0.0.2/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-17 23:29:04.956516 BIDSit-0.0.2/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1115 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      280 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       39 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-17 23:29:04.000000 BIDSit-0.0.2/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.1/PKG-INFO` & `BIDSit-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -19,15 +19,15 @@
 
 Installation
 ------------
 Install ``BIDSit`` and its core dependencies via pip::
 
     pip install BIDSit
 
-Install ``BIDSit`` by cloning GitHub, then move to where the toolbox is
+Or install ``BIDSit`` by cloning GitHub, then move to where the toolbox is
 housed in terminal ::
 
 	cd path/to/BIDSit
 
 Then run ``setup.py`` to install dependencies ::
 
 	Python3 setup.py install
```

### Comparing `BIDSit-0.0.1/README.rst` & `BIDSit-0.0.2/src/BIDSit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+Metadata-Version: 2.1
+Name: BIDSit
+Version: 0.0.2
+Summary: A BIDS conversion tool for fMRI data
+Home-page: https://github.com/jenburrell/BIDSit
+Author: Jen Burrell
+Author-email: jenbur@psych.ubc.ca
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+
 BIDSit
 ===========
 
 The ``BIDSit`` project is a toolbox to organize MRI data into BIDS format written in Python.
 
 Installation
 ------------
 Install ``BIDSit`` and its core dependencies via pip::
 
     pip install BIDSit
 
-Install ``BIDSit`` by cloning GitHub, then move to where the toolbox is
+Or install ``BIDSit`` by cloning GitHub, then move to where the toolbox is
 housed in terminal ::
 
 	cd path/to/BIDSit
 
 Then run ``setup.py`` to install dependencies ::
 
 	Python3 setup.py install
```

### Comparing `BIDSit-0.0.1/setup.py` & `BIDSit-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,9 +68,12 @@
 # git add MANIFEST.in
 
 # python setup.py sdist # to do source distribution
 # tar tzf dist/BIDSit-0.0.1.tar.gz # should show lots of files see pic
 
 ### --- TO PUBLISH --- ###
 # python3 setup.py bdist_wheel sdist
-# python3 install twine
-# python3 upload dist/*
+# pip install twine
+# twine upload dist/*
+
+### --- TO UPDATE --- ###
+#twine upload --skip-existing dist/*
```

### Comparing `BIDSit-0.0.1/src/BIDSit/BIDSit.py` & `BIDSit-0.0.2/src/BIDSit/BIDSit.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import glob
 import shutil
 import json
 import errno
 
 
 def main():
-    modulenames = set(sys.modules) & set(globals())
-    allmodules = [sys.modules[name] for name in modulenames]
-    print(allmodules)
-    exit()
     # - get user input - #
     user_info = start_gui()
 #    print(user_info)
     
     # - define variables in use - #
     in_dir = user_info['in_dir'] # in_dir is where the input files are
     out_dir = user_info['out_dir'] # out_dir is where the output files will go
```

### Comparing `BIDSit-0.0.1/src/BIDSit/Test_script.py` & `BIDSit-0.0.2/src/BIDSit/Test_script.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.1/src/BIDSit/version.py` & `BIDSit-0.0.2/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
```

