# Comparing `tmp/bnipython-0.6.1.tar.gz` & `tmp/bnipython-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-1kgvnvsx/bnipython-0.6.1.tar", last modified: Tue Apr 18 04:28:21 2023, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-d8liuz4m/bnipython-0.6.2.tar", last modified: Tue Apr 18 04:34:48 2023, max compression
```

## Comparing `bnipython-0.6.1.tar` & `bnipython-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.791804 bnipython-0.6.1/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.1/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-18 04:28:21.791397 bnipython-0.6.1/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11494 2023-04-14 08:52:10.000000 bnipython-0.6.1/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.773775 bnipython-0.6.1/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.778638 bnipython-0.6.1/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.781592 bnipython-0.6.1/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 04:26:45.000000 bnipython-0.6.1/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.782933 bnipython-0.6.1/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-14 08:52:10.000000 bnipython-0.6.1/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.785141 bnipython-0.6.1/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.1/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.1/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-14 08:52:10.000000 bnipython-0.6.1/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.778166 bnipython-0.6.1/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12290 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 04:28:21.000000 bnipython-0.6.1/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 04:28:21.791976 bnipython-0.6.1/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 04:27:20.000000 bnipython-0.6.1/setup.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:28:21.789980 bnipython-0.6.1/tests/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-14 08:52:16.000000 bnipython-0.6.1/tests/test_bni_client.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_one_gate_payment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_snap_bi.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.1/tests/test_util.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.591406 bnipython-0.6.2/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.2/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2023-04-18 04:34:48.590858 bnipython-0.6.2/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11603 2023-04-18 04:33:04.000000 bnipython-0.6.2/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.573926 bnipython-0.6.2/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.580139 bnipython-0.6.2/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.582392 bnipython-0.6.2/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 04:33:00.000000 bnipython-0.6.2/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.584094 bnipython-0.6.2/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-18 04:32:36.000000 bnipython-0.6.2/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.586637 bnipython-0.6.2/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.2/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-18 04:32:36.000000 bnipython-0.6.2/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.579758 bnipython-0.6.2/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 04:34:48.591570 bnipython-0.6.2/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 04:33:56.000000 bnipython-0.6.2/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.589774 bnipython-0.6.2/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 04:32:36.000000 bnipython-0.6.2/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_util.py
```

### Comparing `bnipython-0.6.1/LICENSE` & `bnipython-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/PKG-INFO` & `bnipython-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.1
+Version: 0.6.2
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,22 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
+### 1.3 Using PyPI Install Third Party
+
+```
+pip install requests
+pip install pyOpenSSL
+pip install pytz
+```
+
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
```

### Comparing `bnipython-0.6.1/README.md` & `bnipython-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
+### 1.3 Using PyPI Install Third Party
+
+```
+pip install requests
+pip install pyOpenSSL
+pip install pytz
+```
+
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
```

### Comparing `bnipython-0.6.1/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.2/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/api/snapBI.py` & `bnipython-0.6.2/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/bniClient.py` & `bnipython-0.6.2/bnipython/lib/bniClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/net/httpClient.py` & `bnipython-0.6.2/bnipython/lib/net/httpClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/util/constants.py` & `bnipython-0.6.2/bnipython/lib/util/constants.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/util/response.py` & `bnipython-0.6.2/bnipython/lib/util/response.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython/lib/util/utils.py` & `bnipython-0.6.2/bnipython/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.2/bnipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.1
+Version: 0.6.2
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,14 +39,22 @@
 If you are not using PyPI, you can clone or [download](https://github.com/bni-api/bnipython/archive/refs/heads/main.zip) this repository.
 Then import from bnipython folder. Or run Pip install from the repo folder.
 
 ```
 pip install .
 ```
 
+### 1.3 Using PyPI Install Third Party
+
+```
+pip install requests
+pip install pyOpenSSL
+pip install pytz
+```
+
 ## 2. Usage
 
 ### 2.1 Choose an API Product
 
 We have 2 API products you can use:
 - [One Gate Payment](#22A-snap) - A solution for a company to integrate its application / system with banking transaction services. [documentation](https://digitalservices.bni.co.id/en/api-one-gate-payment)
 - [Snap BI](https://apidevportal.bi.go.id/snap/info) - Integrate with SNAP BI [documentation](https://apidevportal.bi.go.id/snap/api-services)
```

### Comparing `bnipython-0.6.1/bnipython.egg-info/SOURCES.txt` & `bnipython-0.6.2/bnipython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/setup.py` & `bnipython-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.6.1",
+    version="0.6.2",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.6.1/tests/test_bni_client.py` & `bnipython-0.6.2/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/tests/test_one_gate_payment.py` & `bnipython-0.6.2/tests/test_one_gate_payment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/tests/test_snap_bi.py` & `bnipython-0.6.2/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.1/tests/test_util.py` & `bnipython-0.6.2/tests/test_util.py`

 * *Files identical despite different names*

