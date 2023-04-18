# Comparing `tmp/karrio.sendle-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.sendle-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6848 bytes, number of entries: 13
--rw-r--r--  2.0 unx      545 b- defN 22-Jul-20 22:36 karrio/mappers/sendle/__init__.py
--rw-r--r--  2.0 unx     4246 b- defN 22-Jul-20 22:36 karrio/mappers/sendle/mapper.py
--rw-r--r--  2.0 unx     1165 b- defN 22-Sep-30 13:07 karrio/mappers/sendle/proxy.py
--rw-r--r--  2.0 unx      440 b- defN 22-Sep-30 13:07 karrio/mappers/sendle/settings.py
--rw-r--r--  2.0 unx      763 b- defN 22-Jul-20 22:36 karrio/providers/sendle/__init__.py
--rw-r--r--  2.0 unx      754 b- defN 22-Jul-20 22:36 karrio/providers/sendle/error.py
--rw-r--r--  2.0 unx     2008 b- defN 22-Apr-29 10:15 karrio/providers/sendle/tracking.py
--rw-r--r--  2.0 unx     1332 b- defN 22-Apr-29 10:15 karrio/providers/sendle/units.py
--rw-r--r--  2.0 unx      687 b- defN 22-Sep-30 13:07 karrio/providers/sendle/utils.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jan-21 08:16 karrio.sendle-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:16 karrio.sendle-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.sendle-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1137 b- defN 23-Jan-21 08:16 karrio.sendle-2023.1rc4.dist-info/RECORD
-13 files, 14139 bytes uncompressed, 4916 bytes compressed:  65.2%
+Zip file size: 6955 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      545 b- defN 22-Nov-15 19:21 karrio/mappers/sendle/__init__.py
+-rw-rw-r--  2.0 unx     4085 b- defN 23-Apr-01 12:45 karrio/mappers/sendle/mapper.py
+-rw-rw-r--  2.0 unx     1165 b- defN 22-Nov-15 19:21 karrio/mappers/sendle/proxy.py
+-rw-rw-r--  2.0 unx      462 b- defN 23-Apr-15 06:44 karrio/mappers/sendle/settings.py
+-rw-rw-r--  2.0 unx      763 b- defN 22-Nov-15 19:21 karrio/providers/sendle/__init__.py
+-rw-rw-r--  2.0 unx      754 b- defN 22-Nov-15 19:21 karrio/providers/sendle/error.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Apr-01 15:18 karrio/providers/sendle/tracking.py
+-rw-rw-r--  2.0 unx     1332 b- defN 22-Nov-15 19:21 karrio/providers/sendle/units.py
+-rw-rw-r--  2.0 unx      687 b- defN 23-Apr-15 02:55 karrio/providers/sendle/utils.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Apr-18 07:09 karrio.sendle-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.sendle-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.sendle-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1125 b- defN 23-Apr-18 07:09 karrio.sendle-2023.4.dist-info/RECORD
+13 files, 14745 bytes uncompressed, 5047 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/sendle/units.py
 Comment: 
 
 Filename: karrio/providers/sendle/utils.py
 Comment: 
 
-Filename: karrio.sendle-2023.1rc4.dist-info/METADATA
+Filename: karrio.sendle-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.sendle-2023.1rc4.dist-info/WHEEL
+Filename: karrio.sendle-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.sendle-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.sendle-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.sendle-2023.1rc4.dist-info/RECORD
+Filename: karrio.sendle-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/sendle/mapper.py

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
@@ -71,54 +69,49 @@
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
 
-
-
-
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

## karrio/mappers/sendle/settings.py

```diff
@@ -14,7 +14,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "sendle"
     account_country_code: str = "AU"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/sendle/tracking.py

```diff
@@ -1,63 +1,72 @@
-from typing import List, Tuple
-from sendle_lib.tracking_response import Tracking
-from karrio.core.utils import (
-    Serializable,
-    DF,
-    DP,
-)
-from karrio.core.models import (
-    TrackingEvent,
-    TrackingDetails,
-    TrackingRequest,
-    Message,
-)
-from karrio.providers.sendle.utils import Settings
-from karrio.providers.sendle.error import parse_error_response
+import sendle_lib.tracking_response as sendle
+import typing
+import karrio.lib as lib
+import karrio.core.models as models
+import karrio.providers.sendle.error as error
+import karrio.providers.sendle.utils as provider_utils
 
 
 def parse_tracking_response(
-    response: List[Tuple[str, dict]], settings: Settings
-) -> Tuple[List[TrackingDetails], List[Message]]:
-    errors = [e for ref, e in response if "error" in e]
+    _response: lib.Deserializable[typing.List[typing.Tuple[str, dict]]],
+    settings: provider_utils.Settings,
+) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
+    errors = [e for _, e in response if "error" in e]
     tracking_details = [
-        _extract_detail((ref, DP.to_object(Tracking, d)), settings)
+        _extract_detail((ref, lib.to_object(sendle.Tracking, d)), settings)
         for ref, d in response
         if "tracking_events" in d
     ]
 
-    return tracking_details, parse_error_response(errors, settings)
+    return tracking_details, error.parse_error_response(errors, settings)
 
 
 def _extract_detail(
-    detail: Tuple[str, Tracking], settings: Settings
-) -> TrackingDetails:
+    detail: typing.Tuple[str, sendle.Tracking], settings: provider_utils.Settings
+) -> models.TrackingDetails:
     tracking_number, tracking_details = detail
     estimated_delivery = (
         tracking_details.scheduling.estimated_delivery_date_minimum
         or tracking_details.scheduling.estimated_delivery_date_maximum
         or tracking_details.scheduling.delivered_on
     )
 
-    return TrackingDetails(
+    return models.TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         tracking_number=tracking_number,
         events=[
-            TrackingEvent(
-                date=DF.fdate(event.scan_time, "%Y-%m-%dT%H:%M:%SZ"),
+            models.TrackingEvent(
+                date=lib.fdatetime(
+                    getattr(event, "local_scan_time", None) or event.scan_time,
+                    try_formats=["%Y-%m-%dT%H:%M:%S", "%Y-%m-%dT%H:%M:%SZ"],
+                    output_format="%Y-%m-%d",
+                ),
                 description=event.description,
-                location=event.location,
+                location=(
+                    lib.text(
+                        event.origin_location,
+                        event.destination_location,
+                        separator=" to ",
+                    )
+                    if (event.origin_location and event.destination_location)
+                    else event.location
+                ),
                 code=event.event_type,
-                time=DF.ftime(event.scan_time, "%Y-%m-%dT%H:%M:%SZ"),
+                time=lib.fdatetime(
+                    getattr(event, "local_scan_time", None) or event.scan_time,
+                    try_formats=["%Y-%m-%dT%H:%M:%S", "%Y-%m-%dT%H:%M:%SZ"],
+                    output_format="%H:%M",
+                ),
             )
             for event in reversed(tracking_details.tracking_events)
         ],
-        estimated_delivery=DF.fdate(estimated_delivery, "%Y-%m-%d"),
+        estimated_delivery=lib.fdate(estimated_delivery, "%Y-%m-%d"),
         delivered=(tracking_details.state == "Delivered"),
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[list]:
+def tracking_request(payload: models.TrackingRequest, _) -> lib.Serializable:
     request = payload.tracking_numbers
 
-    return Serializable(request)
+    return lib.Serializable(request)
```

## Comparing `karrio.sendle-2023.1rc4.dist-info/METADATA` & `karrio.sendle-2023.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.sendle
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Sendle Shipping extension
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
 Requires-Dist: carrier.sendle
+Requires-Dist: karrio
 
 # karrio.sendle
 
 This package is a Sendle extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

