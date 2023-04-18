# Comparing `tmp/karrio.chronopost-2023.3-py3-none-any.whl.zip` & `tmp/karrio.chronopost-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11478 bytes, number of entries: 17
+Zip file size: 11531 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      482 b- defN 22-Nov-15 19:21 karrio/mappers/chronopost/__init__.py
--rw-rw-r--  2.0 unx     2008 b- defN 22-Nov-15 19:21 karrio/mappers/chronopost/mapper.py
--rw-rw-r--  2.0 unx     1798 b- defN 22-Nov-15 19:21 karrio/mappers/chronopost/proxy.py
--rw-rw-r--  2.0 unx      516 b- defN 22-Nov-15 19:21 karrio/mappers/chronopost/settings.py
+-rw-rw-r--  2.0 unx     1910 b- defN 23-Apr-01 13:34 karrio/mappers/chronopost/mapper.py
+-rw-rw-r--  2.0 unx     1742 b- defN 23-Apr-01 13:39 karrio/mappers/chronopost/proxy.py
+-rw-rw-r--  2.0 unx      538 b- defN 23-Apr-15 06:44 karrio/mappers/chronopost/settings.py
 -rw-rw-r--  2.0 unx      407 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/__init__.py
 -rw-rw-r--  2.0 unx      678 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/error.py
--rw-rw-r--  2.0 unx     3009 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/rate.py
--rw-rw-r--  2.0 unx     2897 b- defN 23-Mar-25 12:55 karrio/providers/chronopost/tracking.py
+-rw-rw-r--  2.0 unx     3060 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/rate.py
+-rw-rw-r--  2.0 unx     2959 b- defN 23-Apr-01 15:19 karrio/providers/chronopost/tracking.py
 -rw-rw-r--  2.0 unx     1663 b- defN 23-Jan-11 18:22 karrio/providers/chronopost/units.py
--rw-rw-r--  2.0 unx      800 b- defN 23-Mar-25 12:45 karrio/providers/chronopost/utils.py
+-rw-rw-r--  2.0 unx      800 b- defN 23-Apr-15 02:55 karrio/providers/chronopost/utils.py
 -rw-rw-r--  2.0 unx      236 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/shipment/__init__.py
--rw-rw-r--  2.0 unx     1682 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/shipment/cancel.py
--rw-rw-r--  2.0 unx     8346 b- defN 23-Mar-25 14:28 karrio/providers/chronopost/shipment/create.py
--rw-rw-r--  2.0 unx     1013 b- defN 23-Mar-27 07:12 karrio.chronopost-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.chronopost-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.chronopost-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1580 b- defN 23-Mar-27 07:12 karrio.chronopost-2023.3.dist-info/RECORD
-17 files, 27214 bytes uncompressed, 8812 bytes compressed:  67.6%
+-rw-rw-r--  2.0 unx     1733 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/shipment/cancel.py
+-rw-rw-r--  2.0 unx     8560 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/shipment/create.py
+-rw-rw-r--  2.0 unx     1013 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1580 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/RECORD
+17 files, 27460 bytes uncompressed, 8865 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: karrio/providers/chronopost/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/chronopost/shipment/create.py
 Comment: 
 
-Filename: karrio.chronopost-2023.3.dist-info/METADATA
+Filename: karrio.chronopost-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.chronopost-2023.3.dist-info/WHEEL
+Filename: karrio.chronopost-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.chronopost-2023.3.dist-info/top_level.txt
+Filename: karrio.chronopost-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.chronopost-2023.3.dist-info/RECORD
+Filename: karrio.chronopost-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/chronopost/mapper.py

```diff
@@ -20,31 +20,29 @@
     def create_tracking_request(
         self, payload: models.TrackingRequest
     ) -> lib.Serializable:
         return provider.tracking_request(payload, self.settings)
 
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
-        return provider.parse_rate_response(response.deserialize(), self.settings)
+        return provider.parse_rate_response(response, self.settings)
 
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

## karrio/mappers/chronopost/proxy.py

```diff
@@ -21,27 +21,25 @@
     def get_rates(
         self,
         request: lib.Serializable,
     ) -> lib.Deserializable:
         response = self._send_request(request, path="/quickcost-cxf/QuickcostServiceWS")
         return lib.Deserializable(response, lib.to_element)
 
-    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def create_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = self._send_request(request, path="/shipping-cxf/ShippingServiceWS")
 
         return lib.Deserializable(response, lib.to_element)
 
-    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable[str]:
+    def cancel_shipment(self, request: lib.Serializable) -> lib.Deserializable:
         response = self._send_request(request, path="/tracking-cxf/TrackingServiceWS")
 
         return lib.Deserializable(response, lib.to_element)
 
-    def get_tracking(
-        self, request: lib.Serializable[typing.List[lib.Envelope]]
-    ) -> lib.Deserializable[str]:
+    def get_tracking(self, request: lib.Serializable) -> lib.Deserializable:
         def get_tracking(track_request: str):
             return self._send_request(
                 path="/tracking-cxf/TrackingServiceWS",
                 request=lib.Serializable(track_request),
             )
 
         response: typing.List[str] = lib.run_concurently(
```

## karrio/mappers/chronopost/settings.py

```diff
@@ -14,7 +14,8 @@
     language: str = "en_GB"
 
     id: str = None
     test_mode: bool = False
     carrier_id: str = "chronopost"
     account_country_code: str = "FR"
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/chronopost/rate.py

```diff
@@ -4,16 +4,18 @@
 import karrio.core.models as models
 import karrio.providers.chronopost.error as provider_error
 import karrio.providers.chronopost.units as provider_units
 import karrio.providers.chronopost.utils as provider_utils
 
 
 def parse_rate_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     product_nodes: typing.List[chronopost.product] = lib.find_element(
         "productList", response, chronopost.product
     )
     products: typing.List[models.RateDetails] = [
         _extract_service_details(product_node, settings)
         for product_node in product_nodes
         if product_node.amount > 0.0
@@ -44,15 +46,15 @@
         ],
         meta=dict(service_name=service.name_or_key),
     )
 
 
 def rate_request(
     payload: models.RateRequest, settings: provider_utils.Settings
-) -> lib.Serializable[lib.Envelope]:
+) -> lib.Serializable:
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
     package = lib.to_packages(payload.parcels).single
 
     request = lib.Envelope(
         Body=lib.Body(
             chronopost.calculateProducts(
```

## karrio/providers/chronopost/tracking.py

```diff
@@ -3,17 +3,18 @@
 import karrio.core.models as models
 import karrio.providers.chronopost.utils as provider_utils
 import karrio.providers.chronopost.error as provider_error
 import chronopost_lib.trackingservice as chronopost
 
 
 def parse_tracking_response(
-    responses: lib.Element,
+    _responses: lib.Deserializable[lib.Element],
     settings: provider_utils.Settings,
 ) -> typing.Tuple[typing.List[models.TrackingDetails], typing.List[models.Message]]:
+    responses = _responses.deserialize()
     tracking_nodes: typing.List[chronopost.listEventInfoComps] = lib.find_element(
         "listEventInfoComp", responses, chronopost.listEventInfoComps
     )
     errors = provider_error.parse_error_response(responses, settings)
     tracking_details: typing.List[models.TrackingDetails] = [
         _extract_details(tracking_node, settings) for tracking_node in tracking_nodes
     ]
```

## karrio/providers/chronopost/shipment/cancel.py

```diff
@@ -3,16 +3,18 @@
 import karrio.core.models as models
 import karrio.lib as lib
 import karrio.providers.chronopost.error as provider_error
 import karrio.providers.chronopost.utils as provider_utils
 
 
 def parse_shipment_cancel_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[models.ConfirmationDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = provider_error.parse_error_response(response, settings)
     success = len(errors) == 0
     confirmation: models.ConfirmationDetails = (
         models.ConfirmationDetails(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             success=success,
@@ -23,15 +25,15 @@
     )
 
     return confirmation, errors
 
 
 def shipment_cancel_request(
     payload: models.ShipmentCancelRequest, settings: provider_utils.Settings
-) -> lib.Serializable[lib.Envelope]:
+) -> lib.Serializable:
     request = lib.Envelope(
         Body=lib.Body(
             cancelSkybill(
                 accountNumber=settings.account_number,
                 password=settings.password,
                 language=settings.language,
                 skybillNumber=payload.shipment_identifier,
```

## karrio/providers/chronopost/shipment/create.py

```diff
@@ -6,16 +6,18 @@
 import karrio.core.models as models
 import karrio.providers.chronopost.error as provider_error
 import karrio.providers.chronopost.utils as provider_utils
 import karrio.providers.chronopost.units as provider_units
 
 
 def parse_shipment_response(
-    response: lib.Element, settings: provider_utils.Settings
+    _response: lib.Deserializable[lib.Element],
+    settings: provider_utils.Settings,
 ) -> typing.Tuple[models.ShipmentDetails, typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = provider_error.parse_error_response(response, settings)
     shipment_node = lib.find_element("resultMultiParcelValue", response, first=True)
     shipment = (
         _extract_details(shipment_node, settings) if shipment_node is not None else None
     )
 
     return shipment, errors
@@ -37,15 +39,15 @@
             carrier_tracking_link=settings.tracking_url.format(shipment.skybillNumber),
         ),
     )
 
 
 def shipment_request(
     payload: models.ShipmentRequest, settings: provider_utils.Settings
-) -> lib.Serializable[str]:
+) -> lib.Serializable:
     package = lib.to_packages(
         payload.parcels,
         required=["weight"],
         package_option_type=provider_units.ShippingOption,
     ).single
     shipper = lib.to_address(payload.shipper)
     recipient = lib.to_address(payload.recipient)
@@ -62,15 +64,17 @@
     request = lib.Envelope(
         Body=lib.Body(
             chronopost.shippingMultiParcelV5(
                 esdValue=None,
                 headerValue=settings.header_value,
                 shipperValue=(
                     chronopost.shipperValue(
-                        shipperAdress1=lib.text(shipper.street_number, shipper.address_line1),
+                        shipperAdress1=lib.text(
+                            shipper.street_number, shipper.address_line1
+                        ),
                         shipperAdress2=shipper.address_line2,
                         shipperCity=shipper.city,
                         shipperContactName=shipper.person_name,
                         shipperCountry=shipper.country_code,
                         shipperCountryName=shipper.country_name,
                         shipperEmail=shipper.email,
                         shipperMobilePhone=shipper.phone_number,
@@ -78,15 +82,17 @@
                         shipperName2=shipper.company_name,
                         shipperPreAlert=0,
                         shipperCivility="M",
                         shipperZipCode=shipper.postal_code,
                     ),
                 ),
                 customerValue=chronopost.customerValue(
-                    customerAdress1=lib.text(recipient.street_number, recipient.address_line1),
+                    customerAdress1=lib.text(
+                        recipient.street_number, recipient.address_line1
+                    ),
                     customerAdress2=recipient.address_line2,
                     customerCity=recipient.city,
                     customerContactName=recipient.person_name,
                     customerCountry=recipient.country_code,
                     customerCountryName=recipient.country_name,
                     customerEmail=recipient.email,
                     customerMobilePhone=recipient.phone_number,
@@ -95,15 +101,17 @@
                     customerPreAlert=0,
                     customerZipCode=recipient.postal_code,
                     printAsSender=None,
                     customerCivility="M",
                 ),
                 recipientValue=(
                     chronopost.recipientValue(
-                        recipientAdress1=lib.text(recipient.street_number, recipient.address_line1),
+                        recipientAdress1=lib.text(
+                            recipient.street_number, recipient.address_line1
+                        ),
                         recipientAdress2=recipient.address_line2,
                         recipientCity=recipient.city,
                         recipientContactName=recipient.person_name,
                         recipientCountry=recipient.country_code,
                         recipientCountryName=recipient.country_name,
                         recipientEmail=recipient.email,
                         recipientMobilePhone=recipient.phone_number,
```

## Comparing `karrio.chronopost-2023.3.dist-info/METADATA` & `karrio.chronopost-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.chronopost
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - Chronopost Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.chronopost-2023.3.dist-info/RECORD` & `karrio.chronopost-2023.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 karrio/mappers/chronopost/__init__.py,sha256=noOnutw_jXMzpo6uYVxBOjLyn9YpUz5UrNUp7tF4IP0,482
-karrio/mappers/chronopost/mapper.py,sha256=HS3aAJS0d3lAKmCBTjKJ_EBVmTsR1jEyXNVO1Xa2S8U,2008
-karrio/mappers/chronopost/proxy.py,sha256=WCE3t0aE_Q66aZ3fW3u7p3RRRUC12zczFP0pzvA9vsc,1798
-karrio/mappers/chronopost/settings.py,sha256=hyUrN2gVMS0VpJ54pH3lpfjCMLjofgjoUAW-F4D2ZVg,516
+karrio/mappers/chronopost/mapper.py,sha256=Av-ojaa5-AZppDQ91Ia8PpUBa4ieAKgeCehnASkrxh4,1910
+karrio/mappers/chronopost/proxy.py,sha256=xJ7Qtt4pDszqZtgwNfoSJZjZMF-4AepAxF1n_l-cYrc,1742
+karrio/mappers/chronopost/settings.py,sha256=2QwAx9haMHOX1GUUvX458L9U16V6o5f3ZdfShFvU_pQ,538
 karrio/providers/chronopost/__init__.py,sha256=b7-FY6tNu805ak4GR52E3ri9D7tofMZdo0MWi4cm1Lc,407
 karrio/providers/chronopost/error.py,sha256=5Kt8vVCN0fj0Add9tCii66fBfr3dWTCJ0DVaOMxf_D0,678
-karrio/providers/chronopost/rate.py,sha256=P_kp6_u3ZhHz0NGPvblUL4b9MrZ0F2OWvL10mdibW-s,3009
-karrio/providers/chronopost/tracking.py,sha256=kUqoBsNOJHs6rGgOwUZs2BHXNM4U5oXaCylQXFE7UNc,2897
+karrio/providers/chronopost/rate.py,sha256=UxmtY5CW65abZYQP4KErhG0eeNE4EZHNf3XbNLANNGQ,3060
+karrio/providers/chronopost/tracking.py,sha256=atAPqxxIDsFL45oW2P7BGAflLE_9HQabn6DFE_6sO68,2959
 karrio/providers/chronopost/units.py,sha256=jZVxZgO_1N2w3inhf5_GRoGJ-UHvPL2DKC2LSyGlxyc,1663
 karrio/providers/chronopost/utils.py,sha256=U8a36xPS4zNIAWWeJMxE2S9zoJ8oxnGEWR3UF1s3olE,800
 karrio/providers/chronopost/shipment/__init__.py,sha256=Qps1uXAaxVmDCPV54GVgnGfzqy51KZlDBBiSt5Z4QqY,236
-karrio/providers/chronopost/shipment/cancel.py,sha256=aqV3uWNZjsgeIIrV2EhplDI2EaS8T2C53taGZePtkT0,1682
-karrio/providers/chronopost/shipment/create.py,sha256=I8zlqVlCikMkd3lgPnngm4WXCaEbIX0WBVuwGo0zTtE,8346
-karrio.chronopost-2023.3.dist-info/METADATA,sha256=Svo3tjOBXAP3MwoTfLs0Fdp0GgtR2P8UUoYYXXD5p40,1013
-karrio.chronopost-2023.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.chronopost-2023.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.chronopost-2023.3.dist-info/RECORD,,
+karrio/providers/chronopost/shipment/cancel.py,sha256=IZ4hHC3piisGhdxZRxvZh_7pBfzNDNA3H9Fn52S2EsE,1733
+karrio/providers/chronopost/shipment/create.py,sha256=bcIHVEUjnMbVyyOuPZXdi8dcJyYJb7RJgcJqhqDtnLI,8560
+karrio.chronopost-2023.4.dist-info/METADATA,sha256=us-nnx6xm2pMhE_Gtd6-SyohyZpvsLG72eUMOpsZKak,1013
+karrio.chronopost-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.chronopost-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.chronopost-2023.4.dist-info/RECORD,,
```

