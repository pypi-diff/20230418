# Comparing `tmp/bnipython-0.6.2.tar.gz` & `tmp/bnipython-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-d8liuz4m/bnipython-0.6.2.tar", last modified: Tue Apr 18 04:34:48 2023, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-z9ikt7mw/bnipython-0.6.3.tar", last modified: Tue Apr 18 07:41:55 2023, max compression
```

## Comparing `bnipython-0.6.2.tar` & `bnipython-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.591406 bnipython-0.6.2/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.2/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2023-04-18 04:34:48.590858 bnipython-0.6.2/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11603 2023-04-18 04:33:04.000000 bnipython-0.6.2/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.573926 bnipython-0.6.2/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.580139 bnipython-0.6.2/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.582392 bnipython-0.6.2/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 04:33:00.000000 bnipython-0.6.2/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.584094 bnipython-0.6.2/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3304 2023-04-18 04:32:36.000000 bnipython-0.6.2/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.586637 bnipython-0.6.2/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.2/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1167 2023-04-14 08:10:12.000000 bnipython-0.6.2/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-18 04:32:36.000000 bnipython-0.6.2/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.579758 bnipython-0.6.2/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12399 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 04:34:48.000000 bnipython-0.6.2/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 04:34:48.591570 bnipython-0.6.2/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 04:33:56.000000 bnipython-0.6.2/setup.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 04:34:48.589774 bnipython-0.6.2/tests/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 04:32:36.000000 bnipython-0.6.2/tests/test_bni_client.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    10112 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_one_gate_payment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_snap_bi.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.2/tests/test_util.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.294249 bnipython-0.6.3/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.3/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-04-18 07:41:55.293815 bnipython-0.6.3/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11599 2023-04-18 07:38:12.000000 bnipython-0.6.3/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.279668 bnipython-0.6.3/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.3/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.282934 bnipython-0.6.3/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.284536 bnipython-0.6.3/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-18 07:21:08.000000 bnipython-0.6.3/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.3/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 06:59:40.000000 bnipython-0.6.3/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.286029 bnipython-0.6.3/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2023-04-18 06:59:48.000000 bnipython-0.6.3/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.289053 bnipython-0.6.3/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.3/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1255 2023-04-18 07:30:10.000000 bnipython-0.6.3/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-18 06:59:40.000000 bnipython-0.6.3/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.282046 bnipython-0.6.3/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 07:41:55.294651 bnipython-0.6.3/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 07:39:28.000000 bnipython-0.6.3/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.293032 bnipython-0.6.3/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 06:59:40.000000 bnipython-0.6.3/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10315 2023-04-18 07:37:16.000000 bnipython-0.6.3/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.3/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.3/tests/test_util.py
```

### Comparing `bnipython-0.6.2/LICENSE` & `bnipython-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/PKG-INFO` & `bnipython-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.2
+Version: 0.6.3
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -143,18 +143,18 @@
 })
 ```
 
 #### Get Inter Bank Inquiry
 ```python
 # return as Object
 getInterBankInquiry = ogp.getInterBankInquiry({
-  'customerReferenceNumber': '20170227000000000021', # max 20 char client defined reference number
-  'accountNum': '113183203',
+  'customerReferenceNumber': '20180930112233003', # max 20 char client defined reference number
+  'accountNum': '0115476117',
   'destinationBankCode': '014',
-  'destinationAccountNum': '3333333333'
+  'destinationAccountNum': '01400000'
 })
 ```
 
 #### Get Inter Bank Payment
 ```python
 # return as Object
 getInterBankPayment = ogp.getInterBankPayment({
```

### Comparing `bnipython-0.6.2/README.md` & `bnipython-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,18 @@
 })
 ```
 
 #### Get Inter Bank Inquiry
 ```python
 # return as Object
 getInterBankInquiry = ogp.getInterBankInquiry({
-  'customerReferenceNumber': '20170227000000000021', # max 20 char client defined reference number
-  'accountNum': '113183203',
+  'customerReferenceNumber': '20180930112233003', # max 20 char client defined reference number
+  'accountNum': '0115476117',
   'destinationBankCode': '014',
-  'destinationAccountNum': '3333333333'
+  'destinationAccountNum': '01400000'
 })
 ```
 
 #### Get Inter Bank Payment
 ```python
 # return as Object
 getInterBankPayment = ogp.getInterBankPayment({
```

### Comparing `bnipython-0.6.2/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.3/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/bnipython/lib/api/snapBI.py` & `bnipython-0.6.3/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/bnipython/lib/bniClient.py` & `bnipython-0.6.3/bnipython/lib/bniClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/bnipython/lib/net/httpClient.py` & `bnipython-0.6.3/bnipython/lib/net/httpClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             'Content-Type': 'application/x-www-form-urlencoded'
         }
         payload = 'grant_type=client_credentials'
 
         httpClient.request('POST', options['path'], payload, headers)
         res = httpClient.getresponse()
         data = res.read()
-        print(data)
         return json.loads(str(data.decode('utf-8')))
 
     def request(self, options={'method', 'apiKey', 'accessToken', 'url', 'path', 'data'}):
         url = str(options['url']).replace(
             'http://', '').replace('https://', '')
         httpClient = http.client.HTTPSConnection(
             url, context=ssl._create_unverified_context())
```

### Comparing `bnipython-0.6.2/bnipython/lib/util/constants.py` & `bnipython-0.6.3/bnipython/lib/util/constants.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/bnipython/lib/util/response.py` & `bnipython-0.6.3/bnipython/lib/util/response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 def responseOGP(params={'res', 'resObj'}):
     try:
         if (params['res'][params['resObj']]['parameters']['responseCode'] != '0001'):
-            code = params['res'][params['resObj']
-                                 ]['parameters']['responseCode']
-            message = params['res'][params['resObj']
-                                    ]['parameters']['responseMessage']
-            raise ValueError(f'{code}:{message}')
+            code = params['res'][params['resObj']]['parameters']['responseCode']
+            responseMessage = params['res'][params['resObj']]['parameters']['responseMessage']
+            errorMessage = params['res'][params['resObj']]['parameters']['errorMessage']
+            raise ValueError(f'errorMessage: {errorMessage}, responseMessage: {responseMessage}, code: {code}')
         else:
             return params['res']
     except Exception:
         code = params['res']['Response']['parameters']['responseCode']
         message = params['res']['Response']['parameters']['responseMessage']
         raise ValueError(f'{code}:{message}')
```

### Comparing `bnipython-0.6.2/bnipython/lib/util/utils.py` & `bnipython-0.6.3/bnipython/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.3/bnipython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.2
+Version: 0.6.3
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -143,18 +143,18 @@
 })
 ```
 
 #### Get Inter Bank Inquiry
 ```python
 # return as Object
 getInterBankInquiry = ogp.getInterBankInquiry({
-  'customerReferenceNumber': '20170227000000000021', # max 20 char client defined reference number
-  'accountNum': '113183203',
+  'customerReferenceNumber': '20180930112233003', # max 20 char client defined reference number
+  'accountNum': '0115476117',
   'destinationBankCode': '014',
-  'destinationAccountNum': '3333333333'
+  'destinationAccountNum': '01400000'
 })
 ```
 
 #### Get Inter Bank Payment
 ```python
 # return as Object
 getInterBankPayment = ogp.getInterBankPayment({
```

### Comparing `bnipython-0.6.2/bnipython.egg-info/SOURCES.txt` & `bnipython-0.6.3/bnipython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/setup.py` & `bnipython-0.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.6.2",
+    version="0.6.3",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.6.2/tests/test_bni_client.py` & `bnipython-0.6.3/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/tests/test_one_gate_payment.py` & `bnipython-0.6.3/tests/test_one_gate_payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,121 +121,121 @@
             'bankReference': '657364',
             'holdTransactionDate': '31052010'
         })
         self.assertEqual(res['holdAmountReleaseResponse']
                          ['parameters']['responseCode'], '0001')
         print('should return responseCode 0001')
 
-    ###################### CASES NEGATIVE #####################
+    ##################### CASES NEGATIVE #####################
 
-    def testGetBalanceNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.getBalance({
-            'accountNo': '1154711FF'
-        })
-        data = res['getBalanceResponse']['parameters']['responseCode']
-        self.assertEqual(data, '0001')
-        print('should return responseCode 0001')
-
-    def testGetInHouseInquiryNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.getInHouseInquiry({
-            'accountNo': '1154711FF'
-        })
-        self.assertEqual(res['getInHouseInquiryResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
-
-    def testDoPaymentNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.doPayment({
-            'customerReferenceNumber': '201702270000000000FF',
-            'paymentMethod': '0',
-            'debitAccountNo': '113183203',
-            'creditAccountNo': '115471119',
-            'valueDate': '20170227000000000',
-            'valueCurrency': 'IDR',
-            'valueAmount': 100500,
-            'remark': '?',
-            'beneficiaryEmailAddress': '',
-            'beneficiaryName': 'Mr.X',
-            'beneficiaryAddress1': 'Jakarta',
-            'beneficiaryAddress2': '',
-            'destinationBankCode': 'CENAIDJAXXX',
-            'chargingModelId': 'OUR'
-        })
-        self.assertEqual(res['doPaymentResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
-
-    def testPaymentStatusNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.getPaymentStatus({
-            'customerReferenceNumber': '201702270000000000FF',
-        })
-        self.assertEqual(res['getPaymentStatusResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
-
-    def testGetInterbankInquiry(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.getInterBankInquiry({
-            'customerReferenceNumber': '201809301122330FF',
-            'accountNum': '0115476117',
-            'destinationBankCode': '014',
-            'destinationAccountNum': '01400000'
-        })
-        self.assertEqual(res['getInterbankInquiryResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
+    # def testGetBalanceNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.getBalance({
+    #         'accountNo': '1154711FF'
+    #     })
+    #     data = res['getBalanceResponse']['parameters']['responseCode']
+    #     self.assertEqual(data, '0001')
+    #     print('should return responseCode 0001')
+
+    # def testGetInHouseInquiryNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.getInHouseInquiry({
+    #         'accountNo': '1154711FF'
+    #     })
+    #     self.assertEqual(res['getInHouseInquiryResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
+
+    # def testDoPaymentNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.doPayment({
+    #         'customerReferenceNumber': '201702270000000000FF',
+    #         'paymentMethod': '0',
+    #         'debitAccountNo': '113183203',
+    #         'creditAccountNo': '115471119',
+    #         'valueDate': '20170227000000000',
+    #         'valueCurrency': 'IDR',
+    #         'valueAmount': 100500,
+    #         'remark': '?',
+    #         'beneficiaryEmailAddress': '',
+    #         'beneficiaryName': 'Mr.X',
+    #         'beneficiaryAddress1': 'Jakarta',
+    #         'beneficiaryAddress2': '',
+    #         'destinationBankCode': 'CENAIDJAXXX',
+    #         'chargingModelId': 'OUR'
+    #     })
+    #     self.assertEqual(res['doPaymentResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
+
+    # def testPaymentStatusNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.getPaymentStatus({
+    #         'customerReferenceNumber': '201702270000000000FF',
+    #     })
+    #     self.assertEqual(res['getPaymentStatusResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
+
+    # def testGetInterbankInquiry(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.getInterBankInquiry({
+    #         'customerReferenceNumber': '201809301122330FF',
+    #         'accountNum': '0115476117',
+    #         'destinationBankCode': '014',
+    #         'destinationAccountNum': '01400000'
+    #     })
+    #     self.assertEqual(res['getInterbankInquiryResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
     
-    def testGetInterBankPaymentNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.getInterBankPayment({
-            'customerReferenceNumber': '201809301122330FF',
-            'amount': '12007',
-            'destinationAccountNum': '01400000',
-            'destinationAccountName': 'Bpk HANS',
-            'destinationBankCode': '014',
-            'destinationBankName': 'BCA',
-            'accountNum': '0316031099',
-            'retrievalReffNum': '100000000097'
-        })
-        self.assertEqual(res['getInterbankPaymentResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
-
-    def testHoldAmount(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.holdAmount({
-            'customerReferenceNumber': '201810011122330FF',
-            'amount': '12007',
-            'accountNo': '0115476151',
-            'detail': 'testHold'
-        })
-        self.assertEqual(res['holdAmountResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
-
-    def testHoldAmountReleaseNegative(self):
-        print('\n==============================================')
-        one_gate_payment = OneGatePayment(self.client)
-        res = one_gate_payment.holdAmountRelease({
-            'customerReferenceNumber': '20181001112233010',
-            'amount': '12007',
-            'accountNo': '0115476151',
-            'bankReference': '657364',
-            'holdTransactionDate': '31052010'
-        })
-        self.assertEqual(res['holdAmountReleaseResponse']
-                         ['parameters']['responseCode'], '0001')
-        print('should return responseCode 0001')
+    # def testGetInterBankPaymentNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.getInterBankPayment({
+    #         'customerReferenceNumber': '201809301122330FF',
+    #         'amount': '12007',
+    #         'destinationAccountNum': '01400000',
+    #         'destinationAccountName': 'Bpk HANS',
+    #         'destinationBankCode': '014',
+    #         'destinationBankName': 'BCA',
+    #         'accountNum': '0316031099',
+    #         'retrievalReffNum': '100000000097'
+    #     })
+    #     self.assertEqual(res['getInterbankPaymentResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
+
+    # def testHoldAmount(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.holdAmount({
+    #         'customerReferenceNumber': '201810011122330FF',
+    #         'amount': '12007',
+    #         'accountNo': '0115476151',
+    #         'detail': 'testHold'
+    #     })
+    #     self.assertEqual(res['holdAmountResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
+
+    # def testHoldAmountReleaseNegative(self):
+    #     print('\n==============================================')
+    #     one_gate_payment = OneGatePayment(self.client)
+    #     res = one_gate_payment.holdAmountRelease({
+    #         'customerReferenceNumber': '20181001112233010',
+    #         'amount': '12007',
+    #         'accountNo': '0115476151',
+    #         'bankReference': '657364',
+    #         'holdTransactionDate': '31052010'
+    #     })
+    #     self.assertEqual(res['holdAmountReleaseResponse']
+    #                      ['parameters']['responseCode'], '0001')
+    #     print('should return responseCode 0001')
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bnipython-0.6.2/tests/test_snap_bi.py` & `bnipython-0.6.3/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.2/tests/test_util.py` & `bnipython-0.6.3/tests/test_util.py`

 * *Files identical despite different names*

