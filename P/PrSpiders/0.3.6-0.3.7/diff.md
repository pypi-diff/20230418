# Comparing `tmp/PrSpiders-0.3.6.tar.gz` & `tmp/PrSpiders-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.3.6.tar", last modified: Tue Apr 18 06:21:58 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.7.tar", last modified: Tue Apr 18 06:27:02 2023, max compression
```

## Comparing `PrSpiders-0.3.6.tar` & `PrSpiders-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:21:58.066411 PrSpiders-0.3.6/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:21:58.064415 PrSpiders-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.858409 PrSpiders-0.3.6/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.6/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.6/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.6/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.6/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.6/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.948411 PrSpiders-0.3.6/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.982412 PrSpiders-0.3.6/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-18 06:20:57.000000 PrSpiders-0.3.6/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:21:58.054412 PrSpiders-0.3.6/pkg/prspider/
--rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.3.6/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.6/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.6/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.6/pkg/prspider/start.py
--rw-rw-rw-   0        0        0       42 2023-04-18 06:21:58.066411 PrSpiders-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-18 06:21:04.000000 PrSpiders-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:27:02.003039 PrSpiders-0.3.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:27:01.999040 PrSpiders-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.900040 PrSpiders-0.3.7/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.7/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.7/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.7/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4461 2023-04-18 06:26:14.000000 PrSpiders-0.3.7/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.7/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.950041 PrSpiders-0.3.7/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.958039 PrSpiders-0.3.7/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-18 06:26:26.000000 PrSpiders-0.3.7/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.992041 PrSpiders-0.3.7/pkg/prspider/
+-rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.3.7/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.7/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.7/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.7/pkg/prspider/start.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:27:02.010041 PrSpiders-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-18 06:26:31.000000 PrSpiders-0.3.7/setup.py
```

### Comparing `PrSpiders-0.3.6/LICENSE.txt` & `PrSpiders-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/PKG-INFO` & `PrSpiders-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.6
+Version: 0.3.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.6/PrSpider/PrSpiders.py` & `PrSpiders-0.3.7/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/PrSpider/pxpath.py` & `PrSpiders-0.3.7/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/PrSpider/requestXpath.py` & `PrSpiders-0.3.7/PrSpider/requestXpath.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
    Author :        penr
    date:          2023/02/16
 -------------------------------------------------
    Change Activity:
                    2023/02/16:
 -------------------------------------------------
 """
-__author__ = 'penr'
+__author__ = "penr"
 __version__ = 0.1
-logging.basicConfig(format='%(message)s', level=logging.INFO)
+logging.basicConfig(format="%(message)s", level=logging.INFO)
 
 
 class prequest(Xpath):
     def __init__(self):
         self.response = Response()
         self.start_time = time.time()
 
@@ -37,55 +37,80 @@
         return get_ua()
 
     @property
     def header(self):
         """
         :return: basic header
         """
-        return {'user-agent': self.user_agent}
+        return {"user-agent": self.user_agent}
 
-    def get(self, url, headers=None, retry_time=3, method='GET', meta=None,
-            encoding='utf-8', retry_interval=1, timeout=3, settion=None, *args, **kwargs):
+    def get(
+        self,
+        url,
+        headers=None,
+        retry_time=3,
+        method="GET",
+        meta=None,
+        encoding="utf-8",
+        retry_interval=1,
+        timeout=3,
+        settion=None,
+        *args,
+        **kwargs,
+    ):
         """
         get method
         :param url: target url
         :param header: headers default:
         :param retry_time: retry time default: 3
         :param retry_interval: retry interval default: 1
         :param timeout: network timeout default: 3
         :return:
         """
 
-        self.current_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        self.current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         header = self.header
         self.method = method.upper()
         self.retry_time = retry_time
         self.retry_interval = retry_interval
         self.meta_ = meta
         if headers and isinstance(headers, dict):
-            if headers.get('user-agent') or headers.get('User-Agent'):
+            if headers.get("user-agent") or headers.get("User-Agent"):
                 header = {}
             header.update(headers)
-            print(header)
         while True:
             try:
                 self.response = requests.request(
-                    url=url, headers=header, timeout=timeout, method=self.method, *args, **kwargs)
+                    url=url,
+                    headers=header,
+                    timeout=timeout,
+                    method=self.method,
+                    *args,
+                    **kwargs,
+                )
                 self.response.encoding = encoding
                 if self.response.ok:
                     return self
                 else:
-                    raise Exception(f'Respider {self.retry_interval}s')
+                    raise Exception(f"Respider {self.retry_interval}s")
             except Exception as e:
-                logging.error('%s [ERRORS] [Url] %s [Msg] %s' % (self.current_time, url, e))
+                logging.error(
+                    "%s [ERRORS] [Url] %s [Msg] %s" % (self.current_time, url, e)
+                )
                 if settion.retry:
-                    logging.info('[Retry Url] %s [Interval] %ss' % (url, retry_interval))
+                    logging.info(
+                        "[Retry Url] %s [Interval] %ss" % (url, retry_interval)
+                    )
                 retry_time -= 1
                 if retry_time <= 0 or settion.retry is False:
-                    self.response.status_code = 410 if not self.response.status_code else self.response.status_code
+                    self.response.status_code = (
+                        410
+                        if not self.response.status_code
+                        else self.response.status_code
+                    )
                     return self
                 time.sleep(retry_interval)
 
     @property
     def text(self):
         return self.response.text
```

### Comparing `PrSpiders-0.3.6/PrSpider/useragent.py` & `PrSpiders-0.3.7/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.3.7/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.6
+Version: 0.3.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.6/README.md` & `PrSpiders-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.3.7/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.6/setup.py` & `PrSpiders-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

