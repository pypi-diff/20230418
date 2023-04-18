# Comparing `tmp/pyworxcloud-3.1.2.tar.gz` & `tmp/pyworxcloud-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.2.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.3.tar", max compression
```

## Comparing `pyworxcloud-3.1.2.tar` & `pyworxcloud-3.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-17 10:21:38.844156 pyworxcloud-3.1.2/LICENSE
--rw-r--r--   0        0        0      929 2023-04-17 10:21:38.844156 pyworxcloud-3.1.2/README.md
--rw-r--r--   0        0        0      610 2023-04-17 10:21:52.648889 pyworxcloud-3.1.2/pyproject.toml
--rw-r--r--   0        0        0    28730 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/events.py
--rw-r--r--   0        0        0     1826 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3838 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     7112 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6375 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-04-17 10:21:38.852156 pyworxcloud-3.1.2/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/README.md
+-rw-r--r--   0        0        0      610 2023-04-18 12:33:28.642206 pyworxcloud-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0    28714 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1826 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3609 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     8183 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     2410 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6191 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.3/PKG-INFO
```

### Comparing `pyworxcloud-3.1.2/LICENSE` & `pyworxcloud-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/README.md` & `pyworxcloud-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyproject.toml` & `pyworxcloud-3.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.2"
+version = "v3.1.3"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pyworxcloud-3.1.2/pyworxcloud/__init__.py` & `pyworxcloud-3.1.3/pyworxcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
         self._endpoint = self._mowers[0]["mqtt_endpoint"]
         self._user_id = self._mowers[0]["user_id"]
 
         self._log.debug("Setting up MQTT handler")
         # setup MQTT handler
         self.mqtt = MQTT(
-            self._api.access_token,
+            self._api,
             self._cloud.BRAND_PREFIX,
             self._endpoint,
             self._user_id,
             self._log,
             self._on_update,
         )
 
@@ -604,16 +604,16 @@
             rain_delay (str | int): Rain delay in minutes.
 
         Raises:
             OfflineError: Raised if the device is offline.
         """
         mower = self.get_mower(serial_number)
         if mower["online"]:
-            if not isinstance(rain_delay, str):
-                rain_delay = str(rain_delay)
+            if not isinstance(rain_delay, int):
+                rain_delay = int(rain_delay)
             self.mqtt.publish(
                 serial_number,
                 mower["mqtt_topics"]["command_in"],
                 {"rd": rain_delay},
             )
         else:
             raise OfflineError("The device is currently offline, no action was sent.")
@@ -737,17 +737,17 @@
 
         Raises:
             OfflineError: Raised if the device is offline.
         """
         mower = self.get_mower(serial_number)
         if mower["online"]:
             self.mqtt.publish(
-                serial_number, mower["mqtt_topics"]["command_in"], {"sc": {"m": 1}}
-            ) if enable else str(
-                {"sc": {"m": 0}},
+                serial_number,
+                mower["mqtt_topics"]["command_in"],
+                {"sc": {"m": 1}} if enable else {"sc": {"m": 0}},
             )
         else:
             raise OfflineError("The device is currently offline, no action was sent.")
 
     def ots(self, serial_number: str, boundary: bool, runtime: str) -> None:
         """Start a One-Time-Schedule task
```

### Comparing `pyworxcloud-3.1.2/pyworxcloud/api.py` & `pyworxcloud-3.1.3/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/clouds.py` & `pyworxcloud-3.1.3/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/const.py` & `pyworxcloud-3.1.3/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/events.py` & `pyworxcloud-3.1.3/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.3/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.3/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.3/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/devices.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,25 +96,21 @@
         self.orientation = Orientation([0, 0, 0])
         self.capabilities = Capability(data)
         self.rainsensor = Rainsensor()
         self.status = States()
         self.zone = Zone()
         self.warranty = Warranty(data)
         self.firmware = Firmware(data)
-        self.schedules = Schedule()
+        self.schedules = Schedule(data)
         self.in_topic = data["mqtt_topics"]["command_in"]
         self.out_topic = data["mqtt_topics"]["command_out"]
 
         if data in ["lawn_perimeter", "lawn_size"]:
             self.lawn = Lawn(data["lawn_perimeter"], data["lawn_size"])
 
-        if data in ["auto_schedule_settings", "auto_schedule"]:
-            self.schedules["auto_schedule"]["settings"] = data["auto_schedule_settings"]
-            self.schedules["auto_schedule"]["enabled"] = data["auto_schedule"]
-
         self.name = data["name"]
         self.model = "Model info not available in API"  # f"{self.chassis.default_name}{self.chassis.meters}"
 
         for attr in UNWANTED_ATTRIBS:
             if hasattr(self, attr):
                 delattr(self, attr)
```

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/mqtt.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from logging import Logger
 from typing import Any
 from uuid import uuid4
 
 import paho.mqtt.client as mqtt
 from paho.mqtt.client import connack_string, error_string
 
-from ..exceptions import MQTTException
-
 from ..events import EventHandler, LandroidEvent
+from ..exceptions import MQTTException
 from .landroid_class import LDict
 
 QOS_FLAG = 1
 
 
 class MQTTMsgType(LDict):
     """Define specific message type data."""
@@ -83,15 +82,15 @@
 
 
 class MQTT(LDict):
     """Full MQTT handler class."""
 
     def __init__(
         self,
-        token: str,
+        api: Any,
         brandprefix: str,
         endpoint: str,
         user_id: int,
         logger: Logger,
         callback: Any,
     ) -> dict:
         """Initialize AWSIoT MQTT handler."""
@@ -99,33 +98,37 @@
         # self.client = None
         self._events = EventHandler()
         self._on_update = callback
         self._endpoint = endpoint
         self._log = logger.getChild("MQTT")
         self._disconnected = False
         self._topic: list = []
-
-        accesstokenparts = token.replace("_", "/").replace("-", "+").split(".")
+        self._api = api
 
         self._uuid = uuid4()
 
         self.client = mqtt.Client(
             client_id=f"{brandprefix}/USER/{user_id}/bot/{self._uuid}",
             clean_session=False,
             userdata=None,
             reconnect_on_failure=True,
         )
+
+        accesstokenparts = (
+            api.access_token.replace("_", "/").replace("-", "+").split(".")
+        )
         self.client.username_pw_set(
             username=f"bot?jwt={urllib.parse.quote(accesstokenparts[0])}.{urllib.parse.quote(accesstokenparts[1])}&x-amz-customauthorizer-name=''&x-amz-customauthorizer-signature={urllib.parse.quote(accesstokenparts[2])}",
             password=None,
         )
 
         ssl_context = ssl.create_default_context()
         ssl_context.set_alpn_protocols(["mqtt"])
         self.client.tls_set_context(context=ssl_context)
+        self.client.reconnect_delay_set(min_delay=10, max_delay=300)
 
         self.client.on_connect = self._on_connect
         self.client.on_message = self._forward_on_message
         self.client.on_disconnect = self._on_disconnect
 
     @property
     def connected(self) -> bool:
@@ -140,17 +143,18 @@
         properties: Any | None = None,  # pylint: disable=unused-argument
     ) -> None:
         """MQTT callback method definition."""
         msg = message.payload.decode("utf-8")
         self._log.debug("Received MQTT message:\n%s", msg)
         self._on_update(msg)
 
-    def subscribe(self, topic: str) -> None:
+    def subscribe(self, topic: str, append: bool = True) -> None:
         """Subscribe to MQTT updates."""
-        self._topic.append(topic)
+        if append and topic not in self._topic:
+            self._topic.append(topic)
         self.client.subscribe(topic=topic, qos=QOS_FLAG)
 
     def connect(self) -> None:
         """Connect to the MQTT service."""
         self.client.connect(self._endpoint, 443, 45)
         self.client.loop_start()
 
@@ -167,14 +171,16 @@
         logger.debug(connack_string(rc))
         if rc == 0:
             self._disconnected = False
             logger.debug("MQTT connected")
             self._events.call(
                 LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
             )
+            for topic in self._topic:
+                self.subscribe(topic, False)
         else:
             logger.debug("MQTT connection failed")
             self._events.call(
                 LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
             )
 
     def _on_disconnect(
@@ -183,24 +189,41 @@
         userdata: Any | None,
         rc: int | None,
         properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
     ) -> None:
         """MQTT callback method."""
         logger = self._log.getChild("Conn_State")
         if rc > 0:
-            logger.debug(
-                "Unexpected MQTT disconnect (%s) - retrying", connack_string(rc)
-            )
-            self.client.reconnect_delay_set(min_delay=1, max_delay=120)
-            self.client.reconnect()
+            if rc == 7:
+                logger.debug("Refreshing access token and reconnecting")
+                self._api.update_token()
+                accesstokenparts = (
+                    self._api.access_token.replace("_", "/")
+                    .replace("-", "+")
+                    .split(".")
+                )
+                self.client.username_pw_set(
+                    username=f"bot?jwt={urllib.parse.quote(accesstokenparts[0])}.{urllib.parse.quote(accesstokenparts[1])}&x-amz-customauthorizer-name=''&x-amz-customauthorizer-signature={urllib.parse.quote(accesstokenparts[2])}",
+                    password=None,
+                )
+                self.connect()
+            else:
+                logger.debug(
+                    "Unexpected MQTT disconnect (%s: %s) - retrying",
+                    rc,
+                    connack_string(rc),
+                )
+                self.client.reconnect()
 
     def disconnect(
         self, reasoncode=None, properties=None  # pylint: disable=unused-argument
     ):
         """Disconnect from AWSIoT MQTT server."""
+        for topic in self._topic:
+            self.client.unsubscribe(self._topic.pop(topic))
         self._disconnected = True
         self.client.loop_stop()
         self.client.disconnect()
 
     def ping(self, serial_number: str, topic: str) -> None:
         """Ping (update) the mower."""
         cmd = self.format_message(serial_number, {"cmd": Command.FORCE_REFRESH})
```

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/schedules.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,35 +160,27 @@
 
         return next.strftime("%Y-%m-%d %H:%M:%S")
 
 
 class Schedule(LDict):
     """Represents a schedule."""
 
-    def __init__(
-        self,
-        variation: int = 0,
-        active: bool = True,
-        auto_schedule_settings: dict = {},
-        auto_schedule_enabled: bool | None = None,
-    ) -> dict:
-        """Initialize an empty primary or secondary schedule.
-
-        Args:
-            schedule_type (ScheduleType): Which ScheduleType to initialize.
-        """
+    def __init__(self, data) -> None:
+        """Initialize a schedule."""
         super().__init__()
 
         self["daily_progress"] = None
         self["next_schedule_start"] = None
-        self["time_extension"] = variation
-        self["active"] = active
+        self["time_extension"] = 0
+        self["active"] = True
         self["auto_schedule"] = {
-            "settings": auto_schedule_settings,
-            "enabled": auto_schedule_enabled,
+            "settings": data["auto_schedule_settings"]
+            if "auto_schedule_settings" in data
+            else {},
+            "enabled": data["auto_schedule"] if "auto_schedule" in data else False,
         }
 
     def update_progress_and_next(self, tz: str | None = None) -> None:
         """Update progress and next scheduled start properties."""
 
         info = ScheduleInfo(self, tz)
         self["daily_progress"] = info.calculate_progress()
```

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.3/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.2/PKG-INFO` & `pyworxcloud-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.2
+Version: 3.1.3
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.2 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.3 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests
 (>=2.26.0,<3.0.0) Requires-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug
```

