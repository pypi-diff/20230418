# Comparing `tmp/lazycsv-1.0.1.tar.gz` & `tmp/lazycsv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.0.1.tar", last modified: Tue Apr 18 01:14:15 2023, max compression
+gzip compressed data, was "lazycsv-1.0.2.tar", last modified: Tue Apr 18 01:18:20 2023, max compression
```

## Comparing `lazycsv-1.0.1.tar` & `lazycsv-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:14:15.796744 lazycsv-1.0.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.0.1/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     8492 2023-04-18 01:14:15.796744 lazycsv-1.0.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     7811 2023-04-18 00:23:08.000000 lazycsv-1.0.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-18 01:14:15.796744 lazycsv-1.0.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2042 2023-04-18 01:14:03.000000 lazycsv-1.0.1/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:14:15.796744 lazycsv-1.0.1/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:14:15.796744 lazycsv-1.0.1/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.0.1/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32804 2023-04-18 01:12:36.000000 lazycsv-1.0.1/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:14:15.796744 lazycsv-1.0.1/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     8492 2023-04-18 01:14:15.000000 lazycsv-1.0.1/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-04-18 01:14:15.000000 lazycsv-1.0.1/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-18 01:14:15.000000 lazycsv-1.0.1/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-18 01:14:15.000000 lazycsv-1.0.1/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-18 01:14:15.000000 lazycsv-1.0.1/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:14:15.796744 lazycsv-1.0.1/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    20036 2023-04-15 01:06:00.000000 lazycsv-1.0.1/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.0.2/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     8548 2023-04-18 01:18:20.654179 lazycsv-1.0.2/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     7867 2023-04-18 01:17:52.000000 lazycsv-1.0.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-18 01:18:20.654179 lazycsv-1.0.2/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2042 2023-04-18 01:14:43.000000 lazycsv-1.0.2/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.0.2/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32804 2023-04-18 01:12:36.000000 lazycsv-1.0.2/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8548 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    20036 2023-04-15 01:06:00.000000 lazycsv-1.0.2/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.0.1/LICENSE` & `lazycsv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.0.1/PKG-INFO` & `lazycsv-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.1
+Version: 1.0.2
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -31,23 +31,24 @@
 allows a user to generate PyObject's from a csv file lazily.
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
-This value is always an `unsigned short`, which we found to be the optimal bit
-size for disk usage and execution performance (this can be adjusted in the
-setup.py file). For index values outside the range of an unsigned short, An
-"anchor point" is created, which is a pair of `size_t` values that mark both
-the value which is subtracted from the index value such that the index value
-fits within 16 bits, and the first column of the CSV where the anchor value
-applies. This anchor point is periodically written to the second index file
-when required for a given comma index. Finally, the third index writes the
-index of the first anchor point for each row of the file.
+This value is always a `uint16_t` which we found to be the optimal bit size for
+disk usage and execution performance. (This type can however be changed by
+setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
+type) For index values outside the range of an unsigned short, An "anchor
+point" is created, which is a pair of `size_t` values that mark both the value
+which is subtracted from the index value such that the index value fits within
+16 bits, and the first column of the CSV where the anchor value applies. This
+anchor point is periodically written to the second index file when required for
+a given comma index. Finally, the third index writes the index of the first
+anchor point for each row of the file.
 
 When a user requests a sequence of data (i.e. a row or a column), an iterator
 is created and returned. This iterator uses the value of the requested sequence
 and its internal position state to index into the index files the values
 representing the index of the requested field, and its length. Those two values
 are then used to create a single PyBytes object. These PyBytes objects are then
 yielded to the user per-iteration.
@@ -152,15 +153,15 @@
 1-dimensional numpy array without creating intermediary PyObject*'s for each
 field of the CSV file.
 
 Access to this feature requires numpy to be preinstalled as this feature makes
 numpy a compilation dependency.
 
 ```bash
-$ LAZYCSV_INCLUDE_NUMPY=1 python setup.py build_ext --inplace --force
+$ LAZYCSV_INCLUDE_NUMPY=1 python -m pip install lazycsv
 ```
 ```python
 >>> import numpy as np
 >>> from lazycsv import lazycsv
 >>> lazy = lazycsv.LazyCSV("")
 >>> lazy = lazycsv.LazyCSV("./tests/fixtures/file.csv")
 >>> lazy.sequence(col=0).to_numpy().astype(np.int8)
```

### Comparing `lazycsv-1.0.1/README.md` & `lazycsv-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 allows a user to generate PyObject's from a csv file lazily.
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
-This value is always an `unsigned short`, which we found to be the optimal bit
-size for disk usage and execution performance (this can be adjusted in the
-setup.py file). For index values outside the range of an unsigned short, An
-"anchor point" is created, which is a pair of `size_t` values that mark both
-the value which is subtracted from the index value such that the index value
-fits within 16 bits, and the first column of the CSV where the anchor value
-applies. This anchor point is periodically written to the second index file
-when required for a given comma index. Finally, the third index writes the
-index of the first anchor point for each row of the file.
+This value is always a `uint16_t` which we found to be the optimal bit size for
+disk usage and execution performance. (This type can however be changed by
+setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
+type) For index values outside the range of an unsigned short, An "anchor
+point" is created, which is a pair of `size_t` values that mark both the value
+which is subtracted from the index value such that the index value fits within
+16 bits, and the first column of the CSV where the anchor value applies. This
+anchor point is periodically written to the second index file when required for
+a given comma index. Finally, the third index writes the index of the first
+anchor point for each row of the file.
 
 When a user requests a sequence of data (i.e. a row or a column), an iterator
 is created and returned. This iterator uses the value of the requested sequence
 and its internal position state to index into the index files the values
 representing the index of the requested field, and its length. Those two values
 are then used to create a single PyBytes object. These PyBytes objects are then
 yielded to the user per-iteration.
@@ -132,15 +133,15 @@
 1-dimensional numpy array without creating intermediary PyObject*'s for each
 field of the CSV file.
 
 Access to this feature requires numpy to be preinstalled as this feature makes
 numpy a compilation dependency.
 
 ```bash
-$ LAZYCSV_INCLUDE_NUMPY=1 python setup.py build_ext --inplace --force
+$ LAZYCSV_INCLUDE_NUMPY=1 python -m pip install lazycsv
 ```
 ```python
 >>> import numpy as np
 >>> from lazycsv import lazycsv
 >>> lazy = lazycsv.LazyCSV("")
 >>> lazy = lazycsv.LazyCSV("./tests/fixtures/file.csv")
 >>> lazy.sequence(col=0).to_numpy().astype(np.int8)
```

### Comparing `lazycsv-1.0.1/setup.py` & `lazycsv-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.0.1",
+    version="1.0.2",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an OOM csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
```

### Comparing `lazycsv-1.0.1/src/lazycsv/lazycsv.c` & `lazycsv-1.0.2/src/lazycsv/lazycsv.c`

 * *Files identical despite different names*

### Comparing `lazycsv-1.0.1/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.0.2/src/lazycsv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.1
+Version: 1.0.2
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -31,23 +31,24 @@
 allows a user to generate PyObject's from a csv file lazily.
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
-This value is always an `unsigned short`, which we found to be the optimal bit
-size for disk usage and execution performance (this can be adjusted in the
-setup.py file). For index values outside the range of an unsigned short, An
-"anchor point" is created, which is a pair of `size_t` values that mark both
-the value which is subtracted from the index value such that the index value
-fits within 16 bits, and the first column of the CSV where the anchor value
-applies. This anchor point is periodically written to the second index file
-when required for a given comma index. Finally, the third index writes the
-index of the first anchor point for each row of the file.
+This value is always a `uint16_t` which we found to be the optimal bit size for
+disk usage and execution performance. (This type can however be changed by
+setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
+type) For index values outside the range of an unsigned short, An "anchor
+point" is created, which is a pair of `size_t` values that mark both the value
+which is subtracted from the index value such that the index value fits within
+16 bits, and the first column of the CSV where the anchor value applies. This
+anchor point is periodically written to the second index file when required for
+a given comma index. Finally, the third index writes the index of the first
+anchor point for each row of the file.
 
 When a user requests a sequence of data (i.e. a row or a column), an iterator
 is created and returned. This iterator uses the value of the requested sequence
 and its internal position state to index into the index files the values
 representing the index of the requested field, and its length. Those two values
 are then used to create a single PyBytes object. These PyBytes objects are then
 yielded to the user per-iteration.
@@ -152,15 +153,15 @@
 1-dimensional numpy array without creating intermediary PyObject*'s for each
 field of the CSV file.
 
 Access to this feature requires numpy to be preinstalled as this feature makes
 numpy a compilation dependency.
 
 ```bash
-$ LAZYCSV_INCLUDE_NUMPY=1 python setup.py build_ext --inplace --force
+$ LAZYCSV_INCLUDE_NUMPY=1 python -m pip install lazycsv
 ```
 ```python
 >>> import numpy as np
 >>> from lazycsv import lazycsv
 >>> lazy = lazycsv.LazyCSV("")
 >>> lazy = lazycsv.LazyCSV("./tests/fixtures/file.csv")
 >>> lazy.sequence(col=0).to_numpy().astype(np.int8)
```

### Comparing `lazycsv-1.0.1/tests/test_lazycsv.py` & `lazycsv-1.0.2/tests/test_lazycsv.py`

 * *Files identical despite different names*

