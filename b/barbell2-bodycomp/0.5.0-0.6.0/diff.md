# Comparing `tmp/barbell2_bodycomp-0.5.0.tar.gz` & `tmp/barbell2_bodycomp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_bodycomp-0.5.0.tar", last modified: Sat Apr 15 10:50:04 2023, max compression
+gzip compressed data, was "barbell2_bodycomp-0.6.0.tar", last modified: Tue Apr 18 13:15:19 2023, max compression
```

## Comparing `barbell2_bodycomp-0.5.0.tar` & `barbell2_bodycomp-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.725824 barbell2_bodycomp-0.5.0/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 10:50:04.725562 barbell2_bodycomp-0.5.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.720772 barbell2_bodycomp-0.5.0/barbell2_bodycomp/
--rw-r--r--   0 ralph      (501) staff       (20)      392 2023-04-15 10:50:00.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     4447 2023-04-15 10:49:32.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/calculator.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.724652 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/
--rw-r--r--   0 ralph      (501) staff       (20)      403 2023-04-13 11:54:27.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2npy.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.725060 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/
--rw-r--r--   0 ralph      (501) staff       (20)        0 2023-04-13 11:55:38.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     3434 2023-04-15 08:57:42.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/bodycomp.py
--rw-r--r--   0 ralph      (501) staff       (20)     6054 2023-04-13 11:59:22.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/seg.py
--rw-r--r--   0 ralph      (501) staff       (20)     1394 2023-04-13 12:19:43.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectroi.py
--rw-r--r--   0 ralph      (501) staff       (20)     5804 2023-04-13 12:19:18.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectslice.py
--rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/totalseg.py
--rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.722759 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      882 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       68 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 10:50:04.725902 barbell2_bodycomp-0.5.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1456 2023-04-13 12:44:51.000000 barbell2_bodycomp-0.5.0/setup.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.746585 barbell2_bodycomp-0.6.0/
+-rw-r--r--   0 Ralph      (501) staff       (20)      802 2023-04-18 13:15:19.746323 barbell2_bodycomp-0.6.0/PKG-INFO
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.738920 barbell2_bodycomp-0.6.0/barbell2_bodycomp/
+-rw-r--r--   0 Ralph      (501) staff       (20)      392 2023-04-18 13:15:13.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     4447 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.743760 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 Ralph      (501) staff       (20)      403 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     2200 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1485 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1405 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      853 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     2030 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1059 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      435 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2npy.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.744202 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/
+-rw-r--r--   0 Ralph      (501) staff       (20)        0 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     5705 2023-04-17 10:38:03.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/pipeline/bodycomp.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6054 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1394 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     5804 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1586 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6246 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-04-18 13:15:19.741339 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 Ralph      (501) staff       (20)      802 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 Ralph      (501) staff       (20)      882 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/entry_points.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 Ralph      (501) staff       (20)       68 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       18 2023-04-18 13:15:18.000000 barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-04-18 13:15:19.746668 barbell2_bodycomp-0.6.0/setup.cfg
+-rw-r--r--   0 Ralph      (501) staff       (20)     1456 2023-04-17 09:26:44.000000 barbell2_bodycomp-0.6.0/setup.py
```

### Comparing `barbell2_bodycomp-0.5.0/PKG-INFO` & `barbell2_bodycomp-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2_bodycomp
-Version: 0.5.0
+Version: 0.6.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/calculator.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/calculator.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/seg.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/seg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectroi.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectroi.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectslice.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/selectslice.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/totalseg.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/totalseg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2-bodycomp
-Version: 0.5.0
+Version: 0.6.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.6.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.5.0/setup.py` & `barbell2_bodycomp-0.6.0/setup.py`

 * *Files identical despite different names*

