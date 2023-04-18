# Comparing `tmp/tagoio_sdk-4.0.9.tar.gz` & `tmp/tagoio_sdk-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagoio_sdk-4.0.9.tar", max compression
+gzip compressed data, was "tagoio_sdk-4.1.1.tar", max compression
```

## Comparing `tagoio_sdk-4.0.9.tar` & `tagoio_sdk-4.1.1.tar`

### file list

```diff
@@ -1,41 +1,47 @@
--rw-r--r--   0        0        0    11338 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/LICENSE
--rw-r--r--   0        0        0     1382 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/README.md
--rw-r--r--   0        0        0     1577 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/pyproject.toml
--rw-r--r--   0        0        0      317 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/__init__.py
--rw-r--r--   0        0        0     1161 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/common/Common_Type.py
--rw-r--r--   0        0        0     1063 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/common/tagoio_module.py
--rw-r--r--   0        0        0      282 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/config.py
--rw-r--r--   0        0        0     2797 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/infrastructure/api_request.py
--rw-r--r--   0        0        0     1043 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/infrastructure/api_socket.py
--rw-r--r--   0        0        0      616 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Account.py
--rw-r--r--   0        0        0     2850 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Billing.py
--rw-r--r--   0        0        0     4566 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Billing_Type.py
--rw-r--r--   0        0        0      983 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Buckets.py
--rw-r--r--   0        0        0      774 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Buckets_Type.py
--rw-r--r--   0        0        0     6472 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Dashboards.py
--rw-r--r--   0        0        0     3984 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Dashboards_Type.py
--rw-r--r--   0        0        0     9613 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Device_Type.py
--rw-r--r--   0        0        0     9330 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Devices.py
--rw-r--r--   0        0        0     1481 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Notification_Type.py
--rw-r--r--   0        0        0     1550 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Profile.py
--rw-r--r--   0        0        0     1953 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Profile_Type.py
--rw-r--r--   0        0        0     7940 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Run.py
--rw-r--r--   0        0        0    11787 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Run_Type.py
--rw-r--r--   0        0        0     3128 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Analysis/Analysis.py
--rw-r--r--   0        0        0       37 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Analysis/Analysis_Type.py
--rw-r--r--   0        0        0     5285 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Device/Device.py
--rw-r--r--   0        0        0      814 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Device/Device_Type.py
--rw-r--r--   0        0        0      787 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Attachment.py
--rw-r--r--   0        0        0      579 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Console.py
--rw-r--r--   0        0        0     2358 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Email.py
--rw-r--r--   0        0        0      853 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/MQTT.py
--rw-r--r--   0        0        0      764 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Notification.py
--rw-r--r--   0        0        0     3443 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/PDF.py
--rw-r--r--   0        0        0      623 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/SMS.py
--rw-r--r--   0        0        0      836 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Services.py
--rw-r--r--   0        0        0      707 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/dateParser.py
--rw-r--r--   0        0        0      543 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/envToJson.py
--rw-r--r--   0        0        0      677 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/getDevice.py
--rw-r--r--   0        0        0     1389 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/getTokenByName.py
--rw-r--r--   0        0        0     1196 2023-03-01 20:35:09.836058 tagoio_sdk-4.0.9/src/tagoio_sdk/regions.py
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 tagoio_sdk-4.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/LICENSE
+-rw-r--r--   0        0        0     1208 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/README.md
+-rw-r--r--   0        0        0     1559 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/__init__.py
+-rw-r--r--   0        0        0     2437 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/common/Common_Type.py
+-rw-r--r--   0        0        0     1063 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/common/tagoio_module.py
+-rw-r--r--   0        0        0      282 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/config.py
+-rw-r--r--   0        0        0     2797 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/infrastructure/api_request.py
+-rw-r--r--   0        0        0     1043 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/infrastructure/api_socket.py
+-rw-r--r--   0        0        0     1342 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Account.py
+-rw-r--r--   0        0        0      876 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Account_Types.py
+-rw-r--r--   0        0        0     2850 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Billing.py
+-rw-r--r--   0        0        0     4566 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Billing_Type.py
+-rw-r--r--   0        0        0      983 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Buckets.py
+-rw-r--r--   0        0        0      774 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Buckets_Type.py
+-rw-r--r--   0        0        0     6447 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Dashboards.py
+-rw-r--r--   0        0        0     3877 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Dashboards_Type.py
+-rw-r--r--   0        0        0     9613 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Device_Type.py
+-rw-r--r--   0        0        0     9336 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Devices.py
+-rw-r--r--   0        0        0      274 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Integration.py
+-rw-r--r--   0        0        0     1824 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/IntegrationNetwork.py
+-rw-r--r--   0        0        0     1688 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/IntegrationNetworkType.py
+-rw-r--r--   0        0        0     1481 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Notification_Type.py
+-rw-r--r--   0        0        0     2764 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Profile.py
+-rw-r--r--   0        0        0     1953 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Profile_Type.py
+-rw-r--r--   0        0        0     7926 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Run.py
+-rw-r--r--   0        0        0    11685 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Run_Type.py
+-rw-r--r--   0        0        0     3128 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Analysis/Analysis.py
+-rw-r--r--   0        0        0       37 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Analysis/Analysis_Type.py
+-rw-r--r--   0        0        0     5285 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Device/Device.py
+-rw-r--r--   0        0        0      814 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Device/Device_Type.py
+-rw-r--r--   0        0        0      787 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Attachment.py
+-rw-r--r--   0        0        0      579 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Console.py
+-rw-r--r--   0        0        0     2366 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Email.py
+-rw-r--r--   0        0        0      853 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/MQTT.py
+-rw-r--r--   0        0        0      764 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Notification.py
+-rw-r--r--   0        0        0     3436 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/PDF.py
+-rw-r--r--   0        0        0      623 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/SMS.py
+-rw-r--r--   0        0        0      836 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Services.py
+-rw-r--r--   0        0        0      707 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/dateParser.py
+-rw-r--r--   0        0        0      493 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/envToJson.py
+-rw-r--r--   0        0        0      677 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/getDevice.py
+-rw-r--r--   0        0        0     1389 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/getTokenByName.py
+-rw-r--r--   0        0        0     4041 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/sendDownlink.py
+-rw-r--r--   0        0        0      178 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/utilsType.py
+-rw-r--r--   0        0        0     1196 2023-04-18 15:28:01.629279 tagoio_sdk-4.1.1/src/tagoio_sdk/regions.py
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 tagoio_sdk-4.1.1/PKG-INFO
```

### Comparing `tagoio_sdk-4.0.9/LICENSE` & `tagoio_sdk-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/README.md` & `tagoio_sdk-4.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 <br/>
 <p align="center">
   <img src="https://assets.tago.io/tagoio/sdk.png" width="250px" alt="TagoIO"></img>
 </p>
 
-> NOTE: *This version (4.x.x) is still in development. You can access the current (3.x.x) version in [tago-io/tago-sdk-python](https://github.com/tago-io/tago-sdk-python).*
-
 # TagoIO - Python SDK
 
 Official Python SDK for TagoIO
 
 ## Installation
 
 ```bash
```

### Comparing `tagoio_sdk-4.0.9/pyproject.toml` & `tagoio_sdk-4.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagoio-sdk"
-version = "4.0.9"
+version = "4.1.1"
 description = "Official Python SDK for TagoIO"
 authors = ["Tago LLC <contact@tago.io>"]
 license = "Apache License"
 readme = "README.md"
 homepage = "https://tago.io/"
 repository = "https://github.com/tago-io/sdk-python/"
 documentation = "https://py.sdk.tago.io/"
@@ -21,19 +21,18 @@
 # include = [
     # { path = "poetry.lock", format = "sdist" }
     # { path = "tests", format = "sdist" }
 # ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.2"
+requests = "2.28.2"
 python-dateutil = "^2.8.2"
 python-socketio = {extras = ["asyncio_client"], version = "^5.7.2"}
 aiohttp = "^3.8.4"
-toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 black = "^22.3.0"
 flake8-annotations = "^2.9.0"
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/common/tagoio_module.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/common/tagoio_module.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/infrastructure/api_request.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/infrastructure/api_request.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/infrastructure/api_socket.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/infrastructure/api_socket.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Billing.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Billing.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Billing_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Billing_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Buckets.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Buckets.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Buckets_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Buckets_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Dashboards.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Dashboards.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Optional, TypedDict
-from tagoio_sdk.common.Common_Type import ExpireTimeOption, GenericID
+from tagoio_sdk.common.Common_Type import ExpireTimeOption, GenericID, Query
 from tagoio_sdk.common.tagoio_module import TagoIOModule
 from tagoio_sdk.modules.Account.Dashboards_Type import (
     AnalysisRelated,
     DashboardCreateInfo,
     DashboardInfo,
-    DashboardQuery,
     DevicesRelated,
     PublicKeyResponse,
 )
 from tagoio_sdk.modules.Utils.dateParser import dateParser, dateParserList
 
 
 class Dashboards(TagoIOModule):
-    def listDashboard(self, queryObj: DashboardQuery = {}) -> list[DashboardInfo]:
+    def listDashboard(self, queryObj: Query = {}) -> list[DashboardInfo]:
         """
         Retrieves a list with all dashboards from the account
 
         :default:
 
             queryObj: {
                 "page": 1,
@@ -28,16 +27,16 @@
             }
 
         :param queryObj Search query params
         """
 
         if "orderBy" in queryObj:
             firstArgument = queryObj["orderBy"][0]
-            seccondArgument = queryObj["orderBy"][1]
-            orderBy = f"{firstArgument},{seccondArgument}"
+            secondArgument = queryObj["orderBy"][1]
+            orderBy = f"{firstArgument},{secondArgument}"
         else:
             orderBy = "label,asc"
 
         result = self.doRequest(
             {
                 "path": "/dashboard",
                 "method": "GET",
@@ -138,15 +137,15 @@
         Duplicate the dashboard to your own account
 
         :param dashboardID Dashboard identification
         :param dashboardObj Object with data of the duplicate dashboard
         """
         result = self.doRequest(
             {
-                "path": f"/dashboard/${dashboardID}/duplicate",
+                "path": f"/dashboard/{dashboardID}/duplicate",
                 "method": "POST",
                 "body": dashboardObj,
             }
         )
 
         return result
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Dashboards_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Dashboards_Type.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,10 @@
 class PublicKeyResponse(TypedDict):
     token: GenericToken
     expire_time: ExpireTimeOption
 
 
 EditDataModel = PostDataModel and {id: GenericID}
 
-DashboardQuery = (
-    DashboardInfo and Literal["name", "label", "active", "created_at", "updated_at"]
-)
-
 PublicKeyResponse = PublicKeyResponse
 
 widgetOverwriteOptions = Literal["start_date", "end_date", "timezone"]
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Device_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Device_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Devices.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DeviceListItem,
     DeviceQuery,
     DeviceTokenDataList,
     ListDeviceTokenQuery,
     TokenData,
 )
 from tagoio_sdk.modules.Device.Device_Type import DataQuery, DeviceInfo
-from tagoio_sdk.modules.Utils.dateParser import dateParserList
+from tagoio_sdk.modules.Utils.dateParser import dateParserList, dateParser
 
 
 class Devices(TagoIOModule):
     def listDevice(self, queryObj: DeviceQuery = {}) -> list[DeviceListItem]:
         """
         Retrieves a list with all devices from the account
 
@@ -129,15 +129,15 @@
         result = self.doRequest(
             {
                 "path": f"/device/{deviceID}",
                 "method": "GET",
             }
         )
 
-        result = dateParserList(
+        result = dateParser(
             result,
             [
                 "last_input",
                 "last_output",
                 "updated_at",
                 "created_at",
                 "inspected_at",
@@ -231,16 +231,16 @@
         :param GenericID deviceID: Device ID
 
         :param ListDeviceTokenQuery queryObj: Search query params
         """
 
         if "orderBy" in queryObj:
             firstArgument = queryObj["orderBy"][0]
-            seccondArgument = queryObj["orderBy"][1]
-            orderBy = f"{firstArgument},{seccondArgument}"
+            secondArgument = queryObj["orderBy"][1]
+            orderBy = f"{firstArgument},{secondArgument}"
         else:
             orderBy = "created_at,desc"
 
         result = self.doRequest(
             {
                 "path": f"/device/token/{deviceID}",
                 "method": "GET",
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Notification_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Notification_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Profile_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Profile_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Run.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, TypedDict
-from tagoio_sdk.common.Common_Type import GenericID
+from tagoio_sdk.common.Common_Type import GenericID, Query
 from tagoio_sdk.common.tagoio_module import TagoIOModule
 from tagoio_sdk.modules.Account.Notification_Type import (
     NotificationCreate,
     NotificationInfo,
     NotificationcreateReturn,
 )
 from tagoio_sdk.modules.Account.Run_Type import (
@@ -12,15 +12,14 @@
     LoginAsUserOptions,
     LoginResponse,
     RunInfo,
     RunSAMLEditInfo,
     RunSAMLInfo,
     UserCreateInfo,
     UserInfo,
-    UserQuery,
 )
 from tagoio_sdk.modules.Utils.dateParser import dateParser, dateParserList
 
 
 class Run(TagoIOModule):
     """
     Manage services in account
@@ -47,19 +46,19 @@
                 "method": "PUT",
                 "body": data,
             }
         )
 
         return result
 
-    def listUsers(self, query: UserQuery) -> list[UserInfo]:
+    def listUsers(self, query: Query) -> list[UserInfo]:
         if "orderBy" in query:
             firstArgument = query["orderBy"][0]
-            seccondArgument = query["orderBy"][1]
-            orderBy = f"{firstArgument},{seccondArgument}"
+            secondArgument = query["orderBy"][1]
+            orderBy = f"{firstArgument},{secondArgument}"
         else:
             orderBy = "name,asc"
 
         result = self.doRequest
         (
             {
                 "path": "/run/users",
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Account/Run_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Account/Run_Type.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,12 +500,7 @@
     email: str
     """
     Mailing address for the RUN with custom domain.
 
     If the desired custom domain is `portal.mycompany.com`, this can be either
     `"portal.mycompany.com"` or `"mycompany.com"`.
     """
-
-
-UserQuery = (
-    UserInfo and "name" or "active" or "last_login" or "created_at" or "updated_at"
-)
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Analysis/Analysis.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Device/Device.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Device/Device.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Device/Device_Type.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Device/Device_Type.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Attachment.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Attachment.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Console.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Console.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Email.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Email.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 EmailWithRawText = Union[EmailBase, EmailRawText]
 
 
 class Email(TagoIOModule):
     def send(
         self, email: Union[Any, EmailWithRawText, EmailWithHTML, EmailWithTemplate]
     ) -> str:
-        if email["html"] and email["message"]:
+        if email.get("html") and email.get("message"):
             warnings.warn("HTML field will overwrite message field")
 
         result = self.doRequest(
             {
                 "path": "/analysis/services/email/send",
                 "method": "POST",
                 "body": email,
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/MQTT.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/MQTT.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Notification.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Notification.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/PDF.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/PDF.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,11 +126,11 @@
 class PDFService(TagoIOModule):
     def generate(self, params: PDFParams) -> PDFResult:
         """
         Generate a PDF from html, url or base64
         """
         result = requests.post(
             "https://pdf.middleware.tago.io",
-            data=params,
-            headers={"token": self.params.token},
+            json=params,
+            headers={"token": self.token},
         )
         return result
```

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/SMS.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/SMS.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Services/Services.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Services/Services.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/dateParser.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/dateParser.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/getDevice.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/getDevice.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/modules/Utils/getTokenByName.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/modules/Utils/getTokenByName.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/src/tagoio_sdk/regions.py` & `tagoio_sdk-4.1.1/src/tagoio_sdk/regions.py`

 * *Files identical despite different names*

### Comparing `tagoio_sdk-4.0.9/PKG-INFO` & `tagoio_sdk-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagoio-sdk
-Version: 4.0.9
+Version: 4.1.1
 Summary: Official Python SDK for TagoIO
 Home-page: https://tago.io/
 License: Apache License
 Keywords: tagoio,iot,analysis,tago,sensor,device
 Author: Tago LLC
 Author-email: contact@tago.io
 Requires-Python: >=3.9,<4.0
@@ -16,27 +16,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-socketio[asyncio-client] (>=5.7.2,<6.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: requests (==2.28.2)
 Project-URL: Documentation, https://py.sdk.tago.io/
 Project-URL: Repository, https://github.com/tago-io/sdk-python/
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
   <img src="https://assets.tago.io/tagoio/sdk.png" width="250px" alt="TagoIO"></img>
 </p>
 
-> NOTE: *This version (4.x.x) is still in development. You can access the current (3.x.x) version in [tago-io/tago-sdk-python](https://github.com/tago-io/tago-sdk-python).*
-
 # TagoIO - Python SDK
 
 Official Python SDK for TagoIO
 
 ## Installation
 
 ```bash
```

