# Comparing `tmp/diskcache-5.6.0.tar.gz` & `tmp/diskcache-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diskcache-5.6.0.tar", last modified: Tue Apr 18 03:52:42 2023, max compression
+gzip compressed data, was "diskcache-5.6.1.tar", last modified: Tue Apr 18 05:53:26 2023, max compression
```

## Comparing `diskcache-5.6.0.tar` & `diskcache-5.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 03:51:55.000000 diskcache-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 03:51:55.000000 diskcache-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 03:52:42.413379 diskcache-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-04-18 03:51:55.000000 diskcache-5.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/diskcache/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/djangocache.py
--rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/diskcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:52:42.413379 diskcache-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 03:51:55.000000 diskcache-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    34169 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_deque.py
--rw-r--r--   0 runner    (1001) docker     (123)    43859 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_djangocache.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:53:26.637968 diskcache-5.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 05:52:37.000000 diskcache-5.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 05:52:37.000000 diskcache-5.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 05:53:26.637968 diskcache-5.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-04-18 05:52:37.000000 diskcache-5.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:53:26.637968 diskcache-5.6.1/diskcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81969 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/djangocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-18 05:52:37.000000 diskcache-5.6.1/diskcache/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:53:26.637968 diskcache-5.6.1/diskcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 05:53:26.000000 diskcache-5.6.1/diskcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 05:53:26.000000 diskcache-5.6.1/diskcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 05:53:26.000000 diskcache-5.6.1/diskcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 05:53:26.000000 diskcache-5.6.1/diskcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 05:53:26.637968 diskcache-5.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 05:52:37.000000 diskcache-5.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:53:26.637968 diskcache-5.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_deque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43859 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_djangocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 05:52:37.000000 diskcache-5.6.1/tests/test_recipes.py
```

### Comparing `diskcache-5.6.0/LICENSE` & `diskcache-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/PKG-INFO` & `diskcache-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.6.0
+Version: 5.6.1
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
```

### Comparing `diskcache-5.6.0/README.rst` & `diskcache-5.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/diskcache/__init__.py` & `diskcache-5.6.1/diskcache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 
     __all__.append('DjangoCache')
 except Exception:  # pylint: disable=broad-except  # pragma: no cover
     # Django not installed or not setup so ignore.
     pass
 
 __title__ = 'diskcache'
-__version__ = '5.6.0'
-__build__ = 0x050600
+__version__ = '5.6.1'
+__build__ = 0x050601
 __author__ = 'Grant Jenks'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2016-2023 Grant Jenks'
```

### Comparing `diskcache-5.6.0/diskcache/core.py` & `diskcache-5.6.1/diskcache/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,14 +429,15 @@
         try:
             assert issubclass(disk, Disk)
         except (TypeError, AssertionError):
             raise ValueError('disk must subclass diskcache.Disk') from None
 
         if directory is None:
             directory = tempfile.mkdtemp(prefix='diskcache-')
+        directory = str(directory)
         directory = op.expanduser(directory)
         directory = op.expandvars(directory)
 
         self._directory = directory
         self._timeout = 0  # Manually handle retries during initialization.
         self._local = threading.local()
         self._txn_id = None
```

### Comparing `diskcache-5.6.0/diskcache/djangocache.py` & `diskcache-5.6.1/diskcache/djangocache.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/diskcache/fanout.py` & `diskcache-5.6.1/diskcache/fanout.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         :param float timeout: SQLite connection timeout
         :param disk: `Disk` instance for serialization
         :param settings: any of `DEFAULT_SETTINGS`
 
         """
         if directory is None:
             directory = tempfile.mkdtemp(prefix='diskcache-')
+        directory = str(directory)
         directory = op.expanduser(directory)
         directory = op.expandvars(directory)
 
         default_size_limit = DEFAULT_SETTINGS['size_limit']
         size_limit = settings.pop('size_limit', default_size_limit) / shards
 
         self._count = shards
```

### Comparing `diskcache-5.6.0/diskcache/persistent.py` & `diskcache-5.6.1/diskcache/persistent.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/diskcache/recipes.py` & `diskcache-5.6.1/diskcache/recipes.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/diskcache.egg-info/PKG-INFO` & `diskcache-5.6.1/diskcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.6.0
+Version: 5.6.1
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
```

### Comparing `diskcache-5.6.0/setup.py` & `diskcache-5.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/tests/test_core.py` & `diskcache-5.6.1/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test diskcache.core.Cache."""
 
 import errno
 import hashlib
 import io
 import os
 import os.path as op
+import pathlib
 import pickle
 import shutil
 import sqlite3
 import subprocess as sp
 import tempfile
 import threading
 import time
@@ -33,14 +34,21 @@
     for key, value in dc.DEFAULT_SETTINGS.items():
         assert getattr(cache, key) == value
     cache.check()
     cache.close()
     cache.close()
 
 
+def test_init_path(cache):
+    path = pathlib.Path(cache.directory)
+    other = dc.Cache(path)
+    other.close()
+    assert cache.directory == other.directory
+
+
 def test_init_disk():
     with dc.Cache(disk_pickle_protocol=1, disk_min_file_size=2**20) as cache:
         key = (None, 0, 'abc')
         cache[key] = 0
         cache.check()
         assert cache.disk_min_file_size == 2**20
         assert cache.disk_pickle_protocol == 1
```

### Comparing `diskcache-5.6.0/tests/test_deque.py` & `diskcache-5.6.1/tests/test_deque.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/tests/test_djangocache.py` & `diskcache-5.6.1/tests/test_djangocache.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/tests/test_doctest.py` & `diskcache-5.6.1/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/tests/test_fanout.py` & `diskcache-5.6.1/tests/test_fanout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test diskcache.fanout.FanoutCache."""
 
 import collections as co
 import hashlib
 import io
 import os
 import os.path as op
+import pathlib
 import pickle
 import shutil
 import subprocess as sp
 import tempfile
 import threading
 import time
 import warnings
@@ -40,14 +41,21 @@
 
     for key, value in dc.DEFAULT_SETTINGS.items():
         setattr(cache, key, value)
 
     cache.check()
 
 
+def test_init_path(cache):
+    path = pathlib.Path(cache.directory)
+    other = dc.FanoutCache(path)
+    other.close()
+    assert cache.directory == other.directory
+
+
 def test_set_get_delete(cache):
     for value in range(100):
         cache.set(value, value)
 
     cache.check()
 
     for value in range(100):
```

### Comparing `diskcache-5.6.0/tests/test_index.py` & `diskcache-5.6.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.6.0/tests/test_recipes.py` & `diskcache-5.6.1/tests/test_recipes.py`

 * *Files identical despite different names*

