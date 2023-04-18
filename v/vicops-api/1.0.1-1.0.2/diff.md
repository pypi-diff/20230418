# Comparing `tmp/vicops_api-1.0.1.tar.gz` & `tmp/vicops_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicops_api-1.0.1.tar", last modified: Sat Mar  4 15:38:17 2023, max compression
+gzip compressed data, was "vicops_api-1.0.2.tar", last modified: Tue Apr 18 15:20:40 2023, max compression
```

## Comparing `vicops_api-1.0.1.tar` & `vicops_api-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 15:38:17.634734 vicops_api-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-03-04 14:34:18.000000 vicops_api-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      527 2023-03-04 15:38:17.634228 vicops_api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-03-04 15:36:21.000000 vicops_api-1.0.1/README.md
--rw-rw-rw-   0        0        0       99 2023-03-04 15:18:20.000000 vicops_api-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-04 15:38:17.634734 vicops_api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-03-04 15:38:15.000000 vicops_api-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-04 15:38:17.623614 vicops_api-1.0.1/vicops_api/
--rw-rw-rw-   0        0        0      126 2023-03-04 15:15:33.000000 vicops_api-1.0.1/vicops_api/__init__.py
--rw-rw-rw-   0        0        0     3993 2023-03-04 15:12:04.000000 vicops_api-1.0.1/vicops_api/main.py
-drwxrwxrwx   0        0        0        0 2023-03-04 15:38:17.633215 vicops_api-1.0.1/vicops_api.egg-info/
--rw-rw-rw-   0        0        0      527 2023-03-04 15:38:17.000000 vicops_api-1.0.1/vicops_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-03-04 15:38:17.000000 vicops_api-1.0.1/vicops_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 15:38:17.000000 vicops_api-1.0.1/vicops_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-04 15:38:17.000000 vicops_api-1.0.1/vicops_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-04 15:38:17.000000 vicops_api-1.0.1/vicops_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.897432 vicops_api-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-03-04 14:34:18.000000 vicops_api-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      527 2023-04-18 15:20:40.896430 vicops_api-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-03-04 15:36:21.000000 vicops_api-1.0.2/README.md
+-rw-rw-rw-   0        0        0       99 2023-03-04 15:18:20.000000 vicops_api-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 15:20:40.897432 vicops_api-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-04-18 15:16:27.000000 vicops_api-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.885431 vicops_api-1.0.2/vicops_api/
+-rw-rw-rw-   0        0        0      126 2023-04-18 15:19:30.000000 vicops_api-1.0.2/vicops_api/__init__.py
+-rw-rw-rw-   0        0        0     4623 2023-04-18 15:16:35.000000 vicops_api-1.0.2/vicops_api/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.896430 vicops_api-1.0.2/vicops_api.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/top_level.txt
```

### Comparing `vicops_api-1.0.1/LICENSE` & `vicops_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vicops_api-1.0.1/PKG-INFO` & `vicops_api-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicops_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: python api wrapper for vicops2
 Home-page: https://github.com/ERTH2/vicops-api-py
 Author: artegoser
 License: MIT
 Project-URL: Source Code, https://github.com/ERTH2/vicops-api-py
 Keywords: api,wrapper,vicops
 Requires-Python: >=3.10
```

### Comparing `vicops_api-1.0.1/setup.py` & `vicops_api-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
-with open('README.md', 'r', encoding='utf-8') as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='vicops_api',
-    author='artegoser',
-    description='python api wrapper for vicops2',
-    keywords='api, wrapper, vicops',
+    name="vicops_api",
+    author="artegoser",
+    description="python api wrapper for vicops2",
+    keywords="api, wrapper, vicops",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    license='MIT',
-    url='https://github.com/ERTH2/vicops-api-py',
+    long_description_content_type="text/markdown",
+    license="MIT",
+    url="https://github.com/ERTH2/vicops-api-py",
     project_urls={
-        'Source Code': 'https://github.com/ERTH2/vicops-api-py',
+        "Source Code": "https://github.com/ERTH2/vicops-api-py",
     },
-    version="1.0.1",
+    version="1.0.2",
     packages=["vicops_api"],
-    python_requires='>=3.10',
-    install_requires=['requests'],
+    python_requires=">=3.10",
+    install_requires=["requests"],
 )
```

### Comparing `vicops_api-1.0.1/vicops_api/main.py` & `vicops_api-1.0.2/vicops_api/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 
 
 class VicopsApi:
-    def __init__(self, host: str = "https://vicops.mooo.com"):
+    def __init__(self, host: str = "https://vicops.artegoser.ru"):
         self.host = host
 
     def _getPost(self, url: str, body: object = {}) -> object:
         body["jwt"] = self.jwt
 
         res = requests.post(f"{self.host}{url}", data=body)
 
@@ -35,84 +35,131 @@
         if resp.code != "denied":
             self.jwt = resp.token
         return resp
 
     def connectJwt(self, jwt: str) -> object:
         self.jwt = jwt
 
-    def register(self, name: str, second_name: str, password: str, country: str, type: str, contact: str) -> object:
+    def register(
+        self,
+        name: str,
+        second_name: str,
+        password: str,
+        country: str,
+        type: str,
+        contact: str,
+    ) -> object:
         return self._checkRespAndAddJWT(
-            self._getPost("/api/register", {
-                "name": name,
-                "second_name": second_name,
-                "password": password,
-                "country": country,
-                "type": type,
-                "contact": contact,
-            })
+            self._getPost(
+                "/api/register",
+                {
+                    "name": name,
+                    "second_name": second_name,
+                    "password": password,
+                    "country": country,
+                    "type": type,
+                    "contact": contact,
+                },
+            )
         )
 
-    def transaction(self, recipient_id: str, amount: float, currency_id: str, description: str = "", type: str = "transfer") -> object:
-        return self._getPost("/api/transaction", {
-            "recipient_id": recipient_id,
-            "amount": amount,
-            "currency_id": currency_id,
-            "description": description,
-            "type": type,
-        })
+    def transaction(
+        self,
+        recipient_id: str,
+        amount: float,
+        currency_id: str,
+        description: str = "",
+        type: str = "transfer",
+    ) -> object:
+        return self._getPost(
+            "/api/transaction",
+            {
+                "recipient_id": recipient_id,
+                "amount": amount,
+                "currency_id": currency_id,
+                "description": description,
+                "type": type,
+            },
+        )
 
     def getUser(self) -> object:
         return self._getPost("/api/user")
 
     def getCurrencies(self) -> object:
         return self._getGet("/api/currencies")
 
     def approveUser(self, user_id: str) -> object:
         return self._getPost(f"/api/approve", {"user_id": user_id})
 
-    def addCurrency(self, _id: str, name: str, description: str, type: str, img: str) -> object:
-        return self._getPost(f"/api/add_currency", {
-            "_id": _id,
-            "name": name,
-            "description": description,
-            "type": type,
-            "img": img,
-        })
-
-    def placeOrder(self, buy_currency_id: str, sell_currency_id: str, buy_amount: float, sell_amount: float) -> object:
-        return self._getPost("/api/place_order", {
-            "buy_currency_id": buy_currency_id,
-            "sell_currency_id": sell_currency_id,
-            "buy_amount": buy_amount,
-            "sell_amount": sell_amount,
-        })
+    def addCurrency(
+        self, _id: str, name: str, description: str, type: str, img: str
+    ) -> object:
+        return self._getPost(
+            f"/api/add_currency",
+            {
+                "_id": _id,
+                "name": name,
+                "description": description,
+                "type": type,
+                "img": img,
+            },
+        )
+
+    def placeOrder(
+        self,
+        buy_currency_id: str,
+        sell_currency_id: str,
+        buy_amount: float,
+        sell_amount: float,
+    ) -> object:
+        return self._getPost(
+            "/api/place_order",
+            {
+                "buy_currency_id": buy_currency_id,
+                "sell_currency_id": sell_currency_id,
+                "buy_amount": buy_amount,
+                "sell_amount": sell_amount,
+            },
+        )
 
     def getOrders(self) -> object:
         return self._getGet("/api/orders")
 
     def buyOrder(self, order_id: str) -> object:
-        return self._getPost("/api/buy_order", {
-            "order_id": order_id,
-        })
+        return self._getPost(
+            "/api/buy_order",
+            {
+                "order_id": order_id,
+            },
+        )
 
-    def getOrdersByCurrency(self, buy_currency_id: str, sell_currency_id: str) -> object:
-        return self._getGet(f"/api/orders-by-currencies/{buy_currency_id}/{sell_currency_id}")
+    def getOrdersByCurrency(
+        self, buy_currency_id: str, sell_currency_id: str
+    ) -> object:
+        return self._getGet(
+            f"/api/orders-by-currencies/{buy_currency_id}/{sell_currency_id}"
+        )
 
-    def getBoughtOrdersByCurrency(self, buy_currency_id: str, sell_currency_id: str) -> object:
+    def getBoughtOrdersByCurrency(
+        self, buy_currency_id: str, sell_currency_id: str
+    ) -> object:
         return self._getGet(f"/api/bought-orders/{buy_currency_id}/{sell_currency_id}")
 
     def getOrder(self, order_id: str) -> object:
         return self._getGet(f"/api/orders/{order_id}")
 
     def getBalances(self) -> object:
         return self._getPost("/api/balances")
 
     def getTransactions(self) -> object:
         return self._getPost("/api/transactions")
 
     def login(self, _id: str, password: str) -> object:
         return self._checkRespAndAddJWT(
-            self._getPost("/api/login", {
-                "_id": _id,
-                "password": password,
-            })
+            self._getPost(
+                "/api/login",
+                {
+                    "_id": _id,
+                    "password": password,
+                },
+            )
         )
```

### Comparing `vicops_api-1.0.1/vicops_api.egg-info/PKG-INFO` & `vicops_api-1.0.2/vicops_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicops-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: python api wrapper for vicops2
 Home-page: https://github.com/ERTH2/vicops-api-py
 Author: artegoser
 License: MIT
 Project-URL: Source Code, https://github.com/ERTH2/vicops-api-py
 Keywords: api,wrapper,vicops
 Requires-Python: >=3.10
```

