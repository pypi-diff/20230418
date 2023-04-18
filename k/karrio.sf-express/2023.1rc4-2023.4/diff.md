# Comparing `tmp/karrio.sf_express-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.sf_express-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 6998 bytes, number of entries: 13
--rw-r--r--  2.0 unx      569 b- defN 22-Jul-20 22:36 karrio/mappers/sf_express/__init__.py
--rw-r--r--  2.0 unx     4258 b- defN 22-Jul-20 22:36 karrio/mappers/sf_express/mapper.py
--rw-r--r--  2.0 unx      638 b- defN 22-Sep-30 13:07 karrio/mappers/sf_express/proxy.py
--rw-r--r--  2.0 unx      460 b- defN 22-Sep-30 13:07 karrio/mappers/sf_express/settings.py
--rw-r--r--  2.0 unx      787 b- defN 22-Jul-20 22:36 karrio/providers/sf_express/__init__.py
--rw-r--r--  2.0 unx      546 b- defN 22-Jul-20 22:36 karrio/providers/sf_express/error.py
--rw-r--r--  2.0 unx     1792 b- defN 22-Sep-16 02:38 karrio/providers/sf_express/tracking.py
--rw-r--r--  2.0 unx     1336 b- defN 22-Apr-29 10:15 karrio/providers/sf_express/units.py
--rw-r--r--  2.0 unx     1348 b- defN 22-Sep-30 13:07 karrio/providers/sf_express/utils.py
--rw-r--r--  2.0 unx      995 b- defN 23-Jan-21 08:15 karrio.sf_express-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.sf_express-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.sf_express-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1189 b- defN 23-Jan-21 08:15 karrio.sf_express-2023.1rc4.dist-info/RECORD
-13 files, 14017 bytes uncompressed, 4962 bytes compressed:  64.6%
+-rw-rw-r--  2.0 unx      569 b- defN 22-Nov-15 19:21 karrio/mappers/sf_express/__init__.py
+-rw-rw-r--  2.0 unx     4093 b- defN 23-Apr-01 12:45 karrio/mappers/sf_express/mapper.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Apr-01 12:45 karrio/mappers/sf_express/proxy.py
+-rw-rw-r--  2.0 unx      482 b- defN 23-Apr-15 06:44 karrio/mappers/sf_express/settings.py
+-rw-rw-r--  2.0 unx      787 b- defN 22-Nov-15 19:21 karrio/providers/sf_express/__init__.py
+-rw-rw-r--  2.0 unx      546 b- defN 22-Nov-15 19:21 karrio/providers/sf_express/error.py
+-rw-rw-r--  2.0 unx     1878 b- defN 23-Apr-01 15:18 karrio/providers/sf_express/tracking.py
+-rw-rw-r--  2.0 unx     1336 b- defN 22-Nov-15 19:21 karrio/providers/sf_express/units.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-15 03:00 karrio/providers/sf_express/utils.py
+-rw-rw-r--  2.0 unx     1012 b- defN 23-Apr-18 07:09 karrio.sf_express-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.sf_express-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.sf_express-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1178 b- defN 23-Apr-18 07:09 karrio.sf_express-2023.4.dist-info/RECORD
+13 files, 13961 bytes uncompressed, 4986 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/sf_express/units.py
 Comment: 
 
 Filename: karrio/providers/sf_express/utils.py
 Comment: 
 
-Filename: karrio.sf_express-2023.1rc4.dist-info/METADATA
+Filename: karrio.sf_express-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.sf_express-2023.1rc4.dist-info/WHEEL
+Filename: karrio.sf_express-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.sf_express-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.sf_express-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.sf_express-2023.1rc4.dist-info/RECORD
+Filename: karrio.sf_express-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/sf_express/mapper.py

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

## karrio/mappers/sf_express/proxy.py

```diff
@@ -4,15 +4,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         data = self.settings.parse(request.serialize(), "EXP_RECE_SEARCH_ROUTES")
         response = http(
             url=self.settings.server_url,
             data=data,
             trace=self.trace_as("json"),
             method="POST",
         )
```

## karrio/mappers/sf_express/settings.py

```diff
@@ -14,7 +14,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "sf_express"
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/sf_express/tracking.py

```diff
@@ -10,29 +10,31 @@
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.sf_express.utils import Settings
 from karrio.providers.sf_express.error import parse_error_response
+import karrio.lib as lib
 
 
 def parse_tracking_response(
-    response, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
     tracking_details = [
         _extract_detail(DP.to_object(RouteResp, d), settings)
         for d in response.get("msgData", {}).get("routeResps", [])
     ]
 
     return tracking_details, parse_error_response(response, settings)
 
 
 def _extract_detail(detail: RouteResp, settings: Settings) -> TrackingDetails:
-
     return TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         tracking_number=detail.mailNo,
         events=[
             TrackingEvent(
                 date=DF.fdate(event.acceptTime, "%Y-%m-%d %H:%M:%S"),
@@ -42,15 +44,15 @@
                 time=DF.ftime(event.acceptTime, "%Y-%m-%d %H:%M:%S"),
             )
             for event in detail.routes
         ],
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[Request]:
+def tracking_request(payload: TrackingRequest, _) -> Serializable:
     request = Request(
         requestID="EXP_RECE_SEARCH_ROUTES",
         msgData=SFTrackingRequest(
             language="1",
             trackingType="1",
             methodType="1",
             trackingNumber=payload.tracking_numbers,
```

## Comparing `karrio.sf_express-2023.1rc4.dist-info/METADATA` & `karrio.sf_express-2023.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.sf-express
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - SF-Express Shipping extension
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
 Requires-Dist: carrier.sf-express
+Requires-Dist: karrio
 
 # karrio.sf_express
 
 This package is a SF-Express extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

## Comparing `karrio.sf_express-2023.1rc4.dist-info/RECORD` & `karrio.sf_express-2023.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 karrio/mappers/sf_express/__init__.py,sha256=cHdiI6NgqR3AQMtUKLBdCFqBEJB5iEGRjrlb2EdgvRU,569
-karrio/mappers/sf_express/mapper.py,sha256=8iXZn_0ABT8HzPloE8wMJTzBOtZAIPd1UFt9zt9Pt4c,4258
-karrio/mappers/sf_express/proxy.py,sha256=ZtNJJeja1J-rE7C-xodpqzFbs8D7XJC815iToEHVJpk,638
-karrio/mappers/sf_express/settings.py,sha256=EfnsGSxSBIKw1gMfCzZYBit4aP33SYzPZT6g2mayz-M,460
+karrio/mappers/sf_express/mapper.py,sha256=D6ckFUCNIJzFl59zkqZpG5Jsh3c1gWvu61xJLTFl9wo,4093
+karrio/mappers/sf_express/proxy.py,sha256=02omvMgwvj8YT9sc_6XXn5s_25uSNnsbMmIk7JUDZfw,633
+karrio/mappers/sf_express/settings.py,sha256=bDxRi3MpemOaDk9tFQ7wAYiYhe9s1vZVK8bs_7IxGhA,482
 karrio/providers/sf_express/__init__.py,sha256=RkabgUI6MNuF6sGo72ddeu_u3qSEfiBTRqg2yVomOPA,787
 karrio/providers/sf_express/error.py,sha256=jxHYuw3og9te4MuhRxdf0uggrdv9P6n1CYYnwZ6Se_8,546
-karrio/providers/sf_express/tracking.py,sha256=IfCCZi8B9lJ0Hw3ldXBLKXEjNqA7mPK2DHm0S6Yog1Q,1792
+karrio/providers/sf_express/tracking.py,sha256=9AyxL5cymqzXu36TSQRQtotr_Kl98yfrtrS3n-x_d3k,1878
 karrio/providers/sf_express/units.py,sha256=sw5pMrksLEWRUNm4qqJdvtR6rL3IDR8AwJc45EFzr14,1336
 karrio/providers/sf_express/utils.py,sha256=1_alRcbLS-7qmFcrv9I7oQFNfboYSE6nE8LNsaMOMPE,1348
-karrio.sf_express-2023.1rc4.dist-info/METADATA,sha256=6FQUoq1HPSsZu7kfRxItAb6SJSSwTDW5kzZqJPpgzv8,995
-karrio.sf_express-2023.1rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-karrio.sf_express-2023.1rc4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.sf_express-2023.1rc4.dist-info/RECORD,,
+karrio.sf_express-2023.4.dist-info/METADATA,sha256=kUcSg2szAsp8RdoRjkfbu2CCOQQXwsUoZgqoerIUNO4,1012
+karrio.sf_express-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.sf_express-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.sf_express-2023.4.dist-info/RECORD,,
```

