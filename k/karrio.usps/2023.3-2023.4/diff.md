# Comparing `tmp/karrio.usps-2023.3-py3-none-any.whl.zip` & `tmp/karrio.usps-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 17904 bytes, number of entries: 21
+Zip file size: 18072 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      450 b- defN 22-Nov-15 19:21 karrio/mappers/usps/__init__.py
--rw-rw-r--  2.0 unx     3612 b- defN 22-Nov-15 19:21 karrio/mappers/usps/mapper.py
--rw-rw-r--  2.0 unx     2007 b- defN 22-Nov-15 19:21 karrio/mappers/usps/proxy.py
--rw-rw-r--  2.0 unx      550 b- defN 22-Nov-15 19:21 karrio/mappers/usps/settings.py
+-rw-rw-r--  2.0 unx     3442 b- defN 23-Apr-01 13:34 karrio/mappers/usps/mapper.py
+-rw-rw-r--  2.0 unx     1969 b- defN 23-Apr-01 13:48 karrio/mappers/usps/proxy.py
+-rw-rw-r--  2.0 unx      572 b- defN 23-Apr-15 06:44 karrio/mappers/usps/settings.py
 -rw-rw-r--  2.0 unx      613 b- defN 22-Nov-15 19:21 karrio/providers/usps/__init__.py
 -rw-rw-r--  2.0 unx      722 b- defN 22-Nov-15 19:21 karrio/providers/usps/error.py
--rw-rw-r--  2.0 unx     6136 b- defN 22-Nov-15 19:21 karrio/providers/usps/rate.py
--rw-rw-r--  2.0 unx     3384 b- defN 23-Mar-25 11:42 karrio/providers/usps/tracking.py
--rw-rw-r--  2.0 unx    16295 b- defN 23-Mar-25 13:56 karrio/providers/usps/units.py
--rw-rw-r--  2.0 unx      712 b- defN 23-Mar-25 13:37 karrio/providers/usps/utils.py
+-rw-rw-r--  2.0 unx     6216 b- defN 23-Apr-01 15:18 karrio/providers/usps/rate.py
+-rw-rw-r--  2.0 unx     3419 b- defN 23-Apr-01 15:18 karrio/providers/usps/tracking.py
+-rw-rw-r--  2.0 unx    16295 b- defN 23-Mar-27 07:55 karrio/providers/usps/units.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-Apr-15 06:44 karrio/providers/usps/utils.py
 -rw-rw-r--  2.0 unx      286 b- defN 22-Nov-15 19:21 karrio/providers/usps/pickup/__init__.py
--rw-rw-r--  2.0 unx     1479 b- defN 23-Mar-25 14:59 karrio/providers/usps/pickup/cancel.py
--rw-rw-r--  2.0 unx     1836 b- defN 22-Nov-15 19:21 karrio/providers/usps/pickup/create.py
--rw-rw-r--  2.0 unx     1918 b- defN 22-Nov-15 19:21 karrio/providers/usps/pickup/update.py
+-rw-rw-r--  2.0 unx     1568 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/cancel.py
+-rw-rw-r--  2.0 unx     1926 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/create.py
+-rw-rw-r--  2.0 unx     2008 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/update.py
 -rw-rw-r--  2.0 unx      198 b- defN 22-Nov-15 19:21 karrio/providers/usps/shipment/__init__.py
--rw-rw-r--  2.0 unx     1525 b- defN 22-Nov-15 19:21 karrio/providers/usps/shipment/cancel.py
--rw-rw-r--  2.0 unx     7653 b- defN 23-Mar-25 15:04 karrio/providers/usps/shipment/create.py
--rw-rw-r--  2.0 unx      964 b- defN 23-Mar-27 07:12 karrio.usps-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.usps-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.usps-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1859 b- defN 23-Mar-27 07:12 karrio.usps-2023.3.dist-info/RECORD
-21 files, 52298 bytes uncompressed, 14830 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx     1614 b- defN 23-Apr-01 15:18 karrio/providers/usps/shipment/cancel.py
+-rw-rw-r--  2.0 unx     7701 b- defN 23-Apr-01 15:18 karrio/providers/usps/shipment/create.py
+-rw-rw-r--  2.0 unx      964 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1859 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/RECORD
+21 files, 52655 bytes uncompressed, 14998 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: karrio/providers/usps/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/usps/shipment/create.py
 Comment: 
 
-Filename: karrio.usps-2023.3.dist-info/METADATA
+Filename: karrio.usps-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.usps-2023.3.dist-info/WHEEL
+Filename: karrio.usps-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.usps-2023.3.dist-info/top_level.txt
+Filename: karrio.usps-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.usps-2023.3.dist-info/RECORD
+Filename: karrio.usps-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/usps/mapper.py

```diff
@@ -5,15 +5,14 @@
     ShipmentCancelRequest,
     # PickupUpdateRequest,
     # PickupCancelRequest,
     ShipmentRequest,
     TrackingRequest,
     # PickupRequest,
     RateRequest,
-
     ConfirmationDetails,
     TrackingDetails,
     ShipmentDetails,
     # PickupDetails,
     RateDetails,
     Message,
 )
@@ -21,42 +20,35 @@
     parse_shipment_cancel_response,
     # parse_pickup_update_response,
     # parse_pickup_cancel_response,
     parse_shipment_response,
     parse_tracking_response,
     # parse_pickup_response,
     parse_rate_response,
-
     shipment_cancel_request,
     # pickup_update_request,
     # pickup_cancel_request,
     tracking_request,
     shipment_request,
     # pickup_request,
     rate_request,
 )
 from karrio.mappers.usps.settings import Settings
 
 
 class Mapper(BaseMapper):
     settings: Settings
 
-    def create_rate_request(
-        self, payload: RateRequest
-    ) -> Serializable:
+    def create_rate_request(self, payload: RateRequest) -> Serializable:
         return rate_request(payload, self.settings)
 
-    def create_tracking_request(
-        self, payload: TrackingRequest
-    ) -> Serializable:
+    def create_tracking_request(self, payload: TrackingRequest) -> Serializable:
         return tracking_request(payload, self.settings)
 
-    def create_shipment_request(
-        self, payload: ShipmentRequest
-    ) -> Serializable:
+    def create_shipment_request(self, payload: ShipmentRequest) -> Serializable:
         return shipment_request(payload, self.settings)
 
     # def create_pickup_request(
     #     self, payload: PickupRequest
     # ) -> Serializable:
     #     return pickup_request(payload, self.settings)
     #
@@ -66,47 +58,46 @@
     #     return pickup_update_request(payload, self.settings)
     #
     # def create_cancel_pickup_request(
     #     self, payload: PickupCancelRequest
     # ) -> Serializable:
     #     return pickup_cancel_request(payload, self.settings)
 
-    def create_cancel_shipment_request(self, payload: ShipmentCancelRequest) -> Serializable[str]:
+    def create_cancel_shipment_request(
+        self, payload: ShipmentCancelRequest
+    ) -> Serializable:
         return shipment_cancel_request(payload, self.settings)
 
-    
-
-
     # def parse_cancel_pickup_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_pickup_cancel_response(response.deserialize(), self.settings)
+    #     return parse_pickup_cancel_response(response, self.settings)
 
     def parse_cancel_shipment_response(
         self, response: Deserializable
     ) -> Tuple[ConfirmationDetails, List[Message]]:
-        return parse_shipment_cancel_response(response.deserialize(), self.settings)
+        return parse_shipment_cancel_response(response, self.settings)
 
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
 
     def parse_rate_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[List[RateDetails], List[Message]]:
-        return parse_rate_response(response.deserialize(), self.settings)
+        return parse_rate_response(response, self.settings)
 
     def parse_shipment_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[ShipmentDetails, List[Message]]:
-        return parse_shipment_response(response.deserialize(), self.settings)
+        return parse_shipment_response(response, self.settings)
 
     def parse_tracking_response(
-        self, response: Deserializable[str]
+        self, response: Deserializable
     ) -> Tuple[List[TrackingDetails], List[Message]]:
-        return parse_tracking_response(response.deserialize(), self.settings)
+        return parse_tracking_response(response, self.settings)
```

## karrio/mappers/usps/proxy.py

```diff
@@ -7,17 +7,15 @@
 
 
 class Proxy(BaseProxy):
     settings: Settings
 
     """ Proxy interface method implementations """
 
-    def get_tracking(
-        self, request: Serializable[TrackFieldRequest]
-    ) -> Deserializable[str]:
+    def get_tracking(self, request: Serializable) -> Deserializable:
         query = urllib.parse.urlencode({"API": "TrackV2", "XML": request.serialize()})
         response = http(
             url=f"{self.settings.server_url}?{query}",
             trace=self.trace_as("xml"),
             method="GET",
         )
```

## karrio/mappers/usps/settings.py

```diff
@@ -17,7 +17,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "usps"
     account_country_code: str = "US"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/usps/rate.py

```diff
@@ -14,16 +14,18 @@
 import karrio.core.errors as errors
 import karrio.providers.usps.error as provider_error
 import karrio.providers.usps.units as provider_units
 import karrio.providers.usps.utils as provider_utils
 
 
 def parse_rate_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     rates: typing.List[models.RateDetails] = [
         _extract_details(package, settings)
         for package in lib.find_element("Postage", response)
     ]
     return rates, provider_error.parse_error_response(response, settings)
 
 
@@ -32,19 +34,21 @@
 ) -> models.RateDetails:
     postage: PostageType = lib.to_object(PostageType, postage_node)
 
     service = provider_units.ServiceClassID.map(str(postage.CLASSID))
     charges: typing.List[SpecialServiceType] = getattr(
         postage.SpecialServices, "SpecialService", []
     )
-    rate = lib.to_decimal((
-        lib.find_element("CommercialPlusRate", postage_node, first=True) or
-        lib.find_element("CommercialRate", postage_node, first=True) or
-        lib.find_element("Rate", postage_node, first=True)
-    ).text)
+    rate = lib.to_decimal(
+        (
+            lib.find_element("CommercialPlusRate", postage_node, first=True)
+            or lib.find_element("CommercialRate", postage_node, first=True)
+            or lib.find_element("Rate", postage_node, first=True)
+        ).text
+    )
     commitment_date_node = lib.find_element("CommitmentDate", postage_node, first=True)
     estimated_date = lib.to_date(getattr(commitment_date_node, "text", None))
     transit = (
         (estimated_date.date() - datetime.now().date()).days
         if estimated_date is not None
         else None
     )
@@ -67,15 +71,15 @@
         meta=dict(service_name=(service.name or postage.MailService)),
     )
 
 
 def rate_request(
     payload: models.RateRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[RateV4Request]:
+) -> lib.Serializable:
     """Create the appropriate USPS rate request depending on the destination
 
     :param payload: Karrio unified API rate request data
     :param settings: USPS connection and auth settings
     :return: a domestic or international USPS compatible request
     :raises: an OriginNotServicedError when origin country is not serviced by the carrier
     """
```

## karrio/providers/usps/tracking.py

```diff
@@ -5,17 +5,18 @@
 import karrio.core.models as models
 import karrio.providers.usps.error as error
 import karrio.providers.usps.utils as provider_utils
 import karrio.providers.usps.units as provider_units
 
 
 def parse_tracking_response(
-    response: lib.Element,
+    _response: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     tracks_info = lib.find_element("TrackInfo", response)
     details = [
         _extract_details(node, settings)
         for node in tracks_info
         if len(lib.find_element("TrackDetail", node)) > 0
     ]
 
@@ -41,15 +42,14 @@
             status.name
             for status in list(provider_units.TrackingStatus)
             if str(getattr(events[0], "EventCode", None)) in status.value
         ),
         provider_units.TrackingStatus.in_transit.name,
     )
 
-
     return models.TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         tracking_number=info.ID,
         estimated_delivery=expected_delivery,
         delivered=delivered,
         status=status,
@@ -69,26 +69,26 @@
                 ),
             )
             for event in events
         ],
         info=models.TrackingInfo(
             carrier_tracking_link=settings.tracking_url.format(info.ID),
             shipment_destination_postal_code=info.DestinationZip,
-            shipment_destication_country=info.DestinationCountryCode,
+            shipment_destination_country=info.DestinationCountryCode,
             shipment_origin_country=info.OriginCountryCode,
             shipment_origin_postal_code=info.OriginZip,
             shipment_service=info.Class,
         ),
     )
 
 
 def tracking_request(
     payload: models.TrackingRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[usps.TrackFieldRequest]:
+) -> lib.Serializable:
     request = usps.TrackFieldRequest(
         USERID=settings.username,
         Revision="1",
         ClientIp="127.0.0.1",
         SourceId="Karrio",
         TrackID=[
             usps.TrackIDType(
```

## karrio/providers/usps/utils.py

```diff
@@ -12,14 +12,15 @@
     mailer_id: str = None
     customer_registration_id: str = None
     logistics_manager_mailer_id: str = None
 
     id: str = None
     account_country_code: str = "US"
     metadata: dict = {}
+    config: dict = {}
 
     @property
     def carrier_name(self):
         return "usps"
 
     @property
     def server_url(self):
```

## karrio/providers/usps/pickup/cancel.py

```diff
@@ -1,19 +1,22 @@
 from typing import Tuple, List
 from usps_lib.carrier_pickup_cancel_request import CarrierPickupCancelRequest
 from karrio.core.utils import Serializable, SF
 from karrio.core.models import PickupCancelRequest, ConfirmationDetails, Message
 
 from karrio.providers.usps.error import parse_error_response
 from karrio.providers.usps.utils import Settings
+import karrio.lib as lib
 
 
 def parse_pickup_cancel_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[ConfirmationDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     details = (
         ConfirmationDetails(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             success=True,
             operation="Pickup Cancel",
@@ -24,15 +27,14 @@
 
     return details, errors
 
 
 def pickup_cancel_request(
     payload: PickupCancelRequest, settings: Settings
 ) -> Serializable:
-
     request = CarrierPickupCancelRequest(
         UserID=settings.username,
         FirmName=payload.address.company_name,
         SuiteOrApt=payload.address.address_line1,
         Address2=SF.concat_str(
             payload.address.address_line1, payload.address.address_line2, join=True
         ),
```

## karrio/providers/usps/pickup/create.py

```diff
@@ -10,19 +10,22 @@
     PickupRequest,
     PickupDetails,
     Message,
 )
 
 from karrio.providers.usps.error import parse_error_response
 from karrio.providers.usps.utils import Settings
+import karrio.lib as lib
 
 
 def parse_pickup_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[PickupDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     details = None
 
     return details, errors
 
 
 def pickup_request(payload: PickupRequest, settings: Settings) -> Serializable:
```

## karrio/providers/usps/pickup/update.py

```diff
@@ -10,19 +10,22 @@
     PickupUpdateRequest,
     PickupDetails,
     Message,
 )
 
 from karrio.providers.usps.error import parse_error_response
 from karrio.providers.usps.utils import Settings
+import karrio.lib as lib
 
 
 def parse_pickup_update_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[PickupDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     details = None
 
     return details, errors
 
 
 def pickup_update_request(
```

## karrio/providers/usps/shipment/cancel.py

```diff
@@ -2,19 +2,22 @@
 from usps_lib.evs_cancel_request import eVSCancelRequest
 from usps_lib.evs_cancel_response import eVSCancelResponse
 from karrio.core.utils import Serializable, Element, XP
 from karrio.core.models import ShipmentCancelRequest, ConfirmationDetails, Message
 
 from karrio.providers.usps.error import parse_error_response
 from karrio.providers.usps.utils import Settings
+import karrio.lib as lib
 
 
 def parse_shipment_cancel_response(
-    response: Element, settings: Settings
+    _response: lib.Deserializable[Element],
+    settings: Settings,
 ) -> Tuple[ConfirmationDetails, List[Message]]:
+    response = _response.deserialize()
     errors: List[Message] = parse_error_response(response, settings)
     cancel_response = XP.to_object(eVSCancelResponse, response)
 
     if cancel_response.Status != "Cancelled":
         errors.append(
             Message(
                 carrier_name=settings.carrier_name,
@@ -37,13 +40,12 @@
 
     return details, errors
 
 
 def shipment_cancel_request(
     payload: ShipmentCancelRequest, settings: Settings
 ) -> Serializable:
-
     request = eVSCancelRequest(
         USERID=settings.username, BarcodeNumber=payload.shipment_identifier
     )
 
     return Serializable(request, XP.export)
```

## karrio/providers/usps/shipment/create.py

```diff
@@ -15,16 +15,17 @@
 import karrio.core.errors as errors
 import karrio.providers.usps.error as provider_error
 import karrio.providers.usps.units as provider_units
 import karrio.providers.usps.utils as provider_utils
 
 
 def parse_shipment_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element], settings: provider_utils.Settings
 ) -> typing.Tuple[models.ShipmentDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = provider_error.parse_error_response(response, settings)
     details = _extract_details(response, settings)
 
     return details, errors
 
 
 def _extract_details(
@@ -43,15 +44,15 @@
         ),
     )
 
 
 def shipment_request(
     payload: models.ShipmentRequest,
     settings: provider_utils.Settings,
-) -> lib.Serializable[eVSRequest]:
+) -> lib.Serializable:
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
 
     if (
         shipper.country_code is not None
         and shipper.country_code != units.Country.US.name
     ):
```

## Comparing `karrio.usps-2023.3.dist-info/METADATA` & `karrio.usps-2023.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.usps
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - USPS Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.usps-2023.3.dist-info/RECORD` & `karrio.usps-2023.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 karrio/mappers/usps/__init__.py,sha256=5l5gND_tZRff9K7lkcFTg9FxNE26wQMhm02K5Epd0MA,450
-karrio/mappers/usps/mapper.py,sha256=Mmx7-ppUBh0oUKcJ48SwtlP-4L64LL-xV08utBlo9e0,3612
-karrio/mappers/usps/proxy.py,sha256=2jWI2arnlNqnFk1XrRq4-8bY4pEhDRKuMXY7EbtE3lg,2007
-karrio/mappers/usps/settings.py,sha256=24bCABvVEMEmor2HKMPPTu6XePgNSeL417mWQ885aMw,550
+karrio/mappers/usps/mapper.py,sha256=IrpBySFltW77hA7A7G5k6FTaBjyfrHVH4tUiW2ksYg4,3442
+karrio/mappers/usps/proxy.py,sha256=OGlmf9TkRJ-7KZP3Liw7txDY2GHiam6_iFYJxA3hfp4,1969
+karrio/mappers/usps/settings.py,sha256=IXvSexRZBw6sxGWVplgOkbf5I0sQeQAgj8jRi918S4U,572
 karrio/providers/usps/__init__.py,sha256=llieveNGqPEAGRVVMUMKC40YCsgxwsb8_BGjgfEetFU,613
 karrio/providers/usps/error.py,sha256=awhVC-kiqCKWjHFEOeMq9JOuSzwuMqoAlZH3BcPqUYk,722
-karrio/providers/usps/rate.py,sha256=3i7rQek6EDLu-cvWZC1Cqh1webXSHEFMewfIhaACafw,6136
-karrio/providers/usps/tracking.py,sha256=aWEfhdzB47V-hjooiGkw94LlyxVeOqXquw6OuydUQAk,3384
+karrio/providers/usps/rate.py,sha256=wgr-ADcMh3t7hPwlXRaWR-uicn7P1V6d6axHMb6erxY,6216
+karrio/providers/usps/tracking.py,sha256=78k_j-sC51GDhD3jH3YKftrbmG_9HwWGxSjTHhEZvl8,3419
 karrio/providers/usps/units.py,sha256=KfbiaTZ_F4CFGYYdJdENUw2X8ZWkPB8odKIecX8nBHI,16295
-karrio/providers/usps/utils.py,sha256=IUyp3CEx_yTigyK_q4p2qEsKim-Mov18j9aIW8_ZEBY,712
+karrio/providers/usps/utils.py,sha256=EB5z8FZrk24So3s267pv2TeCtOeKB8zAqzOG4Ba9Ypc,734
 karrio/providers/usps/pickup/__init__.py,sha256=YTFtc6O-bbi1NhsYbug5vag4GmbmvXms88lGbSWeZ0E,286
-karrio/providers/usps/pickup/cancel.py,sha256=mn4Fun6axBT9c6mSB7ruddzhUTrMBEYDehjXxjRYjVY,1479
-karrio/providers/usps/pickup/create.py,sha256=2oyfJ99olFwsFJ-CXlNElmhyeU8JmTworzIixAo7NpU,1836
-karrio/providers/usps/pickup/update.py,sha256=3hHLXTrMu2PvvyowSV-CTl1xIxq9ylSGtefVHGdOibA,1918
+karrio/providers/usps/pickup/cancel.py,sha256=BBewXX3WNjO_aQIoY6h2O4H14cHApe3fsGzeOhBFkZg,1568
+karrio/providers/usps/pickup/create.py,sha256=MtoEZXmbJpPe3q5nZB8XkeFHwWYJa5ykpvMD7EaP67s,1926
+karrio/providers/usps/pickup/update.py,sha256=4xDQRQ36aWlgpu_TEIJp1D_6Zmi6Hznk6__APuD5bAw,2008
 karrio/providers/usps/shipment/__init__.py,sha256=ZGECAADplncp0tiq9F_mawDECcgZS_kOCVMIzVfTnKE,198
-karrio/providers/usps/shipment/cancel.py,sha256=emlLW-EPkHdUtMdS4ely4lJRfKdqfC1Ke7-euS2VtnM,1525
-karrio/providers/usps/shipment/create.py,sha256=6OkDhd-VDHaB1d-YM5YQUpoNJG2yMy7EzgFKMspaJMM,7653
-karrio.usps-2023.3.dist-info/METADATA,sha256=zt0IpqSbx9X7tSHhpnu4aX_8XOilJ1-L-nXiqpfcIsU,964
-karrio.usps-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.usps-2023.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.usps-2023.3.dist-info/RECORD,,
+karrio/providers/usps/shipment/cancel.py,sha256=Noo8-0R1sJIzLaGN1Dx6eF0qT_PDIbkQvisbgV7zbh0,1614
+karrio/providers/usps/shipment/create.py,sha256=toiPyAlVef0LAnBqnhmH2UEMsKUCceQLu3-uosQmSoM,7701
+karrio.usps-2023.4.dist-info/METADATA,sha256=rRhwuhmpls2ORGNrrTil977FC0tBxgp59jsiUazXq-E,964
+karrio.usps-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.usps-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.usps-2023.4.dist-info/RECORD,,
```

