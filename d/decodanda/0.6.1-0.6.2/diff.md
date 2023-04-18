# Comparing `tmp/decodanda-0.6.1.tar.gz` & `tmp/decodanda-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.1.tar", last modified: Tue Apr 18 20:41:05 2023, max compression
+gzip compressed data, was "decodanda-0.6.2.tar", last modified: Tue Apr 18 20:46:56 2023, max compression
```

## Comparing `decodanda-0.6.1.tar` & `decodanda-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.642897 decodanda-0.6.1/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.1/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:41:05.642450 decodanda-0.6.1/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.1/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.638515 decodanda-0.6.1/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.1/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.1/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.1/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.1/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.1/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    22076 2023-04-18 20:39:00.000000 decodanda-0.6.1/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.641756 decodanda-0.6.1/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:41:05.643039 decodanda-0.6.1/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:40:47.000000 decodanda-0.6.1/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.473711 decodanda-0.6.2/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.2/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:46:56.473237 decodanda-0.6.2/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.2/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.468985 decodanda-0.6.2/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.2/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.2/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.2/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.2/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.2/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    22115 2023-04-18 20:45:44.000000 decodanda-0.6.2/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.472592 decodanda-0.6.2/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:46:56.473912 decodanda-0.6.2/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:46:06.000000 decodanda-0.6.2/setup.py
```

### Comparing `decodanda-0.6.1/LICENSE.md` & `decodanda-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/PKG-INFO` & `decodanda-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.1/README.md` & `decodanda-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/decodanda/classes.py` & `decodanda-0.6.2/decodanda/classes.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/decodanda/imports.py` & `decodanda-0.6.2/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/decodanda/in_time.py` & `decodanda-0.6.2/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/decodanda/utilities.py` & `decodanda-0.6.2/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.1/decodanda/visualize.py` & `decodanda-0.6.2/decodanda/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,21 +459,23 @@
         anim.save(savename, writer=mywriter)
     else:
         init()
     mpl.rcParams.update({'figure.autolayout': True})
     return fig
 
 
-def visualize_balanced_MDS(dec, dim=3, savename=None, title='', data=None, null=None, names=None, axs=None):
+def visualize_balanced_MDS(dec, dim=3, ndata=None, savename=None, title='', data=None, null=None, names=None, axs=None):
     # performance and CCGP
 
     mpl.rcParams.update({'figure.autolayout': False})
     rasters = []
     labels = []
-    ndata =  dec._max_conditioned_data
+    if ndata is None:
+        ndata =  dec._max_conditioned_data
+
     for key in dec.conditioned_rasters:
         X = sample_from_rasters(dec.conditioned_rasters[key], ndata)
         rasters.append(X)
         y = np.repeat(key, ndata)
         labels.append(y)
     X = np.vstack(rasters)
     y = np.hstack(labels)
```

### Comparing `decodanda-0.6.1/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.2/decodanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.1/setup.py` & `decodanda-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

