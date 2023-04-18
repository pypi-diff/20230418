# Comparing `tmp/simple-function-cache-0.0.3.tar.gz` & `tmp/simple-function-cache-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple-function-cache-0.0.3.tar", last modified: Tue Feb 15 08:00:56 2022, max compression
+gzip compressed data, was "simple-function-cache-0.0.4.tar", last modified: Tue Apr 18 02:25:39 2023, max compression
```

## Comparing `simple-function-cache-0.0.3.tar` & `simple-function-cache-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 baiyang    (501) staff       (20)        0 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/
--rw-r--r--   0 baiyang    (501) staff       (20)     1065 2022-02-11 07:59:29.000000 simple-function-cache-0.0.3/LICENSE
--rw-r--r--   0 baiyang    (501) staff       (20)      274 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/PKG-INFO
--rw-r--r--   0 baiyang    (501) staff       (20)     3689 2022-02-15 07:56:39.000000 simple-function-cache-0.0.3/README.md
--rw-r--r--   0 baiyang    (501) staff       (20)       38 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/setup.cfg
--rw-r--r--   0 baiyang    (501) staff       (20)      639 2022-02-15 08:00:28.000000 simple-function-cache-0.0.3/setup.py
-drwxr-xr-x   0 baiyang    (501) staff       (20)        0 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_cache/
--rw-r--r--   0 baiyang    (501) staff       (20)      431 2022-02-15 02:42:06.000000 simple-function-cache-0.0.3/simple_cache/__init__.py
--rw-r--r--   0 baiyang    (501) staff       (20)     5395 2022-02-15 02:51:10.000000 simple-function-cache-0.0.3/simple_cache/cache.py
--rw-r--r--   0 baiyang    (501) staff       (20)     1256 2022-02-15 02:51:10.000000 simple-function-cache-0.0.3/simple_cache/single_redis.py
-drwxr-xr-x   0 baiyang    (501) staff       (20)        0 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/
--rw-r--r--   0 baiyang    (501) staff       (20)      274 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/PKG-INFO
--rw-r--r--   0 baiyang    (501) staff       (20)      418 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/SOURCES.txt
--rw-r--r--   0 baiyang    (501) staff       (20)        1 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/dependency_links.txt
--rw-r--r--   0 baiyang    (501) staff       (20)        1 2022-02-15 03:40:46.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/not-zip-safe
--rw-r--r--   0 baiyang    (501) staff       (20)       21 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/requires.txt
--rw-r--r--   0 baiyang    (501) staff       (20)       19 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/simple_function_cache.egg-info/top_level.txt
-drwxr-xr-x   0 baiyang    (501) staff       (20)        0 2022-02-15 08:00:56.000000 simple-function-cache-0.0.3/tests/
--rw-r--r--   0 baiyang    (501) staff       (20)      168 2022-02-08 07:12:42.000000 simple-function-cache-0.0.3/tests/__init__.py
--rw-r--r--   0 baiyang    (501) staff       (20)     2076 2022-02-15 03:40:42.000000 simple-function-cache-0.0.3/tests/test_cache.py
+drwxr-xr-x   0 idr        (501) staff       (20)        0 2023-04-18 02:25:39.736194 simple-function-cache-0.0.4/
+-rw-rw-r--   0 idr        (501) staff       (20)     1065 2022-02-15 08:00:42.000000 simple-function-cache-0.0.4/LICENSE
+-rw-r--r--   0 idr        (501) staff       (20)      311 2023-04-18 02:25:39.736087 simple-function-cache-0.0.4/PKG-INFO
+-rw-rw-r--   0 idr        (501) staff       (20)     3689 2022-02-15 08:00:42.000000 simple-function-cache-0.0.4/README.md
+-rw-r--r--   0 idr        (501) staff       (20)       38 2023-04-18 02:25:39.736233 simple-function-cache-0.0.4/setup.cfg
+-rw-rw-r--   0 idr        (501) staff       (20)      686 2023-04-18 02:25:16.000000 simple-function-cache-0.0.4/setup.py
+drwxr-xr-x   0 idr        (501) staff       (20)        0 2023-04-18 02:25:39.734836 simple-function-cache-0.0.4/simple_cache/
+-rw-rw-r--   0 idr        (501) staff       (20)      433 2023-04-18 02:21:46.000000 simple-function-cache-0.0.4/simple_cache/__init__.py
+-rw-rw-r--   0 idr        (501) staff       (20)     5395 2023-04-18 02:23:10.000000 simple-function-cache-0.0.4/simple_cache/cache.py
+-rw-rw-r--   0 idr        (501) staff       (20)     1256 2022-02-15 08:00:42.000000 simple-function-cache-0.0.4/simple_cache/single_redis.py
+drwxr-xr-x   0 idr        (501) staff       (20)        0 2023-04-18 02:25:39.735957 simple-function-cache-0.0.4/simple_function_cache.egg-info/
+-rw-r--r--   0 idr        (501) staff       (20)      311 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/PKG-INFO
+-rw-r--r--   0 idr        (501) staff       (20)      418 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 idr        (501) staff       (20)        1 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 idr        (501) staff       (20)        1 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/not-zip-safe
+-rw-r--r--   0 idr        (501) staff       (20)       21 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/requires.txt
+-rw-r--r--   0 idr        (501) staff       (20)       19 2023-04-18 02:25:39.000000 simple-function-cache-0.0.4/simple_function_cache.egg-info/top_level.txt
+drwxr-xr-x   0 idr        (501) staff       (20)        0 2023-04-18 02:25:39.735267 simple-function-cache-0.0.4/tests/
+-rw-rw-r--   0 idr        (501) staff       (20)      168 2022-02-15 08:00:42.000000 simple-function-cache-0.0.4/tests/__init__.py
+-rw-rw-r--   0 idr        (501) staff       (20)     2076 2022-02-15 08:00:42.000000 simple-function-cache-0.0.4/tests/test_cache.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simple-function-cache-0.0.3/LICENSE` & `simple-function-cache-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-function-cache-0.0.3/README.md` & `simple-function-cache-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `simple-function-cache-0.0.3/setup.py` & `simple-function-cache-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 # python setup.py sdist upload -r pypi
 
 if __name__ == "__main__":
 
     setup(
         name="simple-function-cache",
-        version='0.0.3',
+        version='0.0.4',
         description="function cache decorator with redis",
         url="https://github.com/byscut/simple-function-cache.git",
         author="byscut",
+        author_email="byscut2010@foxmail.com",
         license="MIT",
         test_suite='tests',
         package_dir={'': '.'},
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         install_requires=[
```

### Comparing `simple-function-cache-0.0.3/simple_cache/cache.py` & `simple-function-cache-0.0.4/simple_cache/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 elif not _refresh and cache_mode_ == CacheMode.refresh.name:
                     _refresh = True
 
                 # no cache, just dry run func
                 if _no_cache:
                     logger.info("cache disable - use no cache")
                     return origin_func(*origin_args, **origin_kwargs)
-                key_prefix = cache_name + '_'
+                key_prefix = cache_name + ':'
                 cache_key = key_func(*origin_args, **origin_kwargs)
                 if type(cache_key) != str:
                     raise CallWithCacheException("key_func should return a str , but got :" + str(type(cache_key)), status='Failed')
                 cache_key = key_prefix + cache_key
                 # refresh cache , delete old one and set new
                 raw_expire = kwargs.get("expire")
                 if type(raw_expire) == int:
```

### Comparing `simple-function-cache-0.0.3/simple_cache/single_redis.py` & `simple-function-cache-0.0.4/simple_cache/single_redis.py`

 * *Files identical despite different names*

### Comparing `simple-function-cache-0.0.3/tests/test_cache.py` & `simple-function-cache-0.0.4/tests/test_cache.py`

 * *Files identical despite different names*

