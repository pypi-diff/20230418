# Comparing `tmp/py_kvstore-0.0.1-py3-none-any.whl.zip` & `tmp/py_kvstore-0.0.2a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4089 bytes, number of entries: 7
--rw-r--r--  2.0 unx       73 b- defN 23-Apr-18 03:31 py_kvstore/__init__.py
+Zip file size: 4113 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-18 03:37 py_kvstore/__init__.py
 -rw-r--r--  2.0 unx     5076 b- defN 23-Apr-18 03:31 py_kvstore/py_kvstore.py
 -rw-r--r--  2.0 unx     1753 b- defN 23-Apr-18 03:31 py_kvstore/test.py
--rw-r--r--  2.0 unx      657 b- defN 23-Apr-18 03:36 py_kvstore-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 03:36 py_kvstore-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 03:36 py_kvstore-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      542 b- defN 23-Apr-18 03:36 py_kvstore-0.0.1.dist-info/RECORD
-7 files, 8204 bytes uncompressed, 3127 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx      659 b- defN 23-Apr-18 03:38 py_kvstore-0.0.2a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 03:38 py_kvstore-0.0.2a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 03:38 py_kvstore-0.0.2a0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      550 b- defN 23-Apr-18 03:38 py_kvstore-0.0.2a0.dist-info/RECORD
+7 files, 8220 bytes uncompressed, 3135 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: py_kvstore/py_kvstore.py
 Comment: 
 
 Filename: py_kvstore/test.py
 Comment: 
 
-Filename: py_kvstore-0.0.1.dist-info/METADATA
+Filename: py_kvstore-0.0.2a0.dist-info/METADATA
 Comment: 
 
-Filename: py_kvstore-0.0.1.dist-info/WHEEL
+Filename: py_kvstore-0.0.2a0.dist-info/WHEEL
 Comment: 
 
-Filename: py_kvstore-0.0.1.dist-info/top_level.txt
+Filename: py_kvstore-0.0.2a0.dist-info/top_level.txt
 Comment: 
 
-Filename: py_kvstore-0.0.1.dist-info/RECORD
+Filename: py_kvstore-0.0.2a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py_kvstore/__init__.py

```diff
@@ -1,6 +1,6 @@
 """
 py_kvstore.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2-alpha"
 __author__ = "Reece Williams"
```

## Comparing `py_kvstore-0.0.1.dist-info/METADATA` & `py_kvstore-0.0.2a0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-kvstore
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: A key value store
 Home-page: https://github.com/shuds13/pyexample
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

