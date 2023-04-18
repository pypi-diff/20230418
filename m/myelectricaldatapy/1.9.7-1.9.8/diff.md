# Comparing `tmp/myelectricaldatapy-1.9.7.tar.gz` & `tmp/myelectricaldatapy-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.7.tar", last modified: Mon Apr 17 15:27:33 2023, max compression
+gzip compressed data, was "myelectricaldatapy-1.9.8.tar", last modified: Tue Apr 18 09:19:12 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.7.tar` & `myelectricaldatapy-1.9.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.639300 myelectricaldatapy-1.9.7/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-17 15:27:32.000000 myelectricaldatapy-1.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-18 09:19:11.000000 myelectricaldatapy-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.7/LICENSE` & `myelectricaldatapy-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/PKG-INFO` & `myelectricaldatapy-1.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.7
+Version: 1.9.8
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.7/README.md` & `myelectricaldatapy-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy/analytics.py` & `myelectricaldatapy-1.9.8/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy/auth.py` & `myelectricaldatapy-1.9.8/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-1.9.8/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-1.9.8/myelectricaldatapy/mypdl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Class for my PDL."""
 from __future__ import annotations
 
 import logging
+from datetime import date
 from datetime import datetime as dt
 from datetime import timedelta
 from typing import Any, Callable, Tuple
 
 import voluptuous as vol
 
-from myelectricaldatapy import Enedis
+from myelectricaldatapy import Enedis, EnedisException
 
 from .analytics import EnedisAnalytics
 from .const import (
     ATTR_CUM_PRICE,
     ATTR_CUM_VALUE,
     ATTR_END,
     ATTR_INTERVALS,
@@ -103,15 +104,15 @@
         self.access: dict[str, Any] = {}
         self.address: dict[str, Any] = {}
         self.contract: dict[str, Any] = {}
         self.ecowatt: dict[str, Any] = {}
         self.has_collected: bool = False
         self.intervals: list[Tuple[str, str]] = []
         self.last_access: dt = dt.now()
-        self.last_refresh: dt | None = None
+        self.last_refresh: date | None = None
         self.max_power: dict[str, Any] = {}
         self.tempo: dict[str, Any] = {}
 
     @property
     def is_connected(self) -> bool:
         """Connect state."""
         return self.access.get("valid", False) is True
@@ -168,38 +169,43 @@
                 tempo=self.tempo,
             )
             stats.update({mode: resultat})
         return stats
 
     async def async_update(self, force_refresh: bool = False) -> None:
         """Update data."""
-        self.access = await self._api.async_valid_access(self.pdl)
-        if "last_call" in self.access:
-            d_last_call = dt.strptime(
-                self.access["last_call"], "%Y-%m-%dT%H:%M:%S.%f"
-            ).date()
-            start = dt.now() - timedelta(days=1095)
-            end = dt.now() + timedelta(days=1)
-            if not self.contract or d_last_call != dt.now().date():
-                self.contract = await self._api.async_get_contract(self.pdl)
-            if not self.address or d_last_call != dt.now().date():
-                self.address = await self._api.async_get_address(self.pdl)
-            if self._ecowatt_subs:
-                self.ecowatt = await self._api.async_get_ecowatt(start, end)
-            if self._maxpower_subs:
-                self.max_power = await self._api.async_get_max_power(
-                    self.pdl, start, end
-                )
-            if self._params and (
-                d_last_call != dt.now().date()
-                or self.has_collected is False
-                or force_refresh is True
-            ):
-                await self.async_update_collects()
-                self.last_refresh = dt.now()
+        try:
+            self.access = await self._api.async_valid_access(self.pdl)
+        except EnedisException as error:
+            raise error from error
+        else:
+            try:
+                if self.is_quota_reached is False:
+                    start = dt.now() - timedelta(days=1095)
+                    end = dt.now() + timedelta(days=1)
+                    if not self.contract or self.last_refresh != dt.now().date():
+                        self.contract = await self._api.async_get_contract(self.pdl)
+                    if not self.address or self.last_refresh != dt.now().date():
+                        self.address = await self._api.async_get_address(self.pdl)
+                    if self._ecowatt_subs:
+                        self.ecowatt = await self._api.async_get_ecowatt(start, end)
+                    if self._maxpower_subs:
+                        self.max_power = await self._api.async_get_max_power(
+                            self.pdl, start, end
+                        )
+                    if self._params and (
+                        self.last_refresh != dt.now().date()
+                        or self.has_collected is False
+                        or force_refresh is True
+                    ):
+                        await self.async_update_collects()
+                        self.last_refresh = dt.now().date()
+            except EnedisException as error:
+                raise error from error
+        finally:
             self.last_access = dt.now()
 
     def tempo_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Tempo Subscription."""
         self._off_subs = False
         self._tempo_subs = activate is True
```

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.7
+Version: 1.9.8
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/pyproject.toml` & `myelectricaldatapy-1.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/setup.py` & `myelectricaldatapy-1.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.7",
+    version="1.9.8",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.7/tests/conftest.py` & `myelectricaldatapy-1.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/tests/consts.py` & `myelectricaldatapy-1.9.8/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/tests/test_analytics.py` & `myelectricaldatapy-1.9.8/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.7/tests/test_load_data.py` & `myelectricaldatapy-1.9.8/tests/test_load_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime as dt
 from unittest.mock import Mock, patch
 
 import pytest
 from freezegun import freeze_time
 
 import myelectricaldatapy
-from myelectricaldatapy import Enedis, EnedisByPDL
+from myelectricaldatapy import Enedis, EnedisByPDL, EnedisException, LimitReached
 
 from .consts import DATASET_30 as DS_30
 from .consts import INVALID_ACCESS, INVALID_ECOWATT
 
 PDL = "012345"
 TOKEN = "xxxxxxxxxxxxx"
 
@@ -111,15 +111,14 @@
 
 
 @pytest.mark.asyncio
 async def test_force_refresh(
     mock_enedis: Mock,  # pylint: disable=unused-argument
 ) -> None:
     """Test refresh object."""
-
     last_call = dt.now().strftime("%Y-%m-%dT%H:%M:%S.%f")
     access = {
         "valid": True,
         "quota_reached": False,
         "last_call": last_call,
     }
     with patch.object(
@@ -128,8 +127,40 @@
         api = EnedisByPDL(pdl=PDL, token=TOKEN)
         api.set_collects("consumption_load_curve")
         await api.async_update()
         save_refresh = api.last_refresh
         await api.async_update()
         assert api.last_refresh == save_refresh
         await api.async_update(force_refresh=True)
-        assert api.last_refresh != save_refresh
+        assert api.last_refresh == save_refresh
+
+
+@pytest.mark.asyncio
+async def test_exception(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
+    """Tests raise exception."""
+    with patch.object(
+        myelectricaldatapy.Enedis, "async_valid_access", side_effect=LimitReached()
+    ):
+        api = EnedisByPDL(pdl=PDL, token=TOKEN)
+        api.set_collects("consumption_load_curve")
+        try:
+            await api.async_update()
+        except EnedisException:
+            pass
+        assert api.last_access is not None
+        assert len(api.access) == 0
+
+    with patch.object(
+        myelectricaldatapy.Enedis,
+        "async_get_details_consumption",
+        side_effect=LimitReached(),
+    ):
+        api = EnedisByPDL(pdl=PDL, token=TOKEN)
+        api.set_collects("consumption_load_curve")
+        try:
+            await api.async_update()
+        except LimitReached:
+            pass
+        assert api.last_access is not None
+        assert api.access["valid"] is True
```

