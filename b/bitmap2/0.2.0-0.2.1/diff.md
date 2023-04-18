# Comparing `tmp/bitmap2-0.2.0.tar.gz` & `tmp/bitmap2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.2.0.tar", last modified: Mon Apr 17 20:19:19 2023, max compression
+gzip compressed data, was "bitmap2-0.2.1.tar", last modified: Tue Apr 18 01:21:27 2023, max compression
```

## Comparing `bitmap2-0.2.0.tar` & `bitmap2-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 20:19:14.000000 bitmap2-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 20:19:14.000000 bitmap2-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 20:19:19.954870 bitmap2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-17 20:19:14.000000 bitmap2-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:19:19.954870 bitmap2-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-17 20:19:14.000000 bitmap2-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 20:19:14.000000 bitmap2-0.2.0/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6425 2023-04-17 20:19:14.000000 bitmap2-0.2.0/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-17 20:19:14.000000 bitmap2-0.2.0/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.268030 bitmap2-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-18 01:21:20.000000 bitmap2-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 01:21:20.000000 bitmap2-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:21:20.000000 bitmap2-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 01:21:27.272030 bitmap2-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-18 01:21:20.000000 bitmap2-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 01:21:27.000000 bitmap2-0.2.1/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:21:27.272030 bitmap2-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-18 01:21:20.000000 bitmap2-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 01:21:20.000000 bitmap2-0.2.1/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6529 2023-04-18 01:21:20.000000 bitmap2-0.2.1/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:21:27.272030 bitmap2-0.2.1/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-18 01:21:20.000000 bitmap2-0.2.1/test/test_bitmap.py
```

### Comparing `bitmap2-0.2.0/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.1/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/.github/workflows/test.yml` & `bitmap2-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/.gitignore` & `bitmap2-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/LICENSE.md` & `bitmap2-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/PKG-INFO` & `bitmap2-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.0
+Version: 0.2.1
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.0/README.md` & `bitmap2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.1/bitmap2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.0
+Version: 0.2.1
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.0/setup.py` & `bitmap2-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.0/src/bitmap.py` & `bitmap2-0.2.1/src/bitmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,18 +210,21 @@
         """
         val = self.tostring()
         st = "{0:0x}".format(int(val, 2))
         return st.zfill(len(self.bitmap) * 2)
 
     def tofile(self, path):
         """
-        Save bitmap as array to file
+        Save bitmap to file
         """
         with open(path, 'wb') as file:
-            self.bitmap.tofile(file)
+            if isinstance(self.bitmap, bytearray):
+                file.write(self.bitmap)
+            else:
+                self.bitmap.tofile(file)
 
     @classmethod
     def fromhexstring(cls, hexstring):
         """
         Construct BitMap from hex string
         """
         bitstring = format(int(hexstring, 16), "0" + str(int(len(hexstring)/4)) + "b")
```

### Comparing `bitmap2-0.2.0/test/test_bitmap.py` & `bitmap2-0.2.1/test/test_bitmap.py`

 * *Files identical despite different names*

