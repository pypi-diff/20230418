# Comparing `tmp/super_map-1.3.2.tar.gz` & `tmp/super_map-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_map-1.3.2.tar", last modified: Mon Nov 28 02:49:15 2022, max compression
+gzip compressed data, was "super_map-1.3.3.tar", last modified: Tue Apr 18 15:10:07 2023, max compression
```

## Comparing `super_map-1.3.2.tar` & `super_map-1.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:49:15.955130 super_map-1.3.2/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1023 2022-11-28 02:49:15.954989 super_map-1.3.2/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-28 02:49:15.955172 super_map-1.3.2/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1141 2022-10-21 14:25:16.000000 super_map-1.3.2/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:49:15.953934 super_map-1.3.2/super_map/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13136 2022-11-28 02:47:30.000000 super_map-1.3.2/super_map/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    16088 2022-10-21 14:25:16.000000 super_map-1.3.2/super_map/neo_map.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-28 02:49:15.954792 super_map-1.3.2/super_map.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1023 2022-11-28 02:49:15.000000 super_map-1.3.2/super_map.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      215 2022-11-28 02:49:15.000000 super_map-1.3.2/super_map.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-28 02:49:15.000000 super_map-1.3.2/super_map.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       16 2022-11-28 02:49:15.000000 super_map-1.3.2/super_map.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       10 2022-11-28 02:49:15.000000 super_map-1.3.2/super_map.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-18 15:10:07.974126 super_map-1.3.3/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1023 2023-04-18 15:10:07.973931 super_map-1.3.3/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-18 15:10:07.974173 super_map-1.3.3/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1141 2022-10-21 14:25:16.000000 super_map-1.3.3/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-18 15:10:07.972530 super_map-1.3.3/super_map/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    14527 2023-04-18 15:07:06.000000 super_map-1.3.3/super_map/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    16088 2022-10-21 14:25:16.000000 super_map-1.3.3/super_map/neo_map.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-18 15:10:07.973474 super_map-1.3.3/super_map.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1023 2023-04-18 15:10:07.000000 super_map-1.3.3/super_map.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      215 2023-04-18 15:10:07.000000 super_map-1.3.3/super_map.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-18 15:10:07.000000 super_map-1.3.3/super_map.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       16 2023-04-18 15:10:07.000000 super_map-1.3.3/super_map.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       10 2023-04-18 15:10:07.000000 super_map-1.3.3/super_map.egg-info/top_level.txt
```

### Comparing `super_map-1.3.2/PKG-INFO` & `super_map-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super_map
-Version: 1.3.2
+Version: 1.3.3
 Summary: Like dict, but easier
 Home-page: https://github.com/jeff-hykin/super_map.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `super_map-1.3.2/setup.py` & `super_map-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `super_map-1.3.2/super_map/__init__.py` & `super_map-1.3.3/super_map/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -289,14 +289,36 @@
                 # TODO: should probably be an error
                 pass
     
     def __json__(self):
         data, secrets = super().__getattribute__("d")
         return data
 
+def recursive_lazy_dict(value):
+    have_seen = set()
+    def _inner_recursive_lazy_dict(value):
+        # not perfect because there are other data structures, but its pretty useful
+        if isinstance(value, (set, list, dict)):
+            if id(value) in have_seen:
+                return value
+            else:
+                have_seen.add(id(value))
+                if isinstance(value, list):
+                    return [ _inner_recursive_lazy_dict(each) for each in value ]
+                elif isinstance(value, set):
+                    return set(_inner_recursive_lazy_dict(each) for each in value)
+                elif isinstance(value, dict):
+                    new_dict = LazyDict()
+                    for each_key, each_value in value.items():
+                        new_dict[each_key] = _inner_recursive_lazy_dict(each_value)
+                    return new_dict
+        else:
+            return value
+    return _inner_recursive_lazy_dict(value)
+
 defaulters = {}
 class LazyDict(dict):
     
     def __init__(self, *args, **kwargs):
         # default vaue
         super(LazyDict, self).__init__(*args, **kwargs)
         self.__dict__ = self
@@ -339,8 +361,22 @@
         if len(args) == 1:
             if callable(args[0]):
                 defaulters[id(self)] = args[0]
             else:
                 defaulters[id(self)] = lambda key: args[0]
             return self
         else:
-            return self.__dict__.setdefault(*args, **kwargs)
+            return super(LazyDict, self).setdefault(*args, **kwargs)
+    
+    def __copy__(self):
+        return LazyDict(self.__dict__)
+    
+    def __deepcopy__(self, memo):
+        from copy import deepcopy
+        
+        address = id(self)
+        if address in memo:
+            return memo[address]
+        new = memo[address] = LazyDict(self.__dict__)
+        for each_key, each_value in new.items():
+            new[each_key] = deepcopy(each_value, memo)
+        return new
```

### Comparing `super_map-1.3.2/super_map/neo_map.py` & `super_map-1.3.3/super_map/neo_map.py`

 * *Files identical despite different names*

### Comparing `super_map-1.3.2/super_map.egg-info/PKG-INFO` & `super_map-1.3.3/super_map.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-map
-Version: 1.3.2
+Version: 1.3.3
 Summary: Like dict, but easier
 Home-page: https://github.com/jeff-hykin/super_map.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

