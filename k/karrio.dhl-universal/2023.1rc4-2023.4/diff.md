# Comparing `tmp/karrio.dhl_universal-2023.1rc4-py3-none-any.whl.zip` & `tmp/karrio.dhl_universal-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 7036 bytes, number of entries: 13
--rw-r--r--  2.0 unx      365 b- defN 22-Jul-20 22:36 karrio/mappers/dhl_universal/__init__.py
--rw-r--r--  2.0 unx     4257 b- defN 22-Jul-20 22:36 karrio/mappers/dhl_universal/mapper.py
--rw-r--r--  2.0 unx     1041 b- defN 22-Sep-30 13:07 karrio/mappers/dhl_universal/proxy.py
--rw-r--r--  2.0 unx      479 b- defN 22-Sep-30 13:07 karrio/mappers/dhl_universal/settings.py
--rw-r--r--  2.0 unx      805 b- defN 22-Jul-20 22:36 karrio/providers/dhl_universal/__init__.py
--rw-r--r--  2.0 unx      703 b- defN 22-Jul-20 22:36 karrio/providers/dhl_universal/error.py
--rw-r--r--  2.0 unx     2423 b- defN 22-May-26 22:07 karrio/providers/dhl_universal/tracking.py
--rw-r--r--  2.0 unx     1339 b- defN 22-Apr-29 10:15 karrio/providers/dhl_universal/units.py
--rw-r--r--  2.0 unx      444 b- defN 22-Sep-30 13:07 karrio/providers/dhl_universal/utils.py
--rw-r--r--  2.0 unx     1026 b- defN 23-Jan-21 08:15 karrio.dhl_universal-2023.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-21 08:15 karrio.dhl_universal-2023.1rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-21 08:15 karrio.dhl_universal-2023.1rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1229 b- defN 23-Jan-21 08:15 karrio.dhl_universal-2023.1rc4.dist-info/RECORD
-13 files, 14210 bytes uncompressed, 4922 bytes compressed:  65.4%
+Zip file size: 8396 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-04 15:04 dhl_universal_lib/__init__.py
+-rw-rw-r--  2.0 unx     4243 b- defN 23-Apr-04 15:04 dhl_universal_lib/tracking.py
+-rw-rw-r--  2.0 unx      365 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_universal/__init__.py
+-rw-rw-r--  2.0 unx     4099 b- defN 23-Apr-01 12:45 karrio/mappers/dhl_universal/mapper.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Apr-01 12:45 karrio/mappers/dhl_universal/proxy.py
+-rw-rw-r--  2.0 unx      526 b- defN 23-Apr-15 06:44 karrio/mappers/dhl_universal/settings.py
+-rw-rw-r--  2.0 unx      805 b- defN 22-Nov-15 19:21 karrio/providers/dhl_universal/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 22-Nov-15 19:21 karrio/providers/dhl_universal/error.py
+-rw-rw-r--  2.0 unx     4587 b- defN 23-Apr-04 15:07 karrio/providers/dhl_universal/tracking.py
+-rw-rw-r--  2.0 unx      222 b- defN 23-Apr-04 15:02 karrio/providers/dhl_universal/units.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Apr-15 02:55 karrio/providers/dhl_universal/utils.py
+-rw-rw-r--  2.0 unx     1006 b- defN 23-Apr-18 07:10 karrio.dhl_universal-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.dhl_universal-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       33 b- defN 23-Apr-18 07:10 karrio.dhl_universal-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1386 b- defN 23-Apr-18 07:10 karrio.dhl_universal-2023.4.dist-info/RECORD
+15 files, 19897 bytes uncompressed, 6038 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: dhl_universal_lib/__init__.py
+Comment: 
+
+Filename: dhl_universal_lib/tracking.py
+Comment: 
+
 Filename: karrio/mappers/dhl_universal/__init__.py
 Comment: 
 
 Filename: karrio/mappers/dhl_universal/mapper.py
 Comment: 
 
 Filename: karrio/mappers/dhl_universal/proxy.py
@@ -21,20 +27,20 @@
 
 Filename: karrio/providers/dhl_universal/units.py
 Comment: 
 
 Filename: karrio/providers/dhl_universal/utils.py
 Comment: 
 
-Filename: karrio.dhl_universal-2023.1rc4.dist-info/METADATA
+Filename: karrio.dhl_universal-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dhl_universal-2023.1rc4.dist-info/WHEEL
+Filename: karrio.dhl_universal-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dhl_universal-2023.1rc4.dist-info/top_level.txt
+Filename: karrio.dhl_universal-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dhl_universal-2023.1rc4.dist-info/RECORD
+Filename: karrio.dhl_universal-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dhl_universal/mapper.py

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

## karrio/mappers/dhl_universal/proxy.py

```diff
@@ -12,15 +12,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         def _get_tracking(tracking_request: dict):
             query = urllib.parse.urlencode(tracking_request)
             return http(
                 url=f"{self.settings.server_url}/track/shipments?{query}",
                 trace=self.trace_as("json"),
                 method="GET",
                 headers={
```

## karrio/mappers/dhl_universal/settings.py

```diff
@@ -7,14 +7,16 @@
 @attr.s(auto_attribs=True)
 class Settings(BaseSettings):
     """DHL Universal connection settings."""
 
     # Carrier specific properties
     consumer_key: str
     consumer_secret: str
+    language: str = "en"
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dhl_universal"
-    account_country_code: str = None
+    account_country_code: str = "DE"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/dhl_universal/tracking.py

```diff
@@ -1,77 +1,128 @@
-from typing import List, Tuple
-from dhl_universal_lib.tracking import TrackingRequest as DHLTrackingRequest, Shipment
-from karrio.core.utils import (
-    Serializable,
-    DP,
-    DF,
-)
-from karrio.core.models import (
-    TrackingEvent,
-    TrackingDetails,
-    TrackingRequest,
-    Message,
-)
-from karrio.providers.dhl_universal.utils import Settings
-from karrio.providers.dhl_universal.error import parse_error_response
+import dhl_universal_lib.tracking as dhl
+import typing
+import karrio.lib as lib
+import karrio.core.models as models
+import karrio.providers.dhl_universal.error as error
+import karrio.providers.dhl_universal.utils as provider_utils
+import karrio.providers.dhl_universal.units as provider_units
 
 date_formats = [
     "%Y-%m-%d",
     "%Y-%m-%dT%H:%M:%S",
     "%Y-%m-%dT%H:%M:%SZ",
     "%Y-%m-%dT%H:%M:%S%z",
     "%Y-%m-%dT%H:%M:%S.%f%z",
 ]
 
 
 def parse_tracking_response(
-    response: List[dict], settings: Settings
-) -> Tuple[List[TrackingDetails], List[Message]]:
+    _response: lib.Deserializable[typing.List[dict]],
+    settings: provider_utils.Settings,
+) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = [e for e in response if "shipments" not in e]
     details = [
-        _extract_detail(DP.to_object(Shipment, d["shipments"][0]), settings)
+        _extract_detail(lib.to_object(dhl.Shipment, d["shipments"][0]), settings)
         for d in response
         if "shipments" in d
     ]
 
-    return details, parse_error_response(errors, settings)
+    return details, error.parse_error_response(errors, settings)
 
 
-def _extract_detail(detail: Shipment, settings: Settings) -> TrackingDetails:
-    delivered = (getattr(detail.status, "statusCode", None) or "") == "delivered" or (
-        getattr(detail.status, "status", None) or ""
-    ).lower() == "delivered"
-    return TrackingDetails(
+def _extract_detail(
+    shipment: dhl.Shipment,
+    settings: provider_utils.Settings,
+) -> models.TrackingDetails:
+    latest_status = lib.failsafe(
+        lambda: (
+            shipment.status.statusCode
+            or shipment.status.status
+            or shipment.events[0].statusCode
+        )
+    ).lower()
+    status = next(
+        (
+            status.name
+            for status in list(provider_units.TrackingStatus)
+            if latest_status in status.value
+        ),
+        provider_units.TrackingStatus.in_transit.name,
+    )
+
+    return models.TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
-        tracking_number=str(detail.id),
+        tracking_number=str(shipment.id),
+        status=status,
         events=[
-            TrackingEvent(
-                date=DF.fdate(event.timestamp, try_formats=date_formats),
+            models.TrackingEvent(
+                date=lib.fdate(event.timestamp, try_formats=date_formats),
                 description=event.description or event.status or " ",
                 location=(
                     event.location.address.addressLocality
                     if event.location is not None and event.location.address is not None
                     else None
                 ),
                 code=event.statusCode or "",
-                time=DF.ftime(event.timestamp, try_formats=date_formats),
+                time=lib.ftime(event.timestamp, try_formats=date_formats),
             )
-            for event in detail.events or []
+            for event in shipment.events or []
         ],
-        estimated_delivery=DF.fdate(
-            detail.estimatedTimeOfDelivery, try_formats=date_formats
+        estimated_delivery=lib.fdate(
+            shipment.estimatedTimeOfDelivery, try_formats=date_formats
+        ),
+        delivered=status == "delivered",
+        info=models.TrackingInfo(
+            carrier_tracking_link=settings.tracking_url.format(shipment.id),
+            shipment_service=lib.failsafe(lambda: shipment.details.product.productName),
+            customer_name=lib.failsafe(
+                lambda: (
+                    lib.text(
+                        shipment.details.receiver.givenName,
+                        shipment.details.receiver.familyName,
+                    )
+                    or lib.text(shipment.details.receiver.name)
+                    or lib.text(shipment.details.receiver.organizationName)
+                )
+            ),
+            shipment_destination_country=lib.failsafe(
+                lambda: shipment.destination.address.countryCode
+            ),
+            shipment_destination_postal_code=lib.failsafe(
+                lambda: shipment.destination.address.postalCode
+            ),
+            shipment_origin_country=lib.failsafe(
+                lambda: shipment.origin.address.countryCode
+            ),
+            shipment_origin_postal_code=lib.failsafe(
+                lambda: shipment.origin.address.postalCode
+            ),
+            package_weight=lib.failsafe(lambda: shipment.details.weight.value),
+            package_weight_unit=lib.failsafe(lambda: shipment.details.weight.unitText),
+            signed_by=lib.failsafe(
+                lambda: (
+                    lib.text(
+                        shipment.details.proofOfDelivery.signed.givenName,
+                        shipment.details.proofOfDelivery.signed.familyName,
+                    )
+                    or lib.text(shipment.details.proofOfDelivery.signed.name)
+                )
+            ),
+        ),
+        meta=dict(
+            reference=lib.failsafe(lambda: shipment.details.references.number),
         ),
-        delivered=delivered,
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[DHLTrackingRequest]:
+def tracking_request(payload: models.TrackingRequest, _) -> lib.Serializable:
     request = [
-        DHLTrackingRequest(
+        dhl.TrackingRequest(
             trackingNumber=number,
             language="en",
         )
         for number in payload.tracking_numbers
     ]
 
-    return Serializable(request, DP.to_dict)
+    return lib.Serializable(request, lib.to_dict)
```

## karrio/providers/dhl_universal/units.py

```diff
@@ -1,45 +1,9 @@
 """ DHL Universal Native Types """
+import karrio.lib as lib
 
-# from karrio.core.utils import Enum, Flag
-#
-# PRESET_DEFAULTS = dict(dimension_unit="CM", weight_unit="KG")
-#
-#
-# class PackagePresets(Flag):
-#     # carrier_envelope = PackagePreset(
-#     #     **dict(weight=0.5, width=35.0, height=27.5, length=1.0, packaging_type="envelope"),
-#     #     **PRESET_DEFAULTS
-#     # )
-#     # carrier_box = PackagePreset(
-#     #     **dict(weight=0.5, width=35.0, height=27.5, length=1.0, packaging_type="medium_box"),
-#     #     **PRESET_DEFAULTS
-#     # )
-#     pass
-#
-#
-# class PackageType(Flag):
-#     carrier_envelope = "ENVELOPE CODE"
-#     carrier_box = "BOX CODE"
-#     carrier_your_packaging = "CUSTOM PACKAGING CODE"
-#
-#     """ Unified Packaging type mapping """
-#     envelope = carrier_envelope
-#     pak = carrier_envelope
-#     tube = carrier_your_packaging
-#     pallet = carrier_your_packaging
-#     small_box = carrier_box
-#     medium_box = carrier_box
-#     large_box = carrier_box
-#     your_packaging = carrier_your_packaging
-#
-#
-# class Service(Enum):
-#     carrier_standard = "STANDARD CODE"
-#     carrier_premium = "PREMIUM CODE"
-#     carrier_overnight = "OVERNIGHT CODE"
-#
-#
-# class Option(Flag):
-#     carrier_signature = "SIGNATURE CODE"
-#     carrier_saturday_delivery = "SATURDAY DELIVERY CODE"
-#     carrier_dry_ice = "DRY ICE CODE"
+
+class TrackingStatus(lib.Enum):
+    delivered = ["delivered"]
+    in_transit = ["transit"]
+    delivery_failed = ["failure"]
+    delivery_delayed = ["unknown"]
```

## karrio/providers/dhl_universal/utils.py

```diff
@@ -3,19 +3,30 @@
 
 class Settings(BaseSettings):
     """DHL Universal connection settings."""
 
     # Carrier specific properties
     consumer_key: str
     consumer_secret: str
+    language: str = "en"
 
-    id: str = None
-    account_country_code: str = None
+    account_country_code: str = "DE"
     metadata: dict = {}
 
     @property
     def carrier_name(self):
         return "dhl_universal"
 
     @property
     def server_url(self):
         return "https://api-eu.dhl.com"
+
+    @property
+    def tracking_url(self):
+        country = self.account_country_code or "DE"
+        language = self.language or "en"
+        locale = f"{country}-{language}".lower()
+        return (
+            "https://www.dhl.com/"
+            + locale
+            + "/home/tracking/tracking-parcel.html?submit=1&tracking-id={}"
+        )
```

## Comparing `karrio.dhl_universal-2023.1rc4.dist-info/METADATA` & `karrio.dhl_universal-2023.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: karrio.dhl-universal
-Version: 2023.1rc4
+Version: 2023.4
 Summary: DHL Universal Tracking karrio extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: karrio
-Requires-Dist: carrier.dhl-universal
 
 # karrio.dhl_universal
 
 This package is a DHL Universal Tracking extension of the [karrio](https://pypi.org/project/karrio) multi carrier shipping SDK.
 
 ## Requirements
 
@@ -39,7 +39,9 @@
     Settings(
         ...
     )
 )
 ```
 
 Check the [Karrio Mutli-carrier SDK docs](https://docs.karrio.io) for Shipping API requests
+
+
```

## Comparing `karrio.dhl_universal-2023.1rc4.dist-info/RECORD` & `karrio.dhl_universal-2023.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+dhl_universal_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dhl_universal_lib/tracking.py,sha256=kZ6e0cwFbOcQNZn7kbCg8_NX0J_Gx8rFLrzILIAAu6I,4243
 karrio/mappers/dhl_universal/__init__.py,sha256=IQ83K6Gqh9FNeuO7jqMoK96B6eCt61KPByqu51lpov8,365
-karrio/mappers/dhl_universal/mapper.py,sha256=x2e3zDNhTttir8Ubq33yF81jnSVsifaKfYjR1mgMvJw,4257
-karrio/mappers/dhl_universal/proxy.py,sha256=NUW1c1yxw8O2grA0CbNxUNiz9VvWsdc0TYoreJ7O4Bs,1041
-karrio/mappers/dhl_universal/settings.py,sha256=H_kTHTu3o5cP-W1GUhzLDrc-lNma287E0d_3Y_MDK-8,479
+karrio/mappers/dhl_universal/mapper.py,sha256=1Vqs6mjOXRIMDjmmkABa32Ut4SkN1rdr2sf2twMQCEU,4099
+karrio/mappers/dhl_universal/proxy.py,sha256=SGN45uuBcpzNoQEflVCFmrwCHBPwMXEGbaP1iWLMBP8,1036
+karrio/mappers/dhl_universal/settings.py,sha256=tBCtAzWIgcQVxIeEHOTIKqdPIFMLTYrRTiGjU-15iiE,526
 karrio/providers/dhl_universal/__init__.py,sha256=-bmW0aBeorKR5xuZHhPGSDZWPaQmkzzhkKtXfhL7EKc,805
 karrio/providers/dhl_universal/error.py,sha256=KJJ-agWimCaEbKPL4Gj7EdUr3jF_3lshJ7Qwx0VIGyQ,703
-karrio/providers/dhl_universal/tracking.py,sha256=JLQhIJHl_vWJONdxQ6eG5V6yIfBASKhIPfK9xmtoe78,2423
-karrio/providers/dhl_universal/units.py,sha256=204yxvHKIz9B-EVW0zwDzVkmK_QSpOurkURyf7BIGuA,1339
-karrio/providers/dhl_universal/utils.py,sha256=XTTLmdTz9tPy-wZipt4z5erKsxF3KTMDDvLUft42X-M,444
-karrio.dhl_universal-2023.1rc4.dist-info/METADATA,sha256=_jM2_a_36-tYk0IP5266m7O6z-_rxIGJK8EeSJ2aPL0,1026
-karrio.dhl_universal-2023.1rc4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-karrio.dhl_universal-2023.1rc4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dhl_universal-2023.1rc4.dist-info/RECORD,,
+karrio/providers/dhl_universal/tracking.py,sha256=3AiUBpkjJgznC9EfnsT_I_WityHIBPkopJxjw297yzA,4587
+karrio/providers/dhl_universal/units.py,sha256=A6AsIfzcgrev3ICnO7VoZ8cnryp5M_sHkZFJbFw-u18,222
+karrio/providers/dhl_universal/utils.py,sha256=SbBM-RV54T3ll2tq0xZTP58A3YfH7jyLiCxdUVuj0Zg,794
+karrio.dhl_universal-2023.4.dist-info/METADATA,sha256=AhN-gyStOGGK0tqcuKh08DeRLHORS1gOMv4EdY5SgQk,1006
+karrio.dhl_universal-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dhl_universal-2023.4.dist-info/top_level.txt,sha256=iwaJXeJNWHTTYYxCNIC5PCDp3yedhWdxjnKmbBUWjvU,33
+karrio.dhl_universal-2023.4.dist-info/RECORD,,
```

