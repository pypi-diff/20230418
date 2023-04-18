# Comparing `tmp/karrio.dicom-2023.3-py3-none-any.whl.zip` & `tmp/karrio.dicom-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 14474 bytes, number of entries: 21
+Zip file size: 14649 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      343 b- defN 22-Nov-15 19:21 karrio/mappers/dicom/__init__.py
--rw-rw-r--  2.0 unx     3718 b- defN 22-Nov-15 19:21 karrio/mappers/dicom/mapper.py
+-rw-rw-r--  2.0 unx     3568 b- defN 23-Apr-01 13:34 karrio/mappers/dicom/mapper.py
 -rw-rw-r--  2.0 unx      978 b- defN 22-Nov-15 19:21 karrio/mappers/dicom/proxy.py
--rw-rw-r--  2.0 unx      475 b- defN 22-Nov-15 19:21 karrio/mappers/dicom/settings.py
+-rw-rw-r--  2.0 unx      497 b- defN 23-Apr-15 06:44 karrio/mappers/dicom/settings.py
 -rw-rw-r--  2.0 unx      634 b- defN 22-Nov-15 19:21 karrio/providers/dicom/__init__.py
 -rw-rw-r--  2.0 unx      576 b- defN 22-Nov-15 19:21 karrio/providers/dicom/error.py
--rw-rw-r--  2.0 unx     4106 b- defN 22-Nov-15 19:21 karrio/providers/dicom/rate.py
--rw-rw-r--  2.0 unx     1465 b- defN 22-Nov-15 19:21 karrio/providers/dicom/tracking.py
+-rw-rw-r--  2.0 unx     4148 b- defN 23-Apr-01 15:18 karrio/providers/dicom/rate.py
+-rw-rw-r--  2.0 unx     1560 b- defN 23-Apr-01 15:18 karrio/providers/dicom/tracking.py
 -rw-rw-r--  2.0 unx     5278 b- defN 23-Jan-11 18:22 karrio/providers/dicom/units.py
--rw-rw-r--  2.0 unx      797 b- defN 22-Nov-15 19:21 karrio/providers/dicom/utils.py
+-rw-rw-r--  2.0 unx      797 b- defN 23-Apr-15 02:55 karrio/providers/dicom/utils.py
 -rw-rw-r--  2.0 unx      289 b- defN 22-Nov-15 19:21 karrio/providers/dicom/pickup/__init__.py
--rw-rw-r--  2.0 unx      891 b- defN 22-Nov-15 19:21 karrio/providers/dicom/pickup/cancel.py
--rw-rw-r--  2.0 unx     3311 b- defN 23-Mar-25 14:33 karrio/providers/dicom/pickup/create.py
--rw-rw-r--  2.0 unx     1805 b- defN 22-Nov-15 19:21 karrio/providers/dicom/pickup/update.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Apr-01 15:18 karrio/providers/dicom/pickup/cancel.py
+-rw-rw-r--  2.0 unx     3393 b- defN 23-Apr-01 15:18 karrio/providers/dicom/pickup/create.py
+-rw-rw-r--  2.0 unx     1898 b- defN 23-Apr-01 15:18 karrio/providers/dicom/pickup/update.py
 -rw-rw-r--  2.0 unx      200 b- defN 22-Nov-15 19:21 karrio/providers/dicom/shipment/__init__.py
--rw-rw-r--  2.0 unx      902 b- defN 22-Nov-15 19:21 karrio/providers/dicom/shipment/cancel.py
--rw-rw-r--  2.0 unx     6896 b- defN 23-Mar-25 14:35 karrio/providers/dicom/shipment/create.py
--rw-rw-r--  2.0 unx      972 b- defN 23-Mar-27 07:12 karrio.dicom-2023.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-27 07:12 karrio.dicom-2023.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-27 07:12 karrio.dicom-2023.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1876 b- defN 23-Mar-27 07:12 karrio.dicom-2023.3.dist-info/RECORD
-21 files, 35611 bytes uncompressed, 11358 bytes compressed:  68.1%
+-rw-rw-r--  2.0 unx      964 b- defN 23-Apr-01 16:33 karrio/providers/dicom/shipment/cancel.py
+-rw-rw-r--  2.0 unx     6933 b- defN 23-Apr-01 15:18 karrio/providers/dicom/shipment/create.py
+-rw-rw-r--  2.0 unx      972 b- defN 23-Apr-18 07:09 karrio.dicom-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.dicom-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.dicom-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1876 b- defN 23-Apr-18 07:09 karrio.dicom-2023.4.dist-info/RECORD
+21 files, 35983 bytes uncompressed, 11533 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: karrio/providers/dicom/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dicom/shipment/create.py
 Comment: 
 
-Filename: karrio.dicom-2023.3.dist-info/METADATA
+Filename: karrio.dicom-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dicom-2023.3.dist-info/WHEEL
+Filename: karrio.dicom-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dicom-2023.3.dist-info/top_level.txt
+Filename: karrio.dicom-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dicom-2023.3.dist-info/RECORD
+Filename: karrio.dicom-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dicom/mapper.py

```diff
@@ -41,17 +41,15 @@
     settings: Settings
 
     # def create_rate_request(
     #     self, payload: RateRequest
     # ) -> Serializable:
     #     return rate_request(payload, self.settings)
 
-    def create_tracking_request(
-        self, payload: TrackingRequest
-    ) -> Serializable:
+    def create_tracking_request(self, payload: TrackingRequest) -> Serializable:
         return tracking_request(payload, self.settings)
 
     # def create_shipment_request(
     #     self, payload: ShipmentRequest
     # ) -> Serializable:
     #     return shipment_request(payload, self.settings)
     #
@@ -66,47 +64,44 @@
     #     return pickup_update_request(payload, self.settings)
     #
     # def create_cancel_pickup_request(
     #     self, payload: PickupCancelRequest
     # ) -> Serializable:
     #     return pickup_cancel_request(payload, self.settings)
     #
-    # def create_cancel_shipment_request(self, payload: ShipmentCancelRequest) -> Serializable[str]:
+    # def create_cancel_shipment_request(self, payload: ShipmentCancelRequest) -> Serializable:
     #     return shipment_cancel_request(payload, self.settings)
 
-
-
-
     # def parse_cancel_pickup_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_pickup_cancel_response(response.deserialize(), self.settings)
+    #     return parse_pickup_cancel_response(response, self.settings)
     #
     # def parse_cancel_shipment_response(
     #     self, response: Deserializable
     # ) -> Tuple[ConfirmationDetails, List[Message]]:
-    #     return parse_shipment_cancel_response(response.deserialize(), self.settings)
+    #     return parse_shipment_cancel_response(response, self.settings)
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
     #
     # def parse_rate_response(
-    #     self, response: Deserializable[str]
+    #     self, response: Deserializable
     # ) -> Tuple[List[RateDetails], List[Message]]:
-    #     return parse_rate_response(response.deserialize(), self.settings)
+    #     return parse_rate_response(response, self.settings)
     #
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

## karrio/mappers/dicom/settings.py

```diff
@@ -15,7 +15,8 @@
 
     # Base properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dicom"
     account_country_code: str = None
     metadata: dict = {}
+    config: dict = {}
```

## karrio/providers/dicom/rate.py

```diff
@@ -12,16 +12,17 @@
 import karrio.core.models as models
 import karrio.providers.dicom.error as provider_error
 import karrio.providers.dicom.units as provider_units
 import karrio.providers.dicom.utils as provider_utils
 
 
 def parse_rate_response(
-    response: dict, settings: provider_utils.Settings
+    _response: lib.Deserializable[dict], settings: provider_utils.Settings
 ) -> typing.Tuple[typing.List[models.RateDetails], typing.List[models.Message]]:
+    response = _response.deserialize()
     errors = provider_error.parse_error_response(response, settings)
     rate_response = (
         lib.to_object(RateResponse, response) if "rates" in response else RateResponse()
     )
     details = [
         _extract_details(rate, rate_response, settings)
         for rate in (rate_response.rates or [])
@@ -58,15 +59,15 @@
         ],
         meta=dict(accountType=rate.accountType),
     )
 
 
 def rate_request(
     payload: models.RateRequest, settings: provider_utils.Settings
-) -> lib.Serializable[DicomRateRequest]:
+) -> lib.Serializable:
     packages = lib.to_packages(payload.parcels)
     service = (
         provider_units.Services(payload.services, provider_units.Service).first
         or provider_units.Service.dicom_ground_delivery.value
     ).value
     options = lib.to_shipping_options(
         payload.options,
```

## karrio/providers/dicom/tracking.py

```diff
@@ -1,44 +1,47 @@
 from typing import Tuple, List
 from dicom_lib.tracking import Tracking
 from karrio.core.utils import Serializable, DF, DP
-from karrio.core.models import (
-    TrackingRequest,
-    TrackingDetails,
-    TrackingEvent,
-    Message
-)
+from karrio.core.models import TrackingRequest, TrackingDetails, TrackingEvent, Message
 
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
+import karrio.lib as lib
 
 
-def parse_tracking_response(response: dict, settings: Settings) -> Tuple[List[TrackingDetails], List[Message]]:
-    errors = [e for e in response if 'activities' not in e]
-    details = [_extract_detail(DP.to_object(Tracking, d), settings) for d in response if 'activities' in d]
+def parse_tracking_response(
+    _response: lib.Deserializable[dict],
+    settings: Settings,
+) -> Tuple[List[TrackingDetails], List[Message]]:
+    response = _response.deserialize()
+    errors = [e for e in response if "activities" not in e]
+    details = [
+        _extract_detail(DP.to_object(Tracking, d), settings)
+        for d in response
+        if "activities" in d
+    ]
 
     return details, parse_error_response(errors, settings)
 
 
 def _extract_detail(detail: Tracking, settings: Settings) -> TrackingDetails:
     return TrackingDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
-
         tracking_number=detail.trackingNumber,
         events=[
             TrackingEvent(
-                date=DF.fdate(event.activityDate, '%Y-%m-%dT%H:%M:%SZ'),
+                date=DF.fdate(event.activityDate, "%Y-%m-%dT%H:%M:%SZ"),
                 description=event.statusDetail,
                 location=event.terminal,
                 code=event.status,
-                time=DF.ftime(event.activityDate, '%Y-%m-%dT%H:%M:%SZ'),
+                time=DF.ftime(event.activityDate, "%Y-%m-%dT%H:%M:%SZ"),
             )
             for event in detail.activities
-        ]
+        ],
     )
 
 
-def tracking_request(payload: TrackingRequest, _) -> Serializable[List[str]]:
+def tracking_request(payload: TrackingRequest, _) -> Serializable:
     request = payload.tracking_numbers
 
     return Serializable(request)
```

## karrio/providers/dicom/pickup/cancel.py

```diff
@@ -1,29 +1,31 @@
 from typing import Tuple, List
 from karrio.core.utils import Serializable
-from karrio.core.models import (
-    PickupCancelRequest,
-    ConfirmationDetails,
-    Message
-)
+from karrio.core.models import PickupCancelRequest, ConfirmationDetails, Message
 
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
+import karrio.lib as lib
 
 
-def parse_pickup_cancel_response(response: dict, settings: Settings) -> Tuple[ConfirmationDetails, List[Message]]:
+def parse_pickup_cancel_response(
+    _response: lib.Deserializable[dict],
+    settings: Settings,
+) -> Tuple[ConfirmationDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     details = (
         ConfirmationDetails(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             success=True,
-            operation="Pickup Cancel"
+            operation="Pickup Cancel",
         )
-        if not any(errors) else None
+        if not any(errors)
+        else None
     )
 
     return details, errors
 
 
 def pickup_cancel_request(payload: PickupCancelRequest, _) -> Serializable:
     request = payload.confirmation_number
```

## karrio/providers/dicom/pickup/create.py

```diff
@@ -8,52 +8,51 @@
     Pickup,
 )
 from karrio.core.utils import Serializable, Pipeline, Job, DP, SF
 from karrio.core.models import PickupRequest, PickupDetails, Message
 
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
+import karrio.lib as lib
 
 
 def parse_pickup_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict], settings: Settings
 ) -> Tuple[PickupDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     pickup = next(
         (DP.to_object(Pickup, pickup) for pickup in response.get("pickups", [])), None
     )
     details = _extract_details(pickup, settings) if pickup is not None else None
 
     return details, errors
 
 
 def _extract_details(pickup: Pickup, settings: Settings) -> PickupDetails:
-
     return PickupDetails(
         carrier_id=settings.carrier_id,
         carrier_name=settings.carrier_name,
         confirmation_number=str(pickup.id),
         closing_time=pickup.officeClose,
         pickup_date=pickup.date,
         ready_time=pickup.ready,
     )
 
 
 def pickup_request(payload: PickupRequest, settings: Settings) -> Serializable:
-
     request: Pipeline = Pipeline(
         create_pickup=lambda *_: _create_pickup(payload),
         retrieve_pickup=partial(_retrieve_pickup, payload=payload, settings=settings),
     )
 
     return Serializable(request)
 
 
 def _create_pickup(payload: PickupRequest) -> Job:
-
     request = DicomPickupRequest(
         date=payload.pickup_date,
         ready=payload.ready_time,
         category=payload.options.get("category", "Parcel"),
         officeClose=payload.closing_time,
         sender=Sender(
             city=payload.address.city,
```

## karrio/providers/dicom/pickup/update.py

```diff
@@ -2,50 +2,56 @@
 from functools import partial
 from karrio.core.utils import Serializable, Pipeline, Job
 from karrio.core.models import (
     PickupCancelRequest,
     PickupUpdateRequest,
     PickupRequest,
     PickupDetails,
-    Message
+    Message,
 )
 
 from karrio.providers.dicom.pickup.create import (
     _create_pickup as _create_pickup_job,
     parse_pickup_response,
-    _retrieve_pickup
+    _retrieve_pickup,
 )
 from karrio.providers.dicom.pickup.cancel import pickup_cancel_request
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
+import karrio.lib as lib
 
 
-def parse_pickup_update_response(response: dict, settings: Settings) -> Tuple[PickupDetails, List[Message]]:
+def parse_pickup_update_response(
+    _response: lib.Deserializable[dict], settings: Settings
+) -> Tuple[PickupDetails, List[Message]]:
+    response = _response.deserialize()
     return parse_pickup_response(response, settings)
 
 
-def pickup_update_request(payload: PickupUpdateRequest, settings: Settings) -> Serializable[Pipeline]:
-
+def pickup_update_request(
+    payload: PickupUpdateRequest, settings: Settings
+) -> Serializable:
     request: Pipeline = Pipeline(
         delete_pickup=lambda *_: _delete_pickup(payload, settings),
         create_pickup=partial(_create_pickup, payload=payload, settings=settings),
-        retrieve_pickup=partial(_retrieve_pickup, payload=payload, settings=settings)
+        retrieve_pickup=partial(_retrieve_pickup, payload=payload, settings=settings),
     )
 
     return Serializable(request)
 
 
 def _delete_pickup(payload: PickupUpdateRequest, settings: Settings) -> Job:
     data = pickup_cancel_request(
-        settings=settings,
-        payload=cast(PickupCancelRequest, payload)
+        settings=settings, payload=cast(PickupCancelRequest, payload)
     )
 
     return Job(id="delete_pickup", data=data)
 
 
 def _create_pickup(deletion_response: str, payload: PickupUpdateRequest) -> Job:
     errors = parse_error_response(deletion_response)
-    create_job: Job = (_create_pickup_job(cast(PickupRequest, payload)) if not any(errors) else None)
-    data = (create_job.data if create_job is not None else None)
+    create_job: Job = (
+        _create_pickup_job(cast(PickupRequest, payload)) if not any(errors) else None
+    )
+    data = create_job.data if create_job is not None else None
 
     return Job(id="create_pickup", data=data, fallback=("{}" if data is None else None))
```

## karrio/providers/dicom/shipment/cancel.py

```diff
@@ -1,29 +1,30 @@
 from typing import Tuple, List
 from karrio.core.utils import Serializable
-from karrio.core.models import (
-    ShipmentCancelRequest,
-    ConfirmationDetails,
-    Message
-)
+from karrio.core.models import ShipmentCancelRequest, ConfirmationDetails, Message
 
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
+import karrio.lib as lib
 
 
-def parse_shipment_cancel_response(response: dict, settings: Settings) -> Tuple[ConfirmationDetails, List[Message]]:
-    errors = parse_error_response(response, settings)
+def parse_shipment_cancel_response(
+    response: lib.Deserializable[dict],
+    settings: Settings,
+) -> Tuple[ConfirmationDetails, List[Message]]:
+    errors = parse_error_response(response.deserialize(), settings)
     details = (
         ConfirmationDetails(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             operation="Shipment Cancel",
             success=True,
         )
-        if not any(errors) else None
+        if not any(errors)
+        else None
     )
 
     return details, errors
 
 
 def shipment_cancel_request(payload: ShipmentCancelRequest, _) -> Serializable:
     request = payload.shipment_identifier
```

## karrio/providers/dicom/shipment/create.py

```diff
@@ -31,16 +31,18 @@
     Purpose,
 )
 from karrio.providers.dicom.error import parse_error_response
 from karrio.providers.dicom.utils import Settings
 
 
 def parse_shipment_response(
-    response: dict, settings: Settings
+    _response: lib.Deserializable[dict],
+    settings: Settings,
 ) -> Tuple[ShipmentDetails, List[Message]]:
+    response = _response.deserialize()
     errors = parse_error_response(response, settings)
     details = (
         _extract_details(response, settings)
         if all(key in response for key in ["label", "shipment"])
         else None
     )
 
@@ -56,17 +58,15 @@
         carrier_id=settings.carrier_id,
         tracking_number=shipment.trackingNumber,
         shipment_identifier=shipment.ID,
         docs=Documents(label=label),
     )
 
 
-def shipment_request(
-    payload: ShipmentRequest, settings: Settings
-) -> Serializable[DicomShipmentRequest]:
+def shipment_request(payload: ShipmentRequest, settings: Settings) -> Serializable:
     packages = Packages(payload.parcels)
     is_international = payload.shipper.country_code != payload.recipient.country_code
     broker_info = payload.options.get("dicom_broker_info", {})
     importer_info = (
         Address(**payload.options.get("importer_info"))
         if "importer_info" in payload.options
         else None
```

## Comparing `karrio.dicom-2023.3.dist-info/METADATA` & `karrio.dicom-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dicom
-Version: 2023.3
+Version: 2023.4
 Summary: Karrio - Dicom Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

