# Comparing `tmp/karrio.easypost-2023.3-py3-none-any.whl.zip` & `tmp/karrio.easypost-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 27776 bytes, number of entries: 24
+Zip file size: 27910 bytes, number of entries: 24
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-03 13:50 easypost_lib/__init__.py
 -rw-rw-r--  2.0 unx      304 b- defN 23-Mar-03 13:50 easypost_lib/error_response.py
 -rw-rw-r--  2.0 unx      267 b- defN 23-Mar-03 13:50 easypost_lib/shipment_purchase.py
 -rw-rw-r--  2.0 unx     2303 b- defN 23-Mar-03 13:50 easypost_lib/shipment_request.py
 -rw-rw-r--  2.0 unx     7274 b- defN 23-Mar-03 13:50 easypost_lib/shipments_response.py
 -rw-rw-r--  2.0 unx     2453 b- defN 23-Mar-03 13:50 easypost_lib/trackers_response.py
 -rw-rw-r--  2.0 unx      527 b- defN 23-Mar-03 13:50 karrio/mappers/easypost/__init__.py
--rw-rw-r--  2.0 unx     2164 b- defN 23-Mar-03 13:50 karrio/mappers/easypost/mapper.py
--rw-rw-r--  2.0 unx     3406 b- defN 23-Mar-03 13:50 karrio/mappers/easypost/proxy.py
--rw-rw-r--  2.0 unx      384 b- defN 23-Mar-03 13:50 karrio/mappers/easypost/settings.py
+-rw-rw-r--  2.0 unx     2108 b- defN 23-Apr-01 12:43 karrio/mappers/easypost/mapper.py
+-rw-rw-r--  2.0 unx     3386 b- defN 23-Apr-01 12:45 karrio/mappers/easypost/proxy.py
+-rw-rw-r--  2.0 unx      406 b- defN 23-Apr-15 06:44 karrio/mappers/easypost/settings.py
 -rw-rw-r--  2.0 unx      333 b- defN 23-Mar-03 13:50 karrio/providers/easypost/__init__.py
 -rw-rw-r--  2.0 unx      598 b- defN 23-Mar-03 13:50 karrio/providers/easypost/error.py
--rw-rw-r--  2.0 unx     5605 b- defN 23-Mar-25 15:12 karrio/providers/easypost/rate.py
--rw-rw-r--  2.0 unx     3948 b- defN 23-Mar-25 13:46 karrio/providers/easypost/tracking.py
+-rw-rw-r--  2.0 unx     5912 b- defN 23-Apr-01 15:18 karrio/providers/easypost/rate.py
+-rw-rw-r--  2.0 unx     3985 b- defN 23-Apr-01 15:19 karrio/providers/easypost/tracking.py
 -rw-rw-r--  2.0 unx    52532 b- defN 23-Mar-03 13:50 karrio/providers/easypost/units.py
--rw-rw-r--  2.0 unx      752 b- defN 23-Mar-03 13:50 karrio/providers/easypost/utils.py
+-rw-rw-r--  2.0 unx      774 b- defN 23-Apr-15 06:44 karrio/providers/easypost/utils.py
 -rw-rw-r--  2.0 unx      232 b- defN 23-Mar-03 13:50 karrio/providers/easypost/shipment/__init__.py
--rw-rw-r--  2.0 unx      887 b- defN 23-Mar-03 13:50 karrio/providers/easypost/shipment/cancel.py
--rw-rw-r--  2.0 unx     7227 b- defN 23-Mar-25 15:15 karrio/providers/easypost/shipment/create.py
--rw-rw-r--  2.0 unx     7650 b- defN 23-Mar-27 07:12 karrio.easypost-2023.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      984 b- defN 23-Mar-27 07:12 karrio.easypost-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.easypost-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       28 b- defN 23-Mar-27 07:12 karrio.easypost-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2166 b- defN 23-Mar-27 07:12 karrio.easypost-2023.3.dist-info/RECORD
-24 files, 102116 bytes uncompressed, 24194 bytes compressed:  76.3%
+-rw-rw-r--  2.0 unx      977 b- defN 23-Apr-01 15:18 karrio/providers/easypost/shipment/cancel.py
+-rw-rw-r--  2.0 unx     7362 b- defN 23-Apr-01 15:18 karrio/providers/easypost/shipment/create.py
+-rw-rw-r--  2.0 unx     7650 b- defN 23-Apr-18 07:09 karrio.easypost-2023.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      984 b- defN 23-Apr-18 07:09 karrio.easypost-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.easypost-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       28 b- defN 23-Apr-18 07:09 karrio.easypost-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2166 b- defN 23-Apr-18 07:09 karrio.easypost-2023.4.dist-info/RECORD
+24 files, 102653 bytes uncompressed, 24328 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: karrio/providers/easypost/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/easypost/shipment/create.py
 Comment: 
 
-Filename: karrio.easypost-2023.3.dist-info/LICENSE
+Filename: karrio.easypost-2023.4.dist-info/LICENSE
 Comment: 
 
-Filename: karrio.easypost-2023.3.dist-info/METADATA
+Filename: karrio.easypost-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.easypost-2023.3.dist-info/WHEEL
+Filename: karrio.easypost-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.easypost-2023.3.dist-info/top_level.txt
+Filename: karrio.easypost-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.easypost-2023.3.dist-info/RECORD
+Filename: karrio.easypost-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/easypost/mapper.py

```diff
@@ -45,23 +45,23 @@
         return tracking_request(payload, self.settings)
 
     # Response Parsers
 
     def parse_rate_response(
         self, response: Deserializable
     ) -> Tuple[List[RateDetails], List[Message]]:
-        return parse_rate_response(response.deserialize(), self.settings)
+        return parse_rate_response(response, self.settings)
 
     def parse_shipment_response(
         self, response: Deserializable
     ) -> Tuple[ShipmentDetails, List[Message]]:
-        return parse_shipment_response(response.deserialize(), self.settings)
+        return parse_shipment_response(response, self.settings)
 
     def parse_cancel_shipment_response(
         self, response: Deserializable
     ) -> Tuple[ConfirmationDetails, List[Message]]:
-        return parse_shipment_cancel_response(response.deserialize(), self.settings)
+        return parse_shipment_cancel_response(response, self.settings)
 
     def parse_tracking_response(
         self, response: Deserializable
     ) -> Tuple[List[TrackingDetails], List[Message]]:
-        return parse_tracking_response(response.deserialize(), self.settings)
+        return parse_tracking_response(response, self.settings)
```

## karrio/mappers/easypost/proxy.py

```diff
@@ -5,22 +5,22 @@
 from karrio.mappers.easypost.settings import Settings
 from karrio.core.utils.serializable import Serializable, Deserializable
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
-    def get_rates(self, request: Serializable) -> Deserializable[str]:
+    def get_rates(self, request: Serializable) -> Deserializable:
         response = self._send_request(
             path="/shipments", request=Serializable(request.serialize(), DP.jsonify)
         )
 
         return Deserializable(response, DP.to_dict)
 
-    def create_shipment(self, request: Serializable) -> Deserializable[str]:
+    def create_shipment(self, request: Serializable) -> Deserializable:
         payload = request.serialize()
 
         def create(request) -> str:
             response = DP.to_dict(
                 self._send_request(
                     path="/shipments", request=Serializable(request, DP.jsonify)
                 )
@@ -52,20 +52,20 @@
                 path=f"/shipments/{response['id']}/buy",
                 request=Serializable(data, DP.jsonify),
             )
 
         response = create(payload["data"])
         return Deserializable(response, DP.to_dict)
 
-    def cancel_shipment(self, request: Serializable) -> Deserializable[str]:
+    def cancel_shipment(self, request: Serializable) -> Deserializable:
         response = self._send_request(path=f"/shipments/{request.serialize()}/refund")
 
         return Deserializable(response, DP.to_dict)
 
-    def get_tracking(self, requests: Serializable) -> Deserializable[str]:
+    def get_tracking(self, requests: Serializable) -> Deserializable:
         track = lambda request: (
             request["tracking_code"],
             self._send_request(
                 **(
                     dict(path="/trackers", request=Serializable(request, DP.jsonify))
                     if request.get("tracker_id") is None
                     else dict(path=f"/trackers/{request['tracker_id']}", method="GET")
```

## karrio/mappers/easypost/settings.py

```diff
@@ -11,7 +11,8 @@
     api_key: str
 
     id: str = None
     test_mode: bool = False
     carrier_id: str = "easypost"
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/easypost/rate.py

```diff
@@ -7,16 +7,18 @@
 import karrio.core.models as models
 import karrio.providers.easypost.error as provider_error
 import karrio.providers.easypost.units as provider_units
 import karrio.providers.easypost.utils as provider_utils
 
 
 def parse_rate_response(
-    response: dict, settings: provider_utils.Settings
+    _response: lib.Deserializable[dict],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[models.RateDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = (
         [provider_error.parse_error_response(response, settings)]
         if "error" in response
         else []
     )
     rates = _extract_details(response, settings) if "error" not in response else []
 
@@ -58,25 +60,30 @@
     options = lib.to_shipping_options(
         payload,
         package_options=package.options,
         initializer=provider_units.shipping_options_initializer,
     )
     is_intl = shipper.country_code != recipient.country_code
     customs = (
-        models.Customs(commodities=(
-            package.parcel.items
-            if any(package.parcel.items)
-            else [models.Commodity(
-                sku="0000",
-                quantity=1,
-                weight=package.weight.value,
-                weight_unit=package.weight_unit.value,
-            )]
-        ))
-        if is_intl else None
+        models.Customs(
+            commodities=(
+                package.parcel.items
+                if any(package.parcel.items)
+                else [
+                    models.Commodity(
+                        sku="0000",
+                        quantity=1,
+                        weight=package.weight.value,
+                        weight_unit=package.weight_unit.value,
+                    )
+                ]
+            )
+        )
+        if is_intl
+        else None
     )
 
     requests = easypost.ShipmentRequest(
         shipment=easypost.Shipment(
             reference=payload.reference,
             to_address=easypost.Address(
                 company=recipient.company_name,
@@ -121,26 +128,31 @@
             customs_info=(
                 easypost.CustomsInfo(
                     contents_type="other",
                     customs_certify=True,
                     customs_signer=shipper.person_name,
                     customs_items=[
                         easypost.CustomsItem(
-                            description=lib.text(item.description or item.title or "N/A"),
+                            description=lib.text(
+                                item.description or item.title or "N/A"
+                            ),
                             origin_country=item.origin_country,
                             quantity=item.quantity,
                             value=item.value_amount,
                             weight=units.Weight(item.weight, item.weight_unit).OZ,
                             code=item.sku,
                             manufacturer=None,
                             currency=item.value_currency,
                             eccn=(item.metadata or {}).get("eccn"),
                             printed_commodity_identifier=(item.sku or item.id),
                             hs_tariff_number=item.hs_code,
-                        ) for item in customs.commodities
+                        )
+                        for item in customs.commodities
                     ],
-                ) if customs else None
+                )
+                if customs
+                else None
             ),
         )
     )
 
     return lib.Serializable(requests, lib.to_dict)
```

## karrio/providers/easypost/tracking.py

```diff
@@ -4,17 +4,18 @@
 import karrio.core.models as models
 import karrio.providers.easypost.error as error
 import karrio.providers.easypost.utils as provider_utils
 import karrio.providers.easypost.units as provider_units
 
 
 def parse_tracking_response(
-    responses: typing.List[typing.Tuple[str, dict]],
+    _responses: lib.Deserializable[typing.List[typing.Tuple[str, dict]]],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    responses = _responses.deserialize()
     errors = [
         error.parse_error_response(response, settings, dict(tracking_number=code))
         for code, response in responses
         if "error" in response
     ]
     trackers = [
         _extract_details(response, settings)
@@ -71,17 +72,15 @@
             shipment_id=tracker.shipment_id,
             tracker_id=tracker.id,
             fees=tracker.fees,
         ),
     )
 
 
-def tracking_request(
-    payload: models.TrackingRequest, _
-) -> lib.Serializable[typing.List[dict]]:
+def tracking_request(payload: models.TrackingRequest, _) -> lib.Serializable:
     """Send one or multiple tracking request(s) to EasyPost.
     the payload must match the following schema:
     {
         "tracking_numbers": ["123456789"],
         "options": {
             "123456789": {
                 "carrier": "usps",
```

## karrio/providers/easypost/utils.py

```diff
@@ -6,14 +6,15 @@
 
 class Settings(BaseSettings):
     """EasyPost connection settings."""
 
     api_key: str
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     @property
     def carrier_name(self):
         return "easypost"
 
     @property
     def server_url(self):
```

## karrio/providers/easypost/shipment/cancel.py

```diff
@@ -1,17 +1,20 @@
 from typing import List, Tuple
 from karrio.core.models import ShipmentCancelRequest, ConfirmationDetails, Message
 from karrio.core.utils import Serializable
 from karrio.providers.easypost.error import parse_error_response
 from karrio.providers.easypost.utils import Settings
+import karrio.lib as lib
 
 
 def parse_shipment_cancel_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[ConfirmationDetails, List[Message]]:
+    response = _response.deserialize()
     status = response.get("status")
     errors = [parse_error_response(response, settings)] if "error" in response else []
 
     details = ConfirmationDetails(
         carrier_id=settings.carrier_id,
         carrier_name=settings.carrier_name,
         success=status != "rejected",
```

## karrio/providers/easypost/shipment/create.py

```diff
@@ -7,16 +7,18 @@
 import karrio.core.models as models
 import karrio.providers.easypost.error as provider_error
 import karrio.providers.easypost.units as provider_units
 import karrio.providers.easypost.utils as provider_utils
 
 
 def parse_shipment_response(
-    response: dict, settings: provider_utils.Settings
+    _response: lib.Deserializable[dict],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[models.ShipmentDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = (
         [provider_error.parse_error_response(response, settings)]
         if "error" in response
         else []
     )
     shipment = _extract_details(response, settings) if "error" not in response else None
 
@@ -145,15 +147,17 @@
                         customs_signer=(customs.signer or shipper.person_name),
                         eel_pfc=customs.options.eel_pfc.state,
                         non_delivery_option=customs.options.non_delivery_option.state,
                         restriction_type=customs.options.restriction_type.state,
                         declaration=customs.options.declaration.state,
                         customs_items=[
                             easypost.CustomsItem(
-                                description=lib.text(item.description or item.title or "N/A"),
+                                description=lib.text(
+                                    item.description or item.title or "N/A"
+                                ),
                                 origin_country=item.origin_country,
                                 quantity=item.quantity,
                                 value=item.value_amount,
                                 weight=units.Weight(item.weight, item.weight_unit).OZ,
                                 code=item.sku,
                                 manufacturer=None,
                                 currency=item.value_currency,
```

## Comparing `karrio.easypost-2023.3.dist-info/LICENSE` & `karrio.easypost-2023.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `karrio.easypost-2023.3.dist-info/METADATA` & `karrio.easypost-2023.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.easypost
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - EasyPost Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.easypost-2023.3.dist-info/RECORD` & `karrio.easypost-2023.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 easypost_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 easypost_lib/error_response.py,sha256=-ArlW7QfFx_xjKysODuoUPzBrVPj58K5aQg4nJQPUiA,304
 easypost_lib/shipment_purchase.py,sha256=CixH51fBD-DXDTT935vBOCwcDg0lKBibQx4Mfjqm_7M,267
 easypost_lib/shipment_request.py,sha256=X0chFG76c95W0BWhpx663dretpbxymHWMZlplWt0XjM,2303
 easypost_lib/shipments_response.py,sha256=grq8YCjc-p4_k3SdTsJGIBrWvUNB50h9z_OjJXEd7Sg,7274
 easypost_lib/trackers_response.py,sha256=zk7zPl2f_-gJ7L0j1IqTYCfjJ0wu-689nSkfeWNIuPI,2453
 karrio/mappers/easypost/__init__.py,sha256=faXipOlK2K0i0-cvi5VmnK_tbYQwd7I9rGjGuFmZ2Lk,527
-karrio/mappers/easypost/mapper.py,sha256=-ln1AbkCb14cWn4xqfiOcKFxsyO94I_SvRXcYZ_KU0U,2164
-karrio/mappers/easypost/proxy.py,sha256=vUS551SL59aQTu49ldQqwERNmLv5diDeuQk-8oJ7l8w,3406
-karrio/mappers/easypost/settings.py,sha256=oAloPZCxMWe44H0Q3ZbMELkPES5p7saiZlyd4KkDg74,384
+karrio/mappers/easypost/mapper.py,sha256=1p2kff10Za5-QlFR4Gz6Kcnnwi2HSmr3DEke6CMkR7k,2108
+karrio/mappers/easypost/proxy.py,sha256=A1oDrv0djpNaNdZvzKLNHV7-ZD4aChqgsTYRarodebw,3386
+karrio/mappers/easypost/settings.py,sha256=tVxN6QXlpYgjslfMRzc-6uvI1E-vp6H6f_NsDpF65AA,406
 karrio/providers/easypost/__init__.py,sha256=v89eaMBV-Kn7Za7WzrXpSkKfFG2HSRB0SXByoI2hOec,333
 karrio/providers/easypost/error.py,sha256=lVCgYoSMBVjVkj61_a5EXlDO-O0wQH-5vpuiZ8zWq_8,598
-karrio/providers/easypost/rate.py,sha256=XAn6R0I-_sHUjCowZ1ffIKeqJQS2XJpjphc4NT9ubNM,5605
-karrio/providers/easypost/tracking.py,sha256=aGYJ9Y_H_D2mk2Z72B-G1V8tXtiCopPjIcpXngZEOz8,3948
+karrio/providers/easypost/rate.py,sha256=W0xZl_D9by5mKuonZmY-J-4Ljq4F-xR3uA4-iwsLces,5912
+karrio/providers/easypost/tracking.py,sha256=d3oJu5xanHiyuUrvmxlMVgbYg1vTXgERa1T-FUC3YIo,3985
 karrio/providers/easypost/units.py,sha256=iTNrbwo6QWq9aaYm_I2yvdgI_RafRzKyQwN5Gih2WLM,52532
-karrio/providers/easypost/utils.py,sha256=qqkz78leQYnEMUZ9tN27vp7VAElGvDt-avGxX2WZiAw,752
+karrio/providers/easypost/utils.py,sha256=rJ1uxvaOXcwCAbPmiklk0UoJwhbix0sjVc6jV1BWbtQ,774
 karrio/providers/easypost/shipment/__init__.py,sha256=oEO3ToyRIVyE5mcc_exdZRpM6WMu6PMD2UpdkUJrKqI,232
-karrio/providers/easypost/shipment/cancel.py,sha256=Rl-5G02uv4mwIyRTdGmJOm8qqnBNMr0jCrwUXhEHnv0,887
-karrio/providers/easypost/shipment/create.py,sha256=PfeISEya2lB52pmomY-BRKuIzr_yanTu-RwIrEFsGc4,7227
-karrio.easypost-2023.3.dist-info/LICENSE,sha256=6or154nLLU6bELzjh0mCreFjt0m2v72zLi3yHE0QbeE,7650
-karrio.easypost-2023.3.dist-info/METADATA,sha256=hivnznktLkDsR-czdZxGsVefm7SKUcIlL3xYYf-AL60,984
-karrio.easypost-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.easypost-2023.3.dist-info/top_level.txt,sha256=mtGDNg50UyITXU_982jx1P6O4yV6vUDpBgo2VKsYV6E,28
-karrio.easypost-2023.3.dist-info/RECORD,,
+karrio/providers/easypost/shipment/cancel.py,sha256=VmYlk9WrSpNFzFLx87PJj-_Z4ruco4_Qu3SJRO8uXr4,977
+karrio/providers/easypost/shipment/create.py,sha256=OtbIZkjFdhlAo4hD5c-rkLvafQAPsY_lTySbg6Elf0U,7362
+karrio.easypost-2023.4.dist-info/LICENSE,sha256=6or154nLLU6bELzjh0mCreFjt0m2v72zLi3yHE0QbeE,7650
+karrio.easypost-2023.4.dist-info/METADATA,sha256=W5ZL2MTtLj4rK3R8AcXPkWPxPpf9IDvhzhBIjsHosGg,984
+karrio.easypost-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.easypost-2023.4.dist-info/top_level.txt,sha256=mtGDNg50UyITXU_982jx1P6O4yV6vUDpBgo2VKsYV6E,28
+karrio.easypost-2023.4.dist-info/RECORD,,
```

