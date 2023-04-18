# Comparing `tmp/pybit-5.1.1.tar.gz` & `tmp/pybit-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybit-5.1.1.tar", last modified: Thu Apr  6 11:16:27 2023, max compression
+gzip compressed data, was "pybit-5.2.0.tar", last modified: Tue Apr 18 19:02:58 2023, max compression
```

## Comparing `pybit-5.1.1.tar` & `pybit-5.2.0.tar`

### file list

```diff
@@ -1,46 +1,55 @@
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-06 11:16:27.012733 pybit-5.1.1/
--rw-r--r--   0 uk09002ml   (502) staff       (20)    20766 2023-04-06 11:16:00.000000 pybit-5.1.1/CHANGELOG.md
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.1.1/LICENSE
--rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.1.1/MANIFEST.in
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-06 11:16:27.013172 pybit-5.1.1/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6294 2023-04-06 11:15:33.000000 pybit-5.1.1/README.md
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-06 11:16:26.979205 pybit-5.1.1/examples/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-03 15:36:24.000000 pybit-5.1.1/examples/.DS_Store
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/direct_session.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1450 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/http_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/http_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/websocket_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/websocket_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.1.1/examples/wrapper_class.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-06 11:16:27.002312 pybit-5.1.1/pybit/
--rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-04-06 11:16:00.000000 pybit-5.1.1/pybit/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    12518 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7591 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13126 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6113 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8520 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     5765 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_v5_user.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    15535 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1647 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1461 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/exceptions.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8681 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/unified_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-04-06 11:15:33.000000 pybit-5.1.1/pybit/user.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-06 11:16:27.011758 pybit-5.1.1/pybit.egg-info/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-06 11:16:26.000000 pybit-5.1.1/pybit.egg-info/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)      926 2023-04-06 11:16:26.000000 pybit-5.1.1/pybit.egg-info/SOURCES.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-04-06 11:16:26.000000 pybit-5.1.1/pybit.egg-info/dependency_links.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.1.1/pybit.egg-info/not-zip-safe
--rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-04-06 11:16:26.000000 pybit-5.1.1/pybit.egg-info/requires.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-04-06 11:16:26.000000 pybit-5.1.1/pybit.egg-info/top_level.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-04-06 11:16:27.014461 pybit-5.1.1/setup.cfg
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1216 2023-04-06 11:16:00.000000 pybit-5.1.1/setup.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.257944 pybit-5.2.0/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    21087 2023-04-18 19:02:46.000000 pybit-5.2.0/CHANGELOG.md
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.2.0/LICENSE
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.2.0/MANIFEST.in
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-18 19:02:58.258483 pybit-5.2.0/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6294 2023-04-06 11:15:33.000000 pybit-5.2.0/README.md
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.212828 pybit-5.2.0/examples/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.2.0/examples/.DS_Store
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/direct_session.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1450 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/http_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/http_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/websocket_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-18 18:56:31.000000 pybit-5.2.0/examples/websocket_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/wrapper_class.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.240763 pybit-5.2.0/pybit/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    12518 2023-04-18 16:03:38.000000 pybit-5.2.0/pybit/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7591 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14814 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/_v5_asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6176 2023-04-18 16:12:52.000000 pybit-5.2.0/pybit/_v5_spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/_v5_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     5765 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_user.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    15535 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1461 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/exceptions.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.257012 pybit-5.2.0/pybit/legacy/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.2.0/pybit/legacy/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    32393 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/copy_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/usdc_options.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/usdc_perpetual.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8681 2023-04-12 17:27:28.000000 pybit-5.2.0/pybit/unified_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/user.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.247269 pybit-5.2.0/pybit.egg-info/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1156 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/SOURCES.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/dependency_links.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.2.0/pybit.egg-info/not-zip-safe
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/requires.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/top_level.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-04-18 19:02:58.259988 pybit-5.2.0/setup.cfg
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1232 2023-04-18 19:02:46.000000 pybit-5.2.0/setup.py
```

### Comparing `pybit-5.1.1/CHANGELOG.md` & `pybit-5.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+
+## [5.2.0] - 2023-04-18
+### Added
+- New asset endpoints: `set_deposit_account()`, `get_internal_deposit_records()`, `get_withdrawable_amount()`
+
+### Fixed
+- Ensure that `legacy` submodule is packaged by `setup.py`
+- Fix non-UTA (normal account) spot margin trading endpoints
+- Fix wrong request method for `set_dcp()`
+
+
 ## [5.1.1] - 2023-04-06
 ### Added
 - HTTP endpoints to the `copy_trading` module
 
 ### Modified
 - Docstrings in the `copy_trading` module to make it easier to find the API documentation for reference
 - Example files
```

### Comparing `pybit-5.1.1/LICENSE` & `pybit-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/PKG-INFO` & `pybit-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.1.1
+Version: 5.2.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.1.1/README.md` & `pybit-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/examples/.DS_Store` & `pybit-5.2.0/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/examples/direct_session.py` & `pybit-5.2.0/examples/direct_session.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/examples/http_example_explanatory.py` & `pybit-5.2.0/examples/http_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/examples/websocket_example_explanatory.py` & `pybit-5.2.0/examples/websocket_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/examples/wrapper_class.py` & `pybit-5.2.0/examples/wrapper_class.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_helpers.py` & `pybit-5.2.0/pybit/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_http_manager.py` & `pybit-5.2.0/pybit/_http_manager.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_v5_account.py` & `pybit-5.2.0/pybit/_v5_account.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_v5_asset.py` & `pybit-5.2.0/pybit/_v5_asset.py`

 * *Files 10% similar despite different names*

```diff
@@ -263,14 +263,33 @@
         return self._submit_request(
             method="GET",
             path=f"{self.endpoint}{Asset.GET_ALLOWED_DEPOSIT_COIN_INFO}",
             query=kwargs,
             auth=True,
         )
 
+    def set_deposit_account(self, **kwargs):
+        """Set auto transfer account after deposit. The same function as the setting for Deposit on web GUI
+
+        Required args:
+            accountType (string): Account type: UNIFIED,SPOT,OPTION,CONTRACT,FUND
+
+        Returns:
+            Request results as dictionary.
+
+        Additional information:
+            https://bybit-exchange.github.io/docs/v5/asset/set-deposit-acct
+        """
+        return self._submit_request(
+            method="POST",
+            path=f"{self.endpoint}{Asset.SET_DEPOSIT_ACCOUNT}",
+            query=kwargs,
+            auth=True,
+        )
+
     def get_deposit_records(self, **kwargs):
         """Query deposit records.
 
         Returns:
             Request results as dictionary.
 
         Additional information:
@@ -298,14 +317,30 @@
         return self._submit_request(
             method="GET",
             path=f"{self.endpoint}{Asset.GET_SUB_ACCOUNT_DEPOSIT_RECORDS}",
             query=kwargs,
             auth=True,
         )
 
+    def get_internal_deposit_records(self, **kwargs):
+        """Query deposit records within the Bybit platform. These transactions are not on the blockchain.
+
+        Returns:
+            Request results as dictionary.
+
+        Additional information:
+            https://bybit-exchange.github.io/docs/v5/asset/internal-deposit-record
+        """
+        return self._submit_request(
+            method="GET",
+            path=f"{self.endpoint}{Asset.GET_INTERNAL_DEPOSIT_RECORDS}",
+            query=kwargs,
+            auth=True,
+        )
+
     def get_master_deposit_address(self, **kwargs):
         """Query the deposit address information of MASTER account.
 
         Required args:
             coin (string): Coin
 
         Returns:
@@ -369,14 +404,33 @@
         return self._submit_request(
             method="GET",
             path=f"{self.endpoint}{Asset.GET_WITHDRAWAL_RECORDS}",
             query=kwargs,
             auth=True,
         )
 
+    def get_withdrawable_amount(self, **kwargs):
+        """Get withdrawable amount
+
+        Required args:
+            coin (string): Coin name
+
+        Returns:
+            Request results as dictionary.
+
+        Additional information:
+            https://bybit-exchange.github.io/docs/v5/asset/delay-amount
+        """
+        return self._submit_request(
+            method="GET",
+            path=f"{self.endpoint}{Asset.GET_WITHDRAWABLE_AMOUNT}",
+            query=kwargs,
+            auth=True,
+        )
+
     def withdraw(self, **kwargs):
         """Withdraw assets from your Bybit account. You can make an off-chain transfer if the target wallet address is from Bybit. This means that no blockchain fee will be charged.
 
         Required args:
             coin (string): Coin
             chain (string): Chain
             address (string): Wallet address
```

### Comparing `pybit-5.1.1/pybit/_v5_market.py` & `pybit-5.2.0/pybit/_v5_market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_v5_position.py` & `pybit-5.2.0/pybit/_v5_position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_v5_spot_leverage_token.py` & `pybit-5.2.0/pybit/_v5_spot_leverage_token.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_v5_spot_margin_trade.py` & `pybit-5.2.0/pybit/_v5_spot_margin_trade.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,34 +47,34 @@
         Required args:
             switch (string): 1: on, 0: off
 
         Returns:
             Request results as dictionary.
 
         Additional information:
-            https://bybit-exchange.github.io/docs/v5/spot-margin-normal/switch-mode
+            https://bybit-exchange.github.io/docs/v5/spot-margin-normal/margin-data
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_MARGIN_COIN_INFO}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_MARGIN_COIN_INFO}",
             query=kwargs,
         )
 
     def spot_margin_trade_normal_get_borrowable_coin_info(self, **kwargs):
         """Normal (non-UTA) account only.
 
         Returns:
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/borrowable-data
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_BORROWABLE_COIN_INFO}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_BORROWABLE_COIN_INFO}",
             query=kwargs,
         )
 
     def spot_margin_trade_normal_get_interest_quota(self, **kwargs):
         """Normal (non-UTA) account only.
 
         Required args:
@@ -84,15 +84,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/interest-quota
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_INTEREST_QUOTA}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_INTEREST_QUOTA}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_get_loan_account_info(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -100,15 +100,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/account-info
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_LOAN_ACCOUNT_INFO}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_LOAN_ACCOUNT_INFO}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_borrow(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -120,15 +120,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/borrow
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{SpotMarginTrade.BORROW}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_BORROW}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_repay(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -139,15 +139,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/repay
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{SpotMarginTrade.REPAY}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_REPAY}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_get_borrow_order_detail(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -155,15 +155,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/borrow-order
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_BORROW_ORDER_DETAIL}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_BORROW_ORDER_DETAIL}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_get_repayment_order_detail(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -171,15 +171,15 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/repay-order
         """
         return self._submit_request(
             method="GET",
-            path=f"{self.endpoint}{SpotMarginTrade.GET_REPAYMENT_ORDER_DETAIL}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_GET_REPAYMENT_ORDER_DETAIL}",
             query=kwargs,
             auth=True,
         )
 
     def spot_margin_trade_normal_toggle_margin_trade(self, **kwargs):
         """Normal (non-UTA) account only.
 
@@ -190,11 +190,11 @@
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/spot-margin-normal/switch-mode
         """
         return self._submit_request(
             method="POST",
-            path=f"{self.endpoint}{SpotMarginTrade.TOGGLE_MARGIN_TRADE}",
+            path=f"{self.endpoint}{SpotMarginTrade.NORMAL_TOGGLE_MARGIN_TRADE}",
             query=kwargs,
             auth=True,
         )
```

### Comparing `pybit-5.1.1/pybit/_v5_trade.py` & `pybit-5.2.0/pybit/_v5_trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,12 +233,12 @@
         Returns:
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/order/dcp
         """
         return self._submit_request(
-            method="GET",
+            method="POST",
             path=f"{self.endpoint}{Trade.SET_DCP}",
             query=kwargs,
             auth=True,
         )
```

### Comparing `pybit-5.1.1/pybit/_v5_user.py` & `pybit-5.2.0/pybit/_v5_user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/_websocket_stream.py` & `pybit-5.2.0/pybit/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/account.py` & `pybit-5.2.0/pybit/account.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/asset.py` & `pybit-5.2.0/pybit/asset.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,23 @@
     GET_SUB_UID = "/v5/asset/transfer/query-sub-member-list"
     ENABLE_UT_FOR_SUB_UID = "/v5/asset/transfer/save-transfer-sub-member"
     CREATE_UNIVERSAL_TRANSFER = "/v5/asset/transfer/universal-transfer"
     GET_UNIVERSAL_TRANSFER_RECORDS = (
         "/v5/asset/transfer/query-universal-transfer-list"
     )
     GET_ALLOWED_DEPOSIT_COIN_INFO = "/v5/asset/deposit/query-allowed-list"
+    SET_DEPOSIT_ACCOUNT = "/v5/asset/deposit/deposit-to-account"
     GET_DEPOSIT_RECORDS = "/v5/asset/deposit/query-record"
     GET_SUB_ACCOUNT_DEPOSIT_RECORDS = (
         "/v5/asset/deposit/query-sub-member-record"
     )
+    GET_INTERNAL_DEPOSIT_RECORDS = "/v5/asset/deposit/query-internal-record"
     GET_MASTER_DEPOSIT_ADDRESS = "/v5/asset/deposit/query-address"
     GET_SUB_DEPOSIT_ADDRESS = "/v5/asset/deposit/query-sub-member-address"
     GET_COIN_INFO = "/v5/asset/coin/query-info"
     GET_WITHDRAWAL_RECORDS = "/v5/asset/withdraw/query-record"
+    GET_WITHDRAWABLE_AMOUNT = "/v5/asset/withdraw/withdrawable-amount"
     WITHDRAW = "/v5/asset/withdraw/create"
     CANCEL_WITHDRAWAL = "/v5/asset/withdraw/cancel"
 
     def __str__(self) -> str:
         return self.value
```

### Comparing `pybit-5.1.1/pybit/exceptions.py` & `pybit-5.2.0/pybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/market.py` & `pybit-5.2.0/pybit/market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/position.py` & `pybit-5.2.0/pybit/position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/spot_margin_trade.py` & `pybit-5.2.0/pybit/spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/trade.py` & `pybit-5.2.0/pybit/trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/unified_trading.py` & `pybit-5.2.0/pybit/unified_trading.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit/user.py` & `pybit-5.2.0/pybit/user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.1.1/pybit.egg-info/PKG-INFO` & `pybit-5.2.0/pybit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.1.1
+Version: 5.2.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
```

### Comparing `pybit-5.1.1/setup.py` & `pybit-5.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pybit',
-    version='5.1.1',
+    version='5.2.0',
     description='Python3 Bybit HTTP/WebSocket API Connector', 
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bybit-exchange/pybit",
     license="MIT License",
     author="Dexter Dickinson",
     author_email="dexter.dickinson@bybit.com",
@@ -24,15 +24,15 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="bybit api connector",
-    packages=["pybit"],
+    packages=["pybit", "pybit.legacy"],
     python_requires=">=3.6",
     install_requires=[
         "requests",
         "websocket-client",
         "websockets",
     ],
 )
```

