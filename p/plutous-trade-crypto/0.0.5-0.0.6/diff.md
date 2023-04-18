# Comparing `tmp/plutous_trade_crypto-0.0.5.tar.gz` & `tmp/plutous_trade_crypto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade_crypto-0.0.5.tar", max compression
+gzip compressed data, was "plutous_trade_crypto-0.0.6.tar", max compression
```

## Comparing `plutous_trade_crypto-0.0.5.tar` & `plutous_trade_crypto-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/LICENSE
--rw-r--r--   0        0        0       54 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/README.md
--rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/__init__.py
--rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/__init__.py
--rw-r--r--   0        0        0       21 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/__init__.py
--rw-r--r--   0        0        0      545 2023-01-13 12:53:06.868724 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/__init__.py
--rw-r--r--   0        0        0    20842 2023-01-24 12:35:54.183331 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/binance.py
--rw-r--r--   0        0        0    10361 2023-01-24 12:16:08.497872 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/bitget.py
--rw-r--r--   0        0        0     9056 2023-01-24 17:08:43.291912 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/bybit.py
--rw-r--r--   0        0        0      243 2023-01-18 17:49:03.301016 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/coinex.py
--rw-r--r--   0        0        0     3432 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/gateio.py
--rw-r--r--   0        0        0     5479 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/huobi.py
--rw-r--r--   0        0        0     2402 2023-01-13 23:16:12.206570 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/kucoin.py
--rw-r--r--   0        0        0     7009 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/mexc.py
--rw-r--r--   0        0        0     5762 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/okx.py
--rw-r--r--   0        0        0     2482 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/phemex.py
--rw-r--r--   0        0        0       51 2023-01-13 23:17:03.314313 plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/woo.py
--rw-r--r--   0        0        0     4368 2023-01-24 05:01:24.733891 plutous_trade_crypto-0.0.5/plutous/trade/crypto/utils.py
--rw-r--r--   0        0        0      662 2023-01-24 17:24:44.257933 plutous_trade_crypto-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 plutous_trade_crypto-0.0.5/setup.py
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 plutous_trade_crypto-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/LICENSE
+-rw-r--r--   0        0        0       54 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/README.md
+-rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/__init__.py
+-rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/__init__.py
+-rw-r--r--   0        0        0       21 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/crypto/__init__.py
+-rw-r--r--   0        0        0      545 2023-01-13 12:53:06.868724 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/__init__.py
+-rw-r--r--   0        0        0    26071 2023-04-17 17:44:16.553723 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/binance.py
+-rw-r--r--   0        0        0     6758 2023-02-09 01:38:34.931606 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/bitget.py
+-rw-r--r--   0        0        0     9056 2023-01-24 17:08:43.291912 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/bybit.py
+-rw-r--r--   0        0        0      243 2023-01-18 17:49:03.301016 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/coinex.py
+-rw-r--r--   0        0        0     3432 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/gateio.py
+-rw-r--r--   0        0        0     5479 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/huobi.py
+-rw-r--r--   0        0        0     2402 2023-01-13 23:16:12.206570 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/kucoin.py
+-rw-r--r--   0        0        0     7009 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/mexc.py
+-rw-r--r--   0        0        0     5762 2023-03-05 16:41:45.182876 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/okx.py
+-rw-r--r--   0        0        0     2482 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/phemex.py
+-rw-r--r--   0        0        0       51 2023-01-13 23:17:03.314313 plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/woo.py
+-rw-r--r--   0        0        0     4492 2023-04-16 15:32:45.977687 plutous_trade_crypto-0.0.6/plutous/trade/crypto/utils.py
+-rw-r--r--   0        0        0      697 2023-04-18 05:01:41.765087 plutous_trade_crypto-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 plutous_trade_crypto-0.0.6/PKG-INFO
```

### Comparing `plutous_trade_crypto-0.0.5/LICENSE` & `plutous_trade_crypto-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/__init__.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/bybit.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/gateio.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/huobi.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/kucoin.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/mexc.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/okx.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/exchanges/phemex.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/exchanges/phemex.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.5/plutous/trade/crypto/utils.py` & `plutous_trade_crypto-0.0.6/plutous/trade/crypto/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,39 +39,39 @@
     ----------
     Callable
         Decorator on given function
     """
 
     def decorator(func: Coroutine) -> Coroutine:
         async def paginate_over_limit(**kwargs) -> list[dict[str, Any]]:
-            params = kwargs["params"]
+            params: dict = kwargs["params"]
             limit = kwargs.get("limit") or float("inf")
             limit_arg = min(limit, max_limit)
             kwargs["limit"] = limit_arg if limit_arg != float("inf") else None
 
             records = await func(**kwargs)
             all_records = records
             limit -= max_limit
             limit = limit if limit != np.nan else 0
 
-            while (records == max_limit) & (limit > 0):
+            while (len(records) == max_limit) & (limit > 0):
                 if id_arg in kwargs:
                     params[id_arg] = int(records[-1]["id"]) + 1
                 elif ("since" in kwargs) or (start_time_arg in params):
                     kwargs["since"] = int(records[-1]["timestamp"]) + 1
                 else:
                     break
                 kwargs["limit"] = min(limit, max_limit)
                 records = await func(**kwargs)
                 all_records.extend(records)
                 limit -= max_limit
             return all_records
 
         async def paginate_over_interval(**kwargs) -> list[dict[str, Any]]:
-            params = kwargs["params"]
+            params: dict = kwargs["params"]
             since: int = kwargs.get("since") or params.get(start_time_arg)
             now = int(datetime.now(timezone.utc).timestamp() * 1000)
             end = params.get(end_time_arg, now)
             if "timeframe" in kwargs:
                 diff = (
                     ccxt.Exchange.parse_timeframe(kwargs["timeframe"])
                     * 1000
@@ -83,18 +83,20 @@
                     int(max_interval.total_seconds() * 1000)
                     if max_interval is not None
                     else (now - since + 1)
                 )
 
             coroutines = []
             for since in range(since, end, diff):
-                params = kwargs.copy()
-                kwargs["since"] = since
+                ckwargs = kwargs.copy()
+                params = params.copy()
+                ckwargs["since"] = since
                 params[end_time_arg] = min(since + diff - 1, end)
-                coroutines.append(paginate_over_limit(**kwargs))
+                ckwargs["params"] = params
+                coroutines.append(paginate_over_limit(**ckwargs))
 
             logger.info(
                 f"Calling {func.__name__} {kwargs} "
                 + f"max_interval: {max_interval} "
                 + f"Paginating over {len(coroutines)} intervals."
             )
             records = []
@@ -107,14 +109,14 @@
         @functools.wraps(func)
         async def wrapper(*args, **kwargs) -> list[dict[str, Any]]:
             co_varnames = func.__code__.co_varnames
             kwargs.update(zip(co_varnames, args))
 
             if id_arg in kwargs:
                 return await paginate_over_limit(**kwargs)
-            if ("since" in kwargs) or (start_time_arg in kwargs["params"]):
+            if (kwargs.get("since") is not None) or (start_time_arg in kwargs.get("params", {})):
                 return await paginate_over_interval(**kwargs)
             return await func(**kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `plutous_trade_crypto-0.0.5/PKG-INFO` & `plutous_trade_crypto-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: plutous-trade-crypto
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plutous Crypto Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ccxt (>=2.4.24)
+Requires-Dist: numpy (==1.23.5)
 Requires-Dist: pandas (>=1.5.2)
 Description-Content-Type: text/markdown
 
 # plutous-trade-crypto
 Plutous Crypto Trading Library
```

