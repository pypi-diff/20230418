# Comparing `tmp/karrio.server.proxy-2023.3.4-py3-none-any.whl.zip` & `tmp/karrio.server.proxy-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 15182 bytes, number of entries: 21
+Zip file size: 15163 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-15 19:21 karrio/server/proxy/__init__.py
 -rw-rw-r--  2.0 unx       63 b- defN 22-Nov-15 19:21 karrio/server/proxy/admin.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Nov-15 19:21 karrio/server/proxy/apps.py
 -rw-rw-r--  2.0 unx       57 b- defN 22-Nov-15 19:21 karrio/server/proxy/models.py
 -rw-rw-r--  2.0 unx       95 b- defN 22-Nov-15 19:21 karrio/server/proxy/router.py
 -rw-rw-r--  2.0 unx      214 b- defN 22-Nov-15 19:21 karrio/server/proxy/urls.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-15 19:21 karrio/server/proxy/migrations/__init__.py
 -rw-rw-r--  2.0 unx      263 b- defN 22-Nov-15 19:21 karrio/server/proxy/tests/__init__.py
 -rw-rw-r--  2.0 unx     8814 b- defN 23-Mar-27 07:55 karrio/server/proxy/tests/test_pickup.py
 -rw-rw-r--  2.0 unx     3112 b- defN 23-Mar-03 13:50 karrio/server/proxy/tests/test_rating.py
 -rw-rw-r--  2.0 unx    10341 b- defN 23-Mar-27 07:55 karrio/server/proxy/tests/test_shipping.py
--rw-rw-r--  2.0 unx     2942 b- defN 23-Mar-29 12:47 karrio/server/proxy/tests/test_tracking.py
+-rw-rw-r--  2.0 unx     2942 b- defN 23-Mar-30 05:44 karrio/server/proxy/tests/test_tracking.py
 -rw-rw-r--  2.0 unx      210 b- defN 22-Nov-15 19:21 karrio/server/proxy/views/__init__.py
 -rw-rw-r--  2.0 unx     4376 b- defN 23-Mar-03 13:50 karrio/server/proxy/views/pickup.py
 -rw-rw-r--  2.0 unx     1669 b- defN 23-Mar-03 13:50 karrio/server/proxy/views/rating.py
 -rw-rw-r--  2.0 unx     4345 b- defN 23-Mar-03 13:50 karrio/server/proxy/views/shipping.py
--rw-rw-r--  2.0 unx     5119 b- defN 23-Mar-29 12:37 karrio/server/proxy/views/tracking.py
--rw-rw-r--  2.0 unx      657 b- defN 23-Mar-29 13:37 karrio.server.proxy-2023.3.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-29 13:37 karrio.server.proxy-2023.3.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-29 13:37 karrio.server.proxy-2023.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1904 b- defN 23-Mar-29 13:37 karrio.server.proxy-2023.3.4.dist-info/RECORD
-21 files, 44379 bytes uncompressed, 11998 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     5119 b- defN 23-Mar-29 20:04 karrio/server/proxy/views/tracking.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Apr-18 10:32 karrio.server.proxy-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 10:32 karrio.server.proxy-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 10:32 karrio.server.proxy-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1896 b- defN 23-Apr-18 10:32 karrio.server.proxy-2023.4.dist-info/RECORD
+21 files, 44369 bytes uncompressed, 11995 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: karrio/server/proxy/views/shipping.py
 Comment: 
 
 Filename: karrio/server/proxy/views/tracking.py
 Comment: 
 
-Filename: karrio.server.proxy-2023.3.4.dist-info/METADATA
+Filename: karrio.server.proxy-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.server.proxy-2023.3.4.dist-info/WHEEL
+Filename: karrio.server.proxy-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.server.proxy-2023.3.4.dist-info/top_level.txt
+Filename: karrio.server.proxy-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.server.proxy-2023.3.4.dist-info/RECORD
+Filename: karrio.server.proxy-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/server/proxy/tests/test_tracking.py

```diff
@@ -58,15 +58,15 @@
             "package_weight_unit": None,
             "shipment_package_count": None,
             "shipment_pickup_date": None,
             "shipment_delivery_date": None,
             "shipment_service": None,
             "shipment_origin_country": None,
             "shipment_origin_postal_code": None,
-            "shipment_destication_country": None,
+            "shipment_destination_country": None,
             "shipment_destination_postal_code": None,
             "shipping_date": None,
             "signed_by": None,
             "source": "api",
         },
         "events": [
             {
```

## Comparing `karrio.server.proxy-2023.3.4.dist-info/METADATA` & `karrio.server.proxy-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.server.proxy
-Version: 2023.3.4
+Version: 2023.4
 Summary: Multi-carrier shipping API Proxy module
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `karrio.server.proxy-2023.3.4.dist-info/RECORD` & `karrio.server.proxy-2023.4.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 karrio/server/proxy/router.py,sha256=IBUR7rfBkdEHQzWxYOPcVSM8NBp3fte9G6Q5BVTUNNw,95
 karrio/server/proxy/urls.py,sha256=DJFUFeaxOTyVNgu_A4opiX4-0gJlciRJNob-ScOkdV4,214
 karrio/server/proxy/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 karrio/server/proxy/tests/__init__.py,sha256=m6Nms0Mg2SsrhNtWGC9Pr67qxpWos3WHipHfQZ6Zslw,263
 karrio/server/proxy/tests/test_pickup.py,sha256=HUOY_FI20Zgqu24e3F_FHz4KONcLwAEKE2IC7sQrjTk,8814
 karrio/server/proxy/tests/test_rating.py,sha256=Iu0WH1oDCxHwjGA2La-IQYNDOuHlvMKroSvQZrGiGAw,3112
 karrio/server/proxy/tests/test_shipping.py,sha256=8yyrYCiCxq8LwVLD2u3T-q57ofJ_0kD0gQoyG6CihBM,10341
-karrio/server/proxy/tests/test_tracking.py,sha256=F8VF0uD0grxQnXQuyhcF4smKV9HtN68wXZb2RLQQ2KU,2942
+karrio/server/proxy/tests/test_tracking.py,sha256=pI_Y6ARRzBZgYxeHUH8PZDH08QPX7yV7PdBNGHM3q5w,2942
 karrio/server/proxy/views/__init__.py,sha256=_sk3DC8jqQOb10eH3jSdnYkoqbtxQSEUxcvL7OKqJAo,210
 karrio/server/proxy/views/pickup.py,sha256=Io3H6cg-yPb0pAZh3_mHp8ClFa9I_Tgi2VSCmD0e_do,4376
 karrio/server/proxy/views/rating.py,sha256=S_rl8NT8xxjwG9FZiaId821wv15eyTsC9LEPOcjp1A0,1669
 karrio/server/proxy/views/shipping.py,sha256=PVlpC9ARkQvrShzDQGIvfafbBLJDJH5N1c4384-Cij0,4345
 karrio/server/proxy/views/tracking.py,sha256=5tRGk9likmD_DsCamy3Cm0KFlyCBd4ps9rMBTnCGcHU,5119
-karrio.server.proxy-2023.3.4.dist-info/METADATA,sha256=9z_tsnE9DQGgu-udUwf3za7_0NczGvEqIOP5VUWih_g,657
-karrio.server.proxy-2023.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.server.proxy-2023.3.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.server.proxy-2023.3.4.dist-info/RECORD,,
+karrio.server.proxy-2023.4.dist-info/METADATA,sha256=QMq0raPRGO67WLzg3rzvzjvLYZtDah3ewG7y0WjEXJw,655
+karrio.server.proxy-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.server.proxy-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.server.proxy-2023.4.dist-info/RECORD,,
```

