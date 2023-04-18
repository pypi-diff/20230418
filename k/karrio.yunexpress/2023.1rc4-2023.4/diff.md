# Comparing `tmp/karrio.yunexpress-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.yunexpress-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6758 bytes, number of entries: 13
--rw-r--r--  2.0 unx      569 b- defN 22-Jul-20 22:36 karrio/mappers/yunexpress/__init__.py
--rw-r--r--  2.0 unx     4258 b- defN 22-Jul-20 22:36 karrio/mappers/yunexpress/mapper.py
--rw-r--r--  2.0 unx      795 b- defN 22-Sep-30 13:07 karrio/mappers/yunexpress/proxy.py
--rw-r--r--  2.0 unx      467 b- defN 22-Sep-30 13:07 karrio/mappers/yunexpress/settings.py
--rw-r--r--  2.0 unx      787 b- defN 22-Jul-20 22:36 karrio/providers/yunexpress/__init__.py
--rw-r--r--  2.0 unx      774 b- defN 22-Jul-20 22:36 karrio/providers/yunexpress/error.py
--rw-r--r--  2.0 unx     1284 b- defN 22-Jul-20 22:36 karrio/providers/yunexpress/tracking.py
--rw-r--r--  2.0 unx     1337 b- defN 22-Apr-29 10:15 karrio/providers/yunexpress/units.py
--rw-r--r--  2.0 unx      654 b- defN 22-Sep-30 13:07 karrio/providers/yunexpress/utils.py
--rw-r--r--  2.0 unx      996 b- defN 23-Jan-21 08:15 karrio.yunexpress-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.yunexpress-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.yunexpress-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1188 b- defN 23-Jan-21 08:15 karrio.yunexpress-2023.1rc4.dist-info/RECORD
-13 files, 13208 bytes uncompressed, 4722 bytes compressed:  64.2%
+Zip file size: 6774 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      569 b- defN 22-Nov-15 19:21 karrio/mappers/yunexpress/__init__.py
+-rw-rw-r--  2.0 unx     4093 b- defN 23-Apr-01 12:45 karrio/mappers/yunexpress/mapper.py
+-rw-rw-r--  2.0 unx      795 b- defN 22-Nov-15 19:21 karrio/mappers/yunexpress/proxy.py
+-rw-rw-r--  2.0 unx      489 b- defN 23-Apr-15 06:44 karrio/mappers/yunexpress/settings.py
+-rw-rw-r--  2.0 unx      787 b- defN 22-Nov-15 19:21 karrio/providers/yunexpress/__init__.py
+-rw-rw-r--  2.0 unx      774 b- defN 22-Nov-15 19:21 karrio/providers/yunexpress/error.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-01 15:18 karrio/providers/yunexpress/tracking.py
+-rw-rw-r--  2.0 unx     1337 b- defN 22-Nov-15 19:21 karrio/providers/yunexpress/units.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Apr-15 06:44 karrio/providers/yunexpress/utils.py
+-rw-rw-r--  2.0 unx     1013 b- defN 23-Apr-18 07:09 karrio.yunexpress-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.yunexpress-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.yunexpress-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1177 b- defN 23-Apr-18 07:09 karrio.yunexpress-2023.4.dist-info/RECORD
+13 files, 13165 bytes uncompressed, 4762 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/yunexpress/units.py
 Comment: 
 
 Filename: karrio/providers/yunexpress/utils.py
 Comment: 
 
-Filename: karrio.yunexpress-2023.1rc4.dist-info/METADATA
+Filename: karrio.yunexpress-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.yunexpress-2023.1rc4.dist-info/WHEEL
+Filename: karrio.yunexpress-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.yunexpress-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.yunexpress-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.yunexpress-2023.1rc4.dist-info/RECORD
+Filename: karrio.yunexpress-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/yunexpress/mapper.py

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

## karrio/mappers/yunexpress/settings.py

```diff
@@ -14,7 +14,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "yunexpress"
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/yunexpress/tracking.py

```diff
@@ -10,35 +10,38 @@
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.yunexpress.utils import Settings
 from karrio.providers.yunexpress.error import parse_error_response
+import karrio.lib as lib
 
 
-def parse_tracking_response(response: dict, settings: Settings) -> Tuple[List[TrackingDetails], List[Message]]:
-    details = [_extract_detail(d, settings) for d in response.get('Items', [])]
+def parse_tracking_response(
+    _response: lib.Deserializable[dict],
+    settings: Settings,
+) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
+    details = [_extract_detail(d, settings) for d in response.get("Items", [])]
 
     return details, parse_error_response(response, settings)
 
 
 def _extract_detail(detail: dict, settings: Settings) -> TrackingDetails:
     order_info = DP.to_object(OrderInfo, detail)
 
     return TrackingDetails(
         # context info
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
-
         tracking_number=order_info.TrackingNumber,
-        events=[TrackingEvent(
-            date=time.strftime('%Y-%m-%d'),
-            description=order_info.msg
-        )],
+        events=[
+            TrackingEvent(date=time.strftime("%Y-%m-%d"), description=order_info.msg)
+        ],
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[List[str]]:
-    request = SF.concat_str(*payload.tracking_numbers, join=True, separator=',')
+def tracking_request(payload: TrackingRequest, _) -> Serializable:
+    request = SF.concat_str(*payload.tracking_numbers, join=True, separator=",")
 
     return Serializable(request)
```

## karrio/providers/yunexpress/utils.py

```diff
@@ -8,14 +8,15 @@
     # Carrier specific properties
     customer_number: str
     api_secret: str
 
     id: str = None
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     @property
     def carrier_name(self):
         return "yunexpress"
 
     @property
     def server_url(self):
```

## Comparing `karrio.yunexpress-2023.1rc4.dist-info/METADATA` & `karrio.yunexpress-2023.4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.yunexpress
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Yunexpress Shipping extension
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
 Requires-Dist: carrier.yunexpress
+Requires-Dist: karrio
 
 # karrio.yunexpress
 
 This package is a Yunexpress extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

