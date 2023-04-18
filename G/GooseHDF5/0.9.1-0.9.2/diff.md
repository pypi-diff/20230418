# Comparing `tmp/GooseHDF5-0.9.1.tar.gz` & `tmp/GooseHDF5-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GooseHDF5-0.9.1.tar", last modified: Wed Oct 21 13:07:22 2020, max compression
+gzip compressed data, was "GooseHDF5-0.9.2.tar", last modified: Fri Jan 29 10:29:07 2021, max compression
```

## Comparing `GooseHDF5-0.9.1.tar` & `GooseHDF5-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 13:07:22.950963 GooseHDF5-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 13:07:22.946963 GooseHDF5-0.9.1/GooseHDF5/
--rw-r--r--   0 runner    (1001) docker     (116)    15262 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 13:07:22.946963 GooseHDF5-0.9.1/GooseHDF5/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     1253 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5check.py
--rw-r--r--   0 runner    (1001) docker     (116)     3808 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5compare.py
--rw-r--r--   0 runner    (1001) docker     (116)     3708 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2292 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5print.py
--rw-r--r--   0 runner    (1001) docker     (116)     1294 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5repack.py
--rw-r--r--   0 runner    (1001) docker     (116)     1341 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/G5repair.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/GooseHDF5/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 13:07:22.946963 GooseHDF5-0.9.1/GooseHDF5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      260 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      419 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       26 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-10-21 13:07:22.000000 GooseHDF5-0.9.1/GooseHDF5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      260 2020-10-21 13:07:22.950963 GooseHDF5-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1544 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-21 13:07:22.950963 GooseHDF5-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      935 2020-10-21 13:07:14.000000 GooseHDF5-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 10:29:07.171942 GooseHDF5-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 10:29:07.167942 GooseHDF5-0.9.2/GooseHDF5/
+-rw-r--r--   0 runner    (1001) docker     (117)    15262 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 10:29:07.171942 GooseHDF5-0.9.2/GooseHDF5/cli/
+-rw-r--r--   0 runner    (1001) docker     (117)     1253 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5check.py
+-rw-r--r--   0 runner    (1001) docker     (117)     3808 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5compare.py
+-rw-r--r--   0 runner    (1001) docker     (117)     3713 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5list.py
+-rw-r--r--   0 runner    (1001) docker     (117)     2292 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5print.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1294 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5repack.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1341 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/G5repair.py
+-rw-r--r--   0 runner    (1001) docker     (117)        0 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/GooseHDF5/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-29 10:29:07.167942 GooseHDF5-0.9.2/GooseHDF5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (117)      260 2021-01-29 10:29:06.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)      419 2021-01-29 10:29:07.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-01-29 10:29:06.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (117)      247 2021-01-29 10:29:06.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       26 2021-01-29 10:29:06.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       10 2021-01-29 10:29:06.000000 GooseHDF5-0.9.2/GooseHDF5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (117)      260 2021-01-29 10:29:07.171942 GooseHDF5-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     1544 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (117)       38 2021-01-29 10:29:07.171942 GooseHDF5-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (117)      935 2021-01-29 10:28:55.000000 GooseHDF5-0.9.2/setup.py
```

### Comparing `GooseHDF5-0.9.1/GooseHDF5/__init__.py` & `GooseHDF5-0.9.2/GooseHDF5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import h5py
 import numpy as np
 import warnings
 
 warnings.filterwarnings("ignore")
 
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 
 def abspath(path):
     r'''
 Return absolute path.
     '''
```

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5check.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5check.py`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5compare.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5compare.py`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5list.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5list.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
             print('"{0:s}"'.format(path))
             print('- prop: size = {0:s}, shape = {1:s}, dtype = {2:s}'.format(
                 str(data.size), str(data.shape), str(data.dtype)))
 
             for key in data.attrs:
                 print('- attr: ' + key + ' = ')
-                print('        ' + data.attrs[key])
+                print('        ' + str(data.attrs[key]))
 
             print('')
 
 def main():
     r'''
 Main function.
     '''
```

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5print.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5print.py`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5repack.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5repack.py`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/GooseHDF5/cli/G5repair.py` & `GooseHDF5-0.9.2/GooseHDF5/cli/G5repair.py`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/README.md` & `GooseHDF5-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `GooseHDF5-0.9.1/setup.py` & `GooseHDF5-0.9.2/setup.py`

 * *Files identical despite different names*

