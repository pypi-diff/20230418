# Comparing `tmp/pymorpheus-0.1.5.tar.gz` & `tmp/pymorpheus-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymorpheus-0.1.5.tar", last modified: Thu Sep  5 23:37:53 2019, max compression
+gzip compressed data, was "/home/ncelebic/dev/pymorpheus/dist/tmpic4ktpwv/pymorpheus-0.1.6.tar", last modified: Tue Apr 18 14:23:36 2023, max compression
```

## Comparing `pymorpheus-0.1.5.tar` & `pymorpheus-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/
--rw-rw-rw-   0        0        0     1699 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2019-09-04 17:22:11.000000 pymorpheus-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus/
--rw-rw-rw-   0        0        0     4960 2019-09-04 17:00:17.000000 pymorpheus-0.1.5/pymorpheus/__init__.py
-drwxrwxrwx   0        0        0        0 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/
--rw-rw-rw-   0        0        0     1699 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/pymorpheus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-09-05 23:37:53.000000 pymorpheus-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      661 2019-09-04 16:51:13.000000 pymorpheus-0.1.5/setup.py
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus/
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     4991 2023-04-18 13:55:11.000000 pymorpheus-0.1.6/pymorpheus/__init__.py
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     1399 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/PKG-INFO
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      222 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/SOURCES.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)        1 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/dependency_links.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       17 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/requires.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       11 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/pymorpheus.egg-info/top_level.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     1068 2021-05-20 13:38:46.000000 pymorpheus-0.1.6/LICENSE.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      977 2021-05-20 13:38:46.000000 pymorpheus-0.1.6/README.md
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      661 2023-03-31 18:40:04.000000 pymorpheus-0.1.6/setup.py
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     1399 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/PKG-INFO
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       38 2023-04-18 14:23:36.000000 pymorpheus-0.1.6/setup.cfg
```

### Comparing `pymorpheus-0.1.5/README.md` & `pymorpheus-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 ## Installation
 
 `pip install pymorpheus`
 
 ## Usage 
 
-MorpheusClient() will either retrieve a token (with username and password args), or use an existing token (with token arg).  Use `sslverify=False` to bypass certificate validation.
+MorpheusClient() will either retrieve a token (with username and password args), or use an existing token (with token arg)
+Use `sslverify=False` to bypass certificate validation.
 
 MorpheusClient.call() accepts the following vars:
 - Required (positional):
   - method: one of string: get, post, put, delete
   - path: api call path after /api/
 - Optional:
   - options: list of tuples eg. `[('max','50')]`
   - jsonpayload: JSON string of payload for POST/PUT methods
 
 Reference at https://bertramdev.github.io/morpheus-apidoc
 
-```
-from pymorpheus import MorpheusClient
+```from pymorpheus import MorpheusClient
+
 morpheus = MorpheusClient("https://yoururl", username="youruser", password="yourpass")
-options = [('max', '10')]
-results = morpheus.call("get", "instances", options=options)
+results = morpheus.call("get", path="instances")
 print(results)
 # JSON Output of results
 ```
```

### Comparing `pymorpheus-0.1.5/pymorpheus/__init__.py` & `pymorpheus-0.1.6/pymorpheus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """
 
 import requests
 import urllib3
 import logging
 import json
 
-name = "pymorpheus"
-
 logger = logging.getLogger(__name__)
 
+name = "MorpheusClient"
+
 
 class MorpheusClientException(Exception):
     """ Base Exception Class """
 
 
 class MethodTypeError(MorpheusClientException):
     """ Exception for bad HTTP request type """
@@ -93,21 +93,21 @@
 
         :return: API Token
         :rtype: str
         """
         return self.token
 
     def _send_call(self, method, path, **kwargs):
-        logger.debug('Calling method: %r to %r with %r' % (method, path, kwargs))
+        print('Calling method: %r to %r with %r' % (method, path, kwargs))
 
         url = ""
         method = method.lower()
 
         if method not in dir(requests.api):
-            logger.error("bad method type: %s" % method)
+            print("bad method type: %s" % method)
             raise MethodTypeError
 
         try:
             if not path.startswith("/"):
                 path = "/" + path
 
             options = ""
@@ -118,39 +118,44 @@
 
             json_string = ""
 
             if "jsonpayload" in kwargs:
                 try:
                     json_string = json.loads(kwargs['jsonpayload'])
                 except ValueError as e:
-                    logger.error("Invalid JSON string passed:")
-                    logger.error(kwargs['jsonpayload'])
-                    logger.error(e)
+                    print("Invalid JSON string passed:")
+                    print(kwargs['jsonpayload'])
+                    print(e)
 
             url = self.morpheus_api + path + "?" + options
-            logger.debug(url)
+            print(url)
 
             r = getattr(requests, method)(url,
                                           headers=self.headers,
                                           verify=self.sslverify,
                                           json=json_string)
+            
+            if r.status_code != 200:
+                print(r.text)
+                raise requests.HTTPError(r)
+
             return r.json()
 
         except requests.ConnectionError as cerr:
-            logger.error("Connection Error: ", cerr)
-            logger.error(url)
+            print("Connection Error: ", cerr)
+            print(url)
         except requests.HTTPError as herr:
-            logger.error("Bad status code returned: ", herr)
-            logger.error(url)
+            print("Bad status code returned: ", herr)
+            print(url)
         except requests.Timeout as terr:
-            logger.error("Timeout: ", terr)
-            logger.error(url)
+            print("Timeout: ", terr)
+            print(url)
         except requests.exceptions.RequestException as err:
-            logger.error("Requests: Something went wrong: ", err)
-            logger.error(url)
+            print("Requests: Something went wrong: ", err)
+            print(url)
 
     def call(self, method, path, **kwargs):
         """
         Calls an API path
 
         :param method: URL request method
         :type method: str
```

### Comparing `pymorpheus-0.1.5/setup.py` & `pymorpheus-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pymorpheus',
-    version='0.1.5',
+    version='0.1.6',
     description='Morpheus API wrapper for Python 3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Nick Celebic',
     author_email='nick@celebic.net',
     license='MIT License',
     packages=setuptools.find_packages(),
```

