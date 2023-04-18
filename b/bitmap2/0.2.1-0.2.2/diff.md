# Comparing `tmp/bitmap2-0.2.1.tar.gz` & `tmp/bitmap2-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.2.1.tar", last modified: Tue Apr 18 01:21:27 2023, max compression
+gzip compressed data, was "bitmap2-0.2.2.tar", last modified: Tue Apr 18 16:43:18 2023, max compression
```

## Comparing `bitmap2-0.2.1.tar` & `bitmap2-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.268030 bitmap2-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 01:21:20.000000 bitmap2-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:21:20.000000 bitmap2-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 01:21:27.272030 bitmap2-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-18 01:21:20.000000 bitmap2-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:21:27.272030 bitmap2-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-18 01:21:20.000000 bitmap2-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 01:21:20.000000 bitmap2-0.2.1/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6529 2023-04-18 01:21:20.000000 bitmap2-0.2.1/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-18 01:21:20.000000 bitmap2-0.2.1/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-18 16:43:12.000000 bitmap2-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 16:43:12.000000 bitmap2-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:43:12.000000 bitmap2-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:43:18.679307 bitmap2-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-18 16:43:12.000000 bitmap2-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 16:43:18.000000 bitmap2-0.2.2/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:43:18.679307 bitmap2-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-18 16:43:12.000000 bitmap2-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 16:43:12.000000 bitmap2-0.2.2/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2023-04-18 16:43:12.000000 bitmap2-0.2.2/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:18.679307 bitmap2-0.2.2/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-18 16:43:12.000000 bitmap2-0.2.2/test/test_bitmap.py
```

### Comparing `bitmap2-0.2.1/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.2/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/.github/workflows/test.yml` & `bitmap2-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/.gitignore` & `bitmap2-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/LICENSE.md` & `bitmap2-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/PKG-INFO` & `bitmap2-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.1
+Version: 0.2.2
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.1/README.md` & `bitmap2-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.2/bitmap2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.1
+Version: 0.2.2
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.1/setup.py` & `bitmap2-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.1/src/bitmap.py` & `bitmap2-0.2.2/src/bitmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             step = item.step
             if not isinstance(item.start, int):
                 start = 0
             if not isinstance(item.step, int):
                 step = 1
             if not isinstance(item.stop, int):
                 stop = self.bit_size()
-            return [self.test(i) for i in range(start, stop, step)]
+            return [self.test(i) for i in range(start, min(stop, self.bit_size()), step)]
         else:
             return self.test(item)
 
     def __setitem__(self, key, value):
         """
         Sets a bit when indexing like a array
         """
@@ -191,17 +191,17 @@
             if not isinstance(key.start, int):
                 start = 0
             if not isinstance(key.step, int):
                 step = 1
             if not isinstance(key.stop, int):
                 stop = self.bit_size()
             if value:
-                [self.set(i) for i in range(start, stop, step)]
+                [self.set(i) for i in range(start, min(stop, self.bit_size()), step)]
             else:
-                [self.reset(i) for i in range(start, stop, step)]
+                [self.reset(i) for i in range(start, min(stop, self.bit_size()), step)]
         else:
             if value:
                 self.set(value)
             else:
                 self.reset(value)
 
     def tohexstring(self):
```

### Comparing `bitmap2-0.2.1/test/test_bitmap.py` & `bitmap2-0.2.2/test/test_bitmap.py`

 * *Files identical despite different names*

