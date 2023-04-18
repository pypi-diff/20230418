# Comparing `tmp/cwsearch_utils-0.1.0-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4997 bytes, number of entries: 7
+Zip file size: 5004 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
 -rw-rw-r--  2.0 unx     7097 b- defN 23-Apr-09 04:52 cwsearch_utils/aggregate.py
--rw-rw-r--  2.0 unx     4723 b- defN 23-Apr-17 18:25 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/RECORD
-7 files, 13075 bytes uncompressed, 3961 bytes compressed:  69.7%
+-rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 00:22 cwsearch_utils-0.1.1.dist-info/RECORD
+7 files, 13132 bytes uncompressed, 3968 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.0.dist-info/METADATA
+Filename: cwsearch_utils-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.0.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.0.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.0.dist-info/RECORD
+Filename: cwsearch_utils-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/infinstor_lock.py

```diff
@@ -39,15 +39,18 @@
     rv = {}
     con = sqlite3.connect(fn)
     cur = con.cursor()
     if not tag:
         tag = 'notag'
     print(f'load_from_db: Loading fn={fn}, tag={tag}')
     res = cur.execute(f"SELECT name, timestamp, link, msg FROM links WHERE tag='{tag}'")
-    while one_entry = res.fetchone():
+    while True:
+        one_entry = res.fetchone()
+        if not one_entry:
+            break
         name = one_entry[0]
         if name in rv:
             rv[name].append((one_entry[1], one_entry[2], one_entry[3]))
         else:
             rv[name] = [(one_entry[1], one_entry[2], one_entry[3])]
     return rv
```

## Comparing `cwsearch_utils-0.1.0.dist-info/METADATA` & `cwsearch_utils-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

