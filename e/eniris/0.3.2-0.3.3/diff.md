# Comparing `tmp/eniris-0.3.2.tar.gz` & `tmp/eniris-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.3.2.tar", last modified: Sun Apr  2 22:49:50 2023, max compression
+gzip compressed data, was "eniris-0.3.3.tar", last modified: Tue Apr 18 11:50:11 2023, max compression
```

## Comparing `eniris-0.3.2.tar` & `eniris-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:49:50.758265 eniris-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-02 22:49:39.000000 eniris-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-02 22:49:50.758265 eniris-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-02 22:49:39.000000 eniris-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:49:50.758265 eniris-0.3.2/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-02 22:49:39.000000 eniris-0.3.2/eniris/ApiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 22:49:39.000000 eniris-0.3.2/eniris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:49:50.758265 eniris-0.3.2/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-02 22:49:50.000000 eniris-0.3.2/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-02 22:49:50.000000 eniris-0.3.2/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 22:49:50.000000 eniris-0.3.2/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-02 22:49:50.000000 eniris-0.3.2/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-02 22:49:50.000000 eniris-0.3.2/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 22:49:50.758265 eniris-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-02 22:49:39.000000 eniris-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 11:50:00.000000 eniris-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-18 11:50:11.643923 eniris-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-18 11:50:00.000000 eniris-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-18 11:50:00.000000 eniris-0.3.3/eniris/ApiDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:50:00.000000 eniris-0.3.3/eniris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:50:11.643923 eniris-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 11:50:00.000000 eniris-0.3.3/setup.py
```

### Comparing `eniris-0.3.2/LICENSE` & `eniris-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.3.2/PKG-INFO` & `eniris-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.3.2
+Version: 0.3.3
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.2.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -36,16 +36,18 @@
 ```
 ## Details
 The driver constructor accepts the following arguments:
 - username (string, required)
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
-- maxRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - timeoutS (int, optional, default: 60): Request timeout in seconds
+- maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
+- initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
+- maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.3.2/README.md` & `eniris-0.3.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 ```
 ## Details
 The driver constructor accepts the following arguments:
 - username (string, required)
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
-- maxRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - timeoutS (int, optional, default: 60): Request timeout in seconds
+- maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
+- initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
+- maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.3.2/eniris/ApiDriver.py` & `eniris-0.3.3/eniris/ApiDriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import datetime
 import requests
 import logging
+import time
 
 class AuthenticationFailure(Exception):
     "Raised when failing to authentiate to the Insights API"
     pass
     
 class RetryFailure(Exception):
     "Raised when authentication was succesful, an API call failed repeatedly"
     pass
 
 # Provide an easy interface to interact with the API, in the style of the requests library (https://docs.python-requests.org/en/master/)
 class ApiDriver:
-  def __init__(self, username:str, password:str, authUrl:str = 'https://authentication.eniris.be', apiUrl:str = 'https://api.eniris.be',  maxRetries:int = 5, timeoutS:int = 60):
+  def __init__(self, username:str, password:str, authUrl:str = 'https://authentication.eniris.be', apiUrl:str = 'https://api.eniris.be', timeoutS:int = 60, maximumRetries:int = 4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60):
     """Constructor. You must specify at least username and password or a credentialsPath where they are stored as a json of the form {'login': USERNAME, 'password': PASSWORD}
 
     Args:
         username (str, optional): Insights username
         password (str, optional): Insights password of the user
         authUrl (str, optional): Url of authentication endpoint. Defaults to https://authentication.eniris.be
         apiUrl (str, optional): Url of api endpoint. Defaults to https://api.eniris.be
-        maxRetries (int, optional): How many times to try again in case of a failure. Defaults to 5.
-        timeout (int, optional): API timeout in seconds. Defaults to 60.
+        timeoutS (int, optional): API timeout in seconds. Defaults to 60.
+        maximumRetries (int, optional): How many times to try again in case of a failure. Defaults to 4.
+        initialRetryDelayS (int, optional): The initial delay between successive retries in seconds. Defaults to 1.
+        maximumRetryDelayS (int, optional): The maximum delay between successive retries in seconds. Defaults to 60.
 
     Raises:
         Exception: _description_
     """
     self.username = username
     self.password = password
     self.authUrl = authUrl
     self.apiUrl = apiUrl
-    self.maxRetries = maxRetries
     self.timeoutS = timeoutS
+    self.maximumRetries = maximumRetries
+    self.initialRetryDelayS = initialRetryDelayS
+    self.maximumRetryDelayS = maximumRetryDelayS
     self.refreshDtAndToken = None
     self.accessDtAndToken = None
     
   def _authenticate(self):
     dt = datetime.datetime.now()
     if self.refreshDtAndToken is None or (dt - self.refreshDtAndToken[0]).total_seconds() > 13*24*60*60: # 13 days
       data = { "username": self.username, "password": self.password }
@@ -78,82 +83,89 @@
         path (str): Path relative to the apiUrl.
         params (dict, optional): URL parameters. Defaults to None.
         retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
-    if retryNr > self.maxRetries:
-      raise RetryFailure()
     self._authenticate()
     try:
       req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
       return requests.get(req_path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     except Exception as e:
-      logging.debug("Retrying after unexpected exception: " + str(e))
-      return self.get(path, params, retryNr+1)
+      if retryNr+1 > self.maximumRetries:
+        raise RetryFailure()
+      else:
+        logging.debug("Retrying after unexpected exception: " + str(e))
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        return self.get(path, params, retryNr+1)
   
   def post(self, path:str, json = None, params = None, data = None, retryNr = 0) -> requests.Response:
     """API POST call
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
         retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
-    if retryNr > self.maxRetries:
-      raise RetryFailure()
     self._authenticate()
     try:
       req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
       return requests.post(req_path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     except Exception as e:
-      logging.debug("Retrying after unexpected exception: " + str(e))
-      return self.post(path, json, params, data, retryNr+1)
+      if retryNr+1 > self.maximumRetries:
+        raise RetryFailure()
+      else:
+        logging.debug("Retrying after unexpected exception: " + str(e))
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        return self.post(path, json, params, data, retryNr+1)
     
   def put(self, path:str, json = None, params = None, data = None, retryNr = 0) -> requests.Response:
     """API PUT call
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
         retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
-    if retryNr > self.maxRetries:
-      raise RetryFailure()
     self._authenticate()
     try:
       req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
       return requests.put(req_path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     except Exception as e:
-      logging.debug("Retrying after unexpected exception: " + str(e))
-      return self.put(path, json, params, data, retryNr+1)
+      if retryNr > self.maximumRetries:
+        raise RetryFailure()
+      else:
+        logging.debug("Retrying after unexpected exception: " + str(e))
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        return self.put(path, json, params, data, retryNr+1)
   
   def delete(self, path:str, params = None, retryNr = 0) -> requests.Response:
     """API DELETE call
 
     Args:
         path (str): Path relative to the baseUrl.
         params (dict, optional): URL parameters. Defaults to None.
         retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
-    if retryNr > self.maxRetries:
-      raise RetryFailure()
     self._authenticate()
     try:
       req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
       return requests.delete(req_path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     except Exception as e:
-      logging.debug("Retrying after unexpected exception: " + str(e))
-      return self.delete(path, params, retryNr+1)
-
+      if retryNr > self.maximumRetries:
+        raise RetryFailure()
+      else:
+        logging.debug("Retrying after unexpected exception: " + str(e))
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        return self.delete(path, params, retryNr+1)
```

### Comparing `eniris-0.3.2/eniris.egg-info/PKG-INFO` & `eniris-0.3.3/eniris.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.3.2
+Version: 0.3.3
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.2.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -36,16 +36,18 @@
 ```
 ## Details
 The driver constructor accepts the following arguments:
 - username (string, required)
 - password (string, required)
 - authUrl (string, optional, default: 'https://authentication.eniris.be'): URL of authentication endpoint
 - apiUrl (string, optional, default: 'https://api.eniris.be'): URL of api endpoint
-- maxRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - timeoutS (int, optional, default: 60): Request timeout in seconds
+- maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
+- initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
+- maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 
 Furthermore, the following methods are exposed:
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
```

### Comparing `eniris-0.3.2/setup.py` & `eniris-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.3.2',
+  version = '0.3.3',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.2.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

