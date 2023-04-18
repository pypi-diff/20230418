# Comparing `tmp/cwsearch_utils-0.1.1-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5004 bytes, number of entries: 7
+Zip file size: 5043 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7097 b- defN 23-Apr-09 04:52 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7248 b- defN 23-Apr-18 05:09 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/RECORD
-7 files, 13132 bytes uncompressed, 3968 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 05:30 cwsearch_utils-0.1.2.dist-info/RECORD
+7 files, 13283 bytes uncompressed, 4007 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.1.dist-info/METADATA
+Filename: cwsearch_utils-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.1.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.1.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.1.dist-info/RECORD
+Filename: cwsearch_utils-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -126,14 +126,15 @@
         os.remove(dnm)
         return True
     except Exception as e:
         print(f"Caught {e} while downloading {key} from bucket {bucket}. Ignoring and trying next object..")
     return False
 
 def populate_names(bucket, prefix, infinstor_time_spec, log_groups, tag):
+    print(f'populate_names: Entered. bucket={bucket}, prefix={prefix}, infinstor_time_spec={infinstor_time_spec}, log_groups={log_groups}, tag={tag}')
     start_time = datetime.datetime.utcnow()
 
     import boto3
     # first list files in reverse chrono order
     try:
         s3client = boto3.client('s3', infinstor_time_spec=infinstor_time_spec)
         files = get_files_list(s3client, bucket, prefix, log_groups, tag)
```

## Comparing `cwsearch_utils-0.1.1.dist-info/METADATA` & `cwsearch_utils-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.1.1.dist-info/RECORD` & `cwsearch_utils-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cwsearch_utils/aggregate.py,sha256=dY3E3EPH4yB1JOcGoZ_ei6XP1LMeuVjmTbjkAoNIGbE,7097
+cwsearch_utils/aggregate.py,sha256=WZ2EhjI_aCKX9SmNgzRoBHzzooLN2anqRdKjmzOj9ok,7248
 cwsearch_utils/infinstor_lock.py,sha256=kxY_afhPD8K50s1C-bxzs0DX3I28HLsayM-fn8H0Sw8,4780
-cwsearch_utils-0.1.1.dist-info/METADATA,sha256=FqcfrRJNtvcsMqv2g9nfAERqKIa5vIFvsN4bVYGLKVQ,570
-cwsearch_utils-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.1.1.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.1.1.dist-info/RECORD,,
+cwsearch_utils-0.1.2.dist-info/METADATA,sha256=TITW1ffWnQZEL5oUtfE-KCRdNIWm53khnorVgZRRqTU,570
+cwsearch_utils-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.1.2.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.1.2.dist-info/RECORD,,
```

