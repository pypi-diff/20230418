# Comparing `tmp/bamsalvage-0.1.3-py3-none-any.whl.zip` & `tmp/bamsalvage-0.1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9962 bytes, number of entries: 7
+Zip file size: 9984 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      294 b- defN 20-Feb-02 00:00 bamsalvage/__init__.py
--rwxr-xr-x  2.0 unx    24508 b- defN 20-Feb-02 00:00 bamsalvage/_bamsalvage.py
-?rw-r--r--  2.0 unx     1917 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      574 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.dist-info/RECORD
-7 files, 28498 bytes uncompressed, 8942 bytes compressed:  68.6%
+-rwxr-xr-x  2.0 unx    24505 b- defN 20-Feb-02 00:00 bamsalvage/_bamsalvage.py
+?rw-r--r--  2.0 unx     1919 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      584 b- defN 20-Feb-02 00:00 bamsalvage-0.1.3.1.dist-info/RECORD
+7 files, 28507 bytes uncompressed, 8944 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: bamsalvage/__init__.py
 Comment: 
 
 Filename: bamsalvage/_bamsalvage.py
 Comment: 
 
-Filename: bamsalvage-0.1.3.dist-info/METADATA
+Filename: bamsalvage-0.1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: bamsalvage-0.1.3.dist-info/WHEEL
+Filename: bamsalvage-0.1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: bamsalvage-0.1.3.dist-info/entry_points.txt
+Filename: bamsalvage-0.1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bamsalvage-0.1.3.dist-info/licenses/LICENSE
+Filename: bamsalvage-0.1.3.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: bamsalvage-0.1.3.dist-info/RECORD
+Filename: bamsalvage-0.1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bamsalvage/_bamsalvage.py

```diff
@@ -1,8 +1,8 @@
-seeimport os, sys, re, io
+import os, sys, re, io
 import argparse, struct
 import mgzip, gzip
 import zlib, logging, json
 import numba
 import numpy as np
```

## Comparing `bamsalvage-0.1.3.dist-info/METADATA` & `bamsalvage-0.1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamsalvage
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: Sequence salvaging script from corrupted BAM files
 Project-URL: Homepage, https://pypi.org/project/bamsalvage/
 Author-email: Example Author <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bamsalvage-0.1.3.dist-info/licenses/LICENSE` & `bamsalvage-0.1.3.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `bamsalvage-0.1.3.dist-info/RECORD` & `bamsalvage-0.1.3.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 bamsalvage/__init__.py,sha256=BDawhNEiBhP5W4k2RtdPP4sBGHR3XmGrFnNfPjd0puw,294
-bamsalvage/_bamsalvage.py,sha256=ZRtVC1MSPFTc2uqhq3ucvnKKmmjU7hq17OJt5pMd8AM,24508
-bamsalvage-0.1.3.dist-info/METADATA,sha256=Oz9RzH-YfFBkO3-fHUUJ8PDUExOv0l73qGi4mwC6rHE,1917
-bamsalvage-0.1.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-bamsalvage-0.1.3.dist-info/entry_points.txt,sha256=Cnt2RJEPQBrBYrjaB-DdT14IAxWYjECB5JzQJ-m134A,47
-bamsalvage-0.1.3.dist-info/licenses/LICENSE,sha256=eYJxrN4tEqZIwQNTXVgv0ifVy72AfkQD2DvMOzPl6rg,1071
-bamsalvage-0.1.3.dist-info/RECORD,,
+bamsalvage/_bamsalvage.py,sha256=bDFpLZt7ijhrq1jchphhgefrGE_HMBhO-7n0pFpSgaQ,24505
+bamsalvage-0.1.3.1.dist-info/METADATA,sha256=xRqUkY9vX31uC6lQy4JhdTU9GZhnanxoH8qjj5yNlvU,1919
+bamsalvage-0.1.3.1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+bamsalvage-0.1.3.1.dist-info/entry_points.txt,sha256=Cnt2RJEPQBrBYrjaB-DdT14IAxWYjECB5JzQJ-m134A,47
+bamsalvage-0.1.3.1.dist-info/licenses/LICENSE,sha256=eYJxrN4tEqZIwQNTXVgv0ifVy72AfkQD2DvMOzPl6rg,1071
+bamsalvage-0.1.3.1.dist-info/RECORD,,
```

