# Comparing `tmp/xlibs-0.0.2-py3-none-any.whl.zip` & `tmp/xlibs-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1503 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      190 b- defN 23-Apr-18 09:43 x/__init__.py
+Zip file size: 1527 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-18 09:56 x/__init__.py
 -rw-rw-rw-  2.0 fat      103 b- defN 23-Apr-18 09:43 x/_ver.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-Apr-18 09:45 xlibs-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 09:45 xlibs-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-18 09:45 xlibs-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      422 b- defN 23-Apr-18 09:45 xlibs-0.0.2.dist-info/RECORD
-6 files, 1053 bytes uncompressed, 741 bytes compressed:  29.6%
+-rw-rw-rw-  2.0 fat      198 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      422 b- defN 23-Apr-18 10:10 xlibs-0.0.3.dist-info/RECORD
+6 files, 1111 bytes uncompressed, 765 bytes compressed:  31.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: x/__init__.py
 Comment: 
 
 Filename: x/_ver.py
 Comment: 
 
-Filename: xlibs-0.0.2.dist-info/METADATA
+Filename: xlibs-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xlibs-0.0.2.dist-info/WHEEL
+Filename: xlibs-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xlibs-0.0.2.dist-info/top_level.txt
+Filename: xlibs-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xlibs-0.0.2.dist-info/RECORD
+Filename: xlibs-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## x/__init__.py

```diff
@@ -1,12 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 x: the everything pkg
 """
 
+#%% imports 
+
 import os
+import sys
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import thelogger as tl
 
-from _ver import __version__
+from icecream import ic
+from ._ver import __version__
+
+#%% fns
+
+def env():
+    return sys.executable
```

