# Comparing `tmp/aiohttp_msal-0.5.2.tar.gz` & `tmp/aiohttp_msal-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_msal-0.5.2.tar", last modified: Tue Feb  7 07:48:00 2023, max compression
+gzip compressed data, was "aiohttp_msal-0.5.4.tar", last modified: Tue Apr 18 18:53:26 2023, max compression
```

## Comparing `aiohttp_msal-0.5.2.tar` & `aiohttp_msal-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/aiohttp_msal/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/msal_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/settings_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/aiohttp_msal/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-07 07:48:00.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-07 07:48:00.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 07:48:00.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-07 07:48:00.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-07 07:48:00.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 07:47:59.000000 aiohttp_msal-0.5.2/aiohttp_msal.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:48:00.185348 aiohttp_msal-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/tests/test_msal_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-07 07:47:48.000000 aiohttp_msal-0.5.2/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:26.095566 aiohttp_msal-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 18:53:26.095566 aiohttp_msal-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:26.091566 aiohttp_msal-0.5.4/aiohttp_msal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/msal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/settings_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/aiohttp_msal/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:26.095566 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 18:53:26.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 18:53:26.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:53:26.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 18:53:26.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 18:53:26.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:53:25.000000 aiohttp_msal-0.5.4/aiohttp_msal.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 18:53:26.095566 aiohttp_msal-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:26.095566 aiohttp_msal-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/tests/test_msal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 18:53:13.000000 aiohttp_msal-0.5.4/tests/test_settings.py
```

### Comparing `aiohttp_msal-0.5.2/LICENSE` & `aiohttp_msal-0.5.4/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 kellerza
+Copyright (c) 2022-2023 kellerza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/__init__.py` & `aiohttp_msal-0.5.4/aiohttp_msal/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """aiohttp_msal."""
 import logging
 from functools import wraps
 from inspect import getfullargspec, iscoroutinefunction
 from typing import Any, Awaitable, Callable, Union
-from urllib.parse import urlparse
 
 from aiohttp import ClientSession, web
 from aiohttp_session import get_session
 from aiohttp_session import setup as _setup
 
 from .msal_async import AsyncMSAL
 from .settings import ENV
 
 _LOGGER = logging.getLogger(__name__)
 
-VERSION = "0.5.2"
+VERSION = "0.5.4"
 
 
 def msal_session(*args: Callable[[AsyncMSAL], Union[Any, Awaitable[Any]]]) -> Callable:
     """Session decorator.
 
     Arguments can include a list of function to perform login tests etc.
     """
@@ -52,28 +51,23 @@
     app: web.Application, max_age: int = 3600 * 24 * 90
 ) -> None:
     """OPTIONAL: Initialize aiohttp_session with Redis storage.
 
     You can initialize your own aiohttp_session & storage provider.
     """
     # pylint: disable=import-outside-toplevel
-    import aioredis
     from aiohttp_session import redis_storage
+    from redis.asyncio import from_url
 
     await check_proxy()
 
     _LOGGER.info("Connect to Redis %s", ENV.REDIS)
-    red = urlparse(ENV.REDIS)
     try:
-        if hasattr(aioredis, "create_redis_pool"):
-            ENV.database = await aioredis.create_redis_pool((red.hostname, red.port))
-        else:
-            # when aioredis migrates to 2.0...
-            ENV.database = aioredis.from_url(ENV.REDIS)  # pylint: disable=no-member
-            # , encoding="utf-8", decode_responses=True
+        ENV.database = from_url(ENV.REDIS)  # pylint: disable=no-member
+        # , encoding="utf-8", decode_responses=True
     except ConnectionRefusedError as err:
         raise ConnectionError("Could not connect to REDIS server") from err
 
     storage = redis_storage.RedisStorage(
         ENV.database,
         max_age=max_age,
         path="/",
```

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/msal_async.py` & `aiohttp_msal-0.5.4/aiohttp_msal/msal_async.py`

 * *Files identical despite different names*

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/routes.py` & `aiohttp_msal-0.5.4/aiohttp_msal/routes.py`

 * *Files identical despite different names*

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/settings.py` & `aiohttp_msal-0.5.4/aiohttp_msal/settings.py`

 * *Files identical despite different names*

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/settings_base.py` & `aiohttp_msal-0.5.4/aiohttp_msal/settings_base.py`

 * *Files identical despite different names*

### Comparing `aiohttp_msal-0.5.2/aiohttp_msal/user_info.py` & `aiohttp_msal-0.5.4/aiohttp_msal/user_info.py`

 * *Files identical despite different names*

### Comparing `aiohttp_msal-0.5.2/setup.cfg` & `aiohttp_msal-0.5.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -22,38 +22,44 @@
 
 [options]
 packages = find:
 python_requires = >=3.9
 include_package_data = True
 tests_requires = file: requirements_test.txt
 install_requires = 
-	msal>=1.18.0b1
-	aiohttp_session>=2.11
+	msal>=1.21.0
+	aiohttp_session>=2.12
 	aiohttp>=3.8
 zip_safe = true
 
 [options.extras_require]
 redis = 
-	aiohttp_session[redis]
+	aiohttp_session[aioredis]>=2.12
+tests = 
+	black==23.3.0
+	pylint
+	flake8
+	pytest-aiohttp
+	pytest
+	pytest-cov
+	pytest-asyncio
+	pytest-env
 
 [isort]
 profile = black
 
 [flake8]
 extend-ignore = E203, E501, W503
 
 [mypy]
 disallow_untyped_defs = True
 
 [mypy-msal.*]
 ignore_missing_imports = True
 
-[mypy-aioredis.*]
-ignore_missing_imports = True
-
 [pydocstyle]
 match_dir = aiohttp_msal
 convention = google
 
 [tool:pytest]
 filterwarnings = 
 	ignore:.+@coroutine.+deprecated.+
```

