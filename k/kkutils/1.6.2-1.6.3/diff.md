# Comparing `tmp/kkutils-1.6.2.tar.gz` & `tmp/kkutils-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkutils-1.6.2.tar", last modified: Mon Feb 27 03:11:59 2023, max compression
+gzip compressed data, was "kkutils-1.6.3.tar", last modified: Tue Apr 18 08:52:44 2023, max compression
```

## Comparing `kkutils-1.6.2.tar` & `kkutils-1.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 03:11:59.178046 kkutils-1.6.2/
--rw-r--r--   0 root         (0) root         (0)      703 2023-02-27 03:11:59.178046 kkutils-1.6.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 03:11:59.170046 kkutils-1.6.2/kkutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-02-27 03:11:59.000000 kkutils-1.6.2/kkutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-02-27 03:11:59.000000 kkutils-1.6.2/kkutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 03:11:59.000000 kkutils-1.6.2/kkutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-02-27 03:11:59.000000 kkutils-1.6.2/kkutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-27 03:11:59.000000 kkutils-1.6.2/kkutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.2/processor.py
--rw-r--r--   0 root         (0) root         (0)      241 2023-01-04 06:45:47.000000 kkutils-1.6.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 03:11:59.178046 kkutils-1.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1190 2023-02-27 03:11:56.000000 kkutils-1.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 03:11:59.174046 kkutils-1.6.2/tornado_utils/
--rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.2/tornado_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.2/tornado_utils/application.py
--rw-r--r--   0 root         (0) root         (0)    10043 2022-12-19 07:46:25.000000 kkutils-1.6.2/tornado_utils/basehandler.py
--rw-r--r--   0 root         (0) root         (0)    12695 2022-12-07 23:58:26.000000 kkutils-1.6.2/tornado_utils/userhandler.py
--rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.2/tornado_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 03:11:59.174046 kkutils-1.6.2/utils/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.2/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10482 2023-02-26 00:49:25.000000 kkutils-1.6.2/utils/base_utils.py
--rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.2/utils/cached_property.py
--rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.2/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-02-19 15:22:17.000000 kkutils-1.6.2/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)    10693 2022-11-04 03:27:22.000000 kkutils-1.6.2/utils/curl_utils.py
--rw-r--r--   0 root         (0) root         (0)    16840 2022-12-18 14:45:35.000000 kkutils-1.6.2/utils/db_utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.2/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4007 2022-07-14 13:13:22.000000 kkutils-1.6.2/utils/email_utils.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.2/utils/fire.py
--rw-r--r--   0 root         (0) root         (0)    26362 2023-02-19 15:22:17.000000 kkutils-1.6.2/utils/http_utils.py
--rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.2/utils/log_utils.py
--rw-r--r--   0 root         (0) root         (0)     6577 2022-07-14 13:13:22.000000 kkutils-1.6.2/utils/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.2/utils/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.2/utils/xdb_searcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-18 08:52:44.391119 kkutils-1.6.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.387119 kkutils-1.6.3/kkutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-18 08:52:44.000000 kkutils-1.6.3/kkutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.3/processor.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 08:52:44.391119 kkutils-1.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-04-18 08:52:41.000000 kkutils-1.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/tornado_utils/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.3/tornado_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.3/tornado_utils/application.py
+-rw-r--r--   0 root         (0) root         (0)    10043 2023-03-06 03:11:06.000000 kkutils-1.6.3/tornado_utils/basehandler.py
+-rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.3/tornado_utils/userhandler.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.3/tornado_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:52:44.391119 kkutils-1.6.3/utils/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.3/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-03-19 08:31:21.000000 kkutils-1.6.3/utils/base_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/cached_property.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-02-19 15:22:17.000000 kkutils-1.6.3/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    10693 2022-11-04 03:27:22.000000 kkutils-1.6.3/utils/curl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.3/utils/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/email_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.3/utils/fire.py
+-rw-r--r--   0 root         (0) root         (0)    26362 2023-02-19 15:22:17.000000 kkutils-1.6.3/utils/http_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.3/utils/log_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2022-07-14 13:13:22.000000 kkutils-1.6.3/utils/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.3/utils/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.3/utils/xdb_searcher.py
```

### Comparing `kkutils-1.6.2/PKG-INFO` & `kkutils-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.2
+Version: 1.6.3
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.2/kkutils.egg-info/PKG-INFO` & `kkutils-1.6.3/kkutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.2
+Version: 1.6.3
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.2/kkutils.egg-info/SOURCES.txt` & `kkutils-1.6.3/kkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/processor.py` & `kkutils-1.6.3/processor.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/setup.py` & `kkutils-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Last modified: 2019-04-07 00:07:43
 '''
 
 from setuptools import setup
 
 setup(
     name="kkutils",
-    version="1.6.2",
+    version="1.6.3",
     description="python utils",
     author="digua",
     author_email="zkdfbb@qq.com",
     url="https://www.ishield.cn",
     license="MIT",
     python_requires='>=3.6',
     data_files=[('', ['requirements.txt'])],
```

### Comparing `kkutils-1.6.2/tornado_utils/application.py` & `kkutils-1.6.3/tornado_utils/application.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/tornado_utils/basehandler.py` & `kkutils-1.6.3/tornado_utils/basehandler.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/tornado_utils/userhandler.py` & `kkutils-1.6.3/tornado_utils/userhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                     await awaitable(self.db.users.update_one({'_id': self.current_user._id}, {'$set': update}))
                 else:
                     ret.id = await awaitable(self.db.users.seq_id)
                     ret.token = uuid.uuid4().hex
                     ret.active = True
                     ret.created_at = datetime.datetime.now().replace(microsecond=0)
                     await awaitable(self.db.users.update_one({'openId': ret.openId}, {'$set': ret}, upsert=True))
-            expires = datetime.datetime.now() + datetime.timedelta(days=30)
-            self.set_cookie('token', ret.token, expires=expires)
+
+            self.set_cookie('token', ret.token, expires_days=365)
             ret.err = 0
 
         return ret
 
 
 @bp.route("/check")
 class CheckHandler(BaseHandler):
@@ -134,23 +134,25 @@
         self.finish(ret)
 
 
 @bp.route("/logout")
 class LogoutHandler(BaseHandler):
 
     def get(self):
-        self.clear_cookie('token')
+        self.clear_all_cookies()
         self.redirect('/')
 
 
 @bp.route("/signup")
 class SignupHandler(BaseHandler):
 
     def get(self):
         self.next = self.get_argument('next', '/')
+        if self.args.from_id:
+            self.set_cookie('from_id', self.args.from_id, expires_days=1)
         self.render('signup.html')
 
     async def post(self):
         ret = await self.check_username()
         if ret.err:
             return self.finish(ret)
         ret = await self.check_email()
@@ -189,15 +191,16 @@
         if not user.id:
             update['id'] = await awaitable(self.db.users.seq_id)
             if update['id'] == 1:
                 update['admin'] = True
         if update:
             await awaitable(self.db.users.update_one({'_id': user._id}, {'$set': update}))
             user.update(update)
-        self.set_cookie('token', token, expires_days=30)
+
+        self.set_cookie('token', token, expires_days=365)
         self.finish({'err': 0, 'user': user})
 
 
 @bp.route("/signin")
 class SigninHandler(BaseHandler):
 
     def get(self):
@@ -215,18 +218,16 @@
             query = {'email': username, 'password': self.encrypt(password)}
         else:
             query = {'username': username, 'password': self.encrypt(password)}
         user = await awaitable(self.db.users.find_one(query))
         if not user:
             return self.finish({'err': 1, 'msg': '用户名或密码错误'})
 
-        if remember == 'on':
-            self.set_cookie('token', user.token, expires_days=30)
-        else:
-            self.set_cookie('token', user.token)
+        expires_days = 365 if remember == 'on' else None
+        self.set_cookie('token', user.token, expires_days=expires_days)
         self.finish({'err': 0, 'user': user})
 
 
 @bp.route("/user")
 class UserHandler(BaseHandler):
 
     async def get(self):
```

### Comparing `kkutils-1.6.2/tornado_utils/utils.py` & `kkutils-1.6.3/tornado_utils/utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/__init__.py` & `kkutils-1.6.3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/base_utils.py` & `kkutils-1.6.3/utils/base_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 import socket
 import sys
 import threading
 import time
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from functools import partial, reduce
+from itertools import chain, zip_longest
 from pathlib import Path
 from socket import inet_aton, inet_ntoa
 from struct import pack, unpack
 
 import requests
 import yaml
 from pymongo.cursor import Cursor
@@ -241,30 +242,25 @@
 
 async def awaitable(ret):
     return await ret if inspect.isawaitable(ret) else ret
 
 
 def multi_apply(func, *args, **kwargs):
     workers = kwargs.pop('workers', os.cpu_count())
-    pool = kwargs.pop('pool', False)
-    pfunc = partial(func, **kwargs) if kwargs else func
-    size = math.ceil(len(args[0]) / workers)
-    pargs = [[arg[i * size:(i + 1) * size] for i in range(workers)] for arg in args]
-    if pool:
-        with ThreadPoolExecutor(workers) as executor:
-            results = executor.map(pfunc, *pargs)
-    else:
-        with ProcessPoolExecutor(workers) as executor:
-            results = executor.map(pfunc, *pargs)
+    backend = kwargs.pop('backend', 'thread')
+    size = len(args[0])
+    args = [[x[i::workers] for i in range(workers)] for x in args]
+    func = partial(func, **kwargs) if kwargs else func
+    Executor = ThreadPoolExecutor if backend == 'thread' else ProcessPoolExecutor
+    with Executor(workers) as executor:
+        results = executor.map(func, *args)
     results = list(results)
-    if len(results) > 0:
-        if isinstance(results[0], list):
-            return reduce(lambda x, y: x + y, results)
-        elif results[0] is not None:
-            return results
+    if all([isinstance(x, (list, tuple)) for x in results]):
+        results = list(chain(*zip_longest(*results)))[:size]
+    return results
 
 
 def floor(number, ndigits=0):
     '''当ndigits大于等于number的小数点位数时，直接返回
     '''
     if ndigits == 0:
         return math.floor(number)
```

### Comparing `kkutils-1.6.2/utils/cached_property.py` & `kkutils-1.6.3/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/config_utils.py` & `kkutils-1.6.3/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/crypto.py` & `kkutils-1.6.3/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/curl_utils.py` & `kkutils-1.6.3/utils/curl_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/db_utils.py` & `kkutils-1.6.3/utils/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,49 +121,42 @@
     def __getitem__(self, name):
         return Collection(self, name)
 
 
 class MongoClient(pymongo.MongoClient):
 
     def __init__(self, **kwargs):
-        env = 'MONGO_LOC' if kwargs.pop('loc', False) and os.environ.get('MONGO_LOC') else 'MONGO_URI'
-        if any([key in kwargs for key in ['host', 'port', 'user', 'password']]):
-            host = kwargs.pop('host', 'localhost')
-            port = kwargs.pop('port', 27017)
-            user = kwargs.pop('user', None)
-            password = kwargs.pop('password', None)
-            uri = f"mongodb://{quote_plus(user)}:{quote_plus(password)}@{host}:{port}" if user and password else f"mongodb://{host}:{port}"
-        elif kwargs.get('uri'):
+        if kwargs.get('uri'):
             uri = kwargs.pop('uri')
-        elif os.environ.get(env):
-            uri = os.environ[env]
+        elif os.environ.get('MONGO_URI'):
+            uri = os.environ.get('MONGO_URI')
         else:
             host = os.environ.get('MONGO_HOST', 'localhost')
             port = os.environ.get('MONGO_PORT', 27017)
             user = os.environ.get('MONGO_USER', None)
             password = os.environ.get('MONGO_PWD', None)
             uri = f"mongodb://{quote_plus(user)}:{quote_plus(password)}@{host}:{port}" if user and password else f"mongodb://{host}:{port}"
 
         kwargs.pop('uri', None)
         kwargs.setdefault('document_class', Dict)
-        self.__db = parse_uri(uri).get('db')
         super(MongoClient, self).__init__(uri, **kwargs)
 
     def __getitem__(self, name):
         return Database(self, name)
 
     def __getattr__(self, name):
         return Database(self, name)
 
 
 class Mongo(Database):
 
-    def __init__(self, db, **kwargs):
+    def __init__(self, db=None, **kwargs):
         client = MongoClient(**kwargs)
-        super(Mongo, self).__init__(client, db)
+        name = db or client.get_default_database().name
+        super(Mongo, self).__init__(client, name)
 
 
 class AgnosticCursor(core.AgnosticCursor):
     __delegate_class__ = Cursor
 
     @coroutine_annotation
     def to_list(self, length=None):
@@ -255,17 +248,18 @@
 MotorClient = create_asyncio_class(AgnosticClient)
 MotorDatabase = create_asyncio_class(AgnosticDatabase)
 MotorCollection = create_asyncio_class(AgnosticCollection)
 
 
 class Motor(MotorDatabase):
 
-    def __init__(self, db='test', **kwargs):
+    def __init__(self, db=None, **kwargs):
         client = MotorClient(**kwargs)
-        super(Motor, self).__init__(client, db)
+        name = db or client.get_default_database().name
+        super(Motor, self).__init__(client, name)
 
 
 class Redis(redis.StrictRedis):
 
     def __init__(self, **kwargs):
         if any([key in kwargs for key in ['host', 'port', 'password']]):
             host = kwargs.pop('host', 'localhost')
```

### Comparing `kkutils-1.6.2/utils/decorator.py` & `kkutils-1.6.3/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/email_utils.py` & `kkutils-1.6.3/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/fire.py` & `kkutils-1.6.3/utils/fire.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/http_utils.py` & `kkutils-1.6.3/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/log_utils.py` & `kkutils-1.6.3/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/rabbitmq.py` & `kkutils-1.6.3/utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/stopwatch.py` & `kkutils-1.6.3/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.2/utils/xdb_searcher.py` & `kkutils-1.6.3/utils/xdb_searcher.py`

 * *Files identical despite different names*

