# Comparing `tmp/genomenotebook-0.3.3.tar.gz` & `tmp/genomenotebook-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomenotebook-0.3.3.tar", last modified: Tue Apr 18 10:44:05 2023, max compression
+gzip compressed data, was "genomenotebook-0.3.4.tar", last modified: Tue Apr 18 11:01:21 2023, max compression
```

## Comparing `genomenotebook-0.3.3.tar` & `genomenotebook-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:44:05.491436 genomenotebook-0.3.3/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.3/LICENSE
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      139 2023-04-18 10:42:53.000000 genomenotebook-0.3.3/MANIFEST.in
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 10:44:05.491436 genomenotebook-0.3.3/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.3/README.md
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:44:05.491436 genomenotebook-0.3.3/genomenotebook/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       58 2023-04-18 10:43:38.000000 genomenotebook-0.3.3/genomenotebook/__init__.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4523 2023-04-18 10:43:38.000000 genomenotebook-0.3.3/genomenotebook/_modidx.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-18 10:43:38.000000 genomenotebook-0.3.3/genomenotebook/browser.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.3/genomenotebook/js_callback_code.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-18 10:43:38.000000 genomenotebook-0.3.3/genomenotebook/plotting.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     2253 2023-04-14 09:18:20.000000 genomenotebook-0.3.3/genomenotebook/search_callback_code.js
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1333 2023-04-14 08:23:37.000000 genomenotebook-0.3.3/genomenotebook/x_range_change_callback_code.js
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:44:05.491436 genomenotebook-0.3.3/genomenotebook.egg-info/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      545 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/SOURCES.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/dependency_links.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/entry_points.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.3/genomenotebook.egg-info/not-zip-safe
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      105 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/requires.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-18 10:44:05.000000 genomenotebook-0.3.3/genomenotebook.egg-info/top_level.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1044 2023-04-18 10:37:16.000000 genomenotebook-0.3.3/settings.ini
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-18 10:44:05.491436 genomenotebook-0.3.3/setup.cfg
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.3/setup.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 11:01:21.521452 genomenotebook-0.3.4/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.4/LICENSE
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      139 2023-04-18 10:42:53.000000 genomenotebook-0.3.4/MANIFEST.in
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 11:01:21.521452 genomenotebook-0.3.4/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.4/README.md
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 11:01:21.511452 genomenotebook-0.3.4/genomenotebook/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       58 2023-04-18 11:00:58.000000 genomenotebook-0.3.4/genomenotebook/__init__.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4523 2023-04-18 11:00:58.000000 genomenotebook-0.3.4/genomenotebook/_modidx.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-18 11:00:58.000000 genomenotebook-0.3.4/genomenotebook/browser.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 11:01:21.521452 genomenotebook-0.3.4/genomenotebook/javascript/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     2253 2023-04-14 09:18:20.000000 genomenotebook-0.3.4/genomenotebook/javascript/search_callback_code.js
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1333 2023-04-14 08:23:37.000000 genomenotebook-0.3.4/genomenotebook/javascript/x_range_change_callback_code.js
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      664 2023-04-18 10:55:30.000000 genomenotebook-0.3.4/genomenotebook/js_callback_code.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-18 11:00:58.000000 genomenotebook-0.3.4/genomenotebook/plotting.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 11:01:21.521452 genomenotebook-0.3.4/genomenotebook.egg-info/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      567 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/SOURCES.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/dependency_links.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/entry_points.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.4/genomenotebook.egg-info/not-zip-safe
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      105 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/requires.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-18 11:01:21.000000 genomenotebook-0.3.4/genomenotebook.egg-info/top_level.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1044 2023-04-18 11:00:40.000000 genomenotebook-0.3.4/settings.ini
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-18 11:01:21.521452 genomenotebook-0.3.4/setup.cfg
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2601 2023-04-18 10:57:17.000000 genomenotebook-0.3.4/setup.py
```

### Comparing `genomenotebook-0.3.3/LICENSE` & `genomenotebook-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/PKG-INFO` & `genomenotebook-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.3
+Version: 0.3.4
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `genomenotebook-0.3.3/README.md` & `genomenotebook-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook/_modidx.py` & `genomenotebook-0.3.4/genomenotebook/_modidx.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook/browser.py` & `genomenotebook-0.3.4/genomenotebook/browser.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook/js_callback_code.py` & `genomenotebook-0.3.4/genomenotebook/js_callback_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 # Get the path of the current Python module
 module_path = os.path.abspath(__file__)
 
 # Construct the path to the file you need to open
-file_path = os.path.join(os.path.dirname(module_path), "x_range_change_callback_code.js")
+file_path = os.path.join(os.path.dirname(module_path), "javascript/x_range_change_callback_code.js")
 
 # Open the file and read its contents
 with open(file_path, 'r') as handle:
     x_range_change_callback_code = ''.join(handle.readlines())
 
 # Construct the path to the file you need to open
-file_path = os.path.join(os.path.dirname(module_path), "search_callback_code.js")
+file_path = os.path.join(os.path.dirname(module_path), "javascript/search_callback_code.js")
 
 with open(file_path, 'r') as handle:
     search_callback_code =''.join(handle.readlines())
 
 def reload():
     pass
```

### Comparing `genomenotebook-0.3.3/genomenotebook/plotting.py` & `genomenotebook-0.3.4/genomenotebook/plotting.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook/search_callback_code.js` & `genomenotebook-0.3.4/genomenotebook/javascript/search_callback_code.js`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook/x_range_change_callback_code.js` & `genomenotebook-0.3.4/genomenotebook/javascript/x_range_change_callback_code.js`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.3/genomenotebook.egg-info/PKG-INFO` & `genomenotebook-0.3.4/genomenotebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.3
+Version: 0.3.4
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `genomenotebook-0.3.3/genomenotebook.egg-info/SOURCES.txt` & `genomenotebook-0.3.4/genomenotebook.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 settings.ini
 setup.py
 genomenotebook/__init__.py
 genomenotebook/_modidx.py
 genomenotebook/browser.py
 genomenotebook/js_callback_code.py
 genomenotebook/plotting.py
-genomenotebook/search_callback_code.js
-genomenotebook/x_range_change_callback_code.js
 genomenotebook.egg-info/PKG-INFO
 genomenotebook.egg-info/SOURCES.txt
 genomenotebook.egg-info/dependency_links.txt
 genomenotebook.egg-info/entry_points.txt
 genomenotebook.egg-info/not-zip-safe
 genomenotebook.egg-info/requires.txt
-genomenotebook.egg-info/top_level.txt
+genomenotebook.egg-info/top_level.txt
+genomenotebook/javascript/search_callback_code.js
+genomenotebook/javascript/x_range_change_callback_code.js
```

### Comparing `genomenotebook-0.3.3/settings.ini` & `genomenotebook-0.3.4/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = genomenotebook
 lib_name = %(repo)s
-version = 0.3.3
+version = 0.3.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = genomenotebook
```

### Comparing `genomenotebook-0.3.3/setup.py` & `genomenotebook-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
+    package_data={'': ['javascript/*']},
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
```

