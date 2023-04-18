# Comparing `tmp/karrio.tnt-2023.3-py3-none-any.whl.zip` & `tmp/karrio.tnt-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 13701 bytes, number of entries: 18
+Zip file size: 13756 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      525 b- defN 22-Nov-15 19:21 karrio/mappers/tnt/__init__.py
--rw-rw-r--  2.0 unx     1711 b- defN 22-Nov-15 19:21 karrio/mappers/tnt/mapper.py
--rw-rw-r--  2.0 unx     1024 b- defN 22-Nov-15 19:21 karrio/mappers/tnt/proxy.py
--rw-rw-r--  2.0 unx      459 b- defN 22-Nov-15 19:21 karrio/mappers/tnt/settings.py
+-rw-rw-r--  2.0 unx     1631 b- defN 23-Apr-01 12:45 karrio/mappers/tnt/mapper.py
+-rw-rw-r--  2.0 unx     1019 b- defN 23-Apr-01 12:45 karrio/mappers/tnt/proxy.py
+-rw-rw-r--  2.0 unx      481 b- defN 23-Apr-15 06:44 karrio/mappers/tnt/settings.py
 -rw-rw-r--  2.0 unx      322 b- defN 22-Nov-15 19:21 karrio/providers/tnt/__init__.py
 -rw-rw-r--  2.0 unx     3963 b- defN 22-Nov-15 19:21 karrio/providers/tnt/error.py
--rw-rw-r--  2.0 unx     4979 b- defN 22-Nov-15 19:21 karrio/providers/tnt/rate.py
--rw-rw-r--  2.0 unx     2345 b- defN 22-Nov-15 19:21 karrio/providers/tnt/tracking.py
+-rw-rw-r--  2.0 unx     5025 b- defN 23-Apr-01 15:18 karrio/providers/tnt/rate.py
+-rw-rw-r--  2.0 unx     2405 b- defN 23-Apr-01 15:57 karrio/providers/tnt/tracking.py
 -rw-rw-r--  2.0 unx     4079 b- defN 23-Jan-11 18:22 karrio/providers/tnt/units.py
--rw-rw-r--  2.0 unx      603 b- defN 22-Nov-15 19:21 karrio/providers/tnt/utils.py
+-rw-rw-r--  2.0 unx      625 b- defN 23-Apr-15 06:44 karrio/providers/tnt/utils.py
 -rw-rw-r--  2.0 unx       91 b- defN 22-Nov-15 19:21 karrio/providers/tnt/shipment/__init__.py
--rw-rw-r--  2.0 unx     2167 b- defN 22-Nov-15 19:21 karrio/providers/tnt/shipment/create.py
--rw-rw-r--  2.0 unx     4809 b- defN 23-Mar-25 14:52 karrio/providers/tnt/shipment/label.py
--rw-rw-r--  2.0 unx     6369 b- defN 23-Mar-25 14:53 karrio/providers/tnt/shipment/request.py
--rw-rw-r--  2.0 unx      956 b- defN 23-Mar-27 07:12 karrio.tnt-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.tnt-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.tnt-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1556 b- defN 23-Mar-27 07:12 karrio.tnt-2023.3.dist-info/RECORD
-18 files, 36057 bytes uncompressed, 11119 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     2236 b- defN 23-Apr-01 15:18 karrio/providers/tnt/shipment/create.py
+-rw-rw-r--  2.0 unx     4841 b- defN 23-Apr-01 13:47 karrio/providers/tnt/shipment/label.py
+-rw-rw-r--  2.0 unx     6515 b- defN 23-Apr-01 13:47 karrio/providers/tnt/shipment/request.py
+-rw-rw-r--  2.0 unx      956 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1556 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/RECORD
+18 files, 36369 bytes uncompressed, 11174 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: karrio/providers/tnt/shipment/label.py
 Comment: 
 
 Filename: karrio/providers/tnt/shipment/request.py
 Comment: 
 
-Filename: karrio.tnt-2023.3.dist-info/METADATA
+Filename: karrio.tnt-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.tnt-2023.3.dist-info/WHEEL
+Filename: karrio.tnt-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.tnt-2023.3.dist-info/top_level.txt
+Filename: karrio.tnt-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.tnt-2023.3.dist-info/RECORD
+Filename: karrio.tnt-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/tnt/mapper.py

```diff
@@ -1,25 +1,23 @@
 from typing import List, Tuple
 from karrio.core.utils.serializable import Serializable, Deserializable
 from karrio.api.mapper import Mapper as BaseMapper
 from karrio.core.models import (
     # ShipmentRequest,
     TrackingRequest,
     RateRequest,
-
     TrackingDetails,
     # ShipmentDetails,
     RateDetails,
     Message,
 )
 from karrio.providers.tnt import (
     # parse_shipment_response,
     parse_tracking_response,
     # parse_rate_response,
-
     tracking_request,
     # shipment_request,
     # rate_request,
 )
 from karrio.mappers.tnt.settings import Settings
 
 
@@ -32,29 +30,24 @@
     #     return rate_request(payload, self.settings)
 
     # def create_shipment_request(
     #     self, payload: ShipmentRequest
     # ) -> Serializable:
     #     return shipment_request(payload, self.settings)
 
-    def create_tracking_request(
-        self, payload: TrackingRequest
-    ) -> Serializable:
+    def create_tracking_request(self, payload: TrackingRequest) -> Serializable:
         return tracking_request(payload, self.settings)
 
-    
-
-
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
 
     def parse_tracking_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[List[TrackingDetails], List[Message]]:
-        return parse_tracking_response(response.deserialize(), self.settings)
+        return parse_tracking_response(response, self.settings)
```

## karrio/mappers/tnt/proxy.py

```diff
@@ -12,15 +12,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy Methods """
 
-    def get_tracking(self, request: Serializable) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         response = self._send_request(request, "/expressconnect/track.do")
 
         return Deserializable(response, XP.to_xml)
 
     """ Private Methods """
 
     def _send_request(self, request: Serializable, path: str) -> str:
```

## karrio/mappers/tnt/settings.py

```diff
@@ -10,12 +10,13 @@
 
     # Carrier specific properties
     username: str
     password: str
     account_number: str = None
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "tnt"
```

## karrio/providers/tnt/rate.py

```diff
@@ -19,17 +19,18 @@
 import karrio.core.models as models
 import karrio.providers.purolator.error as provider_error
 import karrio.providers.purolator.units as provider_units
 import karrio.providers.purolator.utils as provider_utils
 
 
 def parse_rate_response(
-    response: lib.Element,
+    _response: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     price_response = lib.find_element(
         "priceResponse", response, priceResponse, first=True
     )
 
     if price_response is not None and price_response.ratedServices is not None:
         rate_details = [
             _extract_detail((price_response.ratedServices, service), settings)
@@ -73,15 +74,15 @@
         meta=dict(service_name=service.product.productDesc),
     )
 
 
 def rate_request(
     payload: models.RateRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[priceRequest]:
+) -> lib.Serializable:
     package = lib.to_packages(payload.parcels).single
     service = lib.to_services(payload.services, provider_units.ShipmentService).first
     options = lib.to_shipping_options(
         payload.options,
         package_options=package.options,
         initializer=provider_units.shipping_options_initializer,
     )
```

## karrio/providers/tnt/tracking.py

```diff
@@ -11,20 +11,23 @@
     TrackingEvent,
     TrackingDetails,
     TrackingRequest,
     Message,
 )
 from karrio.providers.tnt.utils import Settings
 from karrio.providers.tnt.error import parse_error_response
+import karrio.lib as lib
 
 
 def parse_tracking_response(
-    response, settings: Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: Settings,
 ) -> Tuple[List[TrackingDetails], List[Message]]:
-    details = response.xpath(".//*[local-name() = $name]", name="Consignment")
+    response = _response.deserialize()
+    details = lib.find_element("Consignment", response)
     tracking_details = [_extract_detail(node, settings) for node in details]
 
     return tracking_details, parse_error_response(response, settings)
 
 
 def _extract_detail(node: Element, settings: Settings) -> TrackingDetails:
     detail = XP.to_object(ConsignmentType, node)
@@ -45,17 +48,15 @@
             )
             for status in cast(List[StatusStructure], detail.StatusData)
         ],
         delivered=(detail.SummaryCode == "DEL"),
     )
 
 
-def tracking_request(
-    payload: TrackingRequest, settings: Settings
-) -> Serializable[TrackRequest]:
+def tracking_request(payload: TrackingRequest, settings: Settings) -> Serializable:
     request = TrackRequest(
         locale="en_US",
         version="3.1",
         SearchCriteria=SearchCriteriaType(
             marketType="INTERNATIONAL",
             originCountry=(settings.account_country_code or "US"),
             ConsignmentNumber=payload.tracking_numbers,
```

## karrio/providers/tnt/utils.py

```diff
@@ -6,14 +6,15 @@
     """TNT connection settings."""
 
     username: str
     password: str
     account_number: str = None
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
 
     id: str = None
 
     @property
     def carrier_name(self):
         return "tnt"
```

## karrio/providers/tnt/shipment/create.py

```diff
@@ -16,19 +16,21 @@
 from karrio.providers.tnt.shipment.label import (
     create_label_request,
     parse_label_response,
 )
 from karrio.providers.tnt.shipment.request import create_shipment_request
 from karrio.providers.tnt.error import parse_error_response
 from karrio.providers.tnt.utils import Settings
+import karrio.lib as lib
 
 
 def parse_shipment_response(
-    response: Element, settings: Settings
+    _response: lib.Deserializable[Element], settings: Settings
 ) -> Tuple[ShipmentDetails, List[Message]]:
+    response = _response.deserialize()
     shipment = _extract_detail(response, settings)
 
     return shipment, parse_error_response(response, settings)
 
 
 def _extract_detail(response: Element, settings: Settings) -> Optional[ShipmentDetails]:
     activity: document = XP.find(
@@ -45,17 +47,15 @@
         carrier_id=settings.carrier_id,
         tracking_number=activity.CREATE.CONNUMBER,
         shipment_identifier=activity.CREATE.CONREF,
         docs=Documents(label=label),
     )
 
 
-def shipment_request(
-    payload: ShipmentRequest, settings: Settings
-) -> Serializable[Pipeline]:
+def shipment_request(payload: ShipmentRequest, settings: Settings) -> Serializable:
     def _create_shipment_request(_) -> Job:
         return Job(id="create", data=create_shipment_request(payload, settings))
 
     def _create_label_request(shipment_response: str) -> Job:
         activity = XP.to_object(document, XP.to_xml(shipment_response))
         fallback = shipment_response if activity is None else None
         data = (
```

## karrio/providers/tnt/shipment/label.py

```diff
@@ -18,15 +18,15 @@
 from karrio.core.models import ShipmentRequest, Payment
 from karrio.providers.tnt.units import PaymentType
 from karrio.providers.tnt.utils import Settings
 
 
 def create_label_request(
     activity: document, payload: ShipmentRequest, settings: Settings
-) -> Serializable[labelRequest]:
+) -> Serializable:
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
     package = Packages(payload.parcels).single
     payment = payload.payment or Payment(paid_by="sender")
     price: PRICE = next(activity.RATE.PRICE, PRICE())
 
     request = labelRequest(
@@ -47,15 +47,17 @@
                     exactMatch=None,
                     province=shipper.state_code,
                     postcode=shipper.postal_code,
                     country=shipper.country_code,
                 ),
                 delivery=nameAndAddressRequestType(
                     name=recipient.contact,
-                    addressLine1=lib.text(recipient.street_number, recipient.address_line1),
+                    addressLine1=lib.text(
+                        recipient.street_number, recipient.address_line1
+                    ),
                     addressLine2=recipient.address_line2,
                     addressLine3=None,
                     town=recipient.city,
                     exactMatch=None,
                     province=recipient.state_code,
                     postcode=recipient.postal_code,
                     country=recipient.country_code,
```

## karrio/providers/tnt/shipment/request.py

```diff
@@ -28,15 +28,15 @@
 import karrio.providers.tnt.units as provider_units
 import karrio.providers.tnt.utils as provider_utils
 
 
 def shipment_request(
     payload: models.ShipmentRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[ESHIPPER]:
+) -> lib.Serializable:
     ref = f"ref_{uuid4()}"
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
     package = lib.to_packages(payload.parcels).single
     service = provider_units.ShipmentService.map(payload.service).value_or_key
     options = lib.to_shipping_options(
         payload.options,
@@ -123,21 +123,25 @@
                         HEIGHT=package.height.M,
                         WIDTH=package.width.M,
                         WEIGHT=package.weight.KG,
                         ARTICLE=(
                             [
                                 ARTICLE(
                                     ITEMS=item.quantity,
-                                    DESCRIPTION=lib.text(item.title or item.description or "N/A", max=35),
+                                    DESCRIPTION=lib.text(
+                                        item.title or item.description or "N/A", max=35
+                                    ),
                                     WEIGHT=units.Weight(
                                         item.weight,
                                         units.WeightUnit[item.weight_unit],
                                     ).KG,
                                     INVOICEVALUE=item.value_amount,
-                                    INVOICEDESC=lib.text(item.title or item.description, max=35),
+                                    INVOICEDESC=lib.text(
+                                        item.title or item.description, max=35
+                                    ),
                                     HTS=item.hs_code or item.sku,
                                     COUNTRY=item.origin_country,
                                 )
                                 for item in payload.customs.commodities
                             ]
                             if payload.customs is not None
                             and any(payload.customs.commodities)
```

## Comparing `karrio.tnt-2023.3.dist-info/METADATA` & `karrio.tnt-2023.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.tnt
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - TNT Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.tnt-2023.3.dist-info/RECORD` & `karrio.tnt-2023.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 karrio/mappers/tnt/__init__.py,sha256=t43YmnoGxv1UYCuFeWcPzwKAKL2EYMUMwky5jTm4J-s,525
-karrio/mappers/tnt/mapper.py,sha256=LQOhRnbKf5zmjQCUwlCaQR2XqWmcnbSBuasD0Y0VWnE,1711
-karrio/mappers/tnt/proxy.py,sha256=pELHgYmAq7sowAKUM1UL5NBAyt15VBrCxwqUiIpFy4M,1024
-karrio/mappers/tnt/settings.py,sha256=wIKAdHbyF2fpb7wt8t8NcQgwDOEt1JhBBl3cZ3NfWBQ,459
+karrio/mappers/tnt/mapper.py,sha256=guUGRywuX_lSnxlFM23ckZT7M1PFWVLEzieUfMbWxyc,1631
+karrio/mappers/tnt/proxy.py,sha256=cWd7wt_USe0HxgtzByTTOBNCFdZg1EtqU2s4ZjWAjoY,1019
+karrio/mappers/tnt/settings.py,sha256=Ytuk1kpXlJHXkXvWOduxvAXbcFPtE4u0GiZeliFKaNA,481
 karrio/providers/tnt/__init__.py,sha256=mXQ667KelUTn200EtGlSK10U3XcuLRPacoCRm5k_4sc,322
 karrio/providers/tnt/error.py,sha256=SkoXTZ9HO0-D8xE5x6ikS2HYQdIoCq5wWvTysyTvWjM,3963
-karrio/providers/tnt/rate.py,sha256=4nUi9zgN3ygGCL6aJn2dnIAGinoPYzkL90u3j1h6f1Y,4979
-karrio/providers/tnt/tracking.py,sha256=sPTEsIqn4FJCTkHzZEYUPl78S0JB7hX7vPXZY4wvNhg,2345
+karrio/providers/tnt/rate.py,sha256=b2furEIFdKdLmi8KJXVAxZMmqyqw9BTSXgH1glzdGRo,5025
+karrio/providers/tnt/tracking.py,sha256=96jtTWBhtsjYOdWVRsaRaN1gHbm5tiWPAEgUuV5qP1o,2405
 karrio/providers/tnt/units.py,sha256=3HP4Ve6GXlK_zLzKXFzLIlZr1O5l5_1Hye2Dyy0VJfM,4079
-karrio/providers/tnt/utils.py,sha256=YQ3CMShLawLZDpxJi-rB-GXiqidpkl86bbFRav2H0P0,603
+karrio/providers/tnt/utils.py,sha256=U9QGLpRj8QozSaDvBdxllhywSwPP1NQolLbhoVKHK5A,625
 karrio/providers/tnt/shipment/__init__.py,sha256=UPOD_hgNR9l8Mlkq4f0fB2Znl_iZLDLf2i1b-v2Hw9A,91
-karrio/providers/tnt/shipment/create.py,sha256=KuwVhudleVxleI6F2zHvxzNWJTDrj6pvIsuqPVtey0Q,2167
-karrio/providers/tnt/shipment/label.py,sha256=AWdnafGQYvY4OxC_1pKO5vol7OzVdQdS-_-TKRQlCh4,4809
-karrio/providers/tnt/shipment/request.py,sha256=N_8cVl2sJRdcdkTayCvqM8Kg43UPohidd5ksuPPaw8w,6369
-karrio.tnt-2023.3.dist-info/METADATA,sha256=J_7fE5GDMHyZgex_YTJOuDToEIV32CmJNkbnjhKjEwU,956
-karrio.tnt-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.tnt-2023.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.tnt-2023.3.dist-info/RECORD,,
+karrio/providers/tnt/shipment/create.py,sha256=_ZKiaqqh8BMeaorlmlxjsRRwW-mIKw-1mnE1xb7iD3Q,2236
+karrio/providers/tnt/shipment/label.py,sha256=By2Sjj2T2dNz7id8GtHBfsl2P-lG1PLtiBKkEToGICI,4841
+karrio/providers/tnt/shipment/request.py,sha256=hFsJB_c8GLWkQTV3S8vRymMrisPsR3MD5psrznZoQ_0,6515
+karrio.tnt-2023.4.dist-info/METADATA,sha256=5nn7f0rO4eYPJNnLXpuJGWaGr-Ldg08OFY-Raww3JlM,956
+karrio.tnt-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.tnt-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.tnt-2023.4.dist-info/RECORD,,
```

