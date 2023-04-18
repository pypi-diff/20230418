# Comparing `tmp/atools-0.9.1.tar.gz` & `tmp/atools-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atools-0.9.1.tar", last modified: Thu Dec 12 04:34:31 2019, max compression
+gzip compressed data, was "dist/atools-0.9.2.tar", last modified: Thu Dec 12 05:27:10 2019, max compression
```

## Comparing `atools-0.9.1.tar` & `atools-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 04:34:31.000000 atools-0.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10104 2019-12-12 04:34:31.000000 atools-0.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8165 2019-12-12 04:34:07.000000 atools-0.9.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 04:34:31.000000 atools-0.9.1/atools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4453 2019-12-12 04:34:07.000000 atools-0.9.1/atools/_rate_decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18055 2019-12-12 04:34:07.000000 atools-0.9.1/atools/_memoize_decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-12-12 04:34:07.000000 atools-0.9.1/atools/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10104 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-12-12 04:34:31.000000 atools-0.9.1/atools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-12-12 04:34:31.000000 atools-0.9.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 04:34:31.000000 atools-0.9.1/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2019-12-12 04:34:07.000000 atools-0.9.1/test/test_rate_decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16707 2019-12-12 04:34:07.000000 atools-0.9.1/test/test_memoize_decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2019-12-12 04:34:07.000000 atools-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 05:27:10.000000 atools-0.9.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10104 2019-12-12 05:27:10.000000 atools-0.9.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8165 2019-12-12 05:26:43.000000 atools-0.9.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 05:27:10.000000 atools-0.9.2/atools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-12-12 05:26:43.000000 atools-0.9.2/atools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18137 2019-12-12 05:26:43.000000 atools-0.9.2/atools/_memoize_decorator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4453 2019-12-12 05:26:43.000000 atools-0.9.2/atools/_rate_decorator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10104 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-12-12 05:27:10.000000 atools-0.9.2/atools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-12-12 05:27:10.000000 atools-0.9.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      444 2019-12-12 05:26:43.000000 atools-0.9.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-12 05:27:10.000000 atools-0.9.2/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16707 2019-12-12 05:26:43.000000 atools-0.9.2/test/test_memoize_decorator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2019-12-12 05:26:43.000000 atools-0.9.2/test/test_rate_decorator.py
```

### Comparing `atools-0.9.1/PKG-INFO` & `atools-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atools
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python 3.6+ async/sync memoize and rate decorators
 Home-page: https://github.com/cevans87/atools
 Author: cevans
 Author-email: c.d.evans87@gmail.com
 License: mit
 Description: [![Build Status](https://travis-ci.org/cevans87/atools.svg?branch=master&kill_cache=1)](https://travis-ci.org/cevans87/atools)
         [![Coverage Status](https://coveralls.io/repos/github/cevans87/atools/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/cevans87/atools?branch=master)
```

### Comparing `atools-0.9.1/README.md` & `atools-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `atools-0.9.1/atools/_rate_decorator.py` & `atools-0.9.2/atools/_rate_decorator.py`

 * *Files identical despite different names*

### Comparing `atools-0.9.1/atools/_memoize_decorator.py` & `atools-0.9.2/atools/_memoize_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from asyncio import Lock as AsyncLock
 from collections import ChainMap, OrderedDict
 from dataclasses import dataclass, field
 from datetime import timedelta
 from functools import partial, wraps
+from hashlib import sha256
 import inspect
 from pathlib import Path
 from sqlite3 import connect, Connection
 from textwrap import dedent
 from time import time
 from threading import Lock as SyncLock
 from typing import Any, Callable, Hashable, Mapping, Optional, Tuple, Type, Union
@@ -61,15 +62,15 @@
     expire_order: OrderedDict = field(init=False, default_factory=OrderedDict, hash=False)
     memos: OrderedDict = field(init=False, default_factory=OrderedDict, hash=False)
 
     def __post_init__(self) -> None:
         if self.db is not None:
             self.db.execute(dedent(f'''
                 CREATE TABLE IF NOT EXISTS `{self.table_name}` (
-                  k integer PRIMARY KEY,
+                  k TEXT PRIMARY KEY,
                   t FLOAT,
                   e FLOAT,
                   v TEXT NOT NULL
                 )
             '''))
             if self.duration:
                 self.db.execute(f"DELETE FROM `{self.table_name}` WHERE e < {time()}")
@@ -148,15 +149,15 @@
                 (self.memos[next(iter(self.expire_order))].expire_time < time())
         ):
             (k, _) = self.expire_order.popitem(last=False)
             self.memos.pop(k)
         elif self.size is not None and self.size < len(self.memos):
             (k, _) = self.memos.popitem(last=False)
         if (self.db is not None) and (k is not None):
-            self.db.execute(f"DELETE FROM `{self.table_name}` WHERE k = {k}")
+            self.db.execute(f"DELETE FROM `{self.table_name}` WHERE k = '{k}'")
             self.db.commit()
 
     def finalize_memo(self, memo: _Memo, key: int) -> Any:
         if memo.memo_return_state.raised:
             raise memo.memo_return_state.value
         else:
             if self.db is not None:
@@ -202,15 +203,15 @@
                 key = self.get_key(*args, **kwargs)
                 key = list(key)
                 for i, v in enumerate(key):
                     if inspect.isawaitable(v):
                         key[i] = await v
                 key = tuple(key)
 
-            key = hash(key)
+            key = sha256(str(key).encode()).hexdigest()
 
             memo: _AsyncMemo = self.get_memo(key)
 
             self.expire_one_memo()
 
             async with memo.async_lock:
                 if not memo.memo_return_state.called:
@@ -240,15 +241,15 @@
     def get_decorator(self) -> Callable:
         def decorator(*args, **kwargs):
             if self.get_key is None:
                 key = self.get_default_key(*args, **kwargs)
             else:
                 key = self.get_key(*args, **kwargs)
 
-            key = hash(key)
+            key = sha256(str(key).encode()).hexdigest()
 
             with self._sync_lock:
                 memo: _SyncMemo = self.get_memo(key)
 
             self.expire_one_memo()
 
             with memo.sync_lock:
```

### Comparing `atools-0.9.1/atools.egg-info/PKG-INFO` & `atools-0.9.2/atools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atools
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python 3.6+ async/sync memoize and rate decorators
 Home-page: https://github.com/cevans87/atools
 Author: cevans
 Author-email: c.d.evans87@gmail.com
 License: mit
 Description: [![Build Status](https://travis-ci.org/cevans87/atools.svg?branch=master&kill_cache=1)](https://travis-ci.org/cevans87/atools)
         [![Coverage Status](https://coveralls.io/repos/github/cevans87/atools/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/cevans87/atools?branch=master)
```

### Comparing `atools-0.9.1/test/test_rate_decorator.py` & `atools-0.9.2/test/test_rate_decorator.py`

 * *Files identical despite different names*

### Comparing `atools-0.9.1/test/test_memoize_decorator.py` & `atools-0.9.2/test/test_memoize_decorator.py`

 * *Files identical despite different names*

