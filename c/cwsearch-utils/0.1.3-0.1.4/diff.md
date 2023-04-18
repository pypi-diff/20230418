# Comparing `tmp/cwsearch_utils-0.1.3-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5056 bytes, number of entries: 7
+Zip file size: 5050 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7254 b- defN 23-Apr-18 17:28 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7229 b- defN 23-Apr-18 18:14 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/RECORD
-7 files, 13289 bytes uncompressed, 4020 bytes compressed:  69.7%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 18:15 cwsearch_utils-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 18:15 cwsearch_utils-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 18:15 cwsearch_utils-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 18:15 cwsearch_utils-0.1.4.dist-info/RECORD
+7 files, 13264 bytes uncompressed, 4014 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.3.dist-info/METADATA
+Filename: cwsearch_utils-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.3.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.3.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.3.dist-info/RECORD
+Filename: cwsearch_utils-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -1,13 +1,12 @@
 import os
 import json
 import tempfile
 import datetime
 from arnparse import arnparse
-from infinstor_lock import load_from_db
 
 def my_sort_fnx(a):
     return a[0]
 
 def union(ner_entities, dct, infinstor_time_spec):
     for nm in dct:
         if nm in ner_entities:
@@ -117,15 +116,15 @@
     return rv
 
 def process_file(client, bucket, key, ner_entities, infinstor_time_spec):
     try:
         dnm = os.path.join('/tmp', key[key.rindex('/') + 1:])
         print(f"Downloading object {key} to local file {dnm}")
         client.download_file(bucket, key, dnm)
-        dct = load_from_db(dnm, tag)
+        dct = infinstor_lock.load_from_db(dnm, tag)
         union(ner_entities, dct, infinstor_time_spec)
         os.remove(dnm)
         return True
     except Exception as e:
         print(f"Caught {e} while downloading {key} from bucket {bucket}. Ignoring and trying next object..")
     return False
```

## Comparing `cwsearch_utils-0.1.3.dist-info/METADATA` & `cwsearch_utils-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

