# Comparing `tmp/hxq-1.0.1.tar.gz` & `tmp/hxq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hxq-1.0.1.tar", last modified: Mon Apr 17 15:41:55 2023, max compression
+gzip compressed data, was "dist\hxq-1.0.2.tar", last modified: Tue Apr 18 16:16:59 2023, max compression
```

## Comparing `hxq-1.0.1.tar` & `hxq-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/
--rw-rw-rw-   0        0        0      169 2023-04-17 15:41:55.000000 hxq-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/
--rw-rw-rw-   0        0        0      141 2023-04-17 15:41:39.000000 hxq-1.0.1/hxq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/interface/
--rw-rw-rw-   0        0        0      777 2023-04-17 15:40:51.000000 hxq-1.0.1/hxq/interface/__init__.py
--rw-rw-rw-   0        0        0     4230 2023-04-14 14:47:06.000000 hxq-1.0.1/hxq/interface/db_helper.py
--rw-rw-rw-   0        0        0      300 2023-04-13 13:36:38.000000 hxq-1.0.1/hxq/interface/httpx.py
--rw-rw-rw-   0        0        0      186 2023-04-13 13:11:19.000000 hxq-1.0.1/hxq/interface/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/
--rw-rw-rw-   0        0        0      123 2023-04-13 13:04:22.000000 hxq-1.0.1/hxq/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/db/
--rw-rw-rw-   0        0        0      383 2023-04-13 12:57:46.000000 hxq-1.0.1/hxq/libs/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/httpx/
--rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.1/hxq/libs/httpx/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-13 14:06:06.000000 hxq-1.0.1/hxq/libs/httpx/chrome_agent.py
--rw-rw-rw-   0        0        0     9128 2023-04-17 15:40:28.000000 hxq-1.0.1/hxq/libs/httpx/http.py
--rw-rw-rw-   0        0        0     3167 2023-04-16 10:54:55.000000 hxq-1.0.1/hxq/libs/httpx/session.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/win32/
--rw-rw-rw-   0        0        0     1983 2023-04-13 13:36:03.000000 hxq-1.0.1/hxq/libs/win32/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/utils/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.1/hxq/utils/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-04-13 14:08:04.000000 hxq-1.0.1/hxq/utils/common.py
--rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.1/hxq/utils/decorator.py
--rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.1/hxq/utils/encipher.py
--rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.1/hxq/utils/pic_code.py
--rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.1/hxq/utils/ran_func.py
--rw-rw-rw-   0        0        0     3463 2023-04-09 13:39:58.000000 hxq-1.0.1/hxq/utils/threadx.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/
--rw-rw-rw-   0        0        0      169 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:41:55.000000 hxq-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-04-17 15:41:23.000000 hxq-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/
+-rw-rw-rw-   0        0        0      169 2023-04-18 16:16:59.000000 hxq-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/
+-rw-rw-rw-   0        0        0      141 2023-04-18 16:12:01.000000 hxq-1.0.2/hxq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/interface/
+-rw-rw-rw-   0        0        0      122 2023-04-18 15:01:16.000000 hxq-1.0.2/hxq/interface/__init__.py
+-rw-rw-rw-   0        0        0     4230 2023-04-14 14:47:06.000000 hxq-1.0.2/hxq/interface/db_helper.py
+-rw-rw-rw-   0        0        0      300 2023-04-13 13:36:38.000000 hxq-1.0.2/hxq/interface/httpx.py
+-rw-rw-rw-   0        0        0      186 2023-04-13 13:11:19.000000 hxq-1.0.2/hxq/interface/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/
+-rw-rw-rw-   0        0        0      123 2023-04-13 13:04:22.000000 hxq-1.0.2/hxq/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/db/
+-rw-rw-rw-   0        0        0      383 2023-04-13 12:57:46.000000 hxq-1.0.2/hxq/libs/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/httpx/
+-rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.2/hxq/libs/httpx/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-13 14:06:06.000000 hxq-1.0.2/hxq/libs/httpx/chrome_agent.py
+-rw-rw-rw-   0        0        0     9254 2023-04-18 16:10:44.000000 hxq-1.0.2/hxq/libs/httpx/http.py
+-rw-rw-rw-   0        0        0     3420 2023-04-18 16:09:26.000000 hxq-1.0.2/hxq/libs/httpx/session.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/win32/
+-rw-rw-rw-   0        0        0     1983 2023-04-13 13:36:03.000000 hxq-1.0.2/hxq/libs/win32/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-04-18 16:10:11.000000 hxq-1.0.2/hxq/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/utils/
+-rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.2/hxq/utils/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-04-13 14:08:04.000000 hxq-1.0.2/hxq/utils/common.py
+-rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.2/hxq/utils/decorator.py
+-rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.2/hxq/utils/encipher.py
+-rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.2/hxq/utils/pic_code.py
+-rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.2/hxq/utils/ran_func.py
+-rw-rw-rw-   0        0        0     3460 2023-04-18 14:38:43.000000 hxq-1.0.2/hxq/utils/threadx.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 16:16:59.000000 hxq-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-04-18 16:12:50.000000 hxq-1.0.2/setup.py
```

### Comparing `hxq-1.0.1/hxq/interface/__init__.py` & `hxq-1.0.2/hxq/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2022/5/9 17:10
+# @Time    : 2023/4/18 23:00
 # @Author  : hxq
 # @Software: PyCharm
-# @File    : __init__.py
+# @File    : main.py
 from hxq.interface.db_helper import DBHelper
-from hxq.interface.httpx import http
+from hxq.interface.httpx import HTTP, http
 
 # if __name__ == '__main__':
 #     CONFIG = {
 #         'SQL_CREATOR': 'MySQL',
 #         'SQL_HOST': '127.0.0.1',
 #         'SQL_USER': 'root',
 #         'SQL_PASSWORD': '123456',
 #         'SQL_DATABASE': 'blog'
 #     }
 #     db = DBHelper(config=CONFIG)
 #     print(db.all("SHOW DATABASES;"))
 #     print(db.first("SELECT * FROM  rule_group"))
 
 if __name__ == '__main__':
-    http.download(
-        'https://infinitypro-img.infinitynewtab.com/wallpaper/nature/pad_nature_6.jpg?attname=infinity-328409872.jpg',
-        file_path='3284098721.jpg'
+    HTTP().download(
+        'https://infinitypro-img.infinitynewtab.com/wallpaper/travel/5596.jpg?attname=infinity-19779309.jpg'
     )
```

### Comparing `hxq-1.0.1/hxq/interface/db_helper.py` & `hxq-1.0.2/hxq/interface/db_helper.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/libs/httpx/chrome_agent.py` & `hxq-1.0.2/hxq/libs/httpx/chrome_agent.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/libs/httpx/http.py` & `hxq-1.0.2/hxq/libs/httpx/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/5/7 22:22
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : http.py
-import contextlib
 import importlib
 import sys
 import json
-from asyncio import sleep
 from functools import wraps
 from typing import Union, List
-
-import aiofiles
 from lxml import etree, html
 from requests.packages import urllib3
 from requests import Session, Response, exceptions
 from requests.cookies import cookiejar_from_dict, RequestsCookieJar
-
 from hxq.utils.common import run_event_loop
 
 if sys.version_info >= (3,):
-    from urllib.parse import urlencode
+    from urllib.parse import urlencode, urlparse
     from urllib import parse
 else:
     from urllib import urlencode, parse
 # 关闭错误提示
 urllib3.disable_warnings()
 
 
 @run_event_loop
 async def iter_write_file(file_path: str, r: Response):
+    import aiofiles
     async with aiofiles.open(file_path, 'wb') as file:
         for chunk in r.iter_content(1024 * 10):
             await file.write(chunk)
 
 
 def requests_catch_exception(func):
     """
@@ -178,51 +174,60 @@
         :param code: http状态码
         :param error_reason: http状态原因
         """
         self.ok = False
         self.code = code
         self.error_reason = error_reason
 
+    def close(self):
+        pass
+        # self.res.close()
+
     def __str__(self):
         return "HTTP {}: {}".format(self.code, self.error_reason)
 
 
 class HTTPRequest:
 
     @classmethod
     def get(cls, url, params=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         GET请求
         """
         kwargs.setdefault('allow_redirects', True)
-        with cls.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs) as r:
-            return r
+        r = cls.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
+        r.close()
+        return r
 
     @classmethod
     def post(cls, url, data=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         POST请求
         """
-        with cls.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs) as r:
-            return r
+        r = cls.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
+        r.close()
+        return r
 
     @classmethod
-    def download(cls, url, file_path, params=None, data=None, **kwargs):
+    def download(cls, url, file_path=None, params=None, data=None, **kwargs):
         """
         下载文件
         """
-        kwargs.setdefault('method', 'GET')
         kwargs['stream'] = True
-        with cls.request(kwargs['method'].upper(), url, params=params, data=data, **kwargs) as r:
-            if not r.ok:
-                return r.error_reason
-            iter_write_file(file_path, r.res)
+        request = kwargs.pop('request', cls.request)
+        r = request(kwargs.pop('method', "get").upper(), url, params=params, data=data, **kwargs)
+        if not r.ok:
+            return r.error_reason
+        if not file_path:
+            file_path = urlparse(r.res.url).path.split('/')[-1]
+        iter_write_file(file_path, r.res)
+        r.close()
+        return True
 
     @staticmethod
-    @contextlib.contextmanager
     @requests_catch_exception
     def request(method, url, **kwargs):
         """
         :param method: 大小不敏感，在Session内部upper统一转化为大写
         :param url: 地址
         :param kwargs:
         :return:
@@ -231,17 +236,16 @@
         kwargs.setdefault('ignore_status', True)
         ignore_status = kwargs.pop('ignore_status')
         ua = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 " \
              "Safari/537.36"
         kwargs.setdefault('headers', {"User-Agent": ua})
         results = HTTPResponse(Session().request(method, url, **kwargs))
         if not ignore_status and results.code != 200:
-            yield HTTPError(results.code, '请求状态错异常!')
-        yield results
-        results.close()
+            return HTTPError(results.code, '请求状态错异常!')
+        return results
 
     @staticmethod
     def cookiejar2dict(cookiejar: RequestsCookieJar) -> dict:
         """
         CookieJar转dict
         """
         return (lambda ck: [[ck.update({k: v}) for k, v in cookiejar.items()], ck][1])(dict())
```

### Comparing `hxq-1.0.1/hxq/libs/httpx/session.py` & `hxq-1.0.2/hxq/libs/httpx/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/5/7 22:35
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : session.py
-import contextlib
 from typing import Union
+from urllib.parse import urlparse
 
 from requests import Session
 from requests.structures import CaseInsensitiveDict
 from requests.utils import default_headers
 
-from hxq.libs.httpx.http import HTTPRequest, requests_catch_exception, HTTPResponse, HTTPError
+from hxq.libs.httpx.http import HTTPRequest, requests_catch_exception, HTTPResponse, HTTPError, iter_write_file
 from hxq.libs.httpx.chrome_agent import random_version
 
 
 class SessionRequest(HTTPRequest):
     """基于requests 方便日常使用的简单二次封装"""
 
     def __init__(self, ignore_status=True):
@@ -26,39 +26,45 @@
         self.ignore_status = ignore_status
 
     def get(self, url, params=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         GET请求
         """
         kwargs.setdefault('allow_redirects', True)
-        with self.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs) as r:
-            return r
+        r = self.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
+        r.close()
+        return r
 
     def post(self, url, data=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         POST请求
         """
-        with self.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs) as r:
-            return r
+        r = self.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
+        r.close()
+        return r
+
+    def download(self, url, file_path=None, params=None, data=None, **kwargs):
+        """
+        session 下载文件
+        """
+        return HTTPRequest.download(url, request=self.request, file_path=file_path, params=params, data=data, **kwargs)
 
-    @contextlib.contextmanager
     @requests_catch_exception
     def request(self, method, url, **kwargs):
         """
         :param method: 大小不敏感，在Session内部upper统一转化为大写
         :param url: 地址
         :param kwargs:
         :return:
         """
         # with self.__http.request(method, url, **kwargs) as r:
         results = HTTPResponse(self.__http.request(method, url, **kwargs))
         if not self.ignore_status and results.code != 200:
-            yield HTTPError(results.code, '请求状态错异常!')
-        yield results
-        results.close()
+            return HTTPError(results.code, '请求状态错异常!')
+        return results
 
     @property
     def cookies(self) -> dict:
         """
         读取cookies
         """
         return self.cookiejar2dict(self.__http.cookies)
```

### Comparing `hxq-1.0.1/hxq/libs/win32/__init__.py` & `hxq-1.0.2/hxq/libs/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/utils/common.py` & `hxq-1.0.2/hxq/utils/common.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/utils/decorator.py` & `hxq-1.0.2/hxq/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/utils/encipher.py` & `hxq-1.0.2/hxq/utils/encipher.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.1/hxq/utils/threadx.py` & `hxq-1.0.2/hxq/utils/threadx.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         self.__timer.cancel()
 
 
 # 多线程操作
 class ThreadX(Thread):
     lock = RLock()
 
-    def __init__(self, func: callable, *args, **options):
-        daemon = options.pop("daemon", False)
-        super().__init__(target=func, args=args, kwargs=options, name=func.__name__)
+    def __init__(self, func: callable, *args, **kwargs):
+        daemon = kwargs.pop("daemon", False)
+        super().__init__(target=func, args=args, kwargs=kwargs, name=func.__name__)
         self.setDaemon(daemon)
         self.start()
         self.__flag = Event()  # 用于暂停线程的标识
 
     def pause(self):
         """
         线程阻塞
```

### Comparing `hxq-1.0.1/hxq.egg-info/SOURCES.txt` & `hxq-1.0.2/hxq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 hxq/__init__.py
+hxq/main.py
 hxq.egg-info/PKG-INFO
 hxq.egg-info/SOURCES.txt
 hxq.egg-info/dependency_links.txt
 hxq.egg-info/requires.txt
 hxq.egg-info/top_level.txt
 hxq/interface/__init__.py
 hxq/interface/db_helper.py
```

### Comparing `hxq-1.0.1/setup.py` & `hxq-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(name='hxq',
       author='hxq',
-      version='1.0.1',
+      version='1.0.2',
       packages=find_packages(exclude=["*.demo", "*.demo.*", "tests", "demos"]),
       author_email='337168530@qq.com',
       description="这是一个python工具包",
       license="GPL",
       # 而 extras_require 这里仅表示该模块会依赖这些包,深度使用模块时，才会用到，这里需要你手动安装
       extras_require={
           'HTML': ["bs4>=0.0.1", "xmltodict>=1.2"],
       },
       # install_requires 在安装模块时会自动安装依赖包
       install_requires=[
           'requests>=2.24.0',
           'lxml>=4.9.2',
           'pymysql~=1.0.3',
           'DBUtils~=3.0.2',
+          'aiofiles~=23.1.0',
       ]
       )
```

