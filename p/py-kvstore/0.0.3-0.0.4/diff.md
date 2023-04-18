# Comparing `tmp/py_kvstore-0.0.3.tar.gz` & `tmp/py_kvstore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_kvstore-0.0.3.tar", last modified: Tue Apr 18 03:44:54 2023, max compression
+gzip compressed data, was "py_kvstore-0.0.4.tar", last modified: Tue Apr 18 05:44:11 2023, max compression
```

## Comparing `py_kvstore-0.0.3.tar` & `py_kvstore-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 03:44:54.929714 py_kvstore-0.0.3/
--rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 03:44:54.929714 py_kvstore-0.0.3/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)       13 2023-04-18 03:31:33.000000 py_kvstore-0.0.3/README.md
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 03:44:54.929714 py_kvstore-0.0.3/py_kvstore/
--rw-r--r--   0 reece     (1000) reece     (1001)       73 2023-04-18 03:40:57.000000 py_kvstore-0.0.3/py_kvstore/__init__.py
--rw-r--r--   0 reece     (1000) reece     (1001)     5076 2023-04-18 03:31:33.000000 py_kvstore-0.0.3/py_kvstore/py_kvstore.py
--rw-r--r--   0 reece     (1000) reece     (1001)     1753 2023-04-18 03:31:33.000000 py_kvstore-0.0.3/py_kvstore/test.py
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 03:44:54.929714 py_kvstore-0.0.3/py_kvstore.egg-info/
--rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 03:44:54.000000 py_kvstore-0.0.3/py_kvstore.egg-info/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-18 03:44:54.000000 py_kvstore-0.0.3/py_kvstore.egg-info/SOURCES.txt
--rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-18 03:44:54.000000 py_kvstore-0.0.3/py_kvstore.egg-info/dependency_links.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-18 03:44:54.000000 py_kvstore-0.0.3/py_kvstore.egg-info/top_level.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-18 03:44:54.929714 py_kvstore-0.0.3/setup.cfg
--rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-18 03:44:50.000000 py_kvstore-0.0.3/setup.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/
+-rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)       13 2023-04-18 03:31:33.000000 py_kvstore-0.0.4/README.md
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/py_kvstore/
+-rw-r--r--   0 reece     (1000) reece     (1001)       78 2023-04-18 04:17:04.000000 py_kvstore-0.0.4/py_kvstore/__init__.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     6528 2023-04-18 05:41:02.000000 py_kvstore-0.0.4/py_kvstore/py_kvstore.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     1840 2023-04-18 04:20:33.000000 py_kvstore-0.0.4/py_kvstore/test.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/py_kvstore.egg-info/
+-rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/SOURCES.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/dependency_links.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/top_level.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/setup.cfg
+-rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-18 05:44:09.000000 py_kvstore-0.0.4/setup.py
```

### Comparing `py_kvstore-0.0.3/PKG-INFO` & `py_kvstore-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_kvstore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `py_kvstore-0.0.3/py_kvstore/py_kvstore.py` & `py_kvstore-0.0.4/py_kvstore/py_kvstore.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,21 @@
         return {"value": self.value, "timeout": self.timeout}
 
     @staticmethod
     def fromJSON(json: dict):
         return Pair(json["value"], json["timeout"])
 
 
-class KV:
+@dataclass
+class HashSet(Pair):
+    value: dict[str, Any]
+    timeout: int
+
+
+class KVStore:
     # TODO: Specify in memory or on the disk (slower, but better for large data sets)
     def __init__(self, name: Optional[str] = None, dump_dir=None):
         self.name = name
         self.store: dict[str, Pair] = {}
 
         self.dump_dir = current_dir
         if dump_dir is not None:
@@ -50,108 +56,150 @@
             return
 
         if timeout > 0:
             timeout += int(time.time())
 
         self.store[key] = Pair(value, timeout)
 
-    def incr(self, key: str, value: int = 1) -> int:
+    # hash set and hash get
+    # You can only set the expire time on creation?
+    def hset(self, key: str, field: str, value: Any, timeout: int = -1):
+        self.delete_expired_data_if_applicable(key)
+
+        if key not in self.store:
+            # timeout can only be set on creation
+            self.store[key] = HashSet({}, timeout)
+
+        # grab the current hset
+        hset = self.store[key].value
+        hset[field] = value
+        # reset the store value
+        self.store[key].value = hset
+
+    def hset_expire(self, key: str, timeout: int = -1):
+        if key not in self.store:
+            raise Exception(f"Key {key} does not exist")
+
+        self.store[key].timeout = timeout
+
+    def hget(self, key: str, field: str) -> Any | None:
+        self.delete_expired_data_if_applicable(key)
+        if key not in self.store:
+            return None
+
+        if field not in self.store[key].value:
+            return None
+
+        return self.store[key].value[field]
+
+    def incr(self, key: str, amount: int = 1) -> int:
         """Returns the new value"""
         if key not in self.store:
-            self.set(key, value)
-            return value
+            self.set(key, amount)
+            return amount
 
         # what if key value is not an int?
         if not isinstance(self.store[key].value, int):
             raise Exception(f"key:{key}'s value is not an int")
 
-        self.store[key].value += value
+        self.store[key].value += amount
         return self.store[key].value
 
     def get(self, key) -> Any | None:
         self.delete_expired_data_if_applicable(key)
 
         if key in self.store:
             return self.store[key].value
         return None
 
     def get_keys(self, search_regex: str = "") -> list[str]:
+        search_regex = search_regex.replace("*", ".+")
         self.delete_all_expired_data()
         if len(search_regex) == 0:
             return list(self.store.keys())
         else:
             return [k for k in self.store.keys() if regex.match(search_regex, k)]
 
-    def delete(self, key) -> bool:
-        if key in self.store:
-            del self.store[key]
-            return True
-        return False
+    def delete(self, *keys) -> bool:
+        for key in keys:
+            if key in self.store:
+                del self.store[key]
+            else:
+                return False
+        return True
+
+    def clear(self):
+        self.store = {}
 
     def ttl(self, key) -> int:
         self.delete_expired_data_if_applicable(key)
         if key in self.store:
             p = self.store[key]
             return p.timeout
         return -2
 
     def dbg(self):
         self.delete_all_expired_data()
-        print("dbg", self.store)
+        print("dbg", self.name, self.dump_dir, self.store)
 
     def delete_all_expired_data(self):
         current_time = int(time.time())
         self.store = {
             k: v
             for k, v in self.store.items()
             if v.timeout >= current_time or v.timeout == -1
         }
 
-    def delete_expired_data_if_applicable(self, key: str):
+    def delete_expired_data_if_applicable(self, key: str) -> bool:
         if key in self.store:
             timeout = self.store[key].timeout
             if timeout >= 0 and timeout < int(time.time()):
                 del self.store[key]
+                return True
+        return False
 
     def dump(self):
         file = os.path.join(self.dump_dir, f"{self.name}.json")
+        # print("Dumping to file", file)
 
         with open(file, "w") as f:
             json.dump(
                 self.store,
                 f,
                 default=lambda o: o.toJSON(),
             )
-
         self.delete_all_expired_data()
 
     def load(self):
         current_time = int(time.time())
 
         file = os.path.join(self.dump_dir, f"{self.name}.json")
+        if not os.path.isfile(file):
+            return
+
         with open(file, "r") as f:
             pre_store = json.load(f)
 
         for key, value in pre_store.items():
             p = Pair.fromJSON(value)
             if p.timeout <= current_time and p.timeout != -1:
                 continue
             self.store[key] = p
 
-    def __del__(self):
-        # on close of program, dump the data to a file
-        # print("Garbage Collection: Dumping to file for storage")
-        self.dump()
+    # def __del__(self):
+    #     # on close of program, dump the data to a file
+    #     # print("Garbage Collection: Dumping to file for storage")
+    #     self.dump()
 
     def __str__(self):
         return f"Name: {self.name}, Store Keys Amount: {len(self.store)}"
 
 
 def main():
-    kv1 = KV(name="transactions")
+    kv1 = KVStore(name="transactions")
 
     if True:
         kv1.set("dict", {"test": "other value"})
         kv1.set("list", [])
         kv1.set("apple", 2, 1)
         kv1.set("airplane", 2, 1)
         kv1.set("grass", 2, 1)
@@ -175,8 +223,9 @@
         print(kv1.get("counter"), v)  # 6
 
         # set counter as a string fails
         # kv1.set("counter", "0")
         # kv1.incr("counter")
 
 
-main()
+if __name__ == "__main__":
+    main()
```

### Comparing `py_kvstore-0.0.3/py_kvstore/test.py` & `py_kvstore-0.0.4/py_kvstore/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import os
 import time
 
-from py_kvstore import KV, Pair, current_dir
+from py_kvstore import KVStore, Pair
+
+current_dir = os.path.dirname(os.path.realpath(__file__))
 
 
 def test():
     print("Running KV test")
-    kv_a = KV(name="a")
+    kv_a = KVStore(name="a")
     kv_a_file = os.path.join(current_dir, "a.json")
 
     current_time = int(time.time())
 
     kv_a.set("a", 1, 1)
     kv_a.set("b", 2, 2)
     kv_a.set("c", 3, 3)
@@ -68,8 +70,9 @@
     os.remove(kv_a_file)
 
     # TODO: Add regex test
 
     print("KV test passed")
 
 
-test()
+if __name__ == "__main__":
+    test()
```

### Comparing `py_kvstore-0.0.3/py_kvstore.egg-info/PKG-INFO` & `py_kvstore-0.0.4/py_kvstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-kvstore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `py_kvstore-0.0.3/setup.py` & `py_kvstore-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # pip install twine
 # python setup.py bdist
 # twine upload -r py_kvstore dist/*
 
 setup(
     name="py_kvstore",
-    version="0.0.3",
+    version="0.0.4",
     description="A key value store",
     url="https://github.com/Reecepbcups/py_kvstore",
     author="Reece Willims",
     author_email="reecepbcups@gmail.com",
     license="Apache 2.0",
     packages=["py_kvstore"],
     install_requires=[],
```

