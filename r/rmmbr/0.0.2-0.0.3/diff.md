# Comparing `tmp/rmmbr-0.0.2.tar.gz` & `tmp/rmmbr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.2.tar", last modified: Tue Apr 18 10:34:55 2023, max compression
+gzip compressed data, was "rmmbr-0.0.3.tar", last modified: Tue Apr 18 14:55:24 2023, max compression
```

## Comparing `rmmbr-0.0.2.tar` & `rmmbr-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.728845 rmmbr-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 10:34:55.728845 rmmbr-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.724846 rmmbr-0.0.2/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-18 10:34:44.000000 rmmbr-0.0.2/rmmbr/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:34:55.728845 rmmbr-0.0.2/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 10:34:55.000000 rmmbr-0.0.2/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:34:55.728845 rmmbr-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 10:34:44.000000 rmmbr-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 14:55:24.496362 rmmbr-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:55:24.496362 rmmbr-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 14:55:16.000000 rmmbr-0.0.3/setup.py
```

### Comparing `rmmbr-0.0.2/PKG-INFO` & `rmmbr-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -38,14 +38,15 @@
 
 If you want to persist across devices, we offer a free to use cloud service:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
+  ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
 At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
 We also accept issues for feature requests 👩‍🔧
```

### Comparing `rmmbr-0.0.2/rmmbr/main.py` & `rmmbr-0.0.3/rmmbr/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 import os
 import json
 import hashlib
 import httpx
 import aiofiles
 from aiofiles import os as aiofiles_os
 
@@ -79,18 +80,18 @@
     async def get_cache():
         nonlocal cache
         if cache:
             return cache
         cache = _deserialize(await _read_file_with_default(default_f, file_path))
         return cache
 
-    async def read(key: Key):
+    async def read(key: _Key):
         return (await get_cache()).get(key, None)
 
-    async def write(key: Key, value):
+    async def write(key: _Key, value):
         cache = await get_cache()
         cache[key] = value
         await _write_string_to_file(file_path, _serialize(cache))
 
     return read, write
 
 
@@ -109,31 +110,34 @@
         return response.json()
 
 
 async def _call_api(url: str, method: str, params):
     return await _post_json(url, {"method": method, "params": params})
 
 
-def _set_remote(id: str, url: str):
+def _set_remote(id: str, url: str, ttl: Optional[int]):
     async def func(key, value):
-        await _call_api(url, "set", {"id": id, "key": key, "value": value})
+        params = {"id": id, "key": key, "value": value}
+        if ttl is not None:
+            params["ttl"] = ttl
+        await _call_api(url, "set", params)
 
     return func
 
 
-Key = str
+_Key = str
 
 
 def _get_remote(id: str, url: str):
-    async def func(key: Key):
+    async def func(key: _Key):
         return await _call_api(url, "get", {"id": id, "key": key})
 
     return func
 
 
-def cloud_cache(token: str, url: str):
+def cloud_cache(token: str, url: str, ttl: Optional[int]):
     def inner_func(f):
         return _abstract_cache_params(
-            _key, f, _get_remote(token, url), _set_remote(token, url)
+            _key, f, _get_remote(token, url), _set_remote(token, url, ttl)
         )
 
     return inner_func
```

### Comparing `rmmbr-0.0.2/rmmbr/main_test.py` & `rmmbr-0.0.3/rmmbr/main_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 import redis.asyncio as redis
 
 import asyncio
 import dotenv
 import pathlib
 
 
-def _cache_test_helper(n):
+def _cache_test_helper(instance_implies_new_cache: bool, expires_after_2_seconds: bool):
     async def inner(cacher):
         n_called = 0
 
         async def f(x):
             nonlocal n_called
             n_called += 1
             return await asyncio.sleep(0, x)
 
         f_cached = cacher(f)
         await f_cached(3)
         results = await asyncio.gather(*map(f_cached, [3, 3, 2, 1]))
         assert results == [3, 3, 2, 1]
         await cacher(f)(3)
-        assert n_called == n
+        assert n_called == (4 if instance_implies_new_cache else 3)
+        n_called = 0
+        await asyncio.sleep(2)
+        await f_cached(3)
+        assert n_called == (1 if expires_after_2_seconds else 0)
 
     return inner
 
 
 def _rmdir(directory):
     directory = pathlib.Path(directory)
     for item in directory.iterdir():
@@ -33,34 +37,46 @@
         else:
             item.unlink()
     directory.rmdir()
 
 
 async def test_local_cache():
     cacher = local_cache("some-id")
-    await _cache_test_helper(3)(cacher)
+    await _cache_test_helper(False, False)(cacher)
     _rmdir("./.rmmbr")
 
 
 async def test_memory_cache():
-    await _cache_test_helper(4)(mem_cache)
+    await _cache_test_helper(True, False)(mem_cache)
 
 
 def _env_param(s: str) -> str:
     value = dotenv.dotenv_values(".env")[s]
     assert value
     return value
 
 
-async def _get_client():
-    return await redis.Redis(
+async def _clean_redis():
+    redis_client = await redis.Redis(
         password=_env_param("REDIS_PASSWORD"),
         host=_env_param("REDIS_URL"),
         port=int(_env_param("REDIS_PORT")),
     )
+    await redis_client.flushall()
+
+
+_port = _env_param("PORT")
+_mock_backend_url = f"http://localhost:{_port}"
 
 
 async def test_cloud_cache():
-    redis_client = await _get_client()
-    await redis_client.flushall()
-    port = _env_param("PORT")
-    await _cache_test_helper(3)(cloud_cache("some-token", f"http://localhost:{port}"))
+    await _clean_redis()
+    await _cache_test_helper(False, False)(
+        cloud_cache("some-token", _mock_backend_url, None)
+    )
+
+
+async def test_cloud_cache_expiration():
+    await _clean_redis()
+    await _cache_test_helper(False, True)(
+        cloud_cache("some-token", _mock_backend_url, 1)
+    )
```

### Comparing `rmmbr-0.0.2/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.3/rmmbr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -38,14 +38,15 @@
 
 If you want to persist across devices, we offer a free to use cloud service:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
+  ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
 At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
 We also accept issues for feature requests 👩‍🔧
```

### Comparing `rmmbr-0.0.2/setup.py` & `rmmbr-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import os
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.2",
+    version="0.0.3",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```

