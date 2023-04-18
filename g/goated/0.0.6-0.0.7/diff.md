# Comparing `tmp/goated-0.0.6.tar.gz` & `tmp/goated-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goated-0.0.6.tar", last modified: Wed Apr 12 10:15:14 2023, max compression
+gzip compressed data, was "goated-0.0.7.tar", last modified: Tue Apr 18 08:28:59 2023, max compression
```

## Comparing `goated-0.0.6.tar` & `goated-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.435852 goated-0.0.6/
--rw-r--r--   0 Cian       (502) staff       (20)     1055 2023-03-29 01:31:01.000000 goated-0.0.6/LICENSE.txt
--rw-r--r--   0 Cian       (502) staff       (20)     1121 2023-03-30 06:12:25.000000 goated-0.0.6/MANIFEST.in
--rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-12 10:15:14.435948 goated-0.0.6/PKG-INFO
--rw-r--r--   0 Cian       (502) staff       (20)     2397 2023-04-01 01:28:07.000000 goated-0.0.6/README.md
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.426411 goated-0.0.6/goated/
--rw-r--r--   0 Cian       (502) staff       (20)      396 2023-04-05 23:04:51.000000 goated-0.0.6/goated/__init__.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.428615 goated-0.0.6/goated/client/
--rw-r--r--   0 Cian       (502) staff       (20)      435 2023-04-06 02:23:23.000000 goated-0.0.6/goated/client/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6116 2023-04-01 01:41:05.000000 goated-0.0.6/goated/client/base_client.py
--rw-r--r--   0 Cian       (502) staff       (20)      344 2023-03-30 23:10:14.000000 goated-0.0.6/goated/client/exceptions.py
--rw-r--r--   0 Cian       (502) staff       (20)    19380 2023-03-27 20:32:17.000000 goated-0.0.6/goated/client/trading_client.py
--rw-r--r--   0 Cian       (502) staff       (20)     2535 2023-04-01 01:28:00.000000 goated-0.0.6/goated/example.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.430452 goated-0.0.6/goated/instructions/
--rw-r--r--   0 Cian       (502) staff       (20)      752 2023-04-07 05:15:12.000000 goated-0.0.6/goated/instructions/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)      866 2023-03-16 05:12:07.000000 goated-0.0.6/goated/instructions/cancel_order.py
--rw-r--r--   0 Cian       (502) staff       (20)      617 2023-03-20 04:18:46.000000 goated-0.0.6/goated/instructions/enums.py
--rw-r--r--   0 Cian       (502) staff       (20)     2046 2023-03-16 05:12:03.000000 goated-0.0.6/goated/instructions/new_order.py
--rw-r--r--   0 Cian       (502) staff       (20)     1159 2023-03-16 05:12:11.000000 goated-0.0.6/goated/instructions/reduce_order.py
--rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:12:14.000000 goated-0.0.6/goated/instructions/update_persistence.py
--rw-r--r--   0 Cian       (502) staff       (20)       49 2022-12-19 05:08:12.000000 goated-0.0.6/goated/main.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.432670 goated-0.0.6/goated/state/
--rw-r--r--   0 Cian       (502) staff       (20)      934 2023-04-05 23:17:45.000000 goated-0.0.6/goated/state/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6550 2023-04-11 05:07:54.000000 goated-0.0.6/goated/state/container.py
--rw-r--r--   0 Cian       (502) staff       (20)     7300 2023-04-11 07:18:12.000000 goated-0.0.6/goated/state/market.py
--rw-r--r--   0 Cian       (502) staff       (20)    11919 2023-04-11 07:18:02.000000 goated-0.0.6/goated/state/order.py
--rw-r--r--   0 Cian       (502) staff       (20)    10120 2023-04-11 07:18:09.000000 goated-0.0.6/goated/state/pool.py
--rw-r--r--   0 Cian       (502) staff       (20)     4759 2023-04-11 07:17:49.000000 goated-0.0.6/goated/state/position.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.434285 goated-0.0.6/goated/state/profiles/
--rw-r--r--   0 Cian       (502) staff       (20)      214 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6252 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/current_liquidity_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     8955 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/pool_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     1887 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/position_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)      874 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/target_liquidity_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     3869 2023-04-11 07:17:53.000000 goated-0.0.6/goated/state/selection.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.435586 goated-0.0.6/goated/utils/
--rw-r--r--   0 Cian       (502) staff       (20)      305 2023-04-05 23:06:59.000000 goated-0.0.6/goated/utils/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)    11984 2023-03-30 21:25:55.000000 goated-0.0.6/goated/utils/bucketing.py
--rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:18:05.000000 goated-0.0.6/goated/utils/converter.py
--rw-r--r--   0 Cian       (502) staff       (20)      764 2023-03-29 01:15:50.000000 goated-0.0.6/goated/utils/encoder.py
--rw-r--r--   0 Cian       (502) staff       (20)     7426 2023-03-29 01:15:53.000000 goated-0.0.6/goated/utils/payoff_signature.py
--rw-r--r--   0 Cian       (502) staff       (20)       21 2023-04-12 10:15:11.000000 goated-0.0.6/goated/version.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.427327 goated-0.0.6/goated.egg-info/
--rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/PKG-INFO
--rw-r--r--   0 Cian       (502) staff       (20)     1126 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/SOURCES.txt
--rw-r--r--   0 Cian       (502) staff       (20)        1 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/dependency_links.txt
--rw-r--r--   0 Cian       (502) staff       (20)       31 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/requires.txt
--rw-r--r--   0 Cian       (502) staff       (20)        7 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/top_level.txt
--rw-r--r--   0 Cian       (502) staff       (20)       59 2023-03-29 01:31:01.000000 goated-0.0.6/pyproject.toml
--rw-r--r--   0 Cian       (502) staff       (20)     1017 2023-04-12 10:15:14.436279 goated-0.0.6/setup.cfg
--rw-r--r--   0 Cian       (502) staff       (20)       87 2023-03-29 01:31:02.000000 goated-0.0.6/setup.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.364864 goated-0.0.7/
+-rw-r--r--   0 Cian       (502) staff       (20)     1055 2023-03-29 01:31:01.000000 goated-0.0.7/LICENSE.txt
+-rw-r--r--   0 Cian       (502) staff       (20)     1121 2023-03-30 06:12:25.000000 goated-0.0.7/MANIFEST.in
+-rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-18 08:28:59.365023 goated-0.0.7/PKG-INFO
+-rw-r--r--   0 Cian       (502) staff       (20)     2397 2023-04-01 01:28:07.000000 goated-0.0.7/README.md
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.346370 goated-0.0.7/goated/
+-rw-r--r--   0 Cian       (502) staff       (20)      396 2023-04-05 23:04:51.000000 goated-0.0.7/goated/__init__.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.349237 goated-0.0.7/goated/client/
+-rw-r--r--   0 Cian       (502) staff       (20)      435 2023-04-06 02:23:23.000000 goated-0.0.7/goated/client/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6116 2023-04-01 01:41:05.000000 goated-0.0.7/goated/client/base_client.py
+-rw-r--r--   0 Cian       (502) staff       (20)      344 2023-03-30 23:10:14.000000 goated-0.0.7/goated/client/exceptions.py
+-rw-r--r--   0 Cian       (502) staff       (20)    19380 2023-03-27 20:32:17.000000 goated-0.0.7/goated/client/trading_client.py
+-rw-r--r--   0 Cian       (502) staff       (20)     2535 2023-04-01 01:28:00.000000 goated-0.0.7/goated/example.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.352522 goated-0.0.7/goated/instructions/
+-rw-r--r--   0 Cian       (502) staff       (20)      752 2023-04-07 05:15:12.000000 goated-0.0.7/goated/instructions/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)      866 2023-03-16 05:12:07.000000 goated-0.0.7/goated/instructions/cancel_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)      617 2023-03-20 04:18:46.000000 goated-0.0.7/goated/instructions/enums.py
+-rw-r--r--   0 Cian       (502) staff       (20)     2046 2023-03-16 05:12:03.000000 goated-0.0.7/goated/instructions/new_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1159 2023-03-16 05:12:11.000000 goated-0.0.7/goated/instructions/reduce_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:12:14.000000 goated-0.0.7/goated/instructions/update_persistence.py
+-rw-r--r--   0 Cian       (502) staff       (20)       49 2022-12-19 05:08:12.000000 goated-0.0.7/goated/main.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.358751 goated-0.0.7/goated/state/
+-rw-r--r--   0 Cian       (502) staff       (20)      934 2023-04-05 23:17:45.000000 goated-0.0.7/goated/state/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6550 2023-04-11 05:07:54.000000 goated-0.0.7/goated/state/container.py
+-rw-r--r--   0 Cian       (502) staff       (20)     7322 2023-04-18 08:15:19.000000 goated-0.0.7/goated/state/market.py
+-rw-r--r--   0 Cian       (502) staff       (20)    11919 2023-04-11 07:18:02.000000 goated-0.0.7/goated/state/order.py
+-rw-r--r--   0 Cian       (502) staff       (20)    10120 2023-04-11 07:18:09.000000 goated-0.0.7/goated/state/pool.py
+-rw-r--r--   0 Cian       (502) staff       (20)     4759 2023-04-11 07:17:49.000000 goated-0.0.7/goated/state/position.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.360909 goated-0.0.7/goated/state/profiles/
+-rw-r--r--   0 Cian       (502) staff       (20)      214 2023-03-27 20:01:28.000000 goated-0.0.7/goated/state/profiles/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6252 2023-03-27 20:01:28.000000 goated-0.0.7/goated/state/profiles/current_liquidity_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     8955 2023-03-27 20:01:28.000000 goated-0.0.7/goated/state/profiles/pool_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1887 2023-03-27 20:01:28.000000 goated-0.0.7/goated/state/profiles/position_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)      874 2023-03-27 20:01:28.000000 goated-0.0.7/goated/state/profiles/target_liquidity_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     3869 2023-04-11 07:17:53.000000 goated-0.0.7/goated/state/selection.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.364216 goated-0.0.7/goated/utils/
+-rw-r--r--   0 Cian       (502) staff       (20)      305 2023-04-05 23:06:59.000000 goated-0.0.7/goated/utils/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)    11984 2023-03-30 21:25:55.000000 goated-0.0.7/goated/utils/bucketing.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:18:05.000000 goated-0.0.7/goated/utils/converter.py
+-rw-r--r--   0 Cian       (502) staff       (20)      764 2023-03-29 01:15:50.000000 goated-0.0.7/goated/utils/encoder.py
+-rw-r--r--   0 Cian       (502) staff       (20)     7426 2023-03-29 01:15:53.000000 goated-0.0.7/goated/utils/payoff_signature.py
+-rw-r--r--   0 Cian       (502) staff       (20)       21 2023-04-18 08:28:13.000000 goated-0.0.7/goated/version.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-18 08:28:59.347759 goated-0.0.7/goated.egg-info/
+-rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-18 08:28:59.000000 goated-0.0.7/goated.egg-info/PKG-INFO
+-rw-r--r--   0 Cian       (502) staff       (20)     1126 2023-04-18 08:28:59.000000 goated-0.0.7/goated.egg-info/SOURCES.txt
+-rw-r--r--   0 Cian       (502) staff       (20)        1 2023-04-18 08:28:59.000000 goated-0.0.7/goated.egg-info/dependency_links.txt
+-rw-r--r--   0 Cian       (502) staff       (20)       31 2023-04-18 08:28:59.000000 goated-0.0.7/goated.egg-info/requires.txt
+-rw-r--r--   0 Cian       (502) staff       (20)        7 2023-04-18 08:28:59.000000 goated-0.0.7/goated.egg-info/top_level.txt
+-rw-r--r--   0 Cian       (502) staff       (20)       59 2023-03-29 01:31:01.000000 goated-0.0.7/pyproject.toml
+-rw-r--r--   0 Cian       (502) staff       (20)     1017 2023-04-18 08:28:59.365416 goated-0.0.7/setup.cfg
+-rw-r--r--   0 Cian       (502) staff       (20)       87 2023-03-29 01:31:02.000000 goated-0.0.7/setup.py
```

### Comparing `goated-0.0.6/LICENSE.txt` & `goated-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/MANIFEST.in` & `goated-0.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/PKG-INFO` & `goated-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goated
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python library for interacting with the Goated Exchange API.
 Home-page: https://github.com/goatedsports/python-sdk
 Download-URL: https://github.com/goatedsports/python-sdk/archive/refs/heads/main.zip
 Author: Goated Core Team
 Author-email: cian@goated.com
 License: MIT
 Keywords: goated,betting,trading,sports,sportsbetting,exchange,bet,prediction,market
```

### Comparing `goated-0.0.6/README.md` & `goated-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/client/base_client.py` & `goated-0.0.7/goated/client/base_client.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/client/trading_client.py` & `goated-0.0.7/goated/client/trading_client.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/example.py` & `goated-0.0.7/goated/example.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/__init__.py` & `goated-0.0.7/goated/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/cancel_order.py` & `goated-0.0.7/goated/instructions/cancel_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/enums.py` & `goated-0.0.7/goated/instructions/enums.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/new_order.py` & `goated-0.0.7/goated/instructions/new_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/reduce_order.py` & `goated-0.0.7/goated/instructions/reduce_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/instructions/update_persistence.py` & `goated-0.0.7/goated/instructions/update_persistence.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/__init__.py` & `goated-0.0.7/goated/state/__init__.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/container.py` & `goated-0.0.7/goated/state/container.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/market.py` & `goated-0.0.7/goated/state/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             'expiry_time_utc': self.expiry_time.strftime("%Y-%m-%dT%H:%M:%SZ") if self.expiry_time else None,
             'status': self.status,
             'is_main_market': self.is_main_market,
             'handicap': self.handicap,
             'type': {
                 'id': self.type_id,
                 'name': self.type_name
-            } if self.type else None,
+            } if self.type_name and self.type_id else None,
             'num_winners': self.num_winners,
             'num_selections': self.num_selections,
             'min_post_quantity': f'{self.min_post_quantity:.18f}',
             'supports_in_play': self.supports_in_play,
             'in_play_delay_seconds': self.in_play_delay_seconds,
             'is_cross_matching': self.is_cross_matching,
             'matched_volume': f'{self.matched_volume:.18f}' if self.matched_volume else None,
```

### Comparing `goated-0.0.6/goated/state/order.py` & `goated-0.0.7/goated/state/order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/pool.py` & `goated-0.0.7/goated/state/pool.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/position.py` & `goated-0.0.7/goated/state/position.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/profiles/current_liquidity_profile.py` & `goated-0.0.7/goated/state/profiles/current_liquidity_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/profiles/pool_profile.py` & `goated-0.0.7/goated/state/profiles/pool_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/profiles/position_profile.py` & `goated-0.0.7/goated/state/profiles/position_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/profiles/target_liquidity_profile.py` & `goated-0.0.7/goated/state/profiles/target_liquidity_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/state/selection.py` & `goated-0.0.7/goated/state/selection.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/utils/bucketing.py` & `goated-0.0.7/goated/utils/bucketing.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/utils/converter.py` & `goated-0.0.7/goated/utils/converter.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/utils/encoder.py` & `goated-0.0.7/goated/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated/utils/payoff_signature.py` & `goated-0.0.7/goated/utils/payoff_signature.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/goated.egg-info/PKG-INFO` & `goated-0.0.7/goated.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goated
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python library for interacting with the Goated Exchange API.
 Home-page: https://github.com/goatedsports/python-sdk
 Download-URL: https://github.com/goatedsports/python-sdk/archive/refs/heads/main.zip
 Author: Goated Core Team
 Author-email: cian@goated.com
 License: MIT
 Keywords: goated,betting,trading,sports,sportsbetting,exchange,bet,prediction,market
```

### Comparing `goated-0.0.6/goated.egg-info/SOURCES.txt` & `goated-0.0.7/goated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goated-0.0.6/setup.cfg` & `goated-0.0.7/setup.cfg`

 * *Files identical despite different names*

