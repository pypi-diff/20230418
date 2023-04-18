# Comparing `tmp/karrio.dpd-2023.3.1-py3-none-any.whl.zip` & `tmp/karrio.dpd-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13254 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      392 b- defN 23-Mar-21 13:06 karrio/mappers/dpd/__init__.py
--rw-rw-r--  2.0 unx     1655 b- defN 23-Mar-21 13:06 karrio/mappers/dpd/mapper.py
--rw-rw-r--  2.0 unx     1863 b- defN 23-Mar-21 13:06 karrio/mappers/dpd/proxy.py
--rw-rw-r--  2.0 unx     1248 b- defN 23-Mar-21 13:06 karrio/mappers/dpd/settings.py
--rw-rw-r--  2.0 unx      242 b- defN 23-Mar-21 13:06 karrio/providers/dpd/__init__.py
--rw-rw-r--  2.0 unx     1037 b- defN 23-Mar-21 13:06 karrio/providers/dpd/error.py
--rw-rw-r--  2.0 unx     4178 b- defN 23-Mar-25 13:21 karrio/providers/dpd/tracking.py
--rw-rw-r--  2.0 unx     7720 b- defN 23-Mar-21 13:06 karrio/providers/dpd/units.py
--rw-rw-r--  2.0 unx     3990 b- defN 23-Mar-25 13:21 karrio/providers/dpd/utils.py
--rw-rw-r--  2.0 unx      104 b- defN 23-Mar-21 13:06 karrio/providers/dpd/shipment/__init__.py
--rw-rw-r--  2.0 unx    21942 b- defN 23-Mar-25 13:17 karrio/providers/dpd/shipment/create.py
--rw-rw-r--  2.0 unx      952 b- defN 23-Mar-27 07:31 karrio.dpd-2023.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:31 karrio.dpd-2023.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:31 karrio.dpd-2023.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1291 b- defN 23-Mar-27 07:31 karrio.dpd-2023.3.1.dist-info/RECORD
-15 files, 46713 bytes uncompressed, 11096 bytes compressed:  76.2%
+Zip file size: 13293 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      462 b- defN 23-Mar-30 19:14 karrio/mappers/dpd/__init__.py
+-rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-01 12:45 karrio/mappers/dpd/mapper.py
+-rw-rw-r--  2.0 unx     1855 b- defN 23-Apr-01 12:45 karrio/mappers/dpd/proxy.py
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Apr-15 06:44 karrio/mappers/dpd/settings.py
+-rw-rw-r--  2.0 unx      242 b- defN 23-Mar-27 07:55 karrio/providers/dpd/__init__.py
+-rw-rw-r--  2.0 unx     1037 b- defN 23-Mar-27 07:55 karrio/providers/dpd/error.py
+-rw-rw-r--  2.0 unx     4241 b- defN 23-Apr-01 15:19 karrio/providers/dpd/tracking.py
+-rw-rw-r--  2.0 unx     7720 b- defN 23-Mar-27 07:55 karrio/providers/dpd/units.py
+-rw-rw-r--  2.0 unx     3990 b- defN 23-Mar-27 07:55 karrio/providers/dpd/utils.py
+-rw-rw-r--  2.0 unx      104 b- defN 23-Mar-27 07:55 karrio/providers/dpd/shipment/__init__.py
+-rw-rw-r--  2.0 unx    22002 b- defN 23-Apr-01 15:18 karrio/providers/dpd/shipment/create.py
+-rw-rw-r--  2.0 unx      950 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1283 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/RECORD
+15 files, 46831 bytes uncompressed, 11151 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: karrio/providers/dpd/shipment/__init__.py
 Comment: 
 
 Filename: karrio/providers/dpd/shipment/create.py
 Comment: 
 
-Filename: karrio.dpd-2023.3.1.dist-info/METADATA
+Filename: karrio.dpd-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpd-2023.3.1.dist-info/WHEEL
+Filename: karrio.dpd-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpd-2023.3.1.dist-info/top_level.txt
+Filename: karrio.dpd-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpd-2023.3.1.dist-info/RECORD
+Filename: karrio.dpd-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dpd/__init__.py

```diff
@@ -11,8 +11,10 @@
     label="DPD",
     # Integrations
     Mapper=Mapper,
     Proxy=Proxy,
     Settings=Settings,
     # Data Units
     is_hub=False,
+    services=units.ShippingService,
+    options=units.ShippingOption,
 )
```

## karrio/mappers/dpd/mapper.py

```diff
@@ -22,22 +22,20 @@
 
     def create_shipment_request(
         self, payload: models.ShipmentRequest
     ) -> lib.Serializable:
         return provider.shipment_request(payload, self.settings)
 
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

## karrio/mappers/dpd/proxy.py

```diff
@@ -8,39 +8,39 @@
 
 class Proxy(rating_proxy.RatingMixinProxy, proxy.Proxy):
     settings: provider_settings.Settings
 
     def get_rates(self, request: lib.Serializable) -> lib.Deserializable:
         return super().get_rates(request)
 
-    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = lib.request(
             url=f"{self.settings.server_url}/soap/services/ShipmentService/V3_3",
             data=request.serialize(),
             trace=self.trace_as("xml"),
             method="POST",
             headers={
                 "Content-Type": "text/xml;charset=UTF-8",
-                "SOAPAction": "http://dpd.com/common/service/types/ShipmentService/3.3/storeOrders"
+                "SOAPAction": "http://dpd.com/common/service/types/ShipmentService/3.3/storeOrders",
             },
         )
 
         return lib.Deserializable(response, lib.to_element)
 
-    def get_tracking(self, requests: lib.Serializable) -> lib.Deserializable[str]:
+    def get_tracking(self, requests: lib.Serializable) -> lib.Deserializable:
         def _track(payload):
             tracking_number, data = payload
             return tracking_number, lib.request(
                 url=f"{self.settings.server_url}/soap/services/ParcelLifeCycleService/V2_0",
                 trace=self.trace_as("xml"),
                 method="POST",
                 data=data,
                 headers={
                     "Content-Type": "text/xml;charset=UTF-8",
-                    "SOAPAction": "http://dpd.com/common/service/types/ParcelLifeCycleService/2.0/getTrackingData"
+                    "SOAPAction": "http://dpd.com/common/service/types/ParcelLifeCycleService/2.0/getTrackingData",
                 },
             )
 
         responses = lib.run_concurently(_track, requests.serialize().items())
 
         return lib.Deserializable(
             responses,
```

## karrio/mappers/dpd/settings.py

```diff
@@ -22,16 +22,17 @@
 
     # generic properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dpd"
     account_country_code: str = "BE"
     services: typing.List[models.ServiceLevel] = jstruct.JList[models.ServiceLevel, False, dict(default=provider_units.DEFAULT_SERVICES)]  # type: ignore
-    metadata: dict = {}
     cache: lib.Cache = jstruct.JStruct[lib.Cache]
+    metadata: dict = {}
+    config: dict = {}
 
     @property
     def shipping_services(self) -> typing.List[models.ServiceLevel]:
         if any(self.services or []):
             return self.services
 
         if self.account_country_code == "NL":
```

## karrio/providers/dpd/tracking.py

```diff
@@ -5,17 +5,18 @@
 import karrio.core.models as models
 import karrio.providers.dpd.error as error
 import karrio.providers.dpd.utils as provider_utils
 import karrio.providers.dpd.units as provider_units
 
 
 def parse_tracking_response(
-    responses: typing.List[typing.Tuple[str, lib.Element]],
+    _responses: lib.Deserializable[typing.List[typing.Tuple[str, lib.Element]]],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    responses = _responses.deserialize()
     response_messages = []
     response_details = []
 
     for response in responses:
         results: list = lib.find_element("trackingresult", response[1])
 
         if len(results) > 0:
@@ -77,15 +78,15 @@
             )
             for event in events
         ],
         delivered=delivered,
         status=status,
         info=models.TrackingInfo(
             carrier_tracking_link=settings.tracking_url.format(tracking_number),
-        )
+        ),
     )
 
 
 def tracking_request(
     payload: models.TrackingRequest,
     settings: provider_utils.Settings,
 ) -> lib.Serializable:
```

## karrio/providers/dpd/shipment/create.py

```diff
@@ -6,17 +6,18 @@
 import karrio.core.models as models
 import karrio.providers.dpd.error as error
 import karrio.providers.dpd.utils as provider_utils
 import karrio.providers.dpd.units as provider_units
 
 
 def parse_shipment_response(
-    response: lib.Element,
+    _response: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     response_shipment = lib.find_element("shipmentResponses", response)
 
     messages = error.parse_error_response(response, settings)
     shipment = (
         _extract_details(response, settings) if len(response_shipment) > 0 else None
     )
```

## Comparing `karrio.dpd-2023.3.1.dist-info/METADATA` & `karrio.dpd-2023.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpd
-Version: 2023.3.1
+Version: 2023.4
 Summary: Karrio - DPD Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

