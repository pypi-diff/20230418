# Comparing `tmp/karrio.dpdhl-2023.3.4-py3-none-any.whl.zip` & `tmp/karrio.dpdhl-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14132 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      511 b- defN 22-Nov-15 19:21 karrio/mappers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     2150 b- defN 22-Nov-15 19:21 karrio/mappers/dpdhl/mapper.py
--rw-rw-r--  2.0 unx     2319 b- defN 23-Mar-29 11:28 karrio/mappers/dpdhl/proxy.py
--rw-rw-r--  2.0 unx     1029 b- defN 23-Mar-18 11:05 karrio/mappers/dpdhl/settings.py
+Zip file size: 14351 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      558 b- defN 23-Apr-15 11:02 karrio/mappers/dpdhl/__init__.py
+-rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-01 13:34 karrio/mappers/dpdhl/mapper.py
+-rw-rw-r--  2.0 unx     2304 b- defN 23-Apr-01 12:45 karrio/mappers/dpdhl/proxy.py
+-rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-15 11:01 karrio/mappers/dpdhl/settings.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     3115 b- defN 23-Mar-29 11:28 karrio/providers/dpdhl/error.py
--rw-rw-r--  2.0 unx     3491 b- defN 23-Mar-29 11:21 karrio/providers/dpdhl/tracking.py
--rw-rw-r--  2.0 unx     7452 b- defN 23-Mar-27 07:55 karrio/providers/dpdhl/units.py
--rw-rw-r--  2.0 unx     1296 b- defN 23-Mar-27 07:55 karrio/providers/dpdhl/utils.py
+-rw-rw-r--  2.0 unx     3115 b- defN 23-Mar-29 20:04 karrio/providers/dpdhl/error.py
+-rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-10 06:24 karrio/providers/dpdhl/tracking.py
+-rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-15 11:00 karrio/providers/dpdhl/units.py
+-rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-15 11:02 karrio/providers/dpdhl/utils.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/shipment/__init__.py
--rw-rw-r--  2.0 unx     2366 b- defN 23-Mar-18 11:05 karrio/providers/dpdhl/shipment/cancel.py
--rw-rw-r--  2.0 unx    19499 b- defN 23-Mar-27 07:55 karrio/providers/dpdhl/shipment/create.py
--rw-rw-r--  2.0 unx      994 b- defN 23-Mar-29 13:35 karrio.dpdhl-2023.3.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-29 13:35 karrio.dpdhl-2023.3.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-29 13:35 karrio.dpdhl-2023.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 23-Mar-29 13:35 karrio.dpdhl-2023.3.4.dist-info/RECORD
-16 files, 46279 bytes uncompressed, 11756 bytes compressed:  74.6%
+-rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-01 15:18 karrio/providers/dpdhl/shipment/cancel.py
+-rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-01 15:18 karrio/providers/dpdhl/shipment/create.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1411 b- defN 23-Apr-18 07:09 karrio.dpdhl-2023.4.dist-info/RECORD
+16 files, 47064 bytes uncompressed, 11991 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dpdhl/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dpdhl/shipment/create.py
 Comment: 
 
-Filename: karrio.dpdhl-2023.3.4.dist-info/METADATA
+Filename: karrio.dpdhl-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpdhl-2023.3.4.dist-info/WHEEL
+Filename: karrio.dpdhl-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpdhl-2023.3.4.dist-info/top_level.txt
+Filename: karrio.dpdhl-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpdhl-2023.3.4.dist-info/RECORD
+Filename: karrio.dpdhl-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dpdhl/__init__.py

```diff
@@ -13,8 +13,9 @@
     Mapper=Mapper,
     Proxy=Proxy,
     Settings=Settings,
     # Data Units
     services=units.ShippingService,
     options=units.ShippingOption,
     service_levels=units.DEFAULT_SERVICES,
+    connection_configs=units.ConnectionConfig,
 )
```

## karrio/mappers/dpdhl/mapper.py

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

## karrio/mappers/dpdhl/proxy.py

```diff
@@ -11,45 +11,45 @@
 
 class Proxy(rating_proxy.RatingMixinProxy, proxy.Proxy):
     settings: provider_settings.Settings
 
     def get_rates(self, request: lib.Serializable) -> lib.Deserializable:
         return super().get_rates(request)
 
-    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = lib.request(
             url=f"{self.settings.server_url}/soap",
             data=request.serialize(),
             trace=self.trace_as("xml"),
             method="POST",
             headers={
                 "Authorization": f"Basic {self.settings.basic_authentication}",
                 "SOAPAction": "urn:createShipmentOrder",
             },
             decoder=decoder,
         )
 
         return lib.Deserializable(response, to_element)
 
-    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = lib.request(
             url=f"{self.settings.server_url}/soap",
             data=request.serialize(),
             trace=self.trace_as("xml"),
             method="POST",
             headers={
                 "Authorization": f"Basic {self.settings.basic_authentication}",
                 "SOAPAction": "urn:deleteShipmentOrder",
             },
             decoder=decoder,
         )
 
         return lib.Deserializable(response, to_element)
 
-    def get_tracking(self, requests: lib.Serializable) -> lib.Deserializable[str]:
+    def get_tracking(self, requests: lib.Serializable) -> lib.Deserializable:
         def _track(data):
             return lib.request(
                 url=f"{self.settings.server_url}/rest/sendungsverfolgung",
                 trace=self.trace_as("xml"),
                 method="POST",
                 data=data,
                 headers={
```

## karrio/mappers/dpdhl/settings.py

```diff
@@ -17,17 +17,17 @@
     username: str  # type:ignore
     password: str  # type:ignore
     app_id: str = ""
     app_token: str = ""
     zt_id: str = ""
     zt_password: str = ""
     account_number: str = None
-    language_code: str = "en"
 
     # generic properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dpdhl"
     account_country_code: str = "DE"
     metadata: dict = {}
+    config: dict = {}
 
     services: typing.List[models.ServiceLevel] = jstruct.JList[models.ServiceLevel, False, dict(default=provider_units.DEFAULT_SERVICES)]  # type: ignore
```

## karrio/providers/dpdhl/tracking.py

```diff
@@ -5,17 +5,18 @@
 import karrio.core.models as models
 import karrio.providers.dpdhl.error as error
 import karrio.providers.dpdhl.utils as provider_utils
 import karrio.providers.dpdhl.units as provider_units
 
 
 def parse_tracking_response(
-    responses: typing.List[lib.Element],
+    _responses: lib.Deserializable[typing.List[lib.Element]],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    responses = _responses.deserialize()
     response_messages = [
         result
         for result in responses
         if result.get("code") != "0" or result.get("body") is not None
     ]
     response_details = [
         result[0]
@@ -72,15 +73,15 @@
         delivered=delivered,
         estimated_delivery=lib.fdate(details.delivery_date),
         info=models.TrackingInfo(
             carrier_tracking_link=settings.tracking_url.format(
                 details.piece_identifier
             ),
             customer_name=details.pan_recipient_name,
-            shipment_destication_country=details.dest_country,
+            shipment_destination_country=details.dest_country,
             shipment_destination_postal_code=details.pan_recipient_postalcode,
             shipment_origin_country=details.origin_country,
             shipment_service=details.product_name,
         ),
     )
 
 
@@ -96,9 +97,13 @@
             language_code=settings.language_code,
             piece_code=tracking_number,
         )
         for tracking_number in payload.tracking_numbers
     ]
 
     return lib.Serializable(
-        request, lambda requests: [lib.to_xml(req) for req in requests]
+        request,
+        lambda requests: [
+            f'<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n{lib.to_xml(req)}'
+            for req in requests
+        ],
     )
```

## karrio/providers/dpdhl/units.py

```diff
@@ -63,14 +63,20 @@
     DES = "Delivered Ex Ship"
     EXW = "Ex Works"
     FAS = "Free Alongside Ship"
     FCA = "Free Carrier"
     FOB = "Free On Board"
 
 
+class ConnectionConfig(lib.Enum):
+    language_code = lib.OptionEnum("language_code")
+    shipping_options = lib.OptionEnum("shipping_options", list)
+    shipping_services = lib.OptionEnum("shipping_services", list)
+
+
 class ShippingService(lib.Enum):
     """Carrier specific services"""
 
     dpdhl_paket = "V01PAK"
     dpdhl_paket_international = "V53WPAK"
     dpdhl_europaket = "V54EPAK"
     dpdhl_paket_connect = "V55PAK"
```

## karrio/providers/dpdhl/utils.py

```diff
@@ -16,33 +16,49 @@
     username: str  # type:ignore
     password: str  # type:ignore
     app_id: str = None
     app_token: str = None
     zt_id: str = None
     zt_password: str = None
     account_number: str = None
-    language_code: str = "en"
 
     @property
     def carrier_name(self):
         return "dpdhl"
 
     @property
     def server_url(self):
         return (
             "https://cig.dhl.de/services/sandbox"
             if self.test_mode
             else "https://cig.dhl.de/services/production"
         )
 
     @property
+    def tracking_url(self):
+        return (
+            "https://www.dhl.de/"
+            + self.language_code
+            + "/privatkunden/pakete-empfangen/verfolgen.html?piececode={}"
+        )
+
+    @property
+    def connection_config(self) -> lib.units.Options:
+        from karrio.providers.dpdhl.units import ConnectionConfig
+
+        return lib.to_connection_config(
+            self.config or {},
+            option_type=ConnectionConfig,
+        )
+
+    @property
+    def language_code(self):
+        return self.connection_config.language_code.state or "en"
+
+    @property
     def basic_authentication(self):
         pair = "%s:%s" % (
             (self.username, self.password)
-            if self.test_mode else
-            (self.app_id, self.app_token)
+            if self.test_mode
+            else (self.app_id, self.app_token)
         )
         return base64.b64encode(pair.encode("utf-8")).decode("ascii")
-
-    @property
-    def tracking_url(self):
-        return "https://www.dhl.de/" + self.language_code + "/privatkunden/pakete-empfangen/verfolgen.html?piececode={}"
```

## karrio/providers/dpdhl/shipment/cancel.py

```diff
@@ -4,17 +4,18 @@
 import karrio.core.models as models
 import karrio.providers.dpdhl.error as error
 import karrio.providers.dpdhl.utils as provider_utils
 import karrio.providers.dpdhl.units as provider_units
 
 
 def parse_shipment_cancel_response(
-    response: lib.Element,
+    _response: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[models.ConfirmationDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     messages = error.parse_error_response(response, settings)
     deletion: dpdhl.DeletionState = lib.find_element(
         "DeletionState",
         response,
         dpdhl.DeletionState,
         first=True,
     )
@@ -34,15 +35,14 @@
     return confirmation, messages
 
 
 def shipment_cancel_request(
     payload: models.ShipmentCancelRequest,
     settings: provider_utils.Settings,
 ) -> lib.Serializable:
-
     request = lib.Envelope(
         Header=lib.Header(
             provider_utils.AuthentificationType(
                 user=("2222222222_01" if settings.test_mode else settings.username),
                 signature=("pass" if settings.test_mode else settings.password),
             ),
         ),
```

## karrio/providers/dpdhl/shipment/create.py

```diff
@@ -6,17 +6,18 @@
 import karrio.core.models as models
 import karrio.providers.dpdhl.error as error
 import karrio.providers.dpdhl.utils as provider_utils
 import karrio.providers.dpdhl.units as provider_units
 
 
 def parse_shipment_response(
-    response: lib.Element,
+    _response: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     response_shipment: typing.Optional[dpdhl.CreationState] = lib.find_element(
         "CreationState",
         response,
         dpdhl.CreationState,
         first=True,
     )
```

## Comparing `karrio.dpdhl-2023.3.4.dist-info/METADATA` & `karrio.dpdhl-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpdhl
-Version: 2023.3.4
+Version: 2023.4
 Summary: Karrio - Deutsche Post DHL Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpdhl-2023.3.4.dist-info/RECORD` & `karrio.dpdhl-2023.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-karrio/mappers/dpdhl/__init__.py,sha256=ay6jioD5dFNL71KJPi8CHbYc1oMwXqxvv0jsd8GDZUw,511
-karrio/mappers/dpdhl/mapper.py,sha256=3Qz8S7RKcDxR65BaB8x6nQzyUbEl6ZB4KEhD9UUhjeQ,2150
-karrio/mappers/dpdhl/proxy.py,sha256=AudbuEq80XhnfB38a8tqaNIdpP-olaXRPIGMCybSbA8,2319
-karrio/mappers/dpdhl/settings.py,sha256=GCABQihpGdVj0IpLhRvOPTFCIYXqMUPejcOlHCz60qA,1029
+karrio/mappers/dpdhl/__init__.py,sha256=hI9K0SVajo90niTvmU5BP9iV2QoOFh8tEbtZfVRax_c,558
+karrio/mappers/dpdhl/mapper.py,sha256=PX1mAMSFl8JmtAQ-SaKr8xDrV0eybOXzNLJbrUGKLfM,2030
+karrio/mappers/dpdhl/proxy.py,sha256=vb326Ib_UphV7npB_YfNis1vr-0tt1gv4o1Efao3nCo,2304
+karrio/mappers/dpdhl/settings.py,sha256=nRq7QoFa8Amrg1glJy_UmZ9fQUxuseC8KNKPltbifm0,1021
 karrio/providers/dpdhl/__init__.py,sha256=XtaZQrNssm_oho6v6SAYEH3cViuOZ3VFAPhHgW6f-yw,313
 karrio/providers/dpdhl/error.py,sha256=VoSZ2pyx3nUudmqX3L0nIMQ2yOVlvfr_GJ8DrlczDj4,3115
-karrio/providers/dpdhl/tracking.py,sha256=kXhvZZJoabNdOedRB5gBKNHFwxaemrgtzg0aZX6Nmbw,3491
-karrio/providers/dpdhl/units.py,sha256=WOwVrXmg0U2Q6KhbMpyePVwGT0c1QTLvw2lotxMQHuQ,7452
-karrio/providers/dpdhl/utils.py,sha256=BQQ6fiXmaiQcGIXYq-5VRT1D4T1AK1zZGDtTQ6fkxJQ,1296
+karrio/providers/dpdhl/tracking.py,sha256=Qn2luGRnyIlJkaa2JSRjlawLVq-jMnAkfFGRcJFugqc,3657
+karrio/providers/dpdhl/units.py,sha256=DDQX6MIFiYqMXl6exNkXfRbolbRD2czyMqeAcvMSk1w,7670
+karrio/providers/dpdhl/utils.py,sha256=Hdf1-fC0uK3SlNJlVb5ZlHshn2nC6hH61wO-EFvvCws,1684
 karrio/providers/dpdhl/shipment/__init__.py,sha256=5tF7dih8kTSVa5pw4UXU8_byCMnuvtsJIz_h7VAOOyY,226
-karrio/providers/dpdhl/shipment/cancel.py,sha256=bsb8Y7FrkSXgARZ34W6K_azxzag8_VeY7M4cuL5Y0aw,2366
-karrio/providers/dpdhl/shipment/create.py,sha256=wQARmWkMC9lUYODn9k9zVOqJ50UinJLHQEURMPUb51Q,19499
-karrio.dpdhl-2023.3.4.dist-info/METADATA,sha256=ZZV81xBAXawB_STngkw209YjfgHIFK0fmCYT0np9H-w,994
-karrio.dpdhl-2023.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpdhl-2023.3.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpdhl-2023.3.4.dist-info/RECORD,,
+karrio/providers/dpdhl/shipment/cancel.py,sha256=1Z_h5EUUNLS7LAiLLU04dkEPufmXSJGavvn543FGxQE,2425
+karrio/providers/dpdhl/shipment/create.py,sha256=AKmTE_tcKX3n7wStuyFZGJXU5H8J40WgqZqLVSV96gg,19559
+karrio.dpdhl-2023.4.dist-info/METADATA,sha256=UntfvEJxvKqL1raSR0Jn_hSSprXZ1rrAgv1AhXTxN24,992
+karrio.dpdhl-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpdhl-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpdhl-2023.4.dist-info/RECORD,,
```

