# Comparing `tmp/myelectricaldatapy-1.9.9.tar.gz` & `tmp/myelectricaldatapy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.9.tar", last modified: Tue Apr 18 10:57:45 2023, max compression
+gzip compressed data, was "myelectricaldatapy-2.0.0.tar", last modified: Tue Apr 18 11:45:44 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.9.tar` & `myelectricaldatapy-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 10:57:45.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-18 10:57:43.000000 myelectricaldatapy-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    52825 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 11:45:43.000000 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 11:45:44.000000 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:45:43.000000 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 11:45:43.000000 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 11:45:43.000000 myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-18 11:45:43.000000 myelectricaldatapy-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:45:44.031675 myelectricaldatapy-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52825 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-18 11:45:34.000000 myelectricaldatapy-2.0.0/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.9/LICENSE` & `myelectricaldatapy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/PKG-INFO` & `myelectricaldatapy-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.9
+Version: 2.0.0
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.9/README.md` & `myelectricaldatapy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.0.0/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.0.0/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.0.0/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.0.0/myelectricaldatapy/mypdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import date
 from datetime import datetime as dt
 from datetime import timedelta
 from typing import Any, Callable, Tuple
 
 import voluptuous as vol
 
-from myelectricaldatapy import Enedis, EnedisException
+from myelectricaldatapy import Enedis, EnedisException, LimitReached
 
 from .analytics import EnedisAnalytics
 from .const import (
     ATTR_CUM_PRICE,
     ATTR_CUM_VALUE,
     ATTR_END,
     ATTR_INTERVALS,
@@ -115,19 +115,14 @@
 
     @property
     def is_connected(self) -> bool:
         """Connect state."""
         return self.access.get("valid", False) is True
 
     @property
-    def is_quota_reached(self) -> bool:
-        """Check quota."""
-        return self.access.get("quota_reached", True) is True
-
-    @property
     def has_intervals(self) -> bool:
         """Intervals exist."""
         return len(self.intervals) > 0
 
     @property
     def ecowatt_day(self) -> dict[str, Any]:
         """ecowatt."""
@@ -170,44 +165,44 @@
                 tempo=self.tempo,
             )
             stats.update({mode: resultat})
         return stats
 
     async def async_update(self, force_refresh: bool = False) -> None:
         """Update data."""
+        start = dt.now() - timedelta(days=1095)
+        end = dt.now() + timedelta(days=1)
         if force_refresh or self.last_access.date() != dt.now().date():
             self.contract = {}
             self.address = {}
             self.ecowatt = {}
             self.max_power = {}
             self.has_collected = False
         try:
             self.access = await self._api.async_valid_access(self.pdl)
+            if self.access.get("quota_reached", False):
+                detail = self.access.get("information", "Quota reached")
+                raise LimitReached(409, {"detail": detail})
+            if self.is_connected is False:
+                raise EnedisException(200, {"detail": "Api access not valid"})
+            if not self.contract:
+                self.contract = await self._api.async_get_contract(self.pdl)
+            if not self.address:
+                self.address = await self._api.async_get_address(self.pdl)
+            if not self.ecowatt and self._ecowatt_subs:
+                self.ecowatt = await self._api.async_get_ecowatt(start, end)
+            if not self.max_power and self._maxpower_subs:
+                self.max_power = await self._api.async_get_max_power(
+                    self.pdl, start, end
+                )
+            if self.has_parameters and self.has_collected is False:
+                await self.async_update_collects()
+                self.last_refresh = dt.now()
         except EnedisException as error:
             raise error from error
-        else:
-            try:
-                if self.is_quota_reached is False:
-                    start = dt.now() - timedelta(days=1095)
-                    end = dt.now() + timedelta(days=1)
-                    if not self.contract:
-                        self.contract = await self._api.async_get_contract(self.pdl)
-                    if not self.address:
-                        self.address = await self._api.async_get_address(self.pdl)
-                    if not self.ecowatt and self._ecowatt_subs:
-                        self.ecowatt = await self._api.async_get_ecowatt(start, end)
-                    if not self.max_power and self._maxpower_subs:
-                        self.max_power = await self._api.async_get_max_power(
-                            self.pdl, start, end
-                        )
-                    if self.has_parameters and self.has_collected is False:
-                        await self.async_update_collects()
-                        self.last_refresh = dt.now()
-            except EnedisException as error:
-                raise error from error
         finally:
             self.last_access = dt.now()
 
     def tempo_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Tempo Subscription."""
         self._off_subs = False
         self._tempo_subs = activate is True
```

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.9
+Version: 2.0.0
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.0.0/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/pyproject.toml` & `myelectricaldatapy-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/setup.py` & `myelectricaldatapy-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.9",
+    version="2.0.0",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.9/tests/conftest.py` & `myelectricaldatapy-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/tests/consts.py` & `myelectricaldatapy-2.0.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/tests/test_analytics.py` & `myelectricaldatapy-2.0.0/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.9/tests/test_load_data.py` & `myelectricaldatapy-2.0.0/tests/test_load_data.py`

 * *Files identical despite different names*

