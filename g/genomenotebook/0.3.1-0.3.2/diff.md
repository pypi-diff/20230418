# Comparing `tmp/genomenotebook-0.3.1.tar.gz` & `tmp/genomenotebook-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomenotebook-0.3.1.tar", last modified: Tue Apr 18 09:48:22 2023, max compression
+gzip compressed data, was "genomenotebook-0.3.2.tar", last modified: Tue Apr 18 10:33:37 2023, max compression
```

## Comparing `genomenotebook-0.3.1.tar` & `genomenotebook-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.1/LICENSE
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.3.1/MANIFEST.in
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.1/README.md
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/genomenotebook/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       22 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/__init__.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4566 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/_modidx.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/browser.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 22:03:01.000000 genomenotebook-0.3.1/genomenotebook/examples.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.1/genomenotebook/js_callback_code.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/plotting.py
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/genomenotebook.egg-info/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/SOURCES.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/dependency_links.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/entry_points.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.1/genomenotebook.egg-info/not-zip-safe
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       88 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/requires.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/top_level.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1027 2023-04-18 09:46:20.000000 genomenotebook-0.3.1/settings.ini
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/setup.cfg
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.1/setup.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:33:37.561427 genomenotebook-0.3.2/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.2/LICENSE
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.3.2/MANIFEST.in
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 10:33:37.561427 genomenotebook-0.3.2/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.2/README.md
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:33:37.561427 genomenotebook-0.3.2/genomenotebook/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       58 2023-04-18 10:33:15.000000 genomenotebook-0.3.2/genomenotebook/__init__.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4566 2023-04-18 10:33:15.000000 genomenotebook-0.3.2/genomenotebook/_modidx.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-18 10:33:15.000000 genomenotebook-0.3.2/genomenotebook/browser.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 22:03:01.000000 genomenotebook-0.3.2/genomenotebook/examples.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.2/genomenotebook/js_callback_code.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-18 10:33:15.000000 genomenotebook-0.3.2/genomenotebook/plotting.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 10:33:37.561427 genomenotebook-0.3.2/genomenotebook.egg-info/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/SOURCES.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/dependency_links.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/entry_points.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.2/genomenotebook.egg-info/not-zip-safe
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       96 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/requires.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-18 10:33:37.000000 genomenotebook-0.3.2/genomenotebook.egg-info/top_level.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1035 2023-04-18 10:33:08.000000 genomenotebook-0.3.2/settings.ini
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-18 10:33:37.561427 genomenotebook-0.3.2/setup.cfg
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.2/setup.py
```

### Comparing `genomenotebook-0.3.1/LICENSE` & `genomenotebook-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/PKG-INFO` & `genomenotebook-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.1
+Version: 0.3.2
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `genomenotebook-0.3.1/README.md` & `genomenotebook-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/genomenotebook/_modidx.py` & `genomenotebook-0.3.2/genomenotebook/_modidx.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/genomenotebook/browser.py` & `genomenotebook-0.3.2/genomenotebook/browser.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/genomenotebook/js_callback_code.py` & `genomenotebook-0.3.2/genomenotebook/js_callback_code.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/genomenotebook/plotting.py` & `genomenotebook-0.3.2/genomenotebook/plotting.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.1/genomenotebook.egg-info/PKG-INFO` & `genomenotebook-0.3.2/genomenotebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.1
+Version: 0.3.2
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `genomenotebook-0.3.1/settings.ini` & `genomenotebook-0.3.2/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = genomenotebook
 lib_name = %(repo)s
-version = 0.3.1
+version = 0.3.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = genomenotebook
@@ -34,10 +34,10 @@
 description = A genome browser in your Jupyter notebook
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = dbikard
 
 ### Optional ###
-requirements = numpy>=1.23.5 biopython>=1.78 pandas>=1.5.3 bokeh>=3.1.0 gffpandas>=1.2 pyBigWig
+requirements = numpy>=1.23.5 biopython>=1.78 pandas>=1.5.3 bokeh>=3.1.0 gffpandas>=1.2 pyBigWig jupyter
 # dev_requirements = 
 # console_scripts =
```

### Comparing `genomenotebook-0.3.1/setup.py` & `genomenotebook-0.3.2/setup.py`

 * *Files identical despite different names*

