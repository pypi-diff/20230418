# Comparing `tmp/Mongo-Thingy-0.9.1.tar.gz` & `tmp/Mongo-Thingy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Mongo-Thingy-0.9.1.tar", last modified: Wed Nov  8 17:09:36 2017, max compression
+gzip compressed data, was "dist/Mongo-Thingy-0.9.2.tar", last modified: Wed Nov 15 10:26:32 2017, max compression
```

## Comparing `Mongo-Thingy-0.9.1.tar` & `Mongo-Thingy-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      898 2017-11-08 17:09:04.000000 Mongo-Thingy-0.9.1/setup.py
-drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)       27 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/requires.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2017-04-20 16:38:00.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/not-zip-safe
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     7745 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/PKG-INFO
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)       13 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/top_level.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      317 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/SOURCES.txt
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/dependency_links.txt
-drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/mongo_thingy/
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2626 2017-10-18 13:19:41.000000 Mongo-Thingy-0.9.1/mongo_thingy/versioned.py
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     4103 2017-11-08 14:35:48.000000 Mongo-Thingy-0.9.1/mongo_thingy/__init__.py
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     1041 2017-10-18 13:19:41.000000 Mongo-Thingy-0.9.1/mongo_thingy/cursor.py
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     5345 2017-11-02 20:26:11.000000 Mongo-Thingy-0.9.1/README.rst
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)     7745 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/PKG-INFO
--rw-r--r--   0 ramnes    (1000) ramnes    (1001)      184 2017-11-08 17:09:36.000000 Mongo-Thingy-0.9.1/setup.cfg
+drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      898 2017-11-15 10:25:30.000000 Mongo-Thingy-0.9.2/setup.py
+drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)       27 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/requires.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2017-04-20 16:38:00.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/not-zip-safe
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     7745 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/PKG-INFO
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)       13 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/top_level.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      317 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/SOURCES.txt
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)        1 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/dependency_links.txt
+drwxr-xr-x   0 ramnes    (1000) ramnes    (1001)        0 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/mongo_thingy/
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     2626 2017-10-18 13:19:41.000000 Mongo-Thingy-0.9.2/mongo_thingy/versioned.py
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     4118 2017-11-15 10:24:14.000000 Mongo-Thingy-0.9.2/mongo_thingy/__init__.py
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     1041 2017-10-18 13:19:41.000000 Mongo-Thingy-0.9.2/mongo_thingy/cursor.py
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     5345 2017-11-02 20:26:11.000000 Mongo-Thingy-0.9.2/README.rst
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)     7745 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/PKG-INFO
+-rw-r--r--   0 ramnes    (1000) ramnes    (1001)      184 2017-11-15 10:26:32.000000 Mongo-Thingy-0.9.2/setup.cfg
```

### Comparing `Mongo-Thingy-0.9.1/setup.py` & `Mongo-Thingy-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_description():
     with open("README.rst") as file:
         return file.read()
 
 
 setup(
     name="Mongo-Thingy",
-    version="0.9.1",
+    version="0.9.2",
     url="https://github.com/numberly/mongo-thingy",
     license="MIT",
     author="Guillaume Gelin",
     author_email="ramnes@1000mercis.com",
     description=("The most Pythonic and friendly-yet-powerful way to use "
                  "MongoDB"),
     long_description=get_description(),
```

### Comparing `Mongo-Thingy-0.9.1/Mongo_Thingy.egg-info/PKG-INFO` & `Mongo-Thingy-0.9.2/Mongo_Thingy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Mongo-Thingy
-Version: 0.9.1
+Version: 0.9.2
 Summary: The most Pythonic and friendly-yet-powerful way to use MongoDB
 Home-page: https://github.com/numberly/mongo-thingy
 Author: Guillaume Gelin
 Author-email: ramnes@1000mercis.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: .. _Thingy: https://github.com/numberly/thingy
```

### Comparing `Mongo-Thingy-0.9.1/mongo_thingy/versioned.py` & `Mongo-Thingy-0.9.2/mongo_thingy/versioned.py`

 * *Files identical despite different names*

### Comparing `Mongo-Thingy-0.9.1/mongo_thingy/__init__.py` & `Mongo-Thingy-0.9.2/mongo_thingy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         kwargs.setdefault("background", True)
         if not hasattr(cls, "_indexes"):
             cls._indexes = []
         cls._indexes.append((keys, kwargs))
 
     @classmethod
     def count(cls, *args, **kwargs):
-        return cls.collection.count()
+        return cls.collection.count(*args, **kwargs)
 
     @classmethod
     def connect(cls, *args, **kwargs):
         cls._client = MongoClient(*args, **kwargs)
         try:
             cls._database = cls._client.get_default_database()
         except ConfigurationError:
```

### Comparing `Mongo-Thingy-0.9.1/mongo_thingy/cursor.py` & `Mongo-Thingy-0.9.2/mongo_thingy/cursor.py`

 * *Files identical despite different names*

### Comparing `Mongo-Thingy-0.9.1/README.rst` & `Mongo-Thingy-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `Mongo-Thingy-0.9.1/PKG-INFO` & `Mongo-Thingy-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Mongo-Thingy
-Version: 0.9.1
+Version: 0.9.2
 Summary: The most Pythonic and friendly-yet-powerful way to use MongoDB
 Home-page: https://github.com/numberly/mongo-thingy
 Author: Guillaume Gelin
 Author-email: ramnes@1000mercis.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: .. _Thingy: https://github.com/numberly/thingy
```

