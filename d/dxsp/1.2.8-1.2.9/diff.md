# Comparing `tmp/dxsp-1.2.8.tar.gz` & `tmp/dxsp-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.8.tar", max compression
+gzip compressed data, was "dxsp-1.2.9.tar", max compression
```

## Comparing `dxsp-1.2.8.tar` & `dxsp-1.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-17 19:14:43.677820 dxsp-1.2.8/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-17 19:14:43.677820 dxsp-1.2.8/README.md
--rw-r--r--   0        0        0      136 2023-04-17 19:14:44.365835 dxsp-1.2.8/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-17 19:14:43.677820 dxsp-1.2.8/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-17 19:14:43.677820 dxsp-1.2.8/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    28040 2023-04-17 19:14:43.677820 dxsp-1.2.8/dxsp/main.py
--rw-r--r--   0        0        0      960 2023-04-17 19:14:44.365835 dxsp-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 19:02:16.965228 dxsp-1.2.9/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-18 19:02:16.965228 dxsp-1.2.9/README.md
+-rw-r--r--   0        0        0      136 2023-04-18 19:02:17.621240 dxsp-1.2.9/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    28389 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/main.py
+-rw-r--r--   0        0        0      960 2023-04-18 19:02:17.621240 dxsp-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.9/PKG-INFO
```

### Comparing `dxsp-1.2.8/LICENSE` & `dxsp-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.8/README.md` & `dxsp-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.8/dxsp/assets/blockchains.py` & `dxsp-1.2.9/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.8/dxsp/main.py` & `dxsp-1.2.9/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,17 @@
                     order['id'] = transaction_receipt['transactionHash']
                     order['timestamp'] = transaction_block['timestamp']
                     order['symbol'] = asset_out_symbol
                     order['contract'] = asset_out_address
                     order['amount'] = transaction_amount
                     order['fee'] = transaction_receipt['gasUsed']
                     order['price'] = 'na'
+                    order['confirmation'] = 'na'
+                                #response+= f"\n➕ Size: {round(ex.from_wei(transaction_amount, 'ether'),5)}\n⚫️ Entry: {await fetch_gecko_asset_price(asset_in_symbol)}USD \nℹ️ {txHash}\n⛽️ {txHashDetail['gasUsed']}\n🗓️ {datetime.now()}"
+            #logger.info(msg=f"{response}")
                     return order
         except Exception as e:
             self.logger.debug(f"error get_swap {e}")
             return
 
     async def get_block_explorer_status(self,txHash):
         self.logger.debug(f"get_block_explorer_status {txHash}")
```

### Comparing `dxsp-1.2.8/pyproject.toml` & `dxsp-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.8"
+version = "1.2.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.2.8/PKG-INFO` & `dxsp-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.8
+Version: 1.2.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

