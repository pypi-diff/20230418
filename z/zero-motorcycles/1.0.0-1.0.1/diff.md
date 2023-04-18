# Comparing `tmp/zero_motorcycles-1.0.0.tar.gz` & `tmp/zero_motorcycles-1.0.1.tar.gz`

## Comparing `zero_motorcycles-1.0.0.tar` & `zero_motorcycles-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/test.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/zero_motorcycles/Zero.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/zero_motorcycles/__about__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/zero_motorcycles/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/README.md
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/zero_motorcycles/Zero.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/zero_motorcycles/__about__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/zero_motorcycles/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/README.md
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 zero_motorcycles-1.0.1/PKG-INFO
```

### Comparing `zero_motorcycles-1.0.0/zero_motorcycles/Zero.py` & `zero_motorcycles-1.0.1/zero_motorcycles/Zero.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 # SPDX-FileCopyrightText: 2023-present Matt Zuba <matt.zuba@gmail.com>
 #
-# SPDX-License-Identifier: BSD-3-clause
+# SPDX-License-Identifier: BSD-3-Clause
+
 import base64
 from hashlib import md5
 import json
 import requests.auth
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 from Crypto.Random import get_random_bytes
+from requests.exceptions import HTTPError
 
 
 class Zero:
     API_URL = 'https://api-us-cypherstore-prod.zeromotorcycles.com/starcom/v1'
 
     def __init__(self, username, password):
         self.auth = ZeroAuth(username, password)
         pass
 
-    def get_units(self):
+    async def get_units(self):
         data = {
             "commandname": "get_units"
         }
 
-        return self._make_request(data).json()
+        return self._make_request(data)
 
-    def get_last_transmit(self, unit):
+    async def get_last_transmit(self, unit):
         data = {
             "unitnumber": unit,
             "commandname": "get_last_transmit"
         }
 
-        return self._make_request(data).json()
+        return self._make_request(data)
 
-    def get_expiration_date(self, unit):
+    async def get_expiration_date(self, unit):
         data = {
             "unitnumber": unit,
             "unittype": 5,
             "commandname": "get_expiration_date"
         }
 
-        return self._make_request(data).json()
+        return self._make_request(data)
 
     def _make_request(self, data):
-        return requests.post(self.API_URL, json=data, auth=self.auth, headers={"User-Agent": "ZeroMoto/1.0"})
+        response = requests.post(self.API_URL, json=data, auth=self.auth, headers={"User-Agent": "ZeroMoto/1.0"})
+
+        # Check for the usual errors
+        response.raise_for_status()
+
+        json_data = response.json()
+
+        if response.status_code >= 600:
+            raise HTTPError(json_data['error'], response=response)
+
+        return json_data
 
 
 class ZeroAuth(requests.auth.AuthBase):
     ENCRYPTION_KEY = "8FA043AADEC92367108D0E25D2C6064F"
     SOURCE = "zero"
     FORMAT = "json"
```

### Comparing `zero_motorcycles-1.0.0/LICENSE.txt` & `zero_motorcycles-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zero_motorcycles-1.0.0/README.md` & `zero_motorcycles-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zero_motorcycles-1.0.0/pyproject.toml` & `zero_motorcycles-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zero_motorcycles-1.0.0/PKG-INFO` & `zero_motorcycles-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zero-motorcycles
-Version: 1.0.0
+Version: 1.0.1
 Project-URL: Documentation, https://github.com/mattzuba/zero-motorcycles#readme
 Project-URL: Issues, https://github.com/mattzuba/zero-motorcycles/issues
 Project-URL: Source, https://github.com/mattzuba/zero-motorcycles
 Author-email: Matt Zuba <matt.zuba@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

