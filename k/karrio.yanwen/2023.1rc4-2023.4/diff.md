# Comparing `tmp/karrio.yanwen-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.yanwen-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6155 bytes, number of entries: 12
--rw-r--r--  2.0 unx      545 b- defN 22-Jul-20 22:36 karrio/mappers/yanwen/__init__.py
--rw-r--r--  2.0 unx     4250 b- defN 22-Jul-20 22:36 karrio/mappers/yanwen/mapper.py
--rw-r--r--  2.0 unx      837 b- defN 22-Sep-30 13:07 karrio/mappers/yanwen/proxy.py
--rw-r--r--  2.0 unx      450 b- defN 22-Sep-30 13:07 karrio/mappers/yanwen/settings.py
--rw-r--r--  2.0 unx      763 b- defN 22-Jul-20 22:36 karrio/providers/yanwen/__init__.py
--rw-r--r--  2.0 unx     1940 b- defN 22-Jul-20 22:36 karrio/providers/yanwen/tracking.py
--rw-r--r--  2.0 unx     1332 b- defN 22-Apr-29 10:15 karrio/providers/yanwen/units.py
--rw-r--r--  2.0 unx      407 b- defN 22-Sep-30 13:07 karrio/providers/yanwen/utils.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jan-21 08:15 karrio.yanwen-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.yanwen-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.yanwen-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1048 b- defN 23-Jan-21 08:15 karrio.yanwen-2023.1rc4.dist-info/RECORD
-12 files, 12634 bytes uncompressed, 4363 bytes compressed:  65.5%
+Zip file size: 6173 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx      545 b- defN 22-Nov-15 19:21 karrio/mappers/yanwen/__init__.py
+-rw-rw-r--  2.0 unx     4085 b- defN 23-Apr-01 12:45 karrio/mappers/yanwen/mapper.py
+-rw-rw-r--  2.0 unx      832 b- defN 23-Apr-01 12:45 karrio/mappers/yanwen/proxy.py
+-rw-rw-r--  2.0 unx      472 b- defN 23-Apr-15 06:44 karrio/mappers/yanwen/settings.py
+-rw-rw-r--  2.0 unx      763 b- defN 22-Nov-15 19:21 karrio/providers/yanwen/__init__.py
+-rw-rw-r--  2.0 unx     2068 b- defN 23-Apr-01 15:18 karrio/providers/yanwen/tracking.py
+-rw-rw-r--  2.0 unx     1332 b- defN 22-Nov-15 19:21 karrio/providers/yanwen/units.py
+-rw-rw-r--  2.0 unx      429 b- defN 23-Apr-15 06:44 karrio/providers/yanwen/utils.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Apr-18 07:10 karrio.yanwen-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.yanwen-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.yanwen-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Apr-18 07:10 karrio.yanwen-2023.4.dist-info/RECORD
+12 files, 12641 bytes uncompressed, 4405 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: karrio/providers/yanwen/units.py
 Comment: 
 
 Filename: karrio/providers/yanwen/utils.py
 Comment: 
 
-Filename: karrio.yanwen-2023.1rc4.dist-info/METADATA
+Filename: karrio.yanwen-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.yanwen-2023.1rc4.dist-info/WHEEL
+Filename: karrio.yanwen-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.yanwen-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.yanwen-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.yanwen-2023.1rc4.dist-info/RECORD
+Filename: karrio.yanwen-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/yanwen/mapper.py

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

## karrio/mappers/yanwen/proxy.py

```diff
@@ -5,15 +5,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         query = urllib.parse.urlencode(request.serialize())
         response = http(
             url=f"http://trackapi.yanwentech.com/api/tracking?{query}",
             trace=self.trace_as("json"),
             method="GET",
             headers={
                 "Content-Type": "application/json",
```

## karrio/mappers/yanwen/settings.py

```diff
@@ -14,7 +14,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "yanwen"
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/yanwen/tracking.py

```diff
@@ -1,64 +1,71 @@
 from typing import List, Tuple
-from yanwen_lib.tracking import (
-    Result
-)
+from yanwen_lib.tracking import Result
 from karrio.core.utils import (
     Serializable,
     DF,
     DP,
 )
 from karrio.core.models import (
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.yanwen.utils import Settings
+import karrio.lib as lib
 
 
-def parse_tracking_response(response: dict, settings: Settings) -> Tuple[List[TrackingDetails], List[Message]]:
-    results = response.get('result', [])
-    details = [_extract_detail(d, settings) for d in results if d['tracking_status'] != 'NOTFOUND']
-    messages = [_extract_error(e, settings) for e in results if e['tracking_status'] == 'NOTFOUND']
+def parse_tracking_response(
+    _response: lib.Deserializable[dict],
+    settings: Settings,
+) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
+    results = response.get("result", [])
+    details = [
+        _extract_detail(d, settings)
+        for d in results
+        if d["tracking_status"] != "NOTFOUND"
+    ]
+    messages = [
+        _extract_error(e, settings)
+        for e in results
+        if e["tracking_status"] == "NOTFOUND"
+    ]
 
     return details, messages
 
 
 def _extract_detail(detail: dict, settings: Settings) -> TrackingDetails:
     result = DP.to_object(Result, detail)
     return TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
-
         tracking_number=result.tracking_number,
         events=[
             TrackingEvent(
-                date=DF.fdate(event.time_stamp, '2019-08-15T18:52:19'),
+                date=DF.fdate(event.time_stamp, "2019-08-15T18:52:19"),
                 description=event.message,
                 location=event.location,
                 code=event.tracking_status,
-                time=DF.ftime(event.time_stamp, '2019-08-15T18:52:19'),
+                time=DF.ftime(event.time_stamp, "2019-08-15T18:52:19"),
             )
             for event in result.checkpoints
         ],
-        delivered=(result.tracking_status == 'LM40')
+        delivered=(result.tracking_status == "LM40"),
     )
 
 
 def _extract_error(detail: dict, settings: Settings) -> Message:
     result = DP.to_object(Result, detail)
     return Message(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
-
         code=result.tracking_status,
-        message=f"No tracking details found for {result.tracking_number}"
+        message=f"No tracking details found for {result.tracking_number}",
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[dict]:
-    request = dict(
-        nums=",".join(payload.tracking_numbers)
-    )
+def tracking_request(payload: TrackingRequest, _) -> Serializable:
+    request = dict(nums=",".join(payload.tracking_numbers))
 
     return Serializable(request, DP.to_dict)
```

## karrio/providers/yanwen/utils.py

```diff
@@ -7,14 +7,15 @@
     # Carrier specific properties
     customer_number: str
     license_key: str
 
     id: str = None
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     @property
     def carrier_name(self):
         return "yanwen"
 
     @property
     def server_url(self):
```

## Comparing `karrio.yanwen-2023.1rc4.dist-info/METADATA` & `karrio.yanwen-2023.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.yanwen
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Yanwen Shipping extension
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
 Requires-Dist: carrier.yanwen
+Requires-Dist: karrio
 
 # karrio.yanwen
 
 This package is a Yanwen extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

## Comparing `karrio.yanwen-2023.1rc4.dist-info/RECORD` & `karrio.yanwen-2023.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 karrio/mappers/yanwen/__init__.py,sha256=E9XohMWP7kTQjbL-KfbuChC-T6n9c_f5E9PKX4_BTkI,545
-karrio/mappers/yanwen/mapper.py,sha256=jLzqjKewTZGO_c6SocjCpPI3EZyKd7ZPZV-taa-Pv-4,4250
-karrio/mappers/yanwen/proxy.py,sha256=Qeo4Qmr6n8dh83AHjLH8etMTwQgbfyqGOwMbL6enq0Y,837
-karrio/mappers/yanwen/settings.py,sha256=Yh8OBz_GGDn_aWUc92dmK-qhatKaGXRofhlKp8QGLOE,450
+karrio/mappers/yanwen/mapper.py,sha256=lW7ZHAblSzZwjcihsjiKjOKrfbVPueUkTEdih_Mkoao,4085
+karrio/mappers/yanwen/proxy.py,sha256=CL1BZW7HuHEP5XywS-0c7qrQEUnKeYA3O7HyCHIiAH0,832
+karrio/mappers/yanwen/settings.py,sha256=Apvv_nN0P4EITHI8oB-sDQAOFhq08YQjhCQ27RiE7sw,472
 karrio/providers/yanwen/__init__.py,sha256=dFmeS3qxGanTcbbWutZ00A4z5lnggwZnV_PUIeER-zY,763
-karrio/providers/yanwen/tracking.py,sha256=LZN90O9AQmdHJsJU1lDrte45dnbZPqRKaqoo5x6e3zY,1940
+karrio/providers/yanwen/tracking.py,sha256=6Wj9lOn2yJnEGMMODk3uosSEZ0o_iDjOouqd7MnyXkQ,2068
 karrio/providers/yanwen/units.py,sha256=_7La-8t9z406UuvM4S7JqtWdQz1fFfzJMPjf-WqNRKk,1332
-karrio/providers/yanwen/utils.py,sha256=HRaPehK9OgRadTlP-7ccQ-EksLLFVQSTAIXU8OhI8RU,407
-karrio.yanwen-2023.1rc4.dist-info/METADATA,sha256=8ZUEk_7b70syIuCBgleQitmUsefJRTo8wIbULulEJYE,963
-karrio.yanwen-2023.1rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-karrio.yanwen-2023.1rc4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.yanwen-2023.1rc4.dist-info/RECORD,,
+karrio/providers/yanwen/utils.py,sha256=SppoRVtENwHles_AFr7Ukt276O9qCW609jM3zetSs-k,429
+karrio.yanwen-2023.4.dist-info/METADATA,sha256=xeFfMrsruTF8_5R7wh2ZmxG0Dv1LOU2U_ozuLfneiBw,980
+karrio.yanwen-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.yanwen-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.yanwen-2023.4.dist-info/RECORD,,
```

