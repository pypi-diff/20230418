# Comparing `tmp/karrio.royalmail-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.royalmail-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6842 bytes, number of entries: 13
--rw-r--r--  2.0 unx      564 b- defN 22-Jul-20 22:36 karrio/mappers/royalmail/__init__.py
--rw-r--r--  2.0 unx     4251 b- defN 22-Jul-20 22:36 karrio/mappers/royalmail/mapper.py
--rw-r--r--  2.0 unx     1122 b- defN 22-Sep-30 13:07 karrio/mappers/royalmail/proxy.py
--rw-r--r--  2.0 unx      460 b- defN 22-Sep-30 13:07 karrio/mappers/royalmail/settings.py
--rw-r--r--  2.0 unx      781 b- defN 22-Jul-20 22:36 karrio/providers/royalmail/__init__.py
--rw-r--r--  2.0 unx      728 b- defN 22-Jul-20 22:36 karrio/providers/royalmail/error.py
--rw-r--r--  2.0 unx     1712 b- defN 22-Apr-29 10:15 karrio/providers/royalmail/tracking.py
--rw-r--r--  2.0 unx     1336 b- defN 22-Apr-29 10:15 karrio/providers/royalmail/units.py
--rw-r--r--  2.0 unx      534 b- defN 22-Sep-30 13:07 karrio/providers/royalmail/utils.py
--rw-r--r--  2.0 unx      989 b- defN 23-Jan-21 08:15 karrio.royalmail-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.royalmail-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.royalmail-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1176 b- defN 23-Jan-21 08:15 karrio.royalmail-2023.1rc4.dist-info/RECORD
-13 files, 13752 bytes uncompressed, 4832 bytes compressed:  64.9%
+Zip file size: 6850 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      564 b- defN 22-Nov-15 19:21 karrio/mappers/royalmail/__init__.py
+-rw-rw-r--  2.0 unx     4091 b- defN 23-Apr-01 12:45 karrio/mappers/royalmail/mapper.py
+-rw-rw-r--  2.0 unx     1122 b- defN 22-Nov-15 19:21 karrio/mappers/royalmail/proxy.py
+-rw-rw-r--  2.0 unx      482 b- defN 23-Apr-15 06:44 karrio/mappers/royalmail/settings.py
+-rw-rw-r--  2.0 unx      781 b- defN 22-Nov-15 19:21 karrio/providers/royalmail/__init__.py
+-rw-rw-r--  2.0 unx      728 b- defN 22-Nov-15 19:21 karrio/providers/royalmail/error.py
+-rw-rw-r--  2.0 unx     1795 b- defN 23-Apr-01 15:18 karrio/providers/royalmail/tracking.py
+-rw-rw-r--  2.0 unx     1336 b- defN 22-Nov-15 19:21 karrio/providers/royalmail/units.py
+-rw-rw-r--  2.0 unx      534 b- defN 23-Apr-15 02:55 karrio/providers/royalmail/utils.py
+-rw-rw-r--  2.0 unx     1006 b- defN 23-Apr-18 07:10 karrio.royalmail-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.royalmail-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.royalmail-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Apr-18 07:10 karrio.royalmail-2023.4.dist-info/RECORD
+13 files, 13703 bytes uncompressed, 4864 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: karrio/providers/royalmail/units.py
 Comment: 
 
 Filename: karrio/providers/royalmail/utils.py
 Comment: 
 
-Filename: karrio.royalmail-2023.1rc4.dist-info/METADATA
+Filename: karrio.royalmail-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.royalmail-2023.1rc4.dist-info/WHEEL
+Filename: karrio.royalmail-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.royalmail-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.royalmail-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.royalmail-2023.1rc4.dist-info/RECORD
+Filename: karrio.royalmail-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/royalmail/mapper.py

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
@@ -71,53 +69,49 @@
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

## karrio/mappers/royalmail/settings.py

```diff
@@ -14,7 +14,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "royalmail"
     account_country_code: str = "UK"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/royalmail/tracking.py

```diff
@@ -9,31 +9,33 @@
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.royalmail.utils import Settings
 from karrio.providers.royalmail.error import parse_error_response
+import karrio.lib as lib
 
 
 def parse_tracking_response(
-    response: List[dict], settings: Settings
+    _response: lib.Deserializable[List[dict]],
+    settings: Settings,
 ) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
     errors = [e for e in response if "mailPieces" not in e]
     details = [
         _extract_detail(DP.to_object(MailPieces, d["mailPieces"]), settings)
         for d in response
         if "mailPieces" in d
     ]
 
     return details, parse_error_response(errors, settings)
 
 
 def _extract_detail(detail: MailPieces, settings: Settings) -> TrackingDetails:
-
     return TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         tracking_number=detail.mailPieceId,
         delivered=("Delivered" in detail.summary.get("lastEventName")),
         events=[
             TrackingEvent(
@@ -45,11 +47,11 @@
             )
             for event in detail.events
         ],
         estimated_delivery=DF.fdate(detail.estimatedDelivery.get("date"), "%Y-%m-%d"),
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[dict]:
+def tracking_request(payload: TrackingRequest, _) -> Serializable:
     request = payload.tracking_numbers
 
     return Serializable(request)
```

## Comparing `karrio.royalmail-2023.1rc4.dist-info/METADATA` & `karrio.royalmail-2023.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: karrio.royalmail
-Version: 2023.1rc4
+Version: 2023.4
 Summary: Karrio - Royal Mail Shipping extension
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
 Requires-Dist: carrier.royalmail
+Requires-Dist: karrio
 
 # karrio.royalmail
 
 This package is a Royal Mail extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
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

## Comparing `karrio.royalmail-2023.1rc4.dist-info/RECORD` & `karrio.royalmail-2023.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 karrio/mappers/royalmail/__init__.py,sha256=z7FWTv-MJKPaqQajhTUvvGPrGv5lBuuW6OVSB0jyHjY,564
-karrio/mappers/royalmail/mapper.py,sha256=qT1NhwfYQgncGV3MsXvmRLBuY97w9NfGHntiMtF3MhQ,4251
+karrio/mappers/royalmail/mapper.py,sha256=1X1n1LwODVVaXT6SjqLfL3wu_or4Cqu1Q6bMAbuMGQI,4091
 karrio/mappers/royalmail/proxy.py,sha256=UhWm1pnDIAB97YQyHOtMX9k4dOKC1GWu_sCVz8lvM0I,1122
-karrio/mappers/royalmail/settings.py,sha256=ZVvy9P2VSxRJklcCCDR8iRuCBB1vCbcCKR5cNW-UlLA,460
+karrio/mappers/royalmail/settings.py,sha256=KRtxvBa67-G124vhUfkDS7MNMtgxbbS_fxE6rGnhttg,482
 karrio/providers/royalmail/__init__.py,sha256=qffDByM43WA2dHiclXLtuLmU35EqHwEDuUvGyKSnlNM,781
 karrio/providers/royalmail/error.py,sha256=gyCmKZU9V2PDsH0PTmKXSRL-ve83Kt41fYKZMuHzacA,728
-karrio/providers/royalmail/tracking.py,sha256=YanmUFgbxGZN-CJOhEcOWudjAMeTQ1jU9Z___Bkpg5M,1712
+karrio/providers/royalmail/tracking.py,sha256=M1n_bCNZNXkq_QloA-uuum_YhhfQXfeY5Q9SFB20Qw4,1795
 karrio/providers/royalmail/units.py,sha256=GzCOD-DZSBKE8_McIE8pDNfz1AVE6dwdFqAM-72jZmY,1336
 karrio/providers/royalmail/utils.py,sha256=U_mmAnbzYYoULaOhyGOFdcSPEF9mikOIeI0Ewesc5CQ,534
-karrio.royalmail-2023.1rc4.dist-info/METADATA,sha256=GuZ8FeZiYWCoU6FgY_N-7Sp3QY_-HgOWJOpUKgLE3ow,989
-karrio.royalmail-2023.1rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-karrio.royalmail-2023.1rc4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.royalmail-2023.1rc4.dist-info/RECORD,,
+karrio.royalmail-2023.4.dist-info/METADATA,sha256=awvPLWl2TTtaur5ab94e0Q9ztJ7QgwcXFufBxY9o6wY,1006
+karrio.royalmail-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.royalmail-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.royalmail-2023.4.dist-info/RECORD,,
```

