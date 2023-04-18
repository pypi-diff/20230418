# Comparing `tmp/pybeef-0.0.5-py3-none-any.whl.zip` & `tmp/pybeef-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 6134 bytes, number of entries: 6
+Zip file size: 6844 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      350 b- defN 20-Feb-02 00:00 beef/__init__.py
--rw-r--r--  2.0 unx    11956 b- defN 20-Feb-02 00:00 beef/beef.py
-?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      441 b- defN 20-Feb-02 00:00 pybeef-0.0.5.dist-info/RECORD
-6 files, 16419 bytes uncompressed, 5346 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    11944 b- defN 20-Feb-02 00:00 beef/beef.py
+-rw-r--r--  2.0 unx     1825 b- defN 20-Feb-02 00:00 beef/pool.py
+?rw-r--r--  2.0 unx     2515 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 pybeef-0.0.6.dist-info/RECORD
+7 files, 18301 bytes uncompressed, 5956 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: beef/__init__.py
 Comment: 
 
 Filename: beef/beef.py
 Comment: 
 
-Filename: pybeef-0.0.5.dist-info/METADATA
+Filename: beef/pool.py
 Comment: 
 
-Filename: pybeef-0.0.5.dist-info/WHEEL
+Filename: pybeef-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pybeef-0.0.5.dist-info/licenses/LICENSE
+Filename: pybeef-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pybeef-0.0.5.dist-info/RECORD
+Filename: pybeef-0.0.6.dist-info/licenses/LICENSE
+Comment: 
+
+Filename: pybeef-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beef/beef.py

```diff
@@ -4,14 +4,15 @@
 import uuid
 from enum import Enum
 import inspect
 import json
 from typing import Callable, Awaitable, Any, Optional, NoReturn, Tuple, List, Dict
 import aio_pika
 import aiormq
+from .pool import Pool
 
 AsyncFunction = Callable[..., Awaitable[Any]]
 TaskID = str
 
 class TaskNotFoundError(RuntimeError):
     pass
 
@@ -240,21 +241,21 @@
                     finally:
                         self._task_id.set(None)
 
                     await self._set_status(channel, status)
                     await msg.ack()
 
     @contextlib.asynccontextmanager
-    async def connect(self, url: str, max_channels=10) -> aio_pika.pool.Pool:
+    async def connect(self, url: str, max_channels=10) -> Pool:
         '''
         Opens a (single) connection to AMQP server at :url: and creates a pool of channels
         '''
         connection = await aio_pika.connect_robust(url)
         async with connection:
-            pool = aio_pika.pool.Pool(connection.channel, max_size=max_channels)
+            pool = Pool(connection, max_items=max_channels)
             async with pool:
                 self._pool.set(pool)
                 try:
                     yield pool
                 finally:
                     self._pool.set(None)
```

## Comparing `pybeef-0.0.5.dist-info/METADATA` & `pybeef-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeef
-Version: 0.0.5
+Version: 0.0.6
 Summary: Opinionated distributed RPC using AMQP workers
 Project-URL: Homepage, https://github.com/innodatalabs/beef
 Project-URL: Bug Tracker, https://github.com/pypa/innodatalabs/beef
 Author-email: Mike Kroutikov <mkroutikov@innodata.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pybeef-0.0.5.dist-info/licenses/LICENSE` & `pybeef-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

