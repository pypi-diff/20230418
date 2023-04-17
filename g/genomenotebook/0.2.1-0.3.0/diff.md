# Comparing `tmp/genomenotebook-0.2.1.tar.gz` & `tmp/genomenotebook-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomenotebook-0.2.1.tar", last modified: Mon Apr 17 18:57:59 2023, max compression
+gzip compressed data, was "genomenotebook-0.3.0.tar", last modified: Mon Apr 17 22:23:04 2023, max compression
```

## Comparing `genomenotebook-0.2.1.tar` & `genomenotebook-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 18:57:59.888870 genomenotebook-0.2.1/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.2.1/LICENSE
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.2.1/MANIFEST.in
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1219 2023-04-17 18:57:59.888870 genomenotebook-0.2.1/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      536 2023-04-17 15:11:04.000000 genomenotebook-0.2.1/README.md
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 18:57:59.888870 genomenotebook-0.2.1/genomenotebook/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       22 2023-04-17 14:38:45.000000 genomenotebook-0.2.1/genomenotebook/__init__.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     3722 2023-04-17 14:38:45.000000 genomenotebook-0.2.1/genomenotebook/_modidx.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7357 2023-04-17 14:38:45.000000 genomenotebook-0.2.1/genomenotebook/browser.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 14:38:45.000000 genomenotebook-0.2.1/genomenotebook/examples.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.2.1/genomenotebook/js_callback_code.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-17 14:38:45.000000 genomenotebook-0.2.1/genomenotebook/plotting.py
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 18:57:59.888870 genomenotebook-0.2.1/genomenotebook.egg-info/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1219 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/SOURCES.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/dependency_links.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/entry_points.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.2.1/genomenotebook.egg-info/not-zip-safe
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       88 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/requires.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-17 18:57:59.000000 genomenotebook-0.2.1/genomenotebook.egg-info/top_level.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1027 2023-04-17 14:28:03.000000 genomenotebook-0.2.1/settings.ini
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-17 18:57:59.888870 genomenotebook-0.2.1/setup.cfg
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.2.1/setup.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.0/LICENSE
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.3.0/MANIFEST.in
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1271 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.0/README.md
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/genomenotebook/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       22 2023-04-17 22:21:40.000000 genomenotebook-0.3.0/genomenotebook/__init__.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4566 2023-04-17 22:21:40.000000 genomenotebook-0.3.0/genomenotebook/_modidx.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-17 22:21:39.000000 genomenotebook-0.3.0/genomenotebook/browser.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 22:03:01.000000 genomenotebook-0.3.0/genomenotebook/examples.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.0/genomenotebook/js_callback_code.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-17 22:21:39.000000 genomenotebook-0.3.0/genomenotebook/plotting.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/genomenotebook.egg-info/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1271 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/SOURCES.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/dependency_links.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/entry_points.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.0/genomenotebook.egg-info/not-zip-safe
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       88 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/requires.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/top_level.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1027 2023-04-17 22:15:38.000000 genomenotebook-0.3.0/settings.ini
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/setup.cfg
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.0/setup.py
```

### Comparing `genomenotebook-0.2.1/LICENSE` & `genomenotebook-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.2.1/PKG-INFO` & `genomenotebook-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.2.1
+Version: 0.3.0
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -21,25 +21,23 @@
 genomeNotebook
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
-``` sh
-pip install genomenotebook
-```
+    pip install genomenotebook
 
 ## How to use
 
 Create a simple genome browser with a search bar. The sequence appears
 when zooming in.
 
 ``` python
 g=GenomeBrowser(genome_path="data/MG1655_U00096.fasta",
                 gff_path="data/MG1655_U00096.gff3")
 g.show()
 ```
 
-  <div id="32874c4b-99f2-4464-a479-020e07368d80" data-root-id="p49784" style="display: contents;"></div>
+  <div id="6b515b6f-a015-4aab-922d-c569e7f79b51" data-root-id="p1084" style="display: contents;"></div>
 
-    Output cannot be displayed in a static page
+    Unable to display output for mime type(s): application/javascript, application/vnd.bokehjs_exec.v0+json
```

### Comparing `genomenotebook-0.2.1/genomenotebook/_modidx.py` & `genomenotebook-0.3.0/genomenotebook/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,22 @@
                                         'genomenotebook.browser.GenomeBrowser.add_track': ( 'browser.html#genomebrowser.add_track',
                                                                                             'genomenotebook/browser.py'),
                                         'genomenotebook.browser.GenomeBrowser.get_browser': ( 'browser.html#genomebrowser.get_browser',
                                                                                               'genomenotebook/browser.py'),
                                         'genomenotebook.browser.GenomeBrowser.get_search_box': ( 'browser.html#genomebrowser.get_search_box',
                                                                                                  'genomenotebook/browser.py'),
                                         'genomenotebook.browser.GenomeBrowser.show': ( 'browser.html#genomebrowser.show',
-                                                                                       'genomenotebook/browser.py')},
+                                                                                       'genomenotebook/browser.py'),
+                                        'genomenotebook.browser.Track': ('browser.html#track', 'genomenotebook/browser.py'),
+                                        'genomenotebook.browser.Track.__init__': ( 'browser.html#track.__init__',
+                                                                                   'genomenotebook/browser.py'),
+                                        'genomenotebook.browser.Track.bar': ('browser.html#track.bar', 'genomenotebook/browser.py'),
+                                        'genomenotebook.browser.Track.line': ('browser.html#track.line', 'genomenotebook/browser.py'),
+                                        'genomenotebook.browser.Track.scatter': ( 'browser.html#track.scatter',
+                                                                                  'genomenotebook/browser.py')},
             'genomenotebook.examples': {},
             'genomenotebook.js_callback_code': {},
             'genomenotebook.plotting': { 'genomenotebook.plotting.arrow_patch': ('plotting.html#arrow_patch', 'genomenotebook/plotting.py'),
                                          'genomenotebook.plotting.create_genome_browser_plot': ( 'plotting.html#create_genome_browser_plot',
                                                                                                  'genomenotebook/plotting.py'),
                                          'genomenotebook.plotting.get_all_glyphs': ( 'plotting.html#get_all_glyphs',
                                                                                      'genomenotebook/plotting.py'),
```

### Comparing `genomenotebook-0.2.1/genomenotebook/js_callback_code.py` & `genomenotebook-0.3.0/genomenotebook/js_callback_code.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.2.1/genomenotebook/plotting.py` & `genomenotebook-0.3.0/genomenotebook/plotting.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.2.1/genomenotebook.egg-info/PKG-INFO` & `genomenotebook-0.3.0/genomenotebook.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.2.1
+Version: 0.3.0
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -21,25 +21,23 @@
 genomeNotebook
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
-``` sh
-pip install genomenotebook
-```
+    pip install genomenotebook
 
 ## How to use
 
 Create a simple genome browser with a search bar. The sequence appears
 when zooming in.
 
 ``` python
 g=GenomeBrowser(genome_path="data/MG1655_U00096.fasta",
                 gff_path="data/MG1655_U00096.gff3")
 g.show()
 ```
 
-  <div id="32874c4b-99f2-4464-a479-020e07368d80" data-root-id="p49784" style="display: contents;"></div>
+  <div id="6b515b6f-a015-4aab-922d-c569e7f79b51" data-root-id="p1084" style="display: contents;"></div>
 
-    Output cannot be displayed in a static page
+    Unable to display output for mime type(s): application/javascript, application/vnd.bokehjs_exec.v0+json
```

### Comparing `genomenotebook-0.2.1/settings.ini` & `genomenotebook-0.3.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = genomenotebook
 lib_name = %(repo)s
-version = 0.2.1
+version = 0.3.0
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = genomenotebook
```

### Comparing `genomenotebook-0.2.1/setup.py` & `genomenotebook-0.3.0/setup.py`

 * *Files identical despite different names*

