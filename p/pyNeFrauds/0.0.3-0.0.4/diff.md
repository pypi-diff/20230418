# Comparing `tmp/pyNeFrauds-0.0.3-py3-none-any.whl.zip` & `tmp/pyNeFrauds-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14382 bytes, number of entries: 20
+Zip file size: 14378 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx     4735 b- defN 23-Apr-06 02:46 PyNeFrauds/Constructor.py
 -rw-rw-r--  2.0 unx      110 b- defN 23-Apr-17 08:13 PyNeFrauds/Globals.py
 -rw-rw-r--  2.0 unx     3413 b- defN 23-Apr-17 08:34 PyNeFrauds/Neo4jHandler.py
 -rw-rw-r--  2.0 unx     1564 b- defN 23-Apr-17 08:15 PyNeFrauds/QueryConstructor.py
--rw-rw-r--  2.0 unx       85 b- defN 23-Apr-18 14:44 PyNeFrauds/__init__.py
+-rw-rw-r--  2.0 unx       86 b- defN 23-Apr-18 14:52 PyNeFrauds/__init__.py
 -rw-rw-r--  2.0 unx     2873 b- defN 23-Apr-06 02:42 PyNeFrauds/extractor.py
 -rw-rw-r--  2.0 unx     5851 b- defN 23-Apr-18 02:29 PyNeFrauds/nn/EmbedFetcher.py
 -rw-rw-r--  2.0 unx     2025 b- defN 23-Apr-18 06:03 PyNeFrauds/nn/Evaluation.py
 -rw-rw-r--  2.0 unx     1028 b- defN 23-Apr-18 02:44 PyNeFrauds/nn/ModelBuilder.py
 -rw-rw-r--  2.0 unx      901 b- defN 23-Apr-18 07:39 PyNeFrauds/nn/Trainer.py
 -rw-rw-r--  2.0 unx      179 b- defN 23-Apr-18 05:38 PyNeFrauds/nn/__init__.py
 -rw-rw-r--  2.0 unx     2483 b- defN 23-Apr-18 07:52 PyNeFrauds/nn/toPyGData.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-18 08:40 PyNeFrauds/tests/__init__.py
 -rw-rw-r--  2.0 unx     2721 b- defN 23-Apr-18 11:03 PyNeFrauds/tests/tests.py
 -rw-rw-r--  2.0 unx       27 b- defN 23-Apr-18 14:44 PyNeFrauds/tests/unittest_test.py
--rw-rw-r--  2.0 unx     1050 b- defN 23-Apr-18 14:46 pyNeFrauds-0.0.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      683 b- defN 23-Apr-18 14:46 pyNeFrauds-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 14:46 pyNeFrauds-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Apr-18 14:46 pyNeFrauds-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1642 b- defN 23-Apr-18 14:46 pyNeFrauds-0.0.3.dist-info/RECORD
-20 files, 31473 bytes uncompressed, 11698 bytes compressed:  62.8%
+-rw-rw-r--  2.0 unx     1050 b- defN 23-Apr-18 14:52 pyNeFrauds-0.0.4.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      683 b- defN 23-Apr-18 14:52 pyNeFrauds-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 14:52 pyNeFrauds-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Apr-18 14:52 pyNeFrauds-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1642 b- defN 23-Apr-18 14:52 pyNeFrauds-0.0.4.dist-info/RECORD
+20 files, 31474 bytes uncompressed, 11694 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: PyNeFrauds/tests/tests.py
 Comment: 
 
 Filename: PyNeFrauds/tests/unittest_test.py
 Comment: 
 
-Filename: pyNeFrauds-0.0.3.dist-info/LICENSE.txt
+Filename: pyNeFrauds-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyNeFrauds-0.0.3.dist-info/METADATA
+Filename: pyNeFrauds-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pyNeFrauds-0.0.3.dist-info/WHEEL
+Filename: pyNeFrauds-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyNeFrauds-0.0.3.dist-info/top_level.txt
+Filename: pyNeFrauds-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyNeFrauds-0.0.3.dist-info/RECORD
+Filename: pyNeFrauds-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PyNeFrauds/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .Globals import *
 from .QueryConstructor import QueryConstructor
-import nn as nn
+from . import nn
```

## Comparing `pyNeFrauds-0.0.3.dist-info/LICENSE.txt` & `pyNeFrauds-0.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pyNeFrauds-0.0.3.dist-info/METADATA` & `pyNeFrauds-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNeFrauds
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library that integrates with neo4j facilitating in fraud detection using deep learning techniques.
 Author: Deepam Rai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

## Comparing `pyNeFrauds-0.0.3.dist-info/RECORD` & `pyNeFrauds-0.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 PyNeFrauds/Constructor.py,sha256=urwe8E-33GWrZsbSWYkWSSQMarvUqc6rujsu4OpRmUE,4735
 PyNeFrauds/Globals.py,sha256=lQtryF9kLW3eal8p4dBCUjeHdO-8p1QriF5OixuagtM,110
 PyNeFrauds/Neo4jHandler.py,sha256=joZ7Mziv8PLk0ny-nAJKIf_i9jFlRjgc_OWYF4SmKC0,3413
 PyNeFrauds/QueryConstructor.py,sha256=COTVqXFWpyqABrHkvjJqmr011C4FllnretFDTFOqyKc,1564
-PyNeFrauds/__init__.py,sha256=Qt2R-hwNAeMn57WzDdcTIK6wWy6-pb67H6MIDUE5Buw,85
+PyNeFrauds/__init__.py,sha256=TdJSko4QwIuQqg00S55DMHyP4ZGGnS8Dny4N-oRITLE,86
 PyNeFrauds/extractor.py,sha256=9I3y0UUDRdCBZNc5fcuwZS_KpIWxd67Ss7IK4ZpDTbc,2873
 PyNeFrauds/nn/EmbedFetcher.py,sha256=YjkzWurkKgUp5xLP0vnZV7_Ic_rxdkNTkVz24TRy2D8,5851
 PyNeFrauds/nn/Evaluation.py,sha256=D4rUMqX3UMnOF6zFvGQUBbdVWWsC6c1jm4vxQmt_QSI,2025
 PyNeFrauds/nn/ModelBuilder.py,sha256=VVFgHiCpDhaJDXE4Vsr5hN1vkXHUaTgEISuaR1Y5X68,1028
 PyNeFrauds/nn/Trainer.py,sha256=PrKadsCZdAmhl_G4ryyfn4ILJtbvCl778OdiGJ-WWFs,901
 PyNeFrauds/nn/__init__.py,sha256=iuwjpxY0GYX9oMVMKq2vW0H4k6UiOXavlno427GboxY,179
 PyNeFrauds/nn/toPyGData.py,sha256=cEw-ChifMNA_vF8lrNVfwZwIN89m7qWzGSw6dOxGYZE,2483
 PyNeFrauds/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 PyNeFrauds/tests/tests.py,sha256=s2Rjlhyj73ZoCckukm_wUT1rmJUDP9rsLsLj6gUD6qA,2721
 PyNeFrauds/tests/unittest_test.py,sha256=yuvnAe-uwo0lQUAFKiwE7xYhxt3S2paLuarSaFFy5nY,27
-pyNeFrauds-0.0.3.dist-info/LICENSE.txt,sha256=Y7_zh22DSGssQEoV7hzfqrET9eS_O_Pjwbgbp4TyO0U,1050
-pyNeFrauds-0.0.3.dist-info/METADATA,sha256=dWIkH1LC0gPf-xr08TSj0wqfvrU6zuyM_xjLpZt4LNc,683
-pyNeFrauds-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyNeFrauds-0.0.3.dist-info/top_level.txt,sha256=_z5ugKVthNv9iObuRHmamNyefsJqoRiCmgj4-Hu3Mlw,11
-pyNeFrauds-0.0.3.dist-info/RECORD,,
+pyNeFrauds-0.0.4.dist-info/LICENSE.txt,sha256=Y7_zh22DSGssQEoV7hzfqrET9eS_O_Pjwbgbp4TyO0U,1050
+pyNeFrauds-0.0.4.dist-info/METADATA,sha256=Qy7ppNnvCjyFlGafjBpWZCwh7YecryLN3JVzuq3QS7g,683
+pyNeFrauds-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyNeFrauds-0.0.4.dist-info/top_level.txt,sha256=_z5ugKVthNv9iObuRHmamNyefsJqoRiCmgj4-Hu3Mlw,11
+pyNeFrauds-0.0.4.dist-info/RECORD,,
```

