# Comparing `tmp/rmmbr-0.0.1.tar.gz` & `tmp/rmmbr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.1.tar", last modified: Thu Apr 13 16:07:47 2023, max compression
+gzip compressed data, was "rmmbr-0.0.2.tar", last modified: Tue Apr 18 10:34:55 2023, max compression
```

## Comparing `rmmbr-0.0.1.tar` & `rmmbr-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:07:47.071912 rmmbr-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-13 16:07:47.071912 rmmbr-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:07:47.071912 rmmbr-0.0.1/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 16:07:39.000000 rmmbr-0.0.1/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-13 16:07:39.000000 rmmbr-0.0.1/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-13 16:07:39.000000 rmmbr-0.0.1/rmmbr/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:07:47.071912 rmmbr-0.0.1/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:07:47.000000 rmmbr-0.0.1/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:07:47.071912 rmmbr-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 16:07:39.000000 rmmbr-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.728845 rmmbr-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 10:34:55.728845 rmmbr-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.724846 rmmbr-0.0.2/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.728845 rmmbr-0.0.2/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:34:55.728845 rmmbr-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 10:34:44.000000 rmmbr-0.0.2/setup.py
```

### Comparing `rmmbr-0.0.1/PKG-INFO` & `rmmbr-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -15,44 +15,44 @@
 ```sh
 npm i rmmbr
 ```
 
 ```js
 import { cloudCache, localCache } from "rmmbr";
 
-const cacher = await localCache({ id: "some-id" });
+const cacher = localCache({ id: "some-id" });
 
 let nCalled = 0;
 const f = (x: number) => {
   nCalled++;
   return Promise.resolve(x);
 };
 const fCached = cacher(f);
 await fCached(3);
 await fCached(3);
 // nCalled is 1 here
 ```
 
 The local cache stores data in a text file under a `.rmmbr` directory.
 
-If you want to persist across devices, there is also a free to use cloud service:
+There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
+
+If you want to persist across devices, we offer a free to use cloud service:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
 });
 ```
 
-As a free service, it comes with no guarantees, best effort only.
-
-There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
+At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
-We accept issues for feature requests and SLA requests.
+We also accept issues for feature requests 👩‍🔧
 
 ## Python
 
 ```sh
 pip install rmmbr
 ```
 
-Python largely works the same, with `mem_cache`, `local_cache` and `cloud_cache`.
+The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
```

### Comparing `rmmbr-0.0.1/rmmbr/main.py` & `rmmbr-0.0.2/rmmbr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,33 +65,41 @@
         y = await f(x)
         cache[key_result] = y
         return y
 
     return func
 
 
-async def _make_local_read_write(name: str):
+def _make_local_read_write(name: str):
     def default_f():
         return _serialize({})
 
     file_path = _path_to_cache(name)
-    cache = _deserialize(await _read_file_with_default(default_f, file_path))
+    cache = None
+
+    async def get_cache():
+        nonlocal cache
+        if cache:
+            return cache
+        cache = _deserialize(await _read_file_with_default(default_f, file_path))
+        return cache
 
     async def read(key: Key):
-        return cache.get(key, None)
+        return (await get_cache()).get(key, None)
 
     async def write(key: Key, value):
+        cache = await get_cache()
         cache[key] = value
         await _write_string_to_file(file_path, _serialize(cache))
 
     return read, write
 
 
-async def local_cache(id: str):
-    read, write = await _make_local_read_write(id)
+def local_cache(id: str):
+    read, write = _make_local_read_write(id)
     return lambda f: _abstract_cache_params(_key, f, read, write)
 
 
 async def _post_json(url: str, payload):
     async with httpx.AsyncClient() as client:
         response = await client.post(
             url=url,
```

### Comparing `rmmbr-0.0.1/rmmbr/main_test.py` & `rmmbr-0.0.2/rmmbr/main_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,15 @@
         async def f(x):
             nonlocal n_called
             n_called += 1
             return await asyncio.sleep(0, x)
 
         f_cached = cacher(f)
         await f_cached(3)
-        results = await asyncio.gather(
-            f_cached(3), f_cached(3), f_cached(2), f_cached(1)
-        )
+        results = await asyncio.gather(*map(f_cached, [3, 3, 2, 1]))
         assert results == [3, 3, 2, 1]
         await cacher(f)(3)
         assert n_called == n
 
     return inner
 
 
@@ -34,15 +32,16 @@
             _rmdir(item)
         else:
             item.unlink()
     directory.rmdir()
 
 
 async def test_local_cache():
-    await _cache_test_helper(3)(await local_cache("some-id"))
+    cacher = local_cache("some-id")
+    await _cache_test_helper(3)(cacher)
     _rmdir("./.rmmbr")
 
 
 async def test_memory_cache():
     await _cache_test_helper(4)(mem_cache)
```

### Comparing `rmmbr-0.0.1/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.2/rmmbr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -15,44 +15,44 @@
 ```sh
 npm i rmmbr
 ```
 
 ```js
 import { cloudCache, localCache } from "rmmbr";
 
-const cacher = await localCache({ id: "some-id" });
+const cacher = localCache({ id: "some-id" });
 
 let nCalled = 0;
 const f = (x: number) => {
   nCalled++;
   return Promise.resolve(x);
 };
 const fCached = cacher(f);
 await fCached(3);
 await fCached(3);
 // nCalled is 1 here
 ```
 
 The local cache stores data in a text file under a `.rmmbr` directory.
 
-If you want to persist across devices, there is also a free to use cloud service:
+There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
+
+If you want to persist across devices, we offer a free to use cloud service:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
 });
 ```
 
-As a free service, it comes with no guarantees, best effort only.
-
-There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
+At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
-We accept issues for feature requests and SLA requests.
+We also accept issues for feature requests 👩‍🔧
 
 ## Python
 
 ```sh
 pip install rmmbr
 ```
 
-Python largely works the same, with `mem_cache`, `local_cache` and `cloud_cache`.
+The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
```

### Comparing `rmmbr-0.0.1/setup.py` & `rmmbr-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import os
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.1",
+    version="0.0.2",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```

