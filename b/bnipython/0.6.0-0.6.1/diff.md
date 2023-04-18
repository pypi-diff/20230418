# Comparing `tmp/bnipython-0.6.0.tar.gz` & `tmp/bnipython-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-4nzqzhe0/bnipython-0.6.0.tar", last modified: Fri Apr 14 09:13:26 2023, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-1kgvnvsx/bnipython-0.6.1.tar", last modified: Tue Apr 18 04:28:21 2023, max compression
```

## Comparing `bnipython-0.6.0.tar` & `bnipython-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.058801 bnipython-0.6.0/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.0/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-14 09:13:26.058397 bnipython-0.6.0/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11494 2023-04-14 08:52:10.000000 bnipython-0.6.0/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.045296 bnipython-0.6.0/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.048055 bnipython-0.6.0/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.049881 bnipython-0.6.0/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1056 2023-04-14 08:56:09.000000 bnipython-0.6.0/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.051244 bnipython-0.6.0/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-14 08:52:10.000000 bnipython-0.6.0/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.053787 bnipython-0.6.0/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1251 2023-04-14 08:52:51.000000 bnipython-0.6.0/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.0/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-14 08:52:10.000000 bnipython-0.6.0/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.047704 bnipython-0.6.0/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-14 09:13:26.000000 bnipython-0.6.0/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-14 09:13:26.058905 bnipython-0.6.0/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-14 09:12:57.000000 bnipython-0.6.0/setup.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-14 09:13:26.057023 bnipython-0.6.0/tests/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-14 08:52:16.000000 bnipython-0.6.0/tests/test_bni_client.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_one_gate_payment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_snap_bi.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.0/tests/test_util.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.791804 bnipython-0.6.1/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.1/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-18 04:28:21.791397 bnipython-0.6.1/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11494 2023-04-14 08:52:10.000000 bnipython-0.6.1/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.773775 bnipython-0.6.1/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.778638 bnipython-0.6.1/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.781592 bnipython-0.6.1/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 04:26:45.000000 bnipython-0.6.1/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.782933 bnipython-0.6.1/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-14 08:52:10.000000 bnipython-0.6.1/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.785141 bnipython-0.6.1/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.1/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-14 08:52:10.000000 bnipython-0.6.1/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.778166 bnipython-0.6.1/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 04:28:21.791976 bnipython-0.6.1/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 04:27:20.000000 bnipython-0.6.1/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.789980 bnipython-0.6.1/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-14 08:52:16.000000 bnipython-0.6.1/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_util.py
```

### Comparing `bnipython-0.6.0/LICENSE` & `bnipython-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/PKG-INFO` & `bnipython-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.0
+Version: 0.6.1
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.0/README.md` & `bnipython-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.1/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython/lib/api/snapBI.py` & `bnipython-0.6.1/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython/lib/bniClient.py` & `bnipython-0.6.1/bnipython/lib/bniClient.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
     def getConfig(self):
         return self.config
 
     def getBaseUrl(self):
         if self.config['env'] == 'dev':
             return constants.DEV_BASE_URL
+        elif self.config['env'] == 'uat':
+            return constants.UAT_BASE_URL
         elif self.config['env'] == 'sandbox':
             return constants.SANDBOX_BASE_URL
         elif self.config['env'] == 'sandbox-dev':
             return constants.SANDBOX_DEV_BASE_URL
         elif self.config['env'] == 'prod':
             return constants.PRODUCTION_BASE_URL
```

### Comparing `bnipython-0.6.0/bnipython/lib/net/httpClient.py` & `bnipython-0.6.1/bnipython/lib/net/httpClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython/lib/util/constants.py` & `bnipython-0.6.1/bnipython/lib/util/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 DEV_BASE_URL = 'https://newapidev.bni.co.id:8066';
+UAT_BASE_URL = 'https://newapidev.bni.co.id:8065';
 SANDBOX_BASE_URL = 'https://sandbox.bni.co.id';
-SANDBOX_DEV_BASE_URL = 'http://localhost:8080';
+SANDBOX_DEV_BASE_URL = 'https://sb-dev.harismawan.com';
 PRODUCTION_BASE_URL = 'https://api.bni.co.id';
 # DEV_OGP_URL = 'https://sandbox.harismawan.com'
 # DEV_SNAP_BI = 'https://dev.harismawan.com'
 TOKEN_JWT = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjbGllbnRJZCI6IklEQk5JVkdWemRDQkJVRkE9IiwiYWNjb3VudE5vIjoiMDExNTQ3NjExNyJ9.ljWtFHL0dHhLPw97U8SVWsFV3fRIJItHlQ-HPqCRUwc'
 APP_NAME = 'Test APP'
 APP_NAME_TEST = 'Test Wawat'
 
 CLIENT_ID_BASE64 = 'IDBNIVGVzdCBBUFA='
-API_SECRET = 'test-secret'
+API_SECRET = 'test-secret'  
 API_KEY = '12345'
 CLIENT_ID = 'test12345'
 CLIENT_SECRET = 'test54321'
 ACCOUNT_NO = '0115476117'
 
 CLIENT_ID_ENCRYPT = 'e7954df3-b67b-43e8-9d41-203600c04185'
 CLIENT_SECRET_ENCRYPT = 'a6d4f4db-ef4d-4521-982b-fbf4305e6eee'
```

### Comparing `bnipython-0.6.0/bnipython/lib/util/response.py` & `bnipython-0.6.1/bnipython/lib/util/response.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython/lib/util/utils.py` & `bnipython-0.6.1/bnipython/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.1/bnipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.0
+Version: 0.6.1
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.0/bnipython.egg-info/SOURCES.txt` & `bnipython-0.6.1/bnipython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/setup.py` & `bnipython-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.6.0",
+    version="0.6.1",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.6.0/tests/test_bni_client.py` & `bnipython-0.6.1/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/tests/test_one_gate_payment.py` & `bnipython-0.6.1/tests/test_one_gate_payment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/tests/test_snap_bi.py` & `bnipython-0.6.1/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.0/tests/test_util.py` & `bnipython-0.6.1/tests/test_util.py`

 * *Files identical despite different names*

