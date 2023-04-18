# Comparing `tmp/karrio.dhl_poland-2023.3-py3-none-any.whl.zip` & `tmp/karrio.dhl_poland-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 11986 bytes, number of entries: 16
+Zip file size: 12013 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      583 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_poland/__init__.py
--rw-rw-r--  2.0 unx     2153 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_poland/mapper.py
--rw-rw-r--  2.0 unx     2073 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_poland/proxy.py
--rw-rw-r--  2.0 unx      849 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_poland/settings.py
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Apr-01 13:34 karrio/mappers/dhl_poland/mapper.py
+-rw-rw-r--  2.0 unx     2063 b- defN 23-Apr-01 12:45 karrio/mappers/dhl_poland/proxy.py
+-rw-rw-r--  2.0 unx      871 b- defN 23-Apr-15 06:44 karrio/mappers/dhl_poland/settings.py
 -rw-rw-r--  2.0 unx      328 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/__init__.py
 -rw-rw-r--  2.0 unx      621 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/error.py
--rw-rw-r--  2.0 unx     2866 b- defN 23-Mar-25 13:16 karrio/providers/dhl_poland/tracking.py
--rw-rw-r--  2.0 unx     4184 b- defN 23-Mar-21 13:06 karrio/providers/dhl_poland/units.py
--rw-rw-r--  2.0 unx     1851 b- defN 23-Mar-25 12:46 karrio/providers/dhl_poland/utils.py
+-rw-rw-r--  2.0 unx     2894 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/tracking.py
+-rw-rw-r--  2.0 unx     4184 b- defN 23-Mar-27 07:55 karrio/providers/dhl_poland/units.py
+-rw-rw-r--  2.0 unx     1851 b- defN 23-Apr-15 02:55 karrio/providers/dhl_poland/utils.py
 -rw-rw-r--  2.0 unx      236 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/shipment/__init__.py
--rw-rw-r--  2.0 unx     1490 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/shipment/cancel.py
--rw-rw-r--  2.0 unx    13448 b- defN 23-Mar-25 15:34 karrio/providers/dhl_poland/shipment/create.py
--rw-rw-r--  2.0 unx     1026 b- defN 23-Mar-27 07:12 karrio.dhl_poland-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.dhl_poland-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.dhl_poland-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1490 b- defN 23-Mar-27 07:12 karrio.dhl_poland-2023.3.dist-info/RECORD
-16 files, 33297 bytes uncompressed, 9466 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx     1565 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/shipment/cancel.py
+-rw-rw-r--  2.0 unx    13627 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/shipment/create.py
+-rw-rw-r--  2.0 unx     1026 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1490 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/RECORD
+16 files, 33471 bytes uncompressed, 9493 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dhl_poland/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dhl_poland/shipment/create.py
 Comment: 
 
-Filename: karrio.dhl_poland-2023.3.dist-info/METADATA
+Filename: karrio.dhl_poland-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dhl_poland-2023.3.dist-info/WHEEL
+Filename: karrio.dhl_poland-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dhl_poland-2023.3.dist-info/top_level.txt
+Filename: karrio.dhl_poland-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dhl_poland-2023.3.dist-info/RECORD
+Filename: karrio.dhl_poland-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dhl_poland/mapper.py

```diff
@@ -23,33 +23,29 @@
     def create_shipment_request(
         self, payload: models.ShipmentRequest
     ) -> lib.Serializable:
         return provider.shipment_request(payload, self.settings)
 
     def create_cancel_shipment_request(
         self, payload: models.ShipmentCancelRequest
-    ) -> lib.Serializable[str]:
+    ) -> lib.Serializable:
         return provider.shipment_cancel_request(payload, self.settings)
 
     def parse_cancel_shipment_response(
         self, response: lib.Deserializable
     ) -> typing.Tuple[models.ConfirmationDetails, typing.List[models.Message]]:
-        return provider.parse_shipment_cancel_response(
-            response.deserialize(), self.settings
-        )
+        return provider.parse_shipment_cancel_response(response, self.settings)
 
     def parse_rate_response(
-        self, response: lib.Deserializable[str]
+        self, response: lib.Deserializable
     ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
-        return universal_provider.parse_rate_response(
-            response.deserialize(), self.settings
-        )
+        return universal_provider.parse_rate_response(response, self.settings)
 
     def parse_shipment_response(
-        self, response: lib.Deserializable[str]
+        self, response: lib.Deserializable
     ) -> typing.Tuple[models.ShipmentDetails, typing.List[models.Message]]:
-        return provider.parse_shipment_response(response.deserialize(), self.settings)
+        return provider.parse_shipment_response(response, self.settings)
 
     def parse_tracking_response(
-        self, response: lib.Deserializable[str]
+        self, response: lib.Deserializable
     ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
-        return provider.parse_tracking_response(response.deserialize(), self.settings)
+        return provider.parse_tracking_response(response, self.settings)
```

## karrio/mappers/dhl_poland/proxy.py

```diff
@@ -38,22 +38,22 @@
         return lib.Deserializable(
             responses,
             lambda results: {
                 result["number"]: lib.to_element(result["data"]) for result in results
             },
         )
 
-    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = self._send_request(
             request,
             soapaction=f"{self.settings.server_url}#createShipment",
         )
 
         return lib.Deserializable(response, lib.to_element)
 
-    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = self._send_request(
             request,
             soapaction=f"{self.settings.server_url}#deleteShipment",
         )
 
         return lib.Deserializable(response, lib.to_element)
```

## karrio/mappers/dhl_poland/settings.py

```diff
@@ -18,9 +18,10 @@
     account_number: str = None
 
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dhl_poland"
     account_country_code: str = "PL"
     metadata: dict = {}
+    config: dict = {}
 
     services: List[ServiceLevel] = JList[ServiceLevel, False, dict(default=DEFAULT_SERVICES)]  # type: ignore
```

## karrio/providers/dhl_poland/tracking.py

```diff
@@ -3,17 +3,18 @@
 import karrio.lib as lib
 import karrio.core.models as models
 import karrio.providers.dhl_poland.error as provider_error
 import karrio.providers.dhl_poland.utils as provider_utils
 
 
 def parse_tracking_response(
-    response: typing.Dict[str, lib.Element],
+    _response: lib.Deserializable[typing.Dict[str, lib.Element]],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     details = [
         _extract_tracking_details(node, settings)
         for node in response.values()
         if lib.find_element("getTrackAndTraceInfoResult", node, first=True) is not None
     ]
     errors: typing.List[models.Message] = sum(
         [
@@ -61,15 +62,15 @@
         ),
     )
 
 
 def tracking_request(
     payload: models.TrackingRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[typing.Dict[str, lib.Envelope]]:
+) -> lib.Serializable:
     requests = {
         tracking_number: lib.create_envelope(
             body_prefix="",
             body_content=dhl.getTrackAndTraceInfo(
                 authData=settings.auth_data,
                 shipmentId=tracking_number,
             ),
```

## karrio/providers/dhl_poland/shipment/cancel.py

```diff
@@ -8,19 +8,21 @@
     create_envelope,
     Envelope,
     Element,
     Serializable,
 )
 from karrio.providers.dhl_poland.error import parse_error_response
 from karrio.providers.dhl_poland.utils import Settings
+import karrio.lib as lib
 
 
 def parse_shipment_cancel_response(
-    response: Element, settings: Settings
+    _response: lib.Deserializable[Element], settings: Settings
 ) -> Tuple[ConfirmationDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     success = len(errors) == 0
     confirmation: ConfirmationDetails = (
         ConfirmationDetails(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             success=success,
@@ -31,15 +33,15 @@
     )
 
     return confirmation, errors
 
 
 def shipment_cancel_request(
     payload: ShipmentCancelRequest, settings: Settings
-) -> Serializable[Envelope]:
+) -> Serializable:
     request = create_envelope(
         body_content=deleteShipment(
             authData=settings.auth_data,
             shipment=DeleteShipmentRequest(
                 shipmentIdentificationNumber=payload.shipment_identifier
             ),
         )
```

## karrio/providers/dhl_poland/shipment/create.py

```diff
@@ -6,16 +6,17 @@
 import karrio.core.models as models
 import karrio.providers.dhl_poland.error as provider_error
 import karrio.providers.dhl_poland.units as provider_units
 import karrio.providers.dhl_poland.utils as provider_utils
 
 
 def parse_shipment_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element], settings: provider_utils.Settings
 ) -> typing.Tuple[models.ShipmentDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = provider_error.parse_error_response(response, settings)
     shipment = (
         _extract_details(response, settings)
         if lib.find_element("createShipmentResult", response, first=True) is not None
         else None
     )
 
@@ -46,15 +47,15 @@
         ),
     )
 
 
 def shipment_request(
     payload: models.ShipmentRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[str]:
+) -> lib.Serializable:
     packages = lib.to_packages(
         payload.parcels,
         required=["weight"],
         package_option_type=provider_units.ShippingOption,
     )
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
@@ -154,15 +155,17 @@
                             )
                             else None
                         ),
                         address=dhl.Address(
                             name=(shipper.company_name or shipper.person_name),
                             postalCode=(shipper.postal_code or "").replace("-", ""),
                             city=shipper.city,
-                            street=lib.text(shipper.address_line1, shipper.address_line2),
+                            street=lib.text(
+                                shipper.address_line1, shipper.address_line2
+                            ),
                             houseNumber=(shipper.street_number or "N/A"),
                             apartmentNumber=shipper.suite,
                         ),
                     ),
                     receiver=dhl.ReceiverAddressat(
                         preaviso=(
                             dhl.PreavisoContact(
@@ -199,15 +202,17 @@
                             isPackstation=None,
                             isPostfiliale=None,
                             postnummer=None,
                             addressType=("C" if recipient.residential else "B"),
                             name=(recipient.company_name or recipient.person_name),
                             postalCode=(recipient.postal_code or "").replace("-", ""),
                             city=recipient.city,
-                            street=lib.text(recipient.address_line1, recipient.address_line2),
+                            street=lib.text(
+                                recipient.address_line1, recipient.address_line2
+                            ),
                             houseNumber=(shipper.street_number or "N/A"),
                             apartmentNumber=shipper.suite,
                         ),
                     ),
                     neighbour=None,
                 ),
                 pieceList=dhl.ArrayOfPackage(
```

## Comparing `karrio.dhl_poland-2023.3.dist-info/METADATA` & `karrio.dhl_poland-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dhl-poland
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - DHL Parcel Poland Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dhl_poland-2023.3.dist-info/RECORD` & `karrio.dhl_poland-2023.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 karrio/mappers/dhl_poland/__init__.py,sha256=qGpqTKvzk25rchSJ2Oxe2Uz2wD2L2W0O6bvyv0rPvus,583
-karrio/mappers/dhl_poland/mapper.py,sha256=5C3MRfCiK6iRAA479fboattLs_-_5jJHEqfVgyYWToE,2153
-karrio/mappers/dhl_poland/proxy.py,sha256=G2VeK3GS1C0fQk-beuKXE0t8f5LCMtsQJsiSfoRyqFg,2073
-karrio/mappers/dhl_poland/settings.py,sha256=hCgoQNDvUW-IsIx7ul80d6j8C1JT1LxdRkQn8255-EA,849
+karrio/mappers/dhl_poland/mapper.py,sha256=pRG8aiSv9APty1ZAszfad9BqEmZVCpdmzG1kiyMTKJ8,2033
+karrio/mappers/dhl_poland/proxy.py,sha256=Wy_bhxCnshTI9HeGEmk0dCn1MjOkJmFnxbtuJ5xPYd0,2063
+karrio/mappers/dhl_poland/settings.py,sha256=A_jCHUEt0jh1nRz45_s0J0tqhBic41Wr0752gs_kvFo,871
 karrio/providers/dhl_poland/__init__.py,sha256=oLgXPC778tlkc-zFag7y40sBkgvf5IsTtt10FZ_e9Xk,328
 karrio/providers/dhl_poland/error.py,sha256=OXxiuVdmtW55THG8Uv0UTDC-wXoj_CENVRLK6niV6vs,621
-karrio/providers/dhl_poland/tracking.py,sha256=L0HvBqVGMV0iUD7xHzcoJjzDQaoCcD3B2adF8njCFUk,2866
+karrio/providers/dhl_poland/tracking.py,sha256=s90aAKkmrk1EbC1n_BKHMrc-H-y5-uznsMTE4hgElKU,2894
 karrio/providers/dhl_poland/units.py,sha256=KAQi3dkmsn4U5ghOCyg6uF2BmCSZUfVyTrA7XpXnWQY,4184
 karrio/providers/dhl_poland/utils.py,sha256=ETUe5XsIYzsQCX6seeZ-exzXWyWf87-qGY474x10lmQ,1851
 karrio/providers/dhl_poland/shipment/__init__.py,sha256=kH1OP9BIPNfzxj6k41NI5TGBQX6CZ9y0qinn3BkL9xI,236
-karrio/providers/dhl_poland/shipment/cancel.py,sha256=55N4Nzi9vLdcRjZ5_hXEB9dI3LnBy5yhBkeSxdpwHlw,1490
-karrio/providers/dhl_poland/shipment/create.py,sha256=8Y39gRQOsnL2R361ClKZqXCw6SPe9TRH0pv_IUWvKZE,13448
-karrio.dhl_poland-2023.3.dist-info/METADATA,sha256=oK_eWSrdcWqm2qK8t2ePHq9ulwvt9GgdZ0o_7Cx-dm4,1026
-karrio.dhl_poland-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dhl_poland-2023.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dhl_poland-2023.3.dist-info/RECORD,,
+karrio/providers/dhl_poland/shipment/cancel.py,sha256=kUhh8IVU4j3QPTOy9SLnBsYtfKJesN1Wfo8xuqEKvHk,1565
+karrio/providers/dhl_poland/shipment/create.py,sha256=wCYrVq93jezD5YkbeJLJtY2ccPhwMdvebofGD09mfwc,13627
+karrio.dhl_poland-2023.4.dist-info/METADATA,sha256=dUe30wn3QMD9sckPa3mMgOZiaP9UlK3O3qZpbFzUplk,1026
+karrio.dhl_poland-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dhl_poland-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dhl_poland-2023.4.dist-info/RECORD,,
```

