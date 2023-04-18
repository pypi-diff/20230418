# Comparing `tmp/python_roborock-0.6.6.tar.gz` & `tmp/python_roborock-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.6.tar", max compression
+gzip compressed data, was "python_roborock-0.6.7.tar", max compression
```

## Comparing `python_roborock-0.6.6.tar` & `python_roborock-0.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-17 23:55:00.477835 python_roborock-0.6.6/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-17 23:55:00.477835 python_roborock-0.6.6/README.md
--rw-r--r--   0        0        0     1370 2023-04-17 23:55:01.229832 python_roborock-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/__init__.py
--rw-r--r--   0        0        0    18861 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/cli.py
--rw-r--r--   0        0        0     8595 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/code_mappings.py
--rw-r--r--   0        0        0     9404 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/exceptions.py
--rw-r--r--   0        0        0     7230 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/local_api.py
--rw-r--r--   0        0        0     6108 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12762 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/typing.py
--rw-r--r--   0        0        0      868 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 01:10:57.170099 python_roborock-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-18 01:10:57.170099 python_roborock-0.6.7/README.md
+-rw-r--r--   0        0        0     1370 2023-04-18 01:10:58.046144 python_roborock-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/__init__.py
+-rw-r--r--   0        0        0    18701 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/cli.py
+-rw-r--r--   0        0        0     8408 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9404 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/exceptions.py
+-rw-r--r--   0        0        0     7214 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/local_api.py
+-rw-r--r--   0        0        0      618 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6108 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12762 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/typing.py
+-rw-r--r--   0        0        0      567 2023-04-18 01:10:57.170099 python_roborock-0.6.7/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.7/PKG-INFO
```

### Comparing `python_roborock-0.6.6/LICENSE` & `python_roborock-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/README.md` & `python_roborock-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/pyproject.toml` & `python_roborock-0.6.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.6"
+version = "0.6.7"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.6.6/roborock/api.py` & `python_roborock-0.6.7/roborock/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,19 @@
     RoborockDeviceInfo,
     SmartWashParams,
     Status,
     UserData,
     WashTowelMode,
 )
 from .roborock_message import RoborockMessage
-from .roborock_queue import RoborockQueue
+from .roborock_future import RoborockFuture
 from .typing import RoborockCommand, RoborockDeviceProp, RoborockDockSummary
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
-MQTT_KEEPALIVE = 60
 SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
 
 
 def md5hex(message: str) -> str:
     md5 = hashlib.md5()
@@ -76,72 +75,71 @@
 
 
 class RoborockClient:
     def __init__(self, endpoint: str, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
         self.devices_info = devices_info
         self._endpoint = endpoint
         self._nonce = secrets.token_bytes(16)
-        self._waiting_queue: dict[int, RoborockQueue] = {}
+        self._waiting_queue: dict[int, RoborockFuture] = {}
         self._status_listeners: list[Callable[[int, str], None]] = []
 
     def add_status_listener(self, callback: Callable[[int, str], None]):
         self._status_listeners.append(callback)
 
     async def async_disconnect(self) -> Any:
         raise NotImplementedError
 
-    async def on_message(self, messages: list[RoborockMessage]) -> None:
+    def on_message(self, messages: list[RoborockMessage]) -> None:
         try:
             for data in messages:
                 protocol = data.protocol
                 if protocol == 102 or protocol == 4:
                     payload = json.loads(data.payload.decode())
                     for data_point_number, data_point in payload.get("dps").items():
                         if data_point_number == "102":
                             data_point_response = json.loads(data_point)
                             request_id = data_point_response.get("id")
                             queue = self._waiting_queue.get(request_id)
                             if queue:
                                 if queue.protocol == protocol:
                                     error = data_point_response.get("error")
                                     if error:
-                                        await queue.async_put(
+                                        queue.resolve(
                                             (
                                                 None,
                                                 VacuumError(
                                                     error.get("code"),
                                                     error.get("message"),
                                                 ),
-                                            ),
-                                            timeout=QUEUE_TIMEOUT,
+                                            )
                                         )
                                     else:
                                         result = data_point_response.get("result")
                                         if isinstance(result, list) and len(result) == 1:
                                             result = result[0]
-                                        await queue.async_put((result, None), timeout=QUEUE_TIMEOUT)
+                                        queue.resolve((result, None))
                 elif protocol == 301:
                     payload = data.payload[0:24]
                     [endpoint, _, request_id, _] = struct.unpack("<15sBH6s", payload)
                     if endpoint.decode().startswith(self._endpoint):
                         iv = bytes(AES.block_size)
                         decipher = AES.new(self._nonce, AES.MODE_CBC, iv)
                         decrypted = unpad(decipher.decrypt(data.payload[24:]), AES.block_size)
                         decrypted = gzip.decompress(decrypted)
                         queue = self._waiting_queue.get(request_id)
                         if queue:
                             if isinstance(decrypted, list):
                                 decrypted = decrypted[0]
-                            await queue.async_put((decrypted, None), timeout=QUEUE_TIMEOUT)
+                            queue.resolve((decrypted, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
     async def _async_response(self, request_id: int, protocol_id: int = 0) -> tuple[Any, VacuumError | None]:
         try:
-            queue = RoborockQueue(protocol_id)
+            queue = RoborockFuture(protocol_id)
             self._waiting_queue[request_id] = queue
             (response, err) = await queue.async_get(QUEUE_TIMEOUT)
             return response, err
         except (asyncio.TimeoutError, asyncio.CancelledError):
             raise RoborockTimeout(f"Timeout after {QUEUE_TIMEOUT} seconds waiting for response") from None
         finally:
             del self._waiting_queue[request_id]
```

### Comparing `python_roborock-0.6.6/roborock/cli.py` & `python_roborock-0.6.7/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/cloud_api.py` & `python_roborock-0.6.7/roborock/cloud_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 import paho.mqtt.client as mqtt
 
 from roborock.api import SPECIAL_COMMANDS, RoborockClient, md5hex
 from roborock.exceptions import CommandVacuumError, RoborockException, VacuumError
 
 from .containers import RoborockDeviceInfo, UserData
 from .roborock_message import RoborockMessage, RoborockParser, md5bin
-from .roborock_queue import RoborockQueue
+from .roborock_future import RoborockFuture
 from .typing import RoborockCommand
-from .util import run_in_executor
 
 _LOGGER = logging.getLogger(__name__)
-QUEUE_TIMEOUT = 4
 MQTT_KEEPALIVE = 60
+CONNECT_REQUEST_ID = 0
+DISCONNECT_REQUEST_ID = 1
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
 
     def __init__(self, user_data: UserData, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
         rriot = user_data.rriot
@@ -44,73 +44,70 @@
         self._mqtt_ssl = url.scheme == "ssl"
         if self._mqtt_ssl:
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
         super().username_pw_set(self._hashed_user, self._hashed_password)
         self._endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
-        self._waiting_queue: dict[int, RoborockQueue] = {}
+        self._waiting_queue: dict[int, RoborockFuture] = {}
         self._mutex = Lock()
         self._last_device_msg_in = mqtt.time_func()
         self._last_disconnection = mqtt.time_func()
         self.update_client_id()
 
     def __del__(self) -> None:
         self.sync_disconnect()
 
-    @run_in_executor()
-    async def on_connect(self, _client, _, __, rc, ___=None) -> None:
-        connection_queue = self._waiting_queue.get(0)
+    def on_connect(self, *args, **kwargs) -> None:
+        _, __, ___, rc, ____ = args
+        connection_queue = self._waiting_queue.get(CONNECT_REQUEST_ID)
         if rc != mqtt.MQTT_ERR_SUCCESS:
             message = f"Failed to connect (rc: {rc})"
             _LOGGER.error(message)
             if connection_queue:
-                await connection_queue.async_put((None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT)
+                connection_queue.resolve((None, VacuumError(rc, message)))
             return
         _LOGGER.info(f"Connected to mqtt {self._mqtt_host}:{self._mqtt_port}")
         topic = f"rr/m/o/{self._mqtt_user}/{self._hashed_user}/#"
         (result, mid) = self.subscribe(topic)
         if result != 0:
             message = f"Failed to subscribe (rc: {result})"
             _LOGGER.error(message)
             if connection_queue:
-                await connection_queue.async_put((None, VacuumError(rc, message)), timeout=QUEUE_TIMEOUT)
+                connection_queue.resolve((None, VacuumError(rc, message)))
             return
         _LOGGER.info(f"Subscribed to topic {topic}")
         if connection_queue:
-            await connection_queue.async_put((True, None), timeout=QUEUE_TIMEOUT)
+            connection_queue.resolve((True, None))
 
-    @run_in_executor()
-    async def on_message(self, _client, _, msg, __=None) -> None:
-        async with self._mutex:
-            self._last_device_msg_in = mqtt.time_func()
+    def on_message(self, *args, **kwargs) -> None:
+        _, __, msg = args
+        self._last_device_msg_in = mqtt.time_func()
         device_id = msg.topic.split("/").pop()
         messages, _ = RoborockParser.decode(msg.payload, self.devices_info[device_id].device.local_key)
-        await super().on_message(messages)
+        super().on_message(messages)
 
-    @run_in_executor()
-    async def on_disconnect(self, _client: mqtt.Client, _, rc, __=None) -> None:
+    def on_disconnect(self, *args, **kwargs) -> None:
         try:
+            _, __, rc, ___ = args
             self._last_disconnection = mqtt.time_func()
             message = f"Roborock mqtt client disconnected (rc: {rc})"
             if rc == mqtt.MQTT_ERR_PROTOCOL:
                 self.update_client_id()
             _LOGGER.warning(message)
-            connection_queue = self._waiting_queue.get(1)
+            connection_queue = self._waiting_queue.get(DISCONNECT_REQUEST_ID)
             if connection_queue:
-                await connection_queue.async_put((True, None), timeout=QUEUE_TIMEOUT)
+                connection_queue.resolve((True, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
     def update_client_id(self):
         self._client_id = mqtt.base62(uuid.uuid4().int, padding=22)
 
-    @run_in_executor()
-    async def _async_check_keepalive(self) -> None:
-        async with self._mutex:
+    def _async_check_keepalive(self) -> None:
             now = mqtt.time_func()
             # noinspection PyUnresolvedReferences
             if (
                 now - self._last_disconnection > self._keepalive**2  # type: ignore[attr-defined]
                 and now - self._last_device_msg_in > self._keepalive  # type: ignore[attr-defined]
             ):
                 self._ping_t = self._last_device_msg_in
@@ -152,24 +149,24 @@
                 raise RoborockException(f"Failed to connect (rc:{rc})")
         return rc == mqtt.MQTT_ERR_SUCCESS
 
     async def async_disconnect(self) -> Any:
         async with self._mutex:
             disconnecting = self.sync_disconnect()
             if disconnecting:
-                (response, err) = await self._async_response(1)
+                (response, err) = await self._async_response(DISCONNECT_REQUEST_ID)
                 if err:
                     raise RoborockException(err) from err
                 return response
 
     async def async_connect(self) -> Any:
         async with self._mutex:
             connecting = self.sync_connect()
             if connecting:
-                (response, err) = await self._async_response(0)
+                (response, err) = await self._async_response(CONNECT_REQUEST_ID)
                 if err:
                     raise RoborockException(err) from err
                 return response
 
     async def validate_connection(self) -> None:
         await self.async_connect()
```

### Comparing `python_roborock-0.6.6/roborock/code_mappings.py` & `python_roborock-0.6.7/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/containers.py` & `python_roborock-0.6.7/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/exceptions.py` & `python_roborock-0.6.7/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/local_api.py` & `python_roborock-0.6.7/roborock/local_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 class RoborockSocketListener:
     roborock_port = 58867
 
     def __init__(
         self,
         ip: str,
         local_key: str,
-        on_message: Callable[[list[RoborockMessage]], Awaitable[Any]],
+        on_message: Callable[[list[RoborockMessage]], None],
         timeout: float | int = 4,
     ):
         self.ip = ip
         self.local_key = local_key
         self.socket = RoborockSocket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket.setblocking(False)
         self.loop = get_running_loop_or_create_one()
@@ -130,15 +130,15 @@
                 message = await self.loop.sock_recv(self.socket, 4096)
                 try:
                     if self.remaining:
                         message = self.remaining + message
                         self.remaining = b""
                     (parser_msg, remaining) = RoborockParser.decode(message, self.local_key)
                     self.remaining = remaining
-                    await self.on_message(parser_msg)
+                    self.on_message(parser_msg)
                 except Exception as e:
                     _LOGGER.exception(e)
             except BrokenPipeError as e:
                 _LOGGER.exception(e)
                 await self.disconnect()
 
     async def connect(self):
```

### Comparing `python_roborock-0.6.6/roborock/roborock_message.py` & `python_roborock-0.6.7/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/roborock_queue.py` & `python_roborock-0.6.7/roborock/roborock_future.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-from asyncio import Queue
+from asyncio import Future
 from typing import Any
 
 import async_timeout
 
 from .exceptions import VacuumError
 
 
-class RoborockQueue(Queue):
-    def __init__(self, protocol: int, *args):
-        super().__init__(*args)
+class RoborockFuture:
+    def __init__(self, protocol: int):
         self.protocol = protocol
+        self.fut = Future()
+        self.loop = self.fut.get_loop()
 
-    async def async_put(self, item: tuple[Any, VacuumError | None], timeout: float | int) -> None:
-        async with async_timeout.timeout(timeout):
-            await self.put(item)
+    def resolve(self, item: tuple[Any, VacuumError | None]) -> None:
+        self.loop.call_soon_threadsafe(self.fut.set_result, item)
 
     async def async_get(self, timeout: float | int) -> tuple[Any, VacuumError | None]:
         async with async_timeout.timeout(timeout):
-            return await self.get()
+            return await self.fut
```

### Comparing `python_roborock-0.6.6/roborock/typing.py` & `python_roborock-0.6.7/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.6/roborock/util.py` & `python_roborock-0.6.7/roborock/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,14 @@
         loop = asyncio.get_event_loop()
     except RuntimeError:
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
     return loop
 
 
-def run_in_executor():
-    loop = get_running_loop_or_create_one()
-
-    def decorator(func):
-        @functools.wraps(func)
-        def wrapped(*args, **kwargs):
-            return asyncio.run_coroutine_threadsafe(coro=func(*args, **kwargs), loop=loop)
-
-        return wrapped
-
-    return decorator
-
-
 def run_sync():
     loop = get_running_loop_or_create_one()
 
     def decorator(func):
         @functools.wraps(func)
         def wrapped(*args, **kwargs):
             return loop.run_until_complete(func(*args, **kwargs))
```

### Comparing `python_roborock-0.6.6/PKG-INFO` & `python_roborock-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.6
+Version: 0.6.7
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.6 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.7 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

