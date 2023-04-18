# Comparing `tmp/cwsearch_utils-0.1.2-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5043 bytes, number of entries: 7
+Zip file size: 5056 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7248 b- defN 23-Apr-18 05:09 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7254 b- defN 23-Apr-18 17:28 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/RECORD
-7 files, 13283 bytes uncompressed, 4007 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 17:29 cwsearch_utils-0.1.3.dist-info/RECORD
+7 files, 13289 bytes uncompressed, 4020 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.2.dist-info/METADATA
+Filename: cwsearch_utils-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.2.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.2.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.2.dist-info/RECORD
+Filename: cwsearch_utils-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 import tempfile
 import datetime
 from arnparse import arnparse
+from infinstor_lock import load_from_db
 
 def my_sort_fnx(a):
     return a[0]
 
 def union(ner_entities, dct, infinstor_time_spec):
     for nm in dct:
         if nm in ner_entities:
@@ -116,17 +117,16 @@
     return rv
 
 def process_file(client, bucket, key, ner_entities, infinstor_time_spec):
     try:
         dnm = os.path.join('/tmp', key[key.rindex('/') + 1:])
         print(f"Downloading object {key} to local file {dnm}")
         client.download_file(bucket, key, dnm)
-        with open(dnm, 'r') as fp:
-            dct = json.load(fp)
-            union(ner_entities, dct, infinstor_time_spec)
+        dct = load_from_db(dnm, tag)
+        union(ner_entities, dct, infinstor_time_spec)
         os.remove(dnm)
         return True
     except Exception as e:
         print(f"Caught {e} while downloading {key} from bucket {bucket}. Ignoring and trying next object..")
     return False
 
 def populate_names(bucket, prefix, infinstor_time_spec, log_groups, tag):
```

## Comparing `cwsearch_utils-0.1.2.dist-info/METADATA` & `cwsearch_utils-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.1.2.dist-info/RECORD` & `cwsearch_utils-0.1.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cwsearch_utils/aggregate.py,sha256=WZ2EhjI_aCKX9SmNgzRoBHzzooLN2anqRdKjmzOj9ok,7248
+cwsearch_utils/aggregate.py,sha256=HlqE3LtG7lDF6JzsTw4KyULfD_f9UEX7wXYvuKYOgWQ,7254
 cwsearch_utils/infinstor_lock.py,sha256=kxY_afhPD8K50s1C-bxzs0DX3I28HLsayM-fn8H0Sw8,4780
-cwsearch_utils-0.1.2.dist-info/METADATA,sha256=TITW1ffWnQZEL5oUtfE-KCRdNIWm53khnorVgZRRqTU,570
-cwsearch_utils-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.1.2.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.1.2.dist-info/RECORD,,
+cwsearch_utils-0.1.3.dist-info/METADATA,sha256=6n3o2wGItgvRPWuKqw1bXpn2zlv5YimsPNbywI_W0OM,570
+cwsearch_utils-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.1.3.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.1.3.dist-info/RECORD,,
```

