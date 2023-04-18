# Comparing `tmp/cbcmgr-1.1.8.tar.gz` & `tmp/cbcmgr-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.1.8.tar", last modified: Thu Mar  2 16:48:21 2023, max compression
+gzip compressed data, was "cbcmgr-1.1.9.tar", last modified: Tue Apr 18 19:33:05 2023, max compression
```

## Comparing `cbcmgr-1.1.8.tar` & `cbcmgr-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-03-02 16:48:21.792037 cbcmgr-1.1.8/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.1.8/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-03-02 16:48:21.791917 cbcmgr-1.1.8/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.1.8/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-03-02 16:48:21.790994 cbcmgr-1.1.8/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.1.8/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     9821 2023-03-02 16:45:07.000000 cbcmgr-1.1.8/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19191 2023-03-01 22:58:54.000000 cbcmgr-1.1.8/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-01 15:30:36.000000 cbcmgr-1.1.8/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4051 2023-02-14 15:09:46.000000 cbcmgr-1.1.8/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    10675 2023-02-22 16:29:09.000000 cbcmgr-1.1.8/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.1.8/cbcmgr/retry.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-03-02 16:48:21.791735 cbcmgr-1.1.8/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-03-02 16:48:21.000000 cbcmgr-1.1.8/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      326 2023-03-02 16:48:21.000000 cbcmgr-1.1.8/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-03-02 16:48:21.000000 cbcmgr-1.1.8/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-03-02 16:48:21.000000 cbcmgr-1.1.8/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-03-02 16:48:21.000000 cbcmgr-1.1.8/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-03-02 16:48:21.792085 cbcmgr-1.1.8/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-03-02 16:48:16.000000 cbcmgr-1.1.8/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.734414 cbcmgr-1.1.9/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-04-18 19:33:05.734233 cbcmgr-1.1.9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.1.9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.672721 cbcmgr-1.1.9/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.1.9/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.1.9/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.1.9/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     4051 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    10675 2023-02-22 16:29:09.000000 cbcmgr-1.1.9/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.1.9/cbcmgr/retry.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.733841 cbcmgr-1.1.9/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      326 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-18 19:33:05.734485 cbcmgr-1.1.9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-04-18 19:15:38.000000 cbcmgr-1.1.9/setup.py
```

### Comparing `cbcmgr-1.1.8/LICENSE.txt` & `cbcmgr-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/PKG-INFO` & `cbcmgr-1.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.1.8
+Version: 1.1.9
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.1.8/README.md` & `cbcmgr-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/cbcmgr/cb_connect.py` & `cbcmgr-1.1.9/cbcmgr/cb_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,21 @@
         qim = self._cluster.query_indexes()
         try:
             index_options = DropPrimaryQueryIndexOptions(timeout=timedelta(seconds=timeout), collection_name=self._collection.name, scope_name=self._scope.name)
             qim.drop_primary_index(self._bucket.name, index_options)
         except QueryIndexNotFoundException:
             pass
 
+    def cb_doc_exists(self, doc_id: str):
+        result = self._collection.exists(doc_id)
+        if result.exists:
+            return True
+        else:
+            return False
+
     @retry()
     def cb_get(self, key: Union[int, str]):
         try:
             document_id = self.construct_key(key)
             result = self._collection.get(document_id)
             self.logger.debug(f"cb_get: {document_id}: cas {result.cas}")
             return result.content_as[dict]
```

### Comparing `cbcmgr-1.1.8/cbcmgr/cb_management.py` & `cbcmgr-1.1.9/cbcmgr/cb_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError)
 from .retry import retry, retry_inline
 from .cb_connect import CBConnect
 from datetime import timedelta
 import attr
 import hashlib
 from attr.validators import instance_of as io, optional
-from typing import Protocol, Iterable
+from typing import Protocol, Iterable, Optional
 from couchbase.cluster import Cluster
 from couchbase.options import QueryOptions
 from couchbase.diagnostics import ServiceType, PingState
-from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend
+from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend, BucketSettings
 from couchbase.management.collections import CollectionSpec
 from couchbase.exceptions import (QueryIndexNotFoundException, QueryIndexAlreadyExistsException, BucketAlreadyExistsException, BucketNotFoundException, BucketDoesNotExistException,
                                   WatchQueryIndexTimeoutException, ScopeAlreadyExistsException, CollectionAlreadyExistsException, CollectionNotFoundException)
 from couchbase.management.queries import (CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions, WatchQueryIndexOptions, DropPrimaryQueryIndexOptions, DropQueryIndexOptions)
 from couchbase.management.options import CreateBucketOptions, CreateScopeOptions, CreateCollectionOptions, GetAllQueryIndexOptions
 from couchbase.options import WaitUntilReadyOptions
 
@@ -96,14 +96,21 @@
                 cm = self._bucket.collections()
                 cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=25)))
                 retry_inline(self.get_collection, cm, name)
         except CollectionAlreadyExistsException:
             pass
         self.collection(name)
 
+    def get_bucket(self, name: str) -> Optional[BucketSettings]:
+        try:
+            bm = self._cluster.buckets()
+            return bm.get_bucket(name)
+        except BucketDoesNotExistException:
+            return None
+
     @staticmethod
     def get_scope(cm, scope_name):
         return next((s for s in cm.get_all_scopes() if s.name == scope_name), None)
 
     def get_collection(self, cm, collection_name):
         collection = None
         scope = self.get_scope(cm, self._scope.name)
```

### Comparing `cbcmgr-1.1.8/cbcmgr/cb_session.py` & `cbcmgr-1.1.9/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/cbcmgr/exceptions.py` & `cbcmgr-1.1.9/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.1.9/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/cbcmgr/retry.py` & `cbcmgr-1.1.9/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.8/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.1.9/cbcmgr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.1.8
+Version: 1.1.9
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.1.8/setup.py` & `cbcmgr-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.1.8',
+    version='1.1.9',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

