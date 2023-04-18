# Comparing `tmp/diskcache-5.5.1.tar.gz` & `tmp/diskcache-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diskcache-5.5.1.tar", last modified: Tue Apr 11 06:56:24 2023, max compression
+gzip compressed data, was "diskcache-5.6.0.tar", last modified: Tue Apr 18 03:52:42 2023, max compression
```

## Comparing `diskcache-5.5.1.tar` & `diskcache-5.6.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 06:54:26.000000 diskcache-5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 06:54:26.000000 diskcache-5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-11 06:56:24.908393 diskcache-5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-04-11 06:54:26.000000 diskcache-5.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/diskcache/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/djangocache.py
--rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)    33159 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/diskcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:56:24.908393 diskcache-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 06:54:26.000000 diskcache-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 03:51:55.000000 diskcache-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 03:51:55.000000 diskcache-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 03:52:42.413379 diskcache-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-04-18 03:51:55.000000 diskcache-5.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/diskcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/djangocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-18 03:51:55.000000 diskcache-5.6.0/diskcache/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/diskcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 03:52:42.000000 diskcache-5.6.0/diskcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:52:42.413379 diskcache-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 03:51:55.000000 diskcache-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:52:42.413379 diskcache-5.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    34169 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_deque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43859 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_djangocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 03:51:55.000000 diskcache-5.6.0/tests/test_recipes.py
```

### Comparing `diskcache-5.5.1/LICENSE` & `diskcache-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diskcache-5.5.1/PKG-INFO` & `diskcache-5.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.5.1
+Version: 5.6.0
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
```

### Comparing `diskcache-5.5.1/README.rst` & `diskcache-5.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `diskcache-5.5.1/diskcache/__init__.py` & `diskcache-5.6.0/diskcache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 
     __all__.append('DjangoCache')
 except Exception:  # pylint: disable=broad-except  # pragma: no cover
     # Django not installed or not setup so ignore.
     pass
 
 __title__ = 'diskcache'
-__version__ = '5.5.1'
-__build__ = 0x050501
+__version__ = '5.6.0'
+__build__ = 0x050600
 __author__ = 'Grant Jenks'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2016-2023 Grant Jenks'
```

### Comparing `diskcache-5.5.1/diskcache/core.py` & `diskcache-5.6.0/diskcache/core.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.5.1/diskcache/djangocache.py` & `diskcache-5.6.0/diskcache/djangocache.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,23 @@
 
         :param str name: subdirectory name for Cache
         :return: Cache with given name
 
         """
         return self._cache.cache(name)
 
-    def deque(self, name):
+    def deque(self, name, maxlen=None):
         """Return Deque with given `name` in subdirectory.
 
         :param str name: subdirectory name for Deque
+        :param maxlen: max length (default None, no max)
         :return: Deque with given name
 
         """
-        return self._cache.deque(name)
+        return self._cache.deque(name, maxlen=maxlen)
 
     def index(self, name):
         """Return Index with given `name` in subdirectory.
 
         :param str name: subdirectory name for Index
         :return: Index with given name
```

### Comparing `diskcache-5.5.1/diskcache/fanout.py` & `diskcache-5.6.0/diskcache/fanout.py`

 * *Files 2% similar despite different names*

```diff
@@ -608,28 +608,29 @@
                 timeout=timeout,
                 disk=self._disk if disk is None else Disk,
                 **settings,
             )
             _caches[name] = temp
             return temp
 
-    def deque(self, name):
+    def deque(self, name, maxlen=None):
         """Return Deque with given `name` in subdirectory.
 
         >>> cache = FanoutCache()
         >>> deque = cache.deque('test')
         >>> deque.extend('abc')
         >>> deque.popleft()
         'a'
         >>> deque.pop()
         'c'
         >>> len(deque)
         1
 
         :param str name: subdirectory name for Deque
+        :param maxlen: max length (default None, no max)
         :return: Deque with given name
 
         """
         _deques = self._deques
 
         try:
             return _deques[name]
@@ -637,15 +638,15 @@
             parts = name.split('/')
             directory = op.join(self._directory, 'deque', *parts)
             cache = Cache(
                 directory=directory,
                 disk=self._disk,
                 eviction_policy='none',
             )
-            deque = Deque.fromcache(cache)
+            deque = Deque.fromcache(cache, maxlen=maxlen)
             _deques[name] = deque
             return deque
 
     def index(self, name):
         """Return Index with given `name` in subdirectory.
 
         >>> cache = FanoutCache()
```

### Comparing `diskcache-5.5.1/diskcache/persistent.py` & `diskcache-5.6.0/diskcache/persistent.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,29 +71,30 @@
     -4
     >>> deque.reverse()
     >>> list(deque)
     [3, 2, 1, 0, 0, -1, -2, -3]
 
     """
 
-    def __init__(self, iterable=(), directory=None):
+    def __init__(self, iterable=(), directory=None, maxlen=None):
         """Initialize deque instance.
 
         If directory is None then temporary directory created. The directory
         will *not* be automatically removed.
 
         :param iterable: iterable of items to append to deque
         :param directory: deque directory (default None)
 
         """
         self._cache = Cache(directory, eviction_policy='none')
-        self.extend(iterable)
+        self._maxlen = float('inf') if maxlen is None else maxlen
+        self._extend(iterable)
 
     @classmethod
-    def fromcache(cls, cache, iterable=()):
+    def fromcache(cls, cache, iterable=(), maxlen=None):
         """Initialize deque using `cache`.
 
         >>> cache = Cache()
         >>> deque = Deque.fromcache(cache, [5, 6, 7, 8])
         >>> deque.cache is cache
         True
         >>> len(deque)
@@ -107,27 +108,53 @@
         :param iterable: iterable of items
         :return: initialized Deque
 
         """
         # pylint: disable=no-member,protected-access
         self = cls.__new__(cls)
         self._cache = cache
-        self.extend(iterable)
+        self._maxlen = float('inf') if maxlen is None else maxlen
+        self._extend(iterable)
         return self
 
     @property
     def cache(self):
         """Cache used by deque."""
         return self._cache
 
     @property
     def directory(self):
         """Directory path where deque is stored."""
         return self._cache.directory
 
+    @property
+    def maxlen(self):
+        """Max length of the deque."""
+        return self._maxlen
+
+    @maxlen.setter
+    def maxlen(self, value):
+        """Set max length of the deque.
+
+        Pops items from left while length greater than max.
+
+        >>> deque = Deque()
+        >>> deque.extendleft('abcde')
+        >>> deque.maxlen = 3
+        >>> list(deque)
+        ['c', 'd', 'e']
+
+        :param value: max length
+
+        """
+        self._maxlen = value
+        with self._cache.transact(retry=True):
+            while len(self._cache) > self._maxlen:
+                self._popleft()
+
     def _index(self, index, func):
         len_self = len(self)
 
         if index >= 0:
             if index >= len_self:
                 raise IndexError('deque index out of range')
 
@@ -240,15 +267,15 @@
 
         Extend back side of deque with items from iterable.
 
         :param iterable: iterable of items to append to deque
         :return: deque with added items
 
         """
-        self.extend(iterable)
+        self._extend(iterable)
         return self
 
     def __iter__(self):
         """deque.__iter__() <==> iter(deque)
 
         Return iterator of deque from front to back.
 
@@ -288,62 +315,80 @@
         for key in _cache.iterkeys(reverse=True):
             try:
                 yield _cache[key]
             except KeyError:
                 pass
 
     def __getstate__(self):
-        return self.directory
+        return self.directory, self.maxlen
 
     def __setstate__(self, state):
-        self.__init__(directory=state)
+        directory, maxlen = state
+        self.__init__(directory=directory, maxlen=maxlen)
 
     def append(self, value):
         """Add `value` to back of deque.
 
         >>> deque = Deque()
         >>> deque.append('a')
         >>> deque.append('b')
         >>> deque.append('c')
         >>> list(deque)
         ['a', 'b', 'c']
 
         :param value: value to add to back of deque
 
         """
-        self._cache.push(value, retry=True)
+        with self._cache.transact(retry=True):
+            self._cache.push(value, retry=True)
+            if len(self._cache) > self._maxlen:
+                self._popleft()
+
+    _append = append
 
     def appendleft(self, value):
         """Add `value` to front of deque.
 
         >>> deque = Deque()
         >>> deque.appendleft('a')
         >>> deque.appendleft('b')
         >>> deque.appendleft('c')
         >>> list(deque)
         ['c', 'b', 'a']
 
         :param value: value to add to front of deque
 
         """
-        self._cache.push(value, side='front', retry=True)
+        with self._cache.transact(retry=True):
+            self._cache.push(value, side='front', retry=True)
+            if len(self._cache) > self._maxlen:
+                self._pop()
+
+    _appendleft = appendleft
 
     def clear(self):
         """Remove all elements from deque.
 
         >>> deque = Deque('abc')
         >>> len(deque)
         3
         >>> deque.clear()
         >>> list(deque)
         []
 
         """
         self._cache.clear(retry=True)
 
+    _clear = clear
+
+    def copy(self):
+        """Copy deque with same directory and max length."""
+        TypeSelf = type(self)
+        return TypeSelf(directory=self.directory, maxlen=self.maxlen)
+
     def count(self, value):
         """Return number of occurrences of `value` in deque.
 
         >>> deque = Deque()
         >>> deque += [num for num in range(1, 5) for _ in range(num)]
         >>> deque.count(0)
         0
@@ -361,29 +406,31 @@
     def extend(self, iterable):
         """Extend back side of deque with values from `iterable`.
 
         :param iterable: iterable of values
 
         """
         for value in iterable:
-            self.append(value)
+            self._append(value)
+
+    _extend = extend
 
     def extendleft(self, iterable):
         """Extend front side of deque with value from `iterable`.
 
         >>> deque = Deque()
         >>> deque.extendleft('abc')
         >>> list(deque)
         ['c', 'b', 'a']
 
         :param iterable: iterable of values
 
         """
         for value in iterable:
-            self.appendleft(value)
+            self._appendleft(value)
 
     def peek(self):
         """Peek at value at back of deque.
 
         Faster than indexing deque at -1.
 
         If deque is empty then raise IndexError.
@@ -455,14 +502,16 @@
         """
         default = None, ENOVAL
         _, value = self._cache.pull(default=default, side='back', retry=True)
         if value is ENOVAL:
             raise IndexError('pop from an empty deque')
         return value
 
+    _pop = pop
+
     def popleft(self):
         """Remove and return value at front of deque.
 
         >>> deque = Deque()
         >>> deque += 'ab'
         >>> deque.popleft()
         'a'
@@ -479,14 +528,16 @@
         """
         default = None, ENOVAL
         _, value = self._cache.pull(default=default, retry=True)
         if value is ENOVAL:
             raise IndexError('pop from an empty deque')
         return value
 
+    _popleft = popleft
+
     def remove(self, value):
         """Remove first occurrence of `value` in deque.
 
         >>> deque = Deque()
         >>> deque += 'aab'
         >>> deque.remove('a')
         >>> list(deque)
@@ -526,23 +577,25 @@
         >>> deque = Deque()
         >>> deque += 'abc'
         >>> deque.reverse()
         >>> list(deque)
         ['c', 'b', 'a']
 
         """
+        # pylint: disable=protected-access
         # GrantJ 2019-03-22 Consider using an algorithm that swaps the values
         # at two keys. Like self._cache.swap(key1, key2, retry=True) The swap
         # method would exchange the values at two given keys. Then, using a
-        # forward iterator and a reverse iterator, the reversis method could
+        # forward iterator and a reverse iterator, the reverse method could
         # avoid making copies of the values.
         temp = Deque(iterable=reversed(self))
-        self.clear()
-        self.extend(temp)
+        self._clear()
+        self._extend(temp)
         directory = temp.directory
+        temp._cache.close()
         del temp
         rmtree(directory)
 
     def rotate(self, steps=1):
         """Rotate deque right by `steps`.
 
         If steps is negative then rotate left.
@@ -569,30 +622,30 @@
             return
 
         if steps >= 0:
             steps %= len_self
 
             for _ in range(steps):
                 try:
-                    value = self.pop()
+                    value = self._pop()
                 except IndexError:
                     return
                 else:
-                    self.appendleft(value)
+                    self._appendleft(value)
         else:
             steps *= -1
             steps %= len_self
 
             for _ in range(steps):
                 try:
-                    value = self.popleft()
+                    value = self._popleft()
                 except IndexError:
                     return
                 else:
-                    self.append(value)
+                    self._append(value)
 
     __hash__ = None  # type: ignore
 
     @contextmanager
     def transact(self):
         """Context manager to perform a transaction by locking the deque.
 
@@ -663,15 +716,17 @@
             directory = args[0]
             args = args[1:]
         else:
             if args and args[0] is None:
                 args = args[1:]
             directory = None
         self._cache = Cache(directory, eviction_policy='none')
-        self.update(*args, **kwargs)
+        self._update(*args, **kwargs)
+
+    _update = MutableMapping.update
 
     @classmethod
     def fromcache(cls, cache, *args, **kwargs):
         """Initialize index using `cache` and update items.
 
         >>> cache = Cache()
         >>> index = Index.fromcache(cache, {'a': 1, 'b': 2, 'c': 3})
@@ -689,15 +744,15 @@
         :param kwargs: mapping of items
         :return: initialized Index
 
         """
         # pylint: disable=no-member,protected-access
         self = cls.__new__(cls)
         self._cache = cache
-        self.update(*args, **kwargs)
+        self._update(*args, **kwargs)
         return self
 
     @property
     def cache(self):
         """Cache used by index."""
         return self._cache
```

### Comparing `diskcache-5.5.1/diskcache/recipes.py` & `diskcache-5.6.0/diskcache/recipes.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.5.1/diskcache.egg-info/PKG-INFO` & `diskcache-5.6.0/diskcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.5.1
+Version: 5.6.0
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
```

### Comparing `diskcache-5.5.1/setup.py` & `diskcache-5.6.0/setup.py`

 * *Files identical despite different names*

