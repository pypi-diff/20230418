# Comparing `tmp/reyapi-0.1-py3-none-any.whl.zip` & `tmp/reyapi-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1349 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      236 b- defN 23-Apr-13 02:21 reyapi/__init__.py
--rw-rw-rw-  2.0 fat      174 b- defN 23-Apr-13 02:21 reyapi-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 02:21 reyapi-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-13 02:21 reyapi-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      358 b- defN 23-Apr-13 02:21 reyapi-0.1.dist-info/RECORD
-5 files, 867 bytes uncompressed, 679 bytes compressed:  21.7%
+Zip file size: 1354 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Apr-18 09:19 reyapi/__init__.py
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Apr-18 09:19 reyapi-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 09:19 reyapi-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-18 09:19 reyapi-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      358 b- defN 23-Apr-18 09:19 reyapi-0.2.dist-info/RECORD
+5 files, 869 bytes uncompressed, 684 bytes compressed:  21.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: reyapi/__init__.py
 Comment: 
 
-Filename: reyapi-0.1.dist-info/METADATA
+Filename: reyapi-0.2.dist-info/METADATA
 Comment: 
 
-Filename: reyapi-0.1.dist-info/WHEEL
+Filename: reyapi-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: reyapi-0.1.dist-info/top_level.txt
+Filename: reyapi-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: reyapi-0.1.dist-info/RECORD
+Filename: reyapi-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reyapi/__init__.py

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 @Time    : 2023-02-19 18:59:26
 @Author  : Rey
 @Contact : reyxbo@163.com
-@Explain : Rey's personal API set
+@Explain : Rey's personal API set.
 """
 
 
 from typing import Final
 
 
-__version__: Final[str] = "0.1"
+__version__: Final[str] = "0.2"
```

