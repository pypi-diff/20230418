# Comparing `tmp/karrio.generic-2023.3-py3-none-any.whl.zip` & `tmp/karrio.generic-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4957 bytes, number of entries: 11
+Zip file size: 4960 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      535 b- defN 23-Mar-03 13:50 karrio/mappers/generic/__init__.py
--rw-rw-r--  2.0 unx     1225 b- defN 23-Mar-03 13:50 karrio/mappers/generic/mapper.py
+-rw-rw-r--  2.0 unx     1182 b- defN 23-Apr-01 13:34 karrio/mappers/generic/mapper.py
 -rw-rw-r--  2.0 unx      438 b- defN 23-Mar-03 13:50 karrio/mappers/generic/proxy.py
--rw-rw-r--  2.0 unx      990 b- defN 23-Mar-03 13:50 karrio/mappers/generic/settings.py
+-rw-rw-r--  2.0 unx     1012 b- defN 23-Apr-15 06:44 karrio/mappers/generic/settings.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-03 13:50 karrio/providers/generic/__init__.py
--rw-rw-r--  2.0 unx     2057 b- defN 23-Mar-21 13:06 karrio/providers/generic/units.py
+-rw-rw-r--  2.0 unx     2057 b- defN 23-Mar-27 07:55 karrio/providers/generic/units.py
 -rw-rw-r--  2.0 unx      236 b- defN 23-Mar-03 13:50 karrio/providers/generic/utils.py
--rw-rw-r--  2.0 unx      964 b- defN 23-Mar-27 07:12 karrio.generic-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.generic-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.generic-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      953 b- defN 23-Mar-27 07:12 karrio.generic-2023.3.dist-info/RECORD
-11 files, 7497 bytes uncompressed, 3313 bytes compressed:  55.8%
+-rw-rw-r--  2.0 unx      964 b- defN 23-Apr-18 07:09 karrio.generic-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.generic-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.generic-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      954 b- defN 23-Apr-18 07:09 karrio.generic-2023.4.dist-info/RECORD
+11 files, 7477 bytes uncompressed, 3316 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: karrio/providers/generic/units.py
 Comment: 
 
 Filename: karrio/providers/generic/utils.py
 Comment: 
 
-Filename: karrio.generic-2023.3.dist-info/METADATA
+Filename: karrio.generic-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.generic-2023.3.dist-info/WHEEL
+Filename: karrio.generic-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.generic-2023.3.dist-info/top_level.txt
+Filename: karrio.generic-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.generic-2023.3.dist-info/RECORD
+Filename: karrio.generic-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/generic/mapper.py

```diff
@@ -20,19 +20,19 @@
 
 class Mapper(BaseMapper):
     settings: Settings
 
     def create_rate_request(self, payload: RateRequest) -> Serializable:
         return rate_request(payload, self.settings)
 
-    def create_shipment_request(self, payload: Serializable[str]) -> Serializable:
+    def create_shipment_request(self, payload: Serializable) -> Serializable:
         return shipment_request(payload, self.settings)
 
     def parse_rate_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[List[RateDetails], List[Message]]:
-        return parse_rate_response(response.deserialize(), self.settings)
+        return parse_rate_response(response, self.settings)
 
     def parse_shipment_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[ShipmentDetails, List[Message]]:
-        return parse_shipment_response(response.deserialize(), self.settings)
+        return parse_shipment_response(response, self.settings)
```

## karrio/mappers/generic/settings.py

```diff
@@ -19,10 +19,11 @@
 
     id: str = None
     test_mode: bool = False
     carrier_id: str = "custom-carrier"
     account_number: str = None
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     label_template: LabelTemplate = JStruct[LabelTemplate]
     services: List[ServiceLevel] = JList[ServiceLevel, False, dict(default=DEFAULT_SERVICES)]  # type: ignore
```

## Comparing `karrio.generic-2023.3.dist-info/METADATA` & `karrio.generic-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.generic
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - Custom carrier Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.generic-2023.3.dist-info/RECORD` & `karrio.generic-2023.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 karrio/mappers/generic/__init__.py,sha256=WdDG6VWk3abMU_RTgpVZ_-A7cwaIBEkIl3J5JVaElgs,535
-karrio/mappers/generic/mapper.py,sha256=5QtSd1x7PNxGpq36t8Jllo7up9nH57qpF4Nal5MIJ8E,1225
+karrio/mappers/generic/mapper.py,sha256=vzWGp4DzadAmrUqzBZbVtDdy0-g55iPKCXeSTWuXiCk,1182
 karrio/mappers/generic/proxy.py,sha256=nQxbLSwouoP_Vm0sjiutsELSEQEfz96ZYEqR7I3QAgM,438
-karrio/mappers/generic/settings.py,sha256=ZnyT7Y0gsdal1Uk4P1JkgMBbl7FpAJxUhqt3tV3OY9I,990
+karrio/mappers/generic/settings.py,sha256=tji6NJ_XBhjN2qf-NeBpea7NJKhrvx_HD-lHoz00EF4,1012
 karrio/providers/generic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 karrio/providers/generic/units.py,sha256=BB-fs1FGaR-VyycGuyz--XdYUyUcqb2aVtXcJ0NokKA,2057
 karrio/providers/generic/utils.py,sha256=7XskSiXksgwIg2FrxQktmxv8E_boyAboeANCSBEphb8,236
-karrio.generic-2023.3.dist-info/METADATA,sha256=wgjfmScn79fm5UWbrNdfG2OVqeB296IeEielRWNHq0I,964
-karrio.generic-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.generic-2023.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.generic-2023.3.dist-info/RECORD,,
+karrio.generic-2023.4.dist-info/METADATA,sha256=C2pmK2CMbf1fDpMSvJQVYwWvT4RKKkjWm8mP833O-6I,964
+karrio.generic-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.generic-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.generic-2023.4.dist-info/RECORD,,
```

