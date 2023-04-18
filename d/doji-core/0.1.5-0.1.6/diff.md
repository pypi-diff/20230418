# Comparing `tmp/doji_core-0.1.5.tar.gz` & `tmp/doji_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doji_core-0.1.5.tar", max compression
+gzip compressed data, was "doji_core-0.1.6.tar", max compression
```

## Comparing `doji_core-0.1.5.tar` & `doji_core-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.5/LICENSE
--rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.5/doji/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.5/doji/core/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.5/doji/core/api/classes/__init__.py
--rw-r--r--   0        0        0     6129 2023-04-16 17:22:15.958372 doji_core-0.1.5/doji/core/api/classes/api.py
--rw-r--r--   0        0        0     6368 2023-04-17 14:24:09.341628 doji_core-0.1.5/doji/core/api/classes/api_response.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/api/mixins/__init__.py
--rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/api/mixins/api_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/asset/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/asset/classes/__init__.py
--rw-r--r--   0        0        0     2417 2023-04-17 14:33:19.259397 doji_core-0.1.5/doji/core/asset/classes/asset.py
--rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.5/doji/core/asset/classes/asset_instances.py
--rw-r--r--   0        0        0     3841 2023-04-17 13:37:32.636002 doji_core-0.1.5/doji/core/asset/classes/asset_pair.py
--rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.5/doji/core/asset/classes/asset_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/asset/mixins/__init__.py
--rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.5/doji/core/asset/mixins/asset_pairs_mixin.py
--rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.5/doji/core/asset/mixins/assets_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/classes/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/classes/currency.py
--rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/classes/currency_instances.py
--rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/classes/currency_pair.py
--rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/classes/currency_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/currency/mixins/__init__.py
--rw-r--r--   0        0        0    14781 2023-04-16 17:29:04.462159 doji_core-0.1.5/doji/core/currency/mixins/currencies_mixin.py
--rw-r--r--   0        0        0    10226 2023-04-16 17:29:13.146156 doji_core-0.1.5/doji/core/currency/mixins/currency_pairs_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/exchange/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/exchange/classes/__init__.py
--rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.5/doji/core/exchange/classes/currency_exchange.py
--rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.5/doji/core/exchange/classes/exchange.py
--rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.5/doji/core/py.typed
--rw-r--r--   0        0        0     2719 2023-04-17 14:24:33.933160 doji_core-0.1.5/doji/core/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.5/doji/core/utils/classes/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-17 14:46:16.142220 doji_core-0.1.5/doji/core/utils/classes/instance.py
--rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.5/doji/core/utils/classes/instances.py
--rw-r--r--   0        0        0      565 2023-04-17 14:46:54.234912 doji_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 doji_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.6/doji/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.6/doji/core/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.6/doji/core/api/classes/__init__.py
+-rw-r--r--   0        0        0     6129 2023-04-16 17:22:15.958372 doji_core-0.1.6/doji/core/api/classes/api.py
+-rw-r--r--   0        0        0     6368 2023-04-17 14:24:09.341628 doji_core-0.1.6/doji/core/api/classes/api_response.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/api/mixins/__init__.py
+-rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/api/mixins/api_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/asset/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/asset/classes/__init__.py
+-rw-r--r--   0        0        0     2417 2023-04-17 14:33:19.259397 doji_core-0.1.6/doji/core/asset/classes/asset.py
+-rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.6/doji/core/asset/classes/asset_instances.py
+-rw-r--r--   0        0        0     3841 2023-04-17 13:37:32.636002 doji_core-0.1.6/doji/core/asset/classes/asset_pair.py
+-rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.6/doji/core/asset/classes/asset_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/asset/mixins/__init__.py
+-rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.6/doji/core/asset/mixins/asset_pairs_mixin.py
+-rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.6/doji/core/asset/mixins/assets_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/classes/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/classes/currency.py
+-rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/classes/currency_instances.py
+-rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/classes/currency_pair.py
+-rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/classes/currency_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/currency/mixins/__init__.py
+-rw-r--r--   0        0        0    14781 2023-04-16 17:29:04.462159 doji_core-0.1.6/doji/core/currency/mixins/currencies_mixin.py
+-rw-r--r--   0        0        0    10226 2023-04-16 17:29:13.146156 doji_core-0.1.6/doji/core/currency/mixins/currency_pairs_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/exchange/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/exchange/classes/__init__.py
+-rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.6/doji/core/exchange/classes/currency_exchange.py
+-rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.6/doji/core/exchange/classes/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.6/doji/core/py.typed
+-rw-r--r--   0        0        0     2719 2023-04-17 14:24:33.933160 doji_core-0.1.6/doji/core/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.6/doji/core/utils/classes/__init__.py
+-rw-r--r--   0        0        0     4814 2023-04-18 16:30:12.307359 doji_core-0.1.6/doji/core/utils/classes/instance.py
+-rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.6/doji/core/utils/classes/instances.py
+-rw-r--r--   0        0        0      642 2023-04-18 15:49:16.608940 doji_core-0.1.6/doji/core/utils/classes/nothing.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:44:21.258797 doji_core-0.1.6/doji/core/utils/functions/__init__.py
+-rw-r--r--   0        0        0     4745 2023-04-18 16:18:58.550218 doji_core-0.1.6/doji/core/utils/functions/dict.py
+-rw-r--r--   0        0        0      565 2023-04-18 16:32:18.080416 doji_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 doji_core-0.1.6/PKG-INFO
```

### Comparing `doji_core-0.1.5/LICENSE` & `doji_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/api/classes/api.py` & `doji_core-0.1.6/doji/core/api/classes/api.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/api/classes/api_response.py` & `doji_core-0.1.6/doji/core/api/classes/api_response.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/api/mixins/api_mixin.py` & `doji_core-0.1.6/doji/core/api/mixins/api_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/classes/asset.py` & `doji_core-0.1.6/doji/core/asset/classes/asset.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/classes/asset_instances.py` & `doji_core-0.1.6/doji/core/asset/classes/asset_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/classes/asset_pair.py` & `doji_core-0.1.6/doji/core/asset/classes/asset_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/classes/asset_pair_instances.py` & `doji_core-0.1.6/doji/core/asset/classes/asset_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/mixins/asset_pairs_mixin.py` & `doji_core-0.1.6/doji/core/asset/mixins/asset_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/asset/mixins/assets_mixin.py` & `doji_core-0.1.6/doji/core/asset/mixins/assets_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/classes/currency.py` & `doji_core-0.1.6/doji/core/currency/classes/currency.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/classes/currency_instances.py` & `doji_core-0.1.6/doji/core/currency/classes/currency_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/classes/currency_pair.py` & `doji_core-0.1.6/doji/core/currency/classes/currency_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/classes/currency_pair_instances.py` & `doji_core-0.1.6/doji/core/currency/classes/currency_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/mixins/currencies_mixin.py` & `doji_core-0.1.6/doji/core/currency/mixins/currencies_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/currency/mixins/currency_pairs_mixin.py` & `doji_core-0.1.6/doji/core/currency/mixins/currency_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/exchange/classes/currency_exchange.py` & `doji_core-0.1.6/doji/core/exchange/classes/currency_exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/exchange/classes/exchange.py` & `doji_core-0.1.6/doji/core/exchange/classes/exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/types/__init__.py` & `doji_core-0.1.6/doji/core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/doji/core/utils/classes/instance.py` & `doji_core-0.1.6/doji/core/utils/classes/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 from __future__ import annotations
 
 from pydantic import BaseModel
 from typing import Any, Generator, TypeVar
 
+# ┌─────────────────────────────────────────────────────────────────────────────────────
+# │ PROJECT IMPORTS
+# └─────────────────────────────────────────────────────────────────────────────────────
+
+from doji.core.utils.functions.dict import dget, dset
+
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ INSTANCE
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 T = TypeVar("T", bound="Instance")
 
@@ -38,21 +44,29 @@
     # │ FROM DICT
     # └─────────────────────────────────────────────────────────────────────────────────
 
     @classmethod
     def from_dict(cls: type[T], data: Any, where: dict[str, str] | None = None) -> T:
         """Initializes an instance from a dictionary"""
 
+        # Initialize object
+        obj = data
+
         # Check if data is a dictionary
-        if where and isinstance(data, dict):
-            # Remap keys
-            data = {where.get(key, key): value for key, value in data.items()}
+        if isinstance(data, dict):
+            # Initialize object
+            obj = {}
+
+            # Iterate over where
+            for path_to_set, path_to_get in (where or {}).items():
+                # Remap data
+                dset(obj, path_to_set, dget(data, path_to_get))
 
         # Initialize instance
-        instance = cls.parse_obj(data)
+        instance = cls.parse_obj(obj)
 
         # Return instance
         return instance
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ FROM LIST
     # └─────────────────────────────────────────────────────────────────────────────────
```

### Comparing `doji_core-0.1.5/doji/core/utils/classes/instances.py` & `doji_core-0.1.6/doji/core/utils/classes/instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.5/pyproject.toml` & `doji_core-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doji-core"
-version = "0.1.5"
+version = "0.1.6"
 description = "A repository for Doji, a trade analytics suite written in Python."
 authors = ["Sean O'Leary <seamicole@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "doji"}]
 
 [tool.poetry.dependencies]
```

### Comparing `doji_core-0.1.5/PKG-INFO` & `doji_core-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doji-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: A repository for Doji, a trade analytics suite written in Python.
 License: MIT
 Author: Sean O'Leary
 Author-email: seamicole@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

