# Comparing `tmp/genomenotebook-0.3.0.tar.gz` & `tmp/genomenotebook-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomenotebook-0.3.0.tar", last modified: Mon Apr 17 22:23:04 2023, max compression
+gzip compressed data, was "genomenotebook-0.3.1.tar", last modified: Tue Apr 18 09:48:22 2023, max compression
```

## Comparing `genomenotebook-0.3.0.tar` & `genomenotebook-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.0/LICENSE
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.3.0/MANIFEST.in
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1271 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.0/README.md
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/genomenotebook/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       22 2023-04-17 22:21:40.000000 genomenotebook-0.3.0/genomenotebook/__init__.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4566 2023-04-17 22:21:40.000000 genomenotebook-0.3.0/genomenotebook/_modidx.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-17 22:21:39.000000 genomenotebook-0.3.0/genomenotebook/browser.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 22:03:01.000000 genomenotebook-0.3.0/genomenotebook/examples.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.0/genomenotebook/js_callback_code.py
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-17 22:21:39.000000 genomenotebook-0.3.0/genomenotebook/plotting.py
-drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/genomenotebook.egg-info/
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1271 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/PKG-INFO
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/SOURCES.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/dependency_links.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/entry_points.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.0/genomenotebook.egg-info/not-zip-safe
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       88 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/requires.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-17 22:23:04.000000 genomenotebook-0.3.0/genomenotebook.egg-info/top_level.txt
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1027 2023-04-17 22:15:38.000000 genomenotebook-0.3.0/settings.ini
--rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-17 22:23:04.857743 genomenotebook-0.3.0/setup.cfg
--rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.0/setup.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)    11357 2023-04-17 08:46:32.000000 genomenotebook-0.3.1/LICENSE
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)      111 2023-01-20 02:50:04.000000 genomenotebook-0.3.1/MANIFEST.in
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      588 2023-04-17 22:21:51.000000 genomenotebook-0.3.1/README.md
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/genomenotebook/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       22 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/__init__.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     4566 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/_modidx.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     9751 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/browser.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      294 2023-04-17 22:03:01.000000 genomenotebook-0.3.1/genomenotebook/examples.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      642 2023-04-14 08:24:05.000000 genomenotebook-0.3.1/genomenotebook/js_callback_code.py
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     7515 2023-04-18 09:47:43.000000 genomenotebook-0.3.1/genomenotebook/plotting.py
+drwxr-xr-x   0 dbikard   (1000) dbikard   (1000)        0 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/genomenotebook.egg-info/
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1371 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/PKG-INFO
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)      486 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/SOURCES.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/dependency_links.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       50 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/entry_points.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)        1 2023-04-17 09:24:03.000000 genomenotebook-0.3.1/genomenotebook.egg-info/not-zip-safe
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       88 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/requires.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       15 2023-04-18 09:48:22.000000 genomenotebook-0.3.1/genomenotebook.egg-info/top_level.txt
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)     1027 2023-04-18 09:46:20.000000 genomenotebook-0.3.1/settings.ini
+-rw-r--r--   0 dbikard   (1000) dbikard   (1000)       38 2023-04-18 09:48:22.461386 genomenotebook-0.3.1/setup.cfg
+-rw-rw-r--   0 dbikard   (1000) dbikard   (1000)     2560 2023-01-20 02:50:04.000000 genomenotebook-0.3.1/setup.py
```

### Comparing `genomenotebook-0.3.0/LICENSE` & `genomenotebook-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.0/PKG-INFO` & `genomenotebook-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.0
+Version: 0.3.1
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 genomeNotebook
 ================
```

### Comparing `genomenotebook-0.3.0/README.md` & `genomenotebook-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.0/genomenotebook/_modidx.py` & `genomenotebook-0.3.1/genomenotebook/_modidx.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.0/genomenotebook/browser.py` & `genomenotebook-0.3.1/genomenotebook/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,29 +217,29 @@
     t.fig.x_range = self.x_range
     t.fig.frame_width = self.frame_width
     t.bounds = self.bounds
     self.tracks.append(t)
     return t
     
 
-# %% ../nbs/00_browser.ipynb 13
+# %% ../nbs/00_browser.ipynb 12
 @patch
 def line(self:Track,
          source: pd.DataFrame, #pandas DataFrame containing the data
          pos: str, #name of the column containing the positions along the genome
          y: str, #name of the column containing the data to be plotted on the y-axis
         ):
     source=source.loc[(self.bounds[0] < source[pos]) & (source[pos] < self.bounds[1])]
     self.fig.line(source=source, x=pos, y=y)
 
 
-# %% ../nbs/00_browser.ipynb 17
+# %% ../nbs/00_browser.ipynb 16
 from bokeh.transform import linear_cmap, factor_cmap
 
-# %% ../nbs/00_browser.ipynb 18
+# %% ../nbs/00_browser.ipynb 17
 @patch
 def scatter(self:Track,
          source: pd.DataFrame, #pandas DataFrame containing the data
          pos: str, #name of the column containing the positions along the genome
          y: str, #name of the column containing the data to be plotted on the y-axis
          z: str = None, #name of a column containing numerical data rendered as a linear color map (cannot be used for line plots)
          factors: str = None, #name of a column of values to be used as factors
@@ -255,15 +255,15 @@
         self.fig.legend.title = "ori"
     elif z!=None:
         pass
     else:
         self.fig.scatter(source=source, x=pos, y=y)
 
 
-# %% ../nbs/00_browser.ipynb 21
+# %% ../nbs/00_browser.ipynb 20
 @patch
 def bar(self:Track,
          source: pd.DataFrame, #pandas DataFrame containing the data
          pos: str, #name of the column containing the positions along the genome
          y: str, #name of the column containing the data to be plotted on the y-axis
          z: str = None, #name of a column containing numerical data rendered as a linear color map (cannot be used for line plots)
          factors: str = None, #name of a column of values to be used as factors
```

### Comparing `genomenotebook-0.3.0/genomenotebook/js_callback_code.py` & `genomenotebook-0.3.1/genomenotebook/js_callback_code.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.0/genomenotebook/plotting.py` & `genomenotebook-0.3.1/genomenotebook/plotting.py`

 * *Files identical despite different names*

### Comparing `genomenotebook-0.3.0/genomenotebook.egg-info/PKG-INFO` & `genomenotebook-0.3.1/genomenotebook.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: genomenotebook
-Version: 0.3.0
+Version: 0.3.1
 Summary: A genome browser in your Jupyter notebook
 Home-page: https://github.com/dbikard/genomenotebook
 Author: David
 Author-email: dbikard@pasteur.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 genomeNotebook
 ================
```

### Comparing `genomenotebook-0.3.0/settings.ini` & `genomenotebook-0.3.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = genomenotebook
 lib_name = %(repo)s
-version = 0.3.0
-min_python = 3.9
+version = 0.3.1
+min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = genomenotebook
 nbs_path = nbs
```

### Comparing `genomenotebook-0.3.0/setup.py` & `genomenotebook-0.3.1/setup.py`

 * *Files identical despite different names*

