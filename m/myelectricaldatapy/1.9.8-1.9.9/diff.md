# Comparing `tmp/myelectricaldatapy-1.9.8.tar.gz` & `tmp/myelectricaldatapy-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.8.tar", last modified: Tue Apr 18 09:19:12 2023, max compression
+gzip compressed data, was "myelectricaldatapy-1.9.9.tar", last modified: Tue Apr 18 10:57:45 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.8.tar` & `myelectricaldatapy-1.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 09:19:12.000000 myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-18 09:19:11.000000 myelectricaldatapy-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:12.090294 myelectricaldatapy-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-18 09:19:01.000000 myelectricaldatapy-1.9.8/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 10:57:45.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 10:57:44.000000 myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:57:45.044773 myelectricaldatapy-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-18 10:57:43.000000 myelectricaldatapy-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:45.040773 myelectricaldatapy-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52825 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-18 10:57:34.000000 myelectricaldatapy-1.9.9/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.8/LICENSE` & `myelectricaldatapy-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/PKG-INFO` & `myelectricaldatapy-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.8
+Version: 1.9.9
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.8/README.md` & `myelectricaldatapy-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy/analytics.py` & `myelectricaldatapy-1.9.9/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy/auth.py` & `myelectricaldatapy-1.9.9/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-1.9.9/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-1.9.9/myelectricaldatapy/mypdl.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         self._params: dict[str, dict[str, Any]] = {}
         self._tempo_subs: bool = False
         self.access: dict[str, Any] = {}
         self.address: dict[str, Any] = {}
         self.contract: dict[str, Any] = {}
         self.ecowatt: dict[str, Any] = {}
         self.has_collected: bool = False
+        self.has_parameters: bool = False
         self.intervals: list[Tuple[str, str]] = []
         self.last_access: dt = dt.now()
         self.last_refresh: date | None = None
         self.max_power: dict[str, Any] = {}
         self.tempo: dict[str, Any] = {}
 
     @property
@@ -169,40 +170,42 @@
                 tempo=self.tempo,
             )
             stats.update({mode: resultat})
         return stats
 
     async def async_update(self, force_refresh: bool = False) -> None:
         """Update data."""
+        if force_refresh or self.last_access.date() != dt.now().date():
+            self.contract = {}
+            self.address = {}
+            self.ecowatt = {}
+            self.max_power = {}
+            self.has_collected = False
         try:
             self.access = await self._api.async_valid_access(self.pdl)
         except EnedisException as error:
             raise error from error
         else:
             try:
                 if self.is_quota_reached is False:
                     start = dt.now() - timedelta(days=1095)
                     end = dt.now() + timedelta(days=1)
-                    if not self.contract or self.last_refresh != dt.now().date():
+                    if not self.contract:
                         self.contract = await self._api.async_get_contract(self.pdl)
-                    if not self.address or self.last_refresh != dt.now().date():
+                    if not self.address:
                         self.address = await self._api.async_get_address(self.pdl)
-                    if self._ecowatt_subs:
+                    if not self.ecowatt and self._ecowatt_subs:
                         self.ecowatt = await self._api.async_get_ecowatt(start, end)
-                    if self._maxpower_subs:
+                    if not self.max_power and self._maxpower_subs:
                         self.max_power = await self._api.async_get_max_power(
                             self.pdl, start, end
                         )
-                    if self._params and (
-                        self.last_refresh != dt.now().date()
-                        or self.has_collected is False
-                        or force_refresh is True
-                    ):
+                    if self.has_parameters and self.has_collected is False:
                         await self.async_update_collects()
-                        self.last_refresh = dt.now().date()
+                        self.last_refresh = dt.now()
             except EnedisException as error:
                 raise error from error
         finally:
             self.last_access = dt.now()
 
     def tempo_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Tempo Subscription."""
@@ -275,15 +278,15 @@
         start: dt | None = None,
         end: dt | None = None,
         intervals: list[Tuple[str, str]] | None = None,
         prices: dict[str, Any] | None = None,
         cum_value: dict[str, Any] | None = None,
         cum_price: dict[str, Any] | None = None,
     ) -> None:
-        """Set datas collect."""
+        """Set parameters for data collect."""
         funcs: dict[str, Callable[..., Any]] = {
             DAILY_PROD: self._api.async_get_daily_production,
             DETAIL_PROD: self._api.async_get_details_production,
             DAILY_CONSUM: self._api.async_get_daily_consumption,
             DETAIL_CONSUM: self._api.async_get_details_consumption,
         }
         days = 1095 if service in [DAILY_PROD, DAILY_CONSUM] else 7
@@ -296,27 +299,31 @@
             self._set_intervals(mode, intervals)
         if prices:
             self._set_prices(mode, prices)
         if cum_value:
             self._set_cumsum(mode, "value", cum_value)
         if cum_price:
             self._set_cumsum(mode, "price", cum_price)
+        self.has_parameters = True
 
     async def async_update_collects(self) -> None:
         """Update data to collect."""
-        dataset = {}
         checked = True
         self.has_collected = False
         for mode, _param in self._params.items():
+            dataset = {}
             start = _param[ATTR_START]
             end = _param[ATTR_END]
             if func := _param.get("func"):
-                dataset = await func(self.pdl, start, end)
+                try:
+                    dataset = await func(self.pdl, start, end)
+                except EnedisException as error:
+                    checked = False
+                    _LOGGER.error(error.args[1]["detail"])
                 data = dataset.get("meter_reading", {}).get("interval_reading", {})
                 if len(data) != 0:
                     checked = checked and len(data) != 0
-                    self._params[mode].pop("func")
                     self._params[mode].update({"data": data})
                 if mode == CONSUMPTION and self._tempo_subs:
                     self.tempo = await self._api.async_get_tempo(start, end)
 
         self.has_collected = checked
```

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.8
+Version: 1.9.9
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.8/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-1.9.9/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/pyproject.toml` & `myelectricaldatapy-1.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.8/setup.py` & `myelectricaldatapy-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.8",
+    version="1.9.9",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.8/tests/conftest.py` & `myelectricaldatapy-1.9.9/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Generator
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
 import myelectricaldatapy
 
-from .consts import ACCESS, DATASET_30, DATASET_DAILY, ECOWATT, TEMPO
+from .consts import ACCESS, ADDRESS, CONTRACT, DATASET_30, DATASET_DAILY, ECOWATT, TEMPO
 
 
 @pytest.fixture(name="mock_enedis")
 def mock_enedis() -> Generator[AsyncMock, None, None]:
     """Mock a successful connection."""
     with patch.object(
         myelectricaldatapy.Enedis,
@@ -23,16 +23,16 @@
     ), patch.object(
         myelectricaldatapy.Enedis,
         "async_get_details_consumption",
         return_value=DATASET_30,
     ), patch.object(
         myelectricaldatapy.Enedis, "async_valid_access", return_value=ACCESS
     ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_contract", return_value={}
+        myelectricaldatapy.Enedis, "async_get_contract", return_value=CONTRACT
     ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_address", return_value={}
+        myelectricaldatapy.Enedis, "async_get_address", return_value=ADDRESS
     ), patch.object(
         myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO
     ), patch.object(
         myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=ECOWATT
     ) as service_mock:
         yield service_mock
```

### Comparing `myelectricaldatapy-1.9.8/tests/consts.py` & `myelectricaldatapy-1.9.9/tests/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,71 @@
+"""Test constants."""
+PDL = "01234567890"
+TOKEN = "xxxxxxxxxxxxx"
+
 ACCESS = {
     "valid": True,
     "consent_expiration_date": "2026-01-14T15:32:38",
     "call_number": 7,
     "quota_reached": False,
     "quota_limit": 50,
     "quota_reset_at": "2023-03-01T23:59:59.999999",
     "last_call": "2023-03-01T13:58:24.532501",
     "ban": False,
 }
 
+ADDRESS = {
+    "customer": {
+        "customer_id": "-1137954749",
+        "usage_points": [
+            {
+                "usage_point": {
+                    "usage_point_id": "01234567890",
+                    "usage_point_status": "com",
+                    "meter_type": "AMM",
+                    "usage_point_addresses": {
+                        "street": "1 rue du",
+                        "locality": None,
+                        "postal_code": "00666",
+                        "insee_code": "12345",
+                        "city": "XX YY",
+                        "country": "France",
+                        "geo_points": {},
+                    },
+                }
+            }
+        ],
+    }
+}
+
+CONTRACT = {
+    "customer": {
+        "customer_id": "-1137954749",
+        "usage_points": [
+            {
+                "usage_point": {
+                    "usage_point_id": "01234567890",
+                    "usage_point_status": "com",
+                    "meter_type": "AMM",
+                },
+                "contracts": {
+                    "segment": "C5",
+                    "subscribed_power": "9 kVA",
+                    "last_activation_date": "2006-05-24+02:00",
+                    "distribution_tariff": "BTINFMUDT",
+                    "offpeak_hours": "HC (1H30-8H00;12H30-14H00)",
+                    "contract_status": "SERVC",
+                    "last_distribution_tariff_change_date": "2019-09-13+02:00",
+                },
+            }
+        ],
+    }
+}
+
+
 INVALID_ACCESS = {
     "valid": False,
     "information": "Vous avez dépassé votre quota journalier (50)",
     "consent_expiration_date": "2026-01-14T15:32:38",
     "call_number": 65,
     "quota_reached": True,
     "quota_limit": 50,
@@ -86,15 +139,15 @@
         },
     },
 }
 
 
 DATASET_30 = {
     "meter_reading": {
-        "usage_point_id": "09171201102829",
+        "usage_point_id": "01234567890",
         "start": "2023-03-01",
         "end": "2023-03-08",
         "quality": "BRUT",
         "reading_type": {
             "measurement_kind": "power",
             "unit": "W",
             "aggregate": "average",
@@ -966,15 +1019,15 @@
             },
         ],
     }
 }
 
 DATASET_DAILY_COMPARE = {
     "meter_reading": {
-        "usage_point_id": "012345",
+        "usage_point_id": "01234567890",
         "start": "2022-03-08",
         "end": "2023-03-08",
         "quality": "BRUT",
         "reading_type": {
             "measurement_kind": "energy",
             "measuring_period": "P1D",
             "unit": "Wh",
@@ -986,15 +1039,15 @@
             {"value": "81972", "date": "2023-03-03"},
         ],
     }
 }
 
 DATASET_DAILY = {
     "meter_reading": {
-        "usage_point_id": "012345",
+        "usage_point_id": "01234567890",
         "start": "2022-03-08",
         "end": "2023-03-08",
         "quality": "BRUT",
         "reading_type": {
             "measurement_kind": "energy",
             "measuring_period": "P1D",
             "unit": "Wh",
```

### Comparing `myelectricaldatapy-1.9.8/tests/test_analytics.py` & `myelectricaldatapy-1.9.9/tests/test_analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 
 import pytest
 from freezegun import freeze_time
 
 import myelectricaldatapy
 from myelectricaldatapy import EnedisByPDL
 
-from .consts import DATASET_DAILY_COMPARE
-
-PDL = "012345"
-TOKEN = "xxxxxxxxxxxxx"
+from .consts import DATASET_DAILY_COMPARE, PDL, TOKEN
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
 async def test_compute(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test standard."""
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
@@ -286,7 +283,26 @@
 
     api.set_collects(
         "consumption_load_curve", start=dt.strptime("2023-3-7", "%Y-%m-%d")
     )
     await api.async_update_collects()
     resultat = api.stats["consumption"]
     assert len(resultat) == 0
+
+
+@freeze_time("2023-3-1")
+@pytest.mark.asyncio
+async def test_twice_call(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
+    """Tests raise exception."""
+    intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
+    api = EnedisByPDL(pdl=PDL, token=TOKEN)
+    api.set_collects("consumption_load_curve", intervals=intervals)
+    api.set_collects("daily_production")
+    await api.async_update()
+    assert len(api.stats["consumption"]) != 0
+    assert len(api.stats["production"]) != 0
+    assert api.stats["consumption"][0]["notes"] == "offpeak"
+    assert api.stats["production"][0]["notes"] == "standard"
+    await api.async_update()
+    assert api.last_access is not None
```

### Comparing `myelectricaldatapy-1.9.8/tests/test_load_data.py` & `myelectricaldatapy-1.9.9/tests/test_load_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 import pytest
 from freezegun import freeze_time
 
 import myelectricaldatapy
 from myelectricaldatapy import Enedis, EnedisByPDL, EnedisException, LimitReached
 
-from .consts import DATASET_30 as DS_30
-from .consts import INVALID_ACCESS, INVALID_ECOWATT
-
-PDL = "012345"
-TOKEN = "xxxxxxxxxxxxx"
+from .consts import DATASET_30, INVALID_ACCESS, INVALID_ECOWATT, PDL, TOKEN
 
 
 @freeze_time("2023-01-23")
 @pytest.mark.asyncio
 async def test_ecowatt(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test get ecowatt."""
     api = Enedis(token=TOKEN)
@@ -73,48 +69,30 @@
         assert resultat["quota_reached"] is True
 
 
 @pytest.mark.asyncio
 async def test_fetch_data() -> None:
     """Test fetch data."""
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DS_30
+        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DATASET_30
     ):
         api = Enedis(token=TOKEN)
         resultat = await api.async_fetch_datas(
             service="comsumption_load_curve",
             pdl=PDL,
             start=dt.strptime("2022-12-30", "%Y-%m-%d"),
             end=dt.strptime("2022-12-31", "%Y-%m-%d"),
         )
         assert (
             resultat["meter_reading"]["interval_reading"]
-            == DS_30["meter_reading"]["interval_reading"]  # noqa
+            == DATASET_30["meter_reading"]["interval_reading"]  # noqa
         )
 
 
 @pytest.mark.asyncio
-async def test_load() -> None:
-    """Test load object."""
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DS_30
-    ):
-        api = Enedis(token=TOKEN)
-        await api.async_get_max_power(PDL, dt.now(), dt.now())
-        await api.async_get_contract(PDL)
-        await api.async_get_address(PDL)
-        await api.async_has_offpeak(PDL)
-        await api.async_check_offpeak(PDL, dt.now())
-        await api.async_get_identity(PDL)
-        await api.async_get_daily_consumption(PDL, dt.now(), dt.now())
-        await api.async_get_daily_production(PDL, dt.now(), dt.now())
-        await api.async_get_details_production(PDL, dt.now(), dt.now())
-
-
-@pytest.mark.asyncio
 async def test_force_refresh(
     mock_enedis: Mock,  # pylint: disable=unused-argument
 ) -> None:
     """Test refresh object."""
     last_call = dt.now().strftime("%Y-%m-%dT%H:%M:%S.%f")
     access = {
         "valid": True,
@@ -127,40 +105,58 @@
         api = EnedisByPDL(pdl=PDL, token=TOKEN)
         api.set_collects("consumption_load_curve")
         await api.async_update()
         save_refresh = api.last_refresh
         await api.async_update()
         assert api.last_refresh == save_refresh
         await api.async_update(force_refresh=True)
-        assert api.last_refresh == save_refresh
+        assert api.last_refresh != save_refresh
 
 
 @pytest.mark.asyncio
 async def test_exception(
     mock_enedis: Mock,  # pylint: disable=unused-argument
 ) -> None:
     """Tests raise exception."""
     with patch.object(
-        myelectricaldatapy.Enedis, "async_valid_access", side_effect=LimitReached()
+        myelectricaldatapy.Enedis,
+        "async_valid_access",
+        side_effect=LimitReached(500, {"detail": "Limit reached"}),
     ):
         api = EnedisByPDL(pdl=PDL, token=TOKEN)
         api.set_collects("consumption_load_curve")
         try:
             await api.async_update()
         except EnedisException:
             pass
         assert api.last_access is not None
         assert len(api.access) == 0
 
     with patch.object(
         myelectricaldatapy.Enedis,
         "async_get_details_consumption",
-        side_effect=LimitReached(),
+        side_effect=LimitReached(500, {"detail": "Limit reached"}),
     ):
         api = EnedisByPDL(pdl=PDL, token=TOKEN)
         api.set_collects("consumption_load_curve")
         try:
             await api.async_update()
         except LimitReached:
             pass
         assert api.last_access is not None
         assert api.access["valid"] is True
+
+    with patch.object(
+        myelectricaldatapy.Enedis,
+        "async_get_details_consumption",
+        side_effect=EnedisException(500, {"detail": "Error"}),
+    ):
+        api = EnedisByPDL(pdl=PDL, token=TOKEN)
+        api.set_collects("consumption_load_curve")
+        api.set_collects("daily_production")
+        try:
+            await api.async_update()
+            await api.async_update()
+        except EnedisException:
+            pass
+        assert api.last_access is not None
+        assert api.access["valid"] is True
```

