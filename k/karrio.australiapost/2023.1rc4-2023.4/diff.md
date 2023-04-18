# Comparing `tmp/karrio.australiapost-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.australiapost-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7147 bytes, number of entries: 13
--rw-r--r--  2.0 unx      588 b- defN 22-Jul-20 22:36 karrio/mappers/australiapost/__init__.py
--rw-r--r--  2.0 unx     4257 b- defN 22-Jul-20 22:36 karrio/mappers/australiapost/mapper.py
--rw-r--r--  2.0 unx      918 b- defN 22-Sep-30 13:07 karrio/mappers/australiapost/proxy.py
--rw-r--r--  2.0 unx      493 b- defN 22-Sep-30 13:07 karrio/mappers/australiapost/settings.py
--rw-r--r--  2.0 unx      805 b- defN 22-Jul-20 22:36 karrio/providers/australiapost/__init__.py
--rw-r--r--  2.0 unx      812 b- defN 22-Jul-20 22:36 karrio/providers/australiapost/error.py
--rw-r--r--  2.0 unx     2371 b- defN 22-Sep-16 02:38 karrio/providers/australiapost/tracking.py
--rw-r--r--  2.0 unx     1340 b- defN 22-Apr-29 10:15 karrio/providers/australiapost/units.py
--rw-r--r--  2.0 unx      820 b- defN 22-Sep-30 13:07 karrio/providers/australiapost/utils.py
--rw-r--r--  2.0 unx     1020 b- defN 23-Jan-21 08:15 karrio.australiapost-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.australiapost-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.australiapost-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1228 b- defN 23-Jan-21 08:15 karrio.australiapost-2023.1rc4.dist-info/RECORD
-13 files, 14751 bytes uncompressed, 5033 bytes compressed:  65.9%
+Zip file size: 7122 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      588 b- defN 22-Nov-15 19:21 karrio/mappers/australiapost/__init__.py
+-rw-rw-r--  2.0 unx     4099 b- defN 23-Apr-01 12:45 karrio/mappers/australiapost/mapper.py
+-rw-rw-r--  2.0 unx      913 b- defN 23-Apr-01 12:45 karrio/mappers/australiapost/proxy.py
+-rw-rw-r--  2.0 unx      515 b- defN 23-Apr-15 06:44 karrio/mappers/australiapost/settings.py
+-rw-rw-r--  2.0 unx      805 b- defN 22-Nov-15 19:21 karrio/providers/australiapost/__init__.py
+-rw-rw-r--  2.0 unx      812 b- defN 22-Nov-15 19:21 karrio/providers/australiapost/error.py
+-rw-rw-r--  2.0 unx     2371 b- defN 23-Apr-01 15:18 karrio/providers/australiapost/tracking.py
+-rw-rw-r--  2.0 unx     1340 b- defN 22-Nov-15 19:21 karrio/providers/australiapost/units.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Apr-15 02:55 karrio/providers/australiapost/utils.py
+-rw-rw-r--  2.0 unx     1037 b- defN 23-Apr-18 07:10 karrio.australiapost-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.australiapost-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.australiapost-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1216 b- defN 23-Apr-18 07:10 karrio.australiapost-2023.4.dist-info/RECORD
+13 files, 14615 bytes uncompressed, 5032 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/australiapost/units.py
 Comment: 
 
 Filename: karrio/providers/australiapost/utils.py
 Comment: 
 
-Filename: karrio.australiapost-2023.1rc4.dist-info/METADATA
+Filename: karrio.australiapost-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.australiapost-2023.1rc4.dist-info/WHEEL
+Filename: karrio.australiapost-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.australiapost-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.australiapost-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.australiapost-2023.1rc4.dist-info/RECORD
+Filename: karrio.australiapost-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/australiapost/mapper.py

```diff
@@ -6,15 +6,14 @@
     # ShipmentCancelRequest,
     # PickupUpdateRequest,
     # PickupCancelRequest,
     # ShipmentRequest,
     TrackingRequest,
     # PickupRequest,
     # RateRequest,
-
     # AddressValidationDetails,
     # ConfirmationDetails,
     TrackingDetails,
     # ShipmentDetails,
     # PickupDetails,
     # RateDetails,
     Message,
@@ -24,15 +23,14 @@
     # parse_shipment_cancel_response,
     # parse_pickup_update_response,
     # parse_pickup_cancel_response,
     # parse_shipment_response,
     parse_tracking_response,
     # parse_pickup_response,
     # parse_rate_response,
-
     # address_validation_request,
     # shipment_cancel_request,
     # pickup_update_request,
     # pickup_cancel_request,
     tracking_request,
     # shipment_request,
     # pickup_request,
@@ -71,51 +69,49 @@
     #     self, payload: ShipmentRequest
     # ) -> Serializable:
     #     return shipment_request(payload, self.settings)
     #
     # def create_cancel_shipment_request(self, payload: ShipmentCancelRequest) -> Serializable:
     #     return shipment_cancel_request(payload, self.settings)
 
-    def create_tracking_request(
-        self, payload: TrackingRequest
-    ) -> Serializable:
+    def create_tracking_request(self, payload: TrackingRequest) -> Serializable:
         return tracking_request(payload, self.settings)
 
     # def parse_address_validation_response(
     #     self, response: Deserializable
     # ) -> Tuple[AddressValidationDetails, List[Message]]:
-    #     return parse_address_validation_response(response.deserialize(), self.settings)
+    #     return parse_address_validation_response(response, self.settings)
     #
     # def parse_cancel_pickup_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_pickup_cancel_response(response.deserialize(), self.settings)
+    #     return parse_pickup_cancel_response(response, self.settings)
     #
     # def parse_pickup_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[PickupDetails, List[Message]]:
-    #     return parse_pickup_response(response.deserialize(), self.settings)
+    #     return parse_pickup_response(response, self.settings)
     #
     # def parse_pickup_update_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[PickupDetails, List[Message]]:
-    #     return parse_pickup_update_response(response.deserialize(), self.settings)
+    #     return parse_pickup_update_response(response, self.settings)
 
     # def parse_rate_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[List[RateDetails], List[Message]]:
-    #     return parse_rate_response(response.deserialize(), self.settings)
+    #     return parse_rate_response(response, self.settings)
 
     # def parse_shipment_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[ShipmentDetails, List[Message]]:
-    #     return parse_shipment_response(response.deserialize(), self.settings)
+    #     return parse_shipment_response(response, self.settings)
     #
     # def parse_cancel_shipment_response(
     #     self, response: Deserializable
     # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_shipment_cancel_response(response.deserialize(), self.settings)
+    #     return parse_shipment_cancel_response(response, self.settings)
 
     def parse_tracking_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[List[TrackingDetails], List[Message]]:
-        return parse_tracking_response(response.deserialize(), self.settings)
+        return parse_tracking_response(response, self.settings)
```

## karrio/mappers/australiapost/proxy.py

```diff
@@ -5,15 +5,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         query = urllib.parse.urlencode(request.serialize())
         response = http(
             url=f"{self.settings.server_url}/shipping/v1/track?{query}",
             trace=self.trace_as("json"),
             method="GET",
             headers={
                 "Content-Type": "application/json",
```

## karrio/mappers/australiapost/settings.py

```diff
@@ -15,7 +15,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "australiapost"
     account_country_code: str = "AU"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/australiapost/tracking.py

```diff
@@ -1,41 +1,38 @@
+import karrio.lib as lib
 from typing import List, Tuple
 from australiapost_lib.tracking import (
     TrackingRequest as CarrierTrackingRequest,
     TrackingResult,
 )
-from karrio.core.utils import (
-    Serializable,
-    DF,
-    DP,
-)
 from karrio.core.models import (
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.australiapost.utils import Settings
 from karrio.providers.australiapost.error import parse_error_response
 
 
 def parse_tracking_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict], settings: Settings
 ) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
     tracking_results = response.get("tracking_results", [])
     errors = sum(
         [
-            _extract_error(DP.to_object(TrackingResult, result), settings)
+            _extract_error(lib.to_object(TrackingResult, result), settings)
             for result in tracking_results
             if "errors" in result
         ],
         parse_error_response(response, settings),
     )
     tracking_details = [
-        _extract_detail(DP.to_object(TrackingResult, d), settings)
+        _extract_detail(lib.to_object(TrackingResult, d), settings)
         for d in response.get("tracking_results", [])
         if "trackable_items" in d
     ]
 
     return tracking_details, errors
 
 
@@ -57,24 +54,22 @@
 
     return TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         tracking_number=detail.tracking_id,
         events=[
             TrackingEvent(
-                date=DF.fdate(event.date, "%Y-%m-%dT%H:%M:%S%z"),
+                date=lib.fdate(event.date, "%Y-%m-%dT%H:%M:%S%z"),
                 description=event.description,
                 location=event.location,
-                time=DF.ftime(event.date, "%Y-%m-%dT%H:%M:%S%z"),
+                time=lib.ftime(event.date, "%Y-%m-%dT%H:%M:%S%z"),
             )
             for event in item.events
         ],
         delivered=(detail.status == "Delivered"),
     )
 
 
-def tracking_request(
-    payload: TrackingRequest, _
-) -> Serializable[CarrierTrackingRequest]:
+def tracking_request(payload: TrackingRequest, _) -> lib.Serializable:
     request = CarrierTrackingRequest(tracking_ids=",".join(payload.tracking_numbers))
 
-    return Serializable(request, DP.to_dict)
+    return lib.Serializable(request, lib.to_dict)
```

## Comparing `karrio.australiapost-2023.1rc4.dist-info/METADATA` & `karrio.australiapost-2023.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.australiapost
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Australia Post Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-Requires-Dist: karrio
 Requires-Dist: carrier.australiapost
+Requires-Dist: karrio
 
 # karrio.carrier_name
 
 This package is a Australia Post extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
 ## Requirements
 
@@ -39,7 +40,9 @@
     Settings(
         ...
     )
 )
 ```
 
 Check the [Karrio Mutli-carrier SDK docs](https://docs.karrio.io) for Shipping API requests
+
+
```

## Comparing `karrio.australiapost-2023.1rc4.dist-info/RECORD` & `karrio.australiapost-2023.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 karrio/mappers/australiapost/__init__.py,sha256=V8yq79XycE_TRNjxmFGuczSw5iH6-GPc-uwgLtRb8N4,588
-karrio/mappers/australiapost/mapper.py,sha256=H7MRAcOrZZbBDWmmNKd1xl458DFpRogEva6UGlirZBU,4257
-karrio/mappers/australiapost/proxy.py,sha256=EFSt3eYD5KeiktnC2PtaghRRbuLXwzOdUMSPUz0m7rY,918
-karrio/mappers/australiapost/settings.py,sha256=XPjTrymxg_C3QEZLcHsfRIy0w2zHl6wjRMXQguqIzbI,493
+karrio/mappers/australiapost/mapper.py,sha256=P63Pj8rhRmTb_OGeYtskByUO8BGVvfXcAfbp6X5UiN4,4099
+karrio/mappers/australiapost/proxy.py,sha256=P6Ho7gfXVOfQcf3KPA_qtQbZjoGBH5rz5VwAD_5CX1k,913
+karrio/mappers/australiapost/settings.py,sha256=OwRHtX4ce3IBUZbWKOPe_nAXOv5QTpMOslmrdvE0Ydk,515
 karrio/providers/australiapost/__init__.py,sha256=VWxoktcysztS3NwibUHVCiKCHaO11kMtI8s-khqE2AY,805
 karrio/providers/australiapost/error.py,sha256=rIq0BY1dJLkzu5_l62YDsWtQdlHu2FGW2lP3v5e7Y5Q,812
-karrio/providers/australiapost/tracking.py,sha256=eaVuVkCpDXo4xFMJF3nW-07h_fk3-wx2EOl93hkDoR0,2371
+karrio/providers/australiapost/tracking.py,sha256=saabQr724o1sPWifMo7vToYLO7UL9czjNzg45sKEgPM,2371
 karrio/providers/australiapost/units.py,sha256=IfvgizMZH3jn6PQLrBxtH4Bd7GhPf2TJ7DQRwnFHhvw,1340
 karrio/providers/australiapost/utils.py,sha256=sKweE5MwZ6DvjB9Dvz_RVAbXfBM0GmtGBDy9cEJxJ0k,820
-karrio.australiapost-2023.1rc4.dist-info/METADATA,sha256=-3a7rkCu9RqOnANcBU45Vk71iAwXN_QCGok3ohpkN4k,1020
-karrio.australiapost-2023.1rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-karrio.australiapost-2023.1rc4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.australiapost-2023.1rc4.dist-info/RECORD,,
+karrio.australiapost-2023.4.dist-info/METADATA,sha256=bAyMbg_8Npv674aw5CR-FUusLwrYHV1tBAfP2hQV_Ts,1037
+karrio.australiapost-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.australiapost-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.australiapost-2023.4.dist-info/RECORD,,
```

