# Comparing `tmp/pyiotown-0.4.3.dev3-py3-none-any.whl.zip` & `tmp/pyiotown-0.4.3.dev4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6607 bytes, number of entries: 10
+Zip file size: 6610 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 22-May-02 13:29 pyiotown/__init__.py
--rw-r--r--  2.0 unx     3423 b- defN 23-Mar-01 15:08 pyiotown/get.py
+-rw-r--r--  2.0 unx     3416 b- defN 23-Mar-01 15:28 pyiotown/get.py
 -rw-r--r--  2.0 unx     3794 b- defN 22-Sep-05 13:00 pyiotown/post.py
 -rw-r--r--  2.0 unx     6701 b- defN 23-Mar-01 07:24 pyiotown/post_process.py
--rw-r--r--  2.0 unx     1053 b- defN 23-Mar-01 15:24 pyiotown-0.4.3.dev3.dist-info/LICENSE
--rw-r--r--  2.0 unx      693 b- defN 23-Mar-01 15:24 pyiotown-0.4.3.dev3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-01 15:24 pyiotown-0.4.3.dev3.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-01 15:23 pyiotown-0.4.3.dev3.dist-info/pbr.json
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-01 15:24 pyiotown-0.4.3.dev3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      807 b- defN 23-Mar-01 15:24 pyiotown-0.4.3.dev3.dist-info/RECORD
-10 files, 16619 bytes uncompressed, 5221 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     1053 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      693 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/pbr.json
+-rw-r--r--  2.0 unx        9 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      807 b- defN 23-Mar-01 15:29 pyiotown-0.4.3.dev4.dist-info/RECORD
+10 files, 16612 bytes uncompressed, 5224 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pyiotown/post.py
 Comment: 
 
 Filename: pyiotown/post_process.py
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/LICENSE
+Filename: pyiotown-0.4.3.dev4.dist-info/LICENSE
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/METADATA
+Filename: pyiotown-0.4.3.dev4.dist-info/METADATA
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/WHEEL
+Filename: pyiotown-0.4.3.dev4.dist-info/WHEEL
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/pbr.json
+Filename: pyiotown-0.4.3.dev4.dist-info/pbr.json
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/top_level.txt
+Filename: pyiotown-0.4.3.dev4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyiotown-0.4.3.dev3.dist-info/RECORD
+Filename: pyiotown-0.4.3.dev4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyiotown/get.py

```diff
@@ -4,15 +4,15 @@
 def node(url, token, nid=None, group_id=None, verify=True, timeout=60):
     header = {'Accept':'application/json','token':token}
 
     # only for administrators
     if group_id is not None:
         header['grpid'] = group_id
 
-    uri_prefix = url + "/api/v1.0/" + ("nodes" if nid is None else f"node/{nid}")
+    uri = url + "/api/v1.0/" + ("nodes" if nid is None else f"node/{nid}")
     
     try:
         r = requests.get(uri, headers=header, verify=verify, timeout=timeout)
     except Exception as e:
         print(e)
         return None
```

## Comparing `pyiotown-0.4.3.dev3.dist-info/LICENSE` & `pyiotown-0.4.3.dev4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyiotown-0.4.3.dev3.dist-info/METADATA` & `pyiotown-0.4.3.dev4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiotown
-Version: 0.4.3.dev3
+Version: 0.4.3.dev4
 Summary: IoT.own Library
 Home-page: https://github.com/CoXlabInc/pyiotow
 Author: CoXlab Inc.
 Author-email: support@coxlab.kr
 Maintainer: Jongsoo Jeong
 Maintainer-email: jsjeong@coxlab.k
 License: MIT
```

## Comparing `pyiotown-0.4.3.dev3.dist-info/RECORD` & `pyiotown-0.4.3.dev4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyiotown/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyiotown/get.py,sha256=MmrV6EWNWC3Q3QtmEFVOgVuYr_Bv0sNllmjVQ2kfy14,3423
+pyiotown/get.py,sha256=025Eg17ZnS2VttWiaNgc-6lz1eaKRFsj5kz6hJxMh3U,3416
 pyiotown/post.py,sha256=qdeb2G74anHc8ceymjSSQ7ZnNpO1iQMFghbWYjbj2ms,3794
 pyiotown/post_process.py,sha256=-P0fhTASGbr4TK0om-haJb6Ucuatr-rJ_09FtUnK35U,6701
-pyiotown-0.4.3.dev3.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
-pyiotown-0.4.3.dev3.dist-info/METADATA,sha256=jS8HhEk52vUZGvyJMIowJ6k6245ZEJmC5ZEgPwStC7s,693
-pyiotown-0.4.3.dev3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pyiotown-0.4.3.dev3.dist-info/pbr.json,sha256=i_0VE7Lltirm31rJHlgQ1UuGdbFIMn3zy524VkLJ1hY,47
-pyiotown-0.4.3.dev3.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
-pyiotown-0.4.3.dev3.dist-info/RECORD,,
+pyiotown-0.4.3.dev4.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
+pyiotown-0.4.3.dev4.dist-info/METADATA,sha256=CBMxiF-MFHX456m0SEOubAsUt7LsP7ciiwnSHdihJXY,693
+pyiotown-0.4.3.dev4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyiotown-0.4.3.dev4.dist-info/pbr.json,sha256=M9svONdC0krLiqA-h9b3FX0XZ2sE3bwt0whGV68i-9A,47
+pyiotown-0.4.3.dev4.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
+pyiotown-0.4.3.dev4.dist-info/RECORD,,
```

