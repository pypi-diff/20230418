# Comparing `tmp/streamdeck_sdk-0.2.1.tar.gz` & `tmp/streamdeck_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeck_sdk-0.2.1.tar", last modified: Mon Mar 20 10:28:44 2023, max compression
+gzip compressed data, was "streamdeck_sdk-0.3.0.tar", last modified: Tue Apr 18 14:28:10 2023, max compression
```

## Comparing `streamdeck_sdk-0.2.1.tar` & `streamdeck_sdk-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-03-20 10:28:44.472950 streamdeck_sdk-0.2.1/
--rw-r--r--   0 grisha     (501) staff       (20)    11357 2023-03-09 11:40:53.000000 streamdeck_sdk-0.2.1/LICENSE
--rw-r--r--   0 grisha     (501) staff       (20)     2056 2023-03-20 10:28:44.472829 streamdeck_sdk-0.2.1/PKG-INFO
--rw-r--r--   0 grisha     (501) staff       (20)     1327 2023-03-16 17:17:48.000000 streamdeck_sdk-0.2.1/README.md
--rw-r--r--   0 grisha     (501) staff       (20)       38 2023-03-20 10:28:44.472987 streamdeck_sdk-0.2.1/setup.cfg
--rw-r--r--   0 grisha     (501) staff       (20)     1367 2023-03-20 10:26:06.000000 streamdeck_sdk-0.2.1/setup.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-03-20 10:28:44.468626 streamdeck_sdk-0.2.1/src/
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-03-20 10:28:44.471063 streamdeck_sdk-0.2.1/src/streamdeck_sdk/
--rw-r--r--   0 grisha     (501) staff       (20)      277 2023-03-15 00:54:43.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/__init__.py
--rw-r--r--   0 grisha     (501) staff       (20)     3222 2023-03-16 10:50:56.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/event_routings.py
--rw-r--r--   0 grisha     (501) staff       (20)     4918 2023-03-15 21:21:09.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/events_received_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)     2245 2023-03-09 13:37:45.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/events_sent_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)     1312 2023-03-20 10:22:19.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/logger.py
--rw-r--r--   0 grisha     (501) staff       (20)     6588 2023-03-16 11:47:54.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/mixins.py
--rw-r--r--   0 grisha     (501) staff       (20)      888 2023-03-12 22:52:39.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/registration_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)     7209 2023-03-20 10:26:06.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/sdk.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-03-20 10:28:44.472256 streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/
--rw-r--r--   0 grisha     (501) staff       (20)      125 2023-03-15 00:54:43.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/__init__.py
--rw-r--r--   0 grisha     (501) staff       (20)      620 2023-03-12 23:47:41.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/image_converters.py
--rw-r--r--   0 grisha     (501) staff       (20)     1056 2023-03-15 10:59:31.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/in_separate_thread.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-03-20 10:28:44.471706 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/
--rw-r--r--   0 grisha     (501) staff       (20)     2056 2023-03-20 10:28:44.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/PKG-INFO
--rw-r--r--   0 grisha     (501) staff       (20)      638 2023-03-20 10:28:44.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 grisha     (501) staff       (20)        1 2023-03-20 10:28:44.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 grisha     (501) staff       (20)       83 2023-03-20 10:28:44.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/requires.txt
--rw-r--r--   0 grisha     (501) staff       (20)       15 2023-03-20 10:28:44.000000 streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.091638 streamdeck_sdk-0.3.0/
+-rw-r--r--   0 grisha     (501) staff       (20)    11357 2023-03-09 11:40:53.000000 streamdeck_sdk-0.3.0/LICENSE
+-rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-04-18 14:28:10.091511 streamdeck_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 grisha     (501) staff       (20)     1924 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/README.md
+-rw-r--r--   0 grisha     (501) staff       (20)       38 2023-04-18 14:28:10.091677 streamdeck_sdk-0.3.0/setup.cfg
+-rw-r--r--   0 grisha     (501) staff       (20)     1367 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/setup.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.087964 streamdeck_sdk-0.3.0/src/
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.089475 streamdeck_sdk-0.3.0/src/streamdeck_sdk/
+-rw-r--r--   0 grisha     (501) staff       (20)      258 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1650 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/event_routings.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1531 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/logger.py
+-rw-r--r--   0 grisha     (501) staff       (20)     6902 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/mixins.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.090604 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/
+-rw-r--r--   0 grisha     (501) staff       (20)       98 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)     5392 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_received_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)     2245 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_sent_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)      888 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/registration_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)     7342 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sdk.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.091288 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/
+-rw-r--r--   0 grisha     (501) staff       (20)      125 2023-03-15 00:54:43.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)      620 2023-03-12 23:47:41.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/image_converters.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1110 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/in_separate_thread.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.090060 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/
+-rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 grisha     (501) staff       (20)      701 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 grisha     (501) staff       (20)        1 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 grisha     (501) staff       (20)       83 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/requires.txt
+-rw-r--r--   0 grisha     (501) staff       (20)       15 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/top_level.txt
```

### Comparing `streamdeck_sdk-0.2.1/LICENSE` & `streamdeck_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.2.1/PKG-INFO` & `streamdeck_sdk-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck_sdk
-Version: 0.2.1
+Version: 0.3.0
 Summary: Library for creating Stream Deck plugins in Python.
 Home-page: https://github.com/gri-gus/streamdeck-python-sdk
 Author: Grigoriy Gusev
 Author-email: thegrigus@gmail.com
 License: Apache Software License
 Keywords: python,sdk,streamdeck,streamdeck-sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <a>
-        <img src="https://raw.githubusercontent.com/gri-gus/streamdeck-python-sdk/main/assets/images/cover.png" alt="decohints">
+        <img src="https://raw.githubusercontent.com/gri-gus/streamdeck-python-sdk/main/assets/images/cover.png" alt="streamdeck-python-sdk">
     </a>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/streamdeck-sdk" target="_blank">
         <img src="https://img.shields.io/pypi/v/streamdeck-sdk" alt="PyPI">
     </a>
@@ -59,10 +59,24 @@
 
 or
 
 ```shell
 pip install streamdeck_sdk
 ```
 
+## Features
+
+* Easy use. You can quickly create your own plugin without having to understand how websockets and other complicated
+  things work.
+* Fully typed, using [pydantic](https://github.com/pydantic/pydantic).
+* Includes image to base64 converters for easy installation of icons on keys.
+* Includes a decorator for functions and methods to run on a separate thread.
+* Exception logging and easy logging configuration.
+
+## Examples
+
+[LoremFlickr](https://github.com/gri-gus/loremflickr-streamdeck-plugin) - Plugin for installing images from LoremFlickr
+to button. Supports MacOS and Windows.
+
 ---
-> 🧑‍💻 Documentation and examples under development
+> 🧑‍💻 Documentation under development
```

#### html2text {}

```diff
@@ -1,18 +1,26 @@
-Metadata-Version: 2.1 Name: streamdeck_sdk Version: 0.2.1 Summary: Library for
+Metadata-Version: 2.1 Name: streamdeck_sdk Version: 0.3.0 Summary: Library for
 creating Stream Deck plugins in Python. Home-page: https://github.com/gri-gus/
 streamdeck-python-sdk Author: Grigoriy Gusev Author-email: thegrigus@gmail.com
 License: Apache Software License Keywords: python,sdk,streamdeck,streamdeck-
 sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream
 deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE
-                                  [decohints]
+                            [streamdeck-python-sdk]
                         [PyPI] [PyPI] [Apache] [Elgato]
 # streamdeck-python-sdk Library for creating Stream Deck plugins in Python.
 **PyPi**: https://pypi.org/project/streamdeck-sdk/ **Supported operating
 systems:** * MacOS: 10.14 or later * Windows: 10 or later **Supported Stream
 Deck application:** 6.0, 6.1 **Supported Python:** 3.7 or later ## Installation
 ```shell pip install streamdeck-sdk ``` or ```shell pip install streamdeck_sdk
-``` --- > ð§âð» Documentation and examples under development
+``` ## Features * Easy use. You can quickly create your own plugin without
+having to understand how websockets and other complicated things work. * Fully
+typed, using [pydantic](https://github.com/pydantic/pydantic). * Includes image
+to base64 converters for easy installation of icons on keys. * Includes a
+decorator for functions and methods to run on a separate thread. * Exception
+logging and easy logging configuration. ## Examples [LoremFlickr](https://
+github.com/gri-gus/loremflickr-streamdeck-plugin) - Plugin for installing
+images from LoremFlickr to button. Supports MacOS and Windows. --- >
+ð§âð» Documentation under development
```

### Comparing `streamdeck_sdk-0.2.1/setup.py` & `streamdeck_sdk-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.2.1"
+VERSION = "0.3.0"
 PACKAGE_DIR = "src"
 REQUIREMENTS_FILE = PACKAGE_DIR + "/requirements.txt"
 README = "README.md"
 
 with open(REQUIREMENTS_FILE, "r") as f:
     requirements = f.read().splitlines()
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/events_received_objs.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_received_objs.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,26 @@
 class TouchTapPayload(BaseModel):
     settings: dict
     coordinates: KeyCoordinates
     tapPos: list
     hold: bool
 
 
+class DialDownPayload(BaseModel):
+    controller: str
+    settings: str
+    coordinates: KeyCoordinates
+
+
+class DialUpPayload(BaseModel):
+    controller: str
+    settings: str
+    coordinates: KeyCoordinates
+
+
 # endregion NestedModels
 
 # region Models
 class DidReceiveSettings(BaseModel):
     action: str
     context: str
     device: str
@@ -151,14 +163,30 @@
     action: str
     context: str
     device: str
     payload: TouchTapPayload
     event: str = "touchTap"
 
 
+class DialDown(BaseModel):
+    action: str
+    context: str
+    device: str
+    payload: DialDownPayload
+    event: str = "dialDown"
+
+
+class DialUp(BaseModel):
+    action: str
+    context: str
+    device: str
+    payload: DialUpPayload
+    event: str = "dialUp"
+
+
 class DialPress(BaseModel):
     action: str
     context: str
     device: str
     payload: DialPressPayload
     event: str = "dialPress"
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/events_sent_objs.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_sent_objs.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/logger.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 from functools import wraps
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 from decohints import decohints
 
-logger: logging.Logger = logging.getLogger('default')
+_root_logger: logging.Logger = logging.getLogger()
+_log_errors_decorator_logger = logging.getLogger("log_errors_decorator")
+logger = logging.getLogger("streamdeck_plugin")
 
 
-def init_logger(
+def init_root_logger(
         log_file: Path,
         log_level: int = logging.DEBUG,
         log_max_bytes: int = 3 * 1024 * 1024,
         log_backup_count: int = 2,
 ) -> None:
-    logger.setLevel(log_level)
+    _root_logger.setLevel(log_level)
     logs_dir: Path = log_file.parent
     logs_dir.mkdir(parents=True, exist_ok=True)
     rfh = RotatingFileHandler(
         log_file,
         mode='a',
         maxBytes=log_max_bytes,
         backupCount=log_backup_count,
@@ -26,26 +28,30 @@
         delay=False,
     )
     rfh.setLevel(logging.DEBUG)
     formatter = logging.Formatter(
         "%(asctime)s - [%(levelname)s] - %(name)s - (%(filename)s).%(funcName)s(%(lineno)d): %(message)s"
     )
     rfh.setFormatter(formatter)
-    logger.addHandler(rfh)
+    _root_logger.addHandler(rfh)
 
 
 @decohints
 def log_errors(func):
     """
     A decorator that logs and suppresses errors in the function being decorated.
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             result = func(*args, **kwargs)
         except BaseException as err:
-            logger.error(str(err), exc_info=True)
+            _log_errors_decorator_logger.error(str(err), exc_info=True)
             return
         return result
 
     return wrapper
+
+
+def rename_plugin_logger(name: str):
+    logger.name = name
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/mixins.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 from typing import Union
 
 import pydantic
 import websocket
 from websocket import ABNF
 
-from . import events_received_objs
-from . import events_sent_objs
+from .sd_objs import events_received_objs, events_sent_objs
 from .logger import log_errors
 
 
 class SendMixin:
     ws: websocket.WebSocketApp
 
     @log_errors
@@ -22,15 +21,19 @@
         if isinstance(data, pydantic.BaseModel):
             data = data.json(ensure_ascii=False)
         elif isinstance(data, dict):
             data = json.dumps(data, ensure_ascii=False)
         self.ws.send(data, opcode)
 
 
-class PluginEventsSentMixin(SendMixin):
+class BaseEventSendMixin(SendMixin):
+    pass
+
+
+class PluginEventsSendMixin(BaseEventSendMixin):
     plugin_uuid: str
 
     def set_global_settings(self, payload: dict) -> None:
         message = events_sent_objs.SetGlobalSettings(
             context=self.plugin_uuid,
             payload=payload,
         )
@@ -69,15 +72,15 @@
             payload=events_sent_objs.SwitchToProfilePayload(
                 profile=profile,
             ),
         )
         self.send(message)
 
 
-class ActionEventsSentMixin(SendMixin):
+class ActionEventsSendMixin(BaseEventSendMixin):
     def set_settings(
             self,
             context: str,
             payload: dict,
     ) -> None:
         message = events_sent_objs.SetSettings(
             context=context,
@@ -181,27 +184,37 @@
             action=action,
             context=context,
             payload=payload
         )
         self.send(message)
 
 
-class ActionEventHandlersMixin:
+class BaseEventHandlerMixin:
+    pass
+
+
+class ActionEventHandlersMixin(BaseEventHandlerMixin):
     def on_did_receive_settings(self, obj: events_received_objs.DidReceiveSettings) -> None:
         pass
 
     def on_key_down(self, obj: events_received_objs.KeyDown) -> None:
         pass
 
     def on_key_up(self, obj: events_received_objs.KeyUp) -> None:
         pass
 
     def on_touch_tap(self, obj: events_received_objs.TouchTap) -> None:
         pass
 
+    def on_dial_down(self, obj: events_received_objs.DialDown) -> None:
+        pass
+
+    def on_dial_up(self, obj: events_received_objs.DialUp) -> None:
+        pass
+
     def on_dial_press(self, obj: events_received_objs.DialPress) -> None:
         pass
 
     def on_dial_rotate(self, obj: events_received_objs.DialRotate) -> None:
         pass
 
     def on_will_appear(self, obj: events_received_objs.WillAppear) -> None:
@@ -222,15 +235,15 @@
     def on_send_to_plugin(self, obj: events_received_objs.SendToPlugin) -> None:
         pass
 
     def on_send_to_property_inspector(self, obj: events_received_objs.SendToPropertyInspector) -> None:
         pass
 
 
-class PluginEventHandlersMixin:
+class PluginEventHandlersMixin(BaseEventHandlerMixin):
     def on_did_receive_global_settings(self, obj: events_received_objs.DidReceiveGlobalSettings) -> None:
         pass
 
     def on_device_did_connect(self, obj: events_received_objs.DeviceDidConnect) -> None:
         pass
 
     def on_device_did_disconnect(self, obj: events_received_objs.DeviceDidDisconnect) -> None:
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/registration_objs.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/registration_objs.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/sdk.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 import argparse
 import json
 import logging
 from pathlib import Path
-from typing import Optional, Callable, List
+from typing import Optional, Callable, List, Dict
 
 import pydantic
 import websocket
 
-from . import registration_objs
-from .event_routings import (
-    EventRoutingObj,
-    ACTION_EVENT_ROUTING_MAP,
-    EVENT_ROUTING_MAP,
-    PLUGIN_EVENT_ROUTING_MAP,
-)
-from .logger import logger, init_logger, log_errors
-from .mixins import (
-    PluginEventHandlersMixin,
-    ActionEventHandlersMixin,
-    PluginEventsSentMixin,
-    ActionEventsSentMixin,
-    SendMixin,
+from . import event_routings
+from . import mixins
+from .logger import (
+    init_root_logger,
+    log_errors,
+    rename_plugin_logger,
 )
+from .sd_objs import registration_objs
 
 
 class Base(
-    PluginEventHandlersMixin,
-    ActionEventHandlersMixin,
-    PluginEventsSentMixin,
-    ActionEventsSentMixin,
-    SendMixin,
+    mixins.PluginEventHandlersMixin,
+    mixins.ActionEventHandlersMixin,
+    mixins.PluginEventsSendMixin,
+    mixins.ActionEventsSendMixin,
+    mixins.SendMixin,
 ):
     pass
 
 
+logger = logging.getLogger(__name__)
+
+
 class Action(Base):
     UUID: str  # Required
 
     def __init__(self):
         self.plugin_uuid: Optional[str] = None
         self.ws: Optional[websocket.WebSocketApp] = None
         self.info: Optional[registration_objs.Info] = None
 
 
 class StreamDeck(Base):
     def __init__(
             self,
-            actions: List[Action] = None,
+            actions: Optional[List[Action]] = None,
             *,
-            log_file: Path = None,
+            log_file: Optional[Path] = None,
             log_level: int = logging.DEBUG,
-            log_max_bytes: int = 3 * 1024 * 1024,
+            log_max_bytes: int = 3 * 1024 * 1024,  # 3 MB
             log_backup_count: int = 2,
     ):
         if log_file is not None:
             self.log_file: Path = Path(log_file)
-            init_logger(
+            init_root_logger(
                 log_file=self.log_file,
                 log_level=log_level,
                 log_max_bytes=log_max_bytes,
                 log_backup_count=log_backup_count,
             )
 
         self.actions_list = actions
-        self.actions = {}
+        self.actions: Dict[str, Action] = {}
 
         self.ws: Optional[websocket.WebSocketApp] = None
         self.port: Optional[int] = None
         self.plugin_uuid: Optional[str] = None
         self.register_event: Optional[str] = None
-        self.info: [registration_objs.Info] = None
+        self.info: Optional[registration_objs.Info] = None
 
         self.registration_dict: Optional[dict] = None
 
     @log_errors
     def ws_on_open(
             self,
             ws: websocket.WebSocketApp,  # noqa
@@ -99,77 +95,77 @@
     ) -> None:
         message_dict = json.loads(message)
         logger.debug(f"{message_dict=}")
 
         event = message_dict["event"]
         logger.debug(f"{event=}")
 
-        event_routing = EVENT_ROUTING_MAP.get(event)
+        event_routing = event_routings.EVENT_ROUTING_MAP.get(event)
         if event_routing is None:
             logger.warning("event_routing is None")
             return
 
-        obj = event_routing.obj.parse_obj(message_dict)
+        obj = event_routing.obj_type.parse_obj(message_dict)
         logger.debug(f"{obj=}")
 
-        self.route_plugin_event_in_plugin_handler(event_routing=event_routing, obj=obj)
-        if event in ACTION_EVENT_ROUTING_MAP:
+        self.route_event_in_plugin_handler(event_routing=event_routing, obj=obj)
+        if event_routing.type is event_routings.EventRoutingObjTypes.ACTION:
             self.route_action_event_in_action_handler(event_routing=event_routing, obj=obj)
-        elif event in PLUGIN_EVENT_ROUTING_MAP:
-            self.route_plugin_event_in_actions_handler(event_routing=event_routing, obj=obj)
+        elif event_routing.type is event_routings.EventRoutingObjTypes.PLUGIN:
+            self.route_plugin_event_in_action_handlers(event_routing=event_routing, obj=obj)
 
     @log_errors
     def ws_on_error(
             self,
             ws: websocket.WebSocketApp,  # noqa
             error: str,
     ) -> None:
         logger.error(f"{error=}")
 
     @log_errors
-    def route_plugin_event_in_plugin_handler(
+    def route_event_in_plugin_handler(
             self,
-            event_routing: EventRoutingObj,
+            event_routing: event_routings.EventRoutingObj,
             obj: pydantic.BaseModel,
     ) -> None:
         try:
             handler: Callable = getattr(self, event_routing.handler_name)
         except AttributeError as err:
             logger.error(f"Handler missing: {str(err)}", exc_info=True)
             return
         handler(obj=obj)
 
     @log_errors
     def route_action_event_in_action_handler(
             self,
-            event_routing: EventRoutingObj,
+            event_routing: event_routings.EventRoutingObj,
             obj: pydantic.BaseModel,
     ) -> None:
         try:
             action_uuid = getattr(obj, "action")
         except AttributeError as err:
             logger.error(str(err), exc_info=True)
             return
 
         action_obj = self.actions.get(action_uuid)
         if action_obj is None:
-            logger.info(f"{action_uuid=} not registered")
+            logger.warning(f"{action_uuid=} not registered")
             return
 
         try:
             handler: Callable = getattr(action_obj, event_routing.handler_name)
         except AttributeError as err:
             logger.error(f"Handler missing: {str(err)}", exc_info=True)
             return
         handler(obj=obj)
 
     @log_errors
-    def route_plugin_event_in_actions_handler(
+    def route_plugin_event_in_action_handlers(
             self,
-            event_routing: EventRoutingObj,
+            event_routing: event_routings.EventRoutingObj,
             obj: pydantic.BaseModel,
     ) -> None:
         for action_obj in self.actions.values():
             try:
                 handler: Callable = getattr(action_obj, event_routing.handler_name)
             except AttributeError as err:
                 logger.error(f"Handler missing: {str(err)}", exc_info=True)
@@ -193,14 +189,16 @@
         self.plugin_uuid: str = args.pluginUUID
         logger.debug(f"{self.plugin_uuid=}")
         self.register_event: str = args.registerEvent
         logger.debug(f"{self.register_event=}")
         self.info: registration_objs.Info = registration_objs.Info.parse_obj(json.loads(args.info))
         logger.debug(f"{self.info=}")
 
+        rename_plugin_logger(name=self.info.plugin.uuid)
+
         self.registration_dict = {"event": self.register_event, "uuid": self.plugin_uuid}
         logger.debug(f"{self.registration_dict=}")
         self.ws = websocket.WebSocketApp(
             'ws://localhost:' + str(self.port),
             on_message=self.ws_on_message,
             on_error=self.ws_on_error,
             on_close=self.ws_on_close,
@@ -215,13 +213,13 @@
 
         for action in self.actions_list:
             try:
                 action_uuid = action.UUID
             except AttributeError:
                 action_class = str(action.__class__)
                 message = f"{action_class} must have attribute UUID"
-                logger.error(message)
+                logger.error(message, exc_info=True)
                 raise AttributeError(message)
             action.ws = self.ws
             action.plugin_uuid = self.plugin_uuid
             action.info = self.info
             self.actions[action_uuid] = action
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/image_converters.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/image_converters.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk/utils/in_separate_thread.py` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/in_separate_thread.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+from functools import wraps
 from threading import Thread
 from typing import Callable, Optional
-from functools import wraps
 
 
 class ThreadingFunc:
     def __init__(
             self,
             func: Callable,
             *,
             daemon: Optional[bool] = None,
     ):
         self.func = func
         self.daemon = daemon
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> Thread:
         thread = Thread(target=self.func, args=args, kwargs=kwargs, daemon=self.daemon)
         thread.start()
+        return thread
 
 
 def in_separate_thread(daemon: Optional[bool] = None):
     """
     Decorator for executing the decorated function on a separate thread.
 
-    :param daemon: a daemon thread (True) or not (False). Its initial value is inherited from the creating thread.
+    :param daemon: A daemon thread (True) or not (False). If None, then its initial value is inherited
+        from the creating thread.
     """
 
     def _decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return ThreadingFunc(func=func, daemon=_daemon)(*args, **kwargs)
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/PKG-INFO` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck-sdk
-Version: 0.2.1
+Version: 0.3.0
 Summary: Library for creating Stream Deck plugins in Python.
 Home-page: https://github.com/gri-gus/streamdeck-python-sdk
 Author: Grigoriy Gusev
 Author-email: thegrigus@gmail.com
 License: Apache Software License
 Keywords: python,sdk,streamdeck,streamdeck-sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <a>
-        <img src="https://raw.githubusercontent.com/gri-gus/streamdeck-python-sdk/main/assets/images/cover.png" alt="decohints">
+        <img src="https://raw.githubusercontent.com/gri-gus/streamdeck-python-sdk/main/assets/images/cover.png" alt="streamdeck-python-sdk">
     </a>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/streamdeck-sdk" target="_blank">
         <img src="https://img.shields.io/pypi/v/streamdeck-sdk" alt="PyPI">
     </a>
@@ -59,10 +59,24 @@
 
 or
 
 ```shell
 pip install streamdeck_sdk
 ```
 
+## Features
+
+* Easy use. You can quickly create your own plugin without having to understand how websockets and other complicated
+  things work.
+* Fully typed, using [pydantic](https://github.com/pydantic/pydantic).
+* Includes image to base64 converters for easy installation of icons on keys.
+* Includes a decorator for functions and methods to run on a separate thread.
+* Exception logging and easy logging configuration.
+
+## Examples
+
+[LoremFlickr](https://github.com/gri-gus/loremflickr-streamdeck-plugin) - Plugin for installing images from LoremFlickr
+to button. Supports MacOS and Windows.
+
 ---
-> 🧑‍💻 Documentation and examples under development
+> 🧑‍💻 Documentation under development
```

#### html2text {}

```diff
@@ -1,18 +1,26 @@
-Metadata-Version: 2.1 Name: streamdeck-sdk Version: 0.2.1 Summary: Library for
+Metadata-Version: 2.1 Name: streamdeck-sdk Version: 0.3.0 Summary: Library for
 creating Stream Deck plugins in Python. Home-page: https://github.com/gri-gus/
 streamdeck-python-sdk Author: Grigoriy Gusev Author-email: thegrigus@gmail.com
 License: Apache Software License Keywords: python,sdk,streamdeck,streamdeck-
 sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream
 deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE
-                                  [decohints]
+                            [streamdeck-python-sdk]
                         [PyPI] [PyPI] [Apache] [Elgato]
 # streamdeck-python-sdk Library for creating Stream Deck plugins in Python.
 **PyPi**: https://pypi.org/project/streamdeck-sdk/ **Supported operating
 systems:** * MacOS: 10.14 or later * Windows: 10 or later **Supported Stream
 Deck application:** 6.0, 6.1 **Supported Python:** 3.7 or later ## Installation
 ```shell pip install streamdeck-sdk ``` or ```shell pip install streamdeck_sdk
-``` --- > ð§âð» Documentation and examples under development
+``` ## Features * Easy use. You can quickly create your own plugin without
+having to understand how websockets and other complicated things work. * Fully
+typed, using [pydantic](https://github.com/pydantic/pydantic). * Includes image
+to base64 converters for easy installation of icons on keys. * Includes a
+decorator for functions and methods to run on a separate thread. * Exception
+logging and easy logging configuration. ## Examples [LoremFlickr](https://
+github.com/gri-gus/loremflickr-streamdeck-plugin) - Plugin for installing
+images from LoremFlickr to button. Supports MacOS and Windows. --- >
+ð§âð» Documentation under development
```

### Comparing `streamdeck_sdk-0.2.1/src/streamdeck_sdk.egg-info/SOURCES.txt` & `streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 LICENSE
 README.md
 setup.py
 src/streamdeck_sdk/__init__.py
 src/streamdeck_sdk/event_routings.py
-src/streamdeck_sdk/events_received_objs.py
-src/streamdeck_sdk/events_sent_objs.py
 src/streamdeck_sdk/logger.py
 src/streamdeck_sdk/mixins.py
-src/streamdeck_sdk/registration_objs.py
 src/streamdeck_sdk/sdk.py
 src/streamdeck_sdk.egg-info/PKG-INFO
 src/streamdeck_sdk.egg-info/SOURCES.txt
 src/streamdeck_sdk.egg-info/dependency_links.txt
 src/streamdeck_sdk.egg-info/requires.txt
 src/streamdeck_sdk.egg-info/top_level.txt
+src/streamdeck_sdk/sd_objs/__init__.py
+src/streamdeck_sdk/sd_objs/events_received_objs.py
+src/streamdeck_sdk/sd_objs/events_sent_objs.py
+src/streamdeck_sdk/sd_objs/registration_objs.py
 src/streamdeck_sdk/utils/__init__.py
 src/streamdeck_sdk/utils/image_converters.py
 src/streamdeck_sdk/utils/in_separate_thread.py
```

