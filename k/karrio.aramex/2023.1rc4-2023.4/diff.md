# Comparing `tmp/karrio.aramex-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.aramex-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7411 bytes, number of entries: 13
--rw-r--r--  2.0 unx      545 b- defN 22-Jul-20 22:36 karrio/mappers/aramex/__init__.py
--rw-r--r--  2.0 unx     4243 b- defN 22-Jul-20 22:36 karrio/mappers/aramex/mapper.py
--rw-r--r--  2.0 unx      801 b- defN 22-Sep-30 13:07 karrio/mappers/aramex/proxy.py
--rw-r--r--  2.0 unx      502 b- defN 22-Sep-30 13:07 karrio/mappers/aramex/settings.py
--rw-r--r--  2.0 unx      763 b- defN 22-Jul-20 22:36 karrio/providers/aramex/__init__.py
--rw-r--r--  2.0 unx      774 b- defN 22-Jul-20 22:36 karrio/providers/aramex/error.py
--rw-r--r--  2.0 unx     3189 b- defN 22-Sep-16 02:38 karrio/providers/aramex/tracking.py
--rw-r--r--  2.0 unx     1330 b- defN 22-Apr-29 10:15 karrio/providers/aramex/units.py
--rw-r--r--  2.0 unx     1419 b- defN 22-Sep-30 13:07 karrio/providers/aramex/utils.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jan-21 08:15 karrio.aramex-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.aramex-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.aramex-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1137 b- defN 23-Jan-21 08:15 karrio.aramex-2023.1rc4.dist-info/RECORD
-13 files, 15765 bytes uncompressed, 5479 bytes compressed:  65.2%
+Zip file size: 7007 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      545 b- defN 22-Nov-15 19:21 karrio/mappers/aramex/__init__.py
+-rw-rw-r--  2.0 unx      677 b- defN 23-Apr-01 12:45 karrio/mappers/aramex/mapper.py
+-rw-rw-r--  2.0 unx      796 b- defN 23-Apr-01 12:45 karrio/mappers/aramex/proxy.py
+-rw-rw-r--  2.0 unx      524 b- defN 23-Apr-15 06:44 karrio/mappers/aramex/settings.py
+-rw-rw-r--  2.0 unx      763 b- defN 22-Nov-15 19:21 karrio/providers/aramex/__init__.py
+-rw-rw-r--  2.0 unx      774 b- defN 22-Nov-15 19:21 karrio/providers/aramex/error.py
+-rw-rw-r--  2.0 unx     3186 b- defN 23-Apr-01 15:18 karrio/providers/aramex/tracking.py
+-rw-rw-r--  2.0 unx     1330 b- defN 22-Nov-15 19:21 karrio/providers/aramex/units.py
+-rw-rw-r--  2.0 unx     1419 b- defN 22-Nov-15 19:21 karrio/providers/aramex/utils.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Apr-18 07:09 karrio.aramex-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.aramex-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.aramex-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1124 b- defN 23-Apr-18 07:09 karrio.aramex-2023.4.dist-info/RECORD
+13 files, 12217 bytes uncompressed, 5099 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/aramex/units.py
 Comment: 
 
 Filename: karrio/providers/aramex/utils.py
 Comment: 
 
-Filename: karrio.aramex-2023.1rc4.dist-info/METADATA
+Filename: karrio.aramex-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.aramex-2023.1rc4.dist-info/WHEEL
+Filename: karrio.aramex-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.aramex-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.aramex-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.aramex-2023.1rc4.dist-info/RECORD
+Filename: karrio.aramex-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/aramex/mapper.py

```diff
@@ -1,121 +1,20 @@
-from typing import List, Tuple
-from karrio.core.utils.serializable import Serializable, Deserializable
-from karrio.api.mapper import Mapper as BaseMapper
-from karrio.core.models import (
-    # AddressValidationRequest,
-    # ShipmentCancelRequest,
-    # PickupUpdateRequest,
-    # PickupCancelRequest,
-    # ShipmentRequest,
-    TrackingRequest,
-    # PickupRequest,
-    # RateRequest,
+import typing
+import karrio.lib as lib
+import karrio.api.mapper as mapper
+import karrio.core.models as models
+import karrio.providers.aramex as provider
+import karrio.mappers.aramex.settings as settings
 
-    # AddressValidationDetails,
-    # ConfirmationDetails,
-    TrackingDetails,
-    # ShipmentDetails,
-    # PickupDetails,
-    # RateDetails,
-    Message,
-)
-from karrio.providers.aramex import (
-    # parse_address_validation_response,
-    # parse_shipment_cancel_response,
-    # parse_pickup_update_response,
-    # parse_pickup_cancel_response,
-    # parse_shipment_response,
-    parse_tracking_response,
-    # parse_pickup_response,
-    # parse_rate_response,
 
-    # address_validation_request,
-    # shipment_cancel_request,
-    # pickup_update_request,
-    # pickup_cancel_request,
-    tracking_request,
-    # shipment_request,
-    # pickup_request,
-    # rate_request,
-)
-from karrio.mappers.aramex.settings import Settings
-
-
-class Mapper(BaseMapper):
-    settings: Settings
-
-    # def create_address_validation_request(self, payload: AddressValidationRequest) -> Serializable:
-    #     return address_validation_request(payload, self.settings)
-    #
-    # def create_pickup_request(
-    #     self, payload: PickupRequest
-    # ) -> Serializable:
-    #     return pickup_request(payload, self.settings)
-    #
-    # def create_pickup_update_request(
-    #     self, payload: PickupUpdateRequest
-    # ) -> Serializable:
-    #     return pickup_update_request(payload, self.settings)
-    #
-    # def create_cancel_pickup_request(
-    #     self, payload: PickupCancelRequest
-    # ) -> Serializable:
-    #     return pickup_cancel_request(payload, self.settings)
-
-    # def create_rate_request(
-    #     self, payload: RateRequest
-    # ) -> Serializable:
-    #     return rate_request(payload, self.settings)
-
-    # def create_shipment_request(
-    #     self, payload: ShipmentRequest
-    # ) -> Serializable:
-    #     return shipment_request(payload, self.settings)
-    #
-    # def create_cancel_shipment_request(self, payload: ShipmentCancelRequest) -> Serializable:
-    #     return shipment_cancel_request(payload, self.settings)
+class Mapper(mapper.Mapper):
+    settings: settings.Settings
 
     def create_tracking_request(
-        self, payload: TrackingRequest
-    ) -> Serializable:
-        return tracking_request(payload, self.settings)
-
-    # def parse_address_validation_response(
-    #     self, response: Deserializable
-    # ) -> Tuple[AddressValidationDetails, List[Message]]:
-    #     return parse_address_validation_response(response.deserialize(), self.settings)
-    #
-    # def parse_cancel_pickup_response(
-    #     self, response: Deserializable[str]
-    # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_pickup_cancel_response(response.deserialize(), self.settings)
-    #
-    # def parse_pickup_response(
-    #     self, response: Deserializable[str]
-    # ) -> Tuple[PickupDetails, List[Message]]:
-    #     return parse_pickup_response(response.deserialize(), self.settings)
-    #
-    # def parse_pickup_update_response(
-    #     self, response: Deserializable[str]
-    # ) -> Tuple[PickupDetails, List[Message]]:
-    #     return parse_pickup_update_response(response.deserialize(), self.settings)
-
-    # def parse_rate_response(
-    #     self, response: Deserializable[str]
-    # ) -> Tuple[List[RateDetails], List[Message]]:
-    #     return parse_rate_response(response.deserialize(), self.settings)
-
-    # def parse_shipment_response(
-    #     self, response: Deserializable[str]
-    # ) -> Tuple[ShipmentDetails, List[Message]]:
-    #     return parse_shipment_response(response.deserialize(), self.settings)
-    #
-    # def parse_cancel_shipment_response(
-    #     self, response: Deserializable
-    # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_shipment_cancel_response(response.deserialize(), self.settings)
+        self, payload: models.TrackingRequest
+    ) -> lib.Serializable:
+        return provider.tracking_request(payload, self.settings)
 
     def parse_tracking_response(
-        self, response: Deserializable[str]
-    ) -> Tuple[List[TrackingDetails], List[Message]]:
-        return parse_tracking_response(response.deserialize(), self.settings)
+        self, response: lib.Deserializable
+    ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+        return provider.parse_tracking_response(response, self.settings)
```

## karrio/mappers/aramex/proxy.py

```diff
@@ -4,15 +4,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         response = http(
             url=f"{self.settings.server_url}/ShippingAPI.V2/Tracking/Service_1_0.svc",
             data=request.serialize(),
             trace=self.trace_as("xml"),
             method="POST",
             headers={
                 "Content-Type": "text/xml; charset=utf-8",
```

## karrio/mappers/aramex/settings.py

```diff
@@ -17,7 +17,8 @@
     account_country_code: str
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "aramex"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/aramex/tracking.py

```diff
@@ -1,42 +1,42 @@
 from typing import List, Tuple
 from functools import partial
 from aramex_lib.array_of_string import ArrayOfstring
 from aramex_lib.tracking import ShipmentTrackingRequest, ClientInfo, TrackingResult
 from karrio.core.utils import (
     create_envelope,
-    Envelope,
     Element,
     Serializable,
     XP,
     DF,
 )
 from karrio.core.models import (
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.aramex.utils import Settings
 from karrio.providers.aramex.error import parse_error_response
+import karrio.lib as lib
 
 
 def parse_tracking_response(
-    response, settings: Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: Settings,
 ) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
     non_existents = next(
         (
             XP.to_object(ArrayOfstring, n)
-            for n in response.xpath(
-                ".//*[local-name() = $name]", name="NonExistingWaybills"
-            )
+            for n in lib.find_element("NonExistingWaybills", response)
         ),
         ArrayOfstring(),
     )
-    results = response.xpath(".//*[local-name() = $name]", name="TrackingResult")
+    results = lib.find_element("TrackingResult", response)
     tracking_details = [_extract_detail(node, settings) for node in results]
     errors = _extract_errors(non_existents, settings) + parse_error_response(
         response, settings
     )
 
     return tracking_details, errors
 
@@ -67,17 +67,15 @@
                 code=detail.UpdateCode,
                 time=DF.ftime(detail.UpdateDateTime, "%Y-%m-%dT%H:%M:%S"),
             )
         ],
     )
 
 
-def tracking_request(
-    payload: TrackingRequest, settings: Settings
-) -> Serializable[Envelope]:
+def tracking_request(payload: TrackingRequest, settings: Settings) -> Serializable:
     request = create_envelope(
         body_content=ShipmentTrackingRequest(
             ClientInfo=ClientInfo(
                 UserName=settings.username,
                 Password=settings.password,
                 Version="1.0",
                 AccountNumber=settings.account_number,
```

## Comparing `karrio.aramex-2023.1rc4.dist-info/METADATA` & `karrio.aramex-2023.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.aramex
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Aramex Shipping extension
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
 Requires-Dist: carrier.aramex
+Requires-Dist: karrio
 
 # karrio.aramex
 
 This package is a Aramex extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

