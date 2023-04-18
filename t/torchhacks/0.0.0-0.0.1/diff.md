# Comparing `tmp/torchhacks-0.0.0-py3-none-any.whl.zip` & `tmp/torchhacks-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 5534 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 19:53 torchhacks/__init__.py
--rw-r--r--  2.0 unx    11950 b- defN 23-Apr-17 19:55 torchhacks-0.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      322 b- defN 23-Apr-17 19:55 torchhacks-0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 19:55 torchhacks-0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-17 19:55 torchhacks-0.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      477 b- defN 23-Apr-17 19:55 torchhacks-0.0.0.dist-info/RECORD
-6 files, 12852 bytes uncompressed, 4664 bytes compressed:  63.7%
+Zip file size: 6940 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       32 b- defN 23-Apr-17 20:07 torchhacks/__init__.py
+-rw-r--r--  2.0 unx     3825 b- defN 23-Apr-18 11:13 torchhacks/lazyload.py
+-rw-r--r--  2.0 unx    11950 b- defN 23-Apr-18 11:15 torchhacks-0.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      322 b- defN 23-Apr-18 11:15 torchhacks-0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 11:15 torchhacks-0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 11:15 torchhacks-0.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      557 b- defN 23-Apr-18 11:15 torchhacks-0.0.1.dist-info/RECORD
+7 files, 16789 bytes uncompressed, 5950 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: torchhacks/__init__.py
 Comment: 
 
-Filename: torchhacks-0.0.0.dist-info/LICENSE
+Filename: torchhacks/lazyload.py
 Comment: 
 
-Filename: torchhacks-0.0.0.dist-info/METADATA
+Filename: torchhacks-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: torchhacks-0.0.0.dist-info/WHEEL
+Filename: torchhacks-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: torchhacks-0.0.0.dist-info/top_level.txt
+Filename: torchhacks-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: torchhacks-0.0.0.dist-info/RECORD
+Filename: torchhacks-0.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: torchhacks-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchhacks/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 6c61 7a79 6c6f 6164 2069  from .lazyload i
+00000010: 6d70 6f72 7420 6c61 7a79 5f6c 6f61 640a  mport lazy_load.
```

## Comparing `torchhacks-0.0.0.dist-info/LICENSE` & `torchhacks-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

