# Comparing `tmp/ta-cmi-1.4.0.tar.gz` & `tmp/ta-cmi-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-1.4.0.tar", last modified: Wed Jan 25 18:18:40 2023, max compression
+gzip compressed data, was "ta-cmi-2.0.0.dev1.tar", last modified: Tue Apr 18 16:39:08 2023, max compression
```

## Comparing `ta-cmi-1.4.0.tar` & `ta-cmi-2.0.0.dev1.tar`

### file list

```diff
@@ -1,19 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 18:18:40.067926 ta-cmi-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7096 2023-01-25 18:18:40.066926 ta-cmi-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5525 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-25 18:18:40.067926 ta-cmi-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 18:18:40.064926 ta-cmi-1.4.0/ta_cmi/
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/baseApi.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/cmi.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/const.py
--rw-rw-rw-   0 root         (0) root         (0)     4994 2023-01-25 18:18:23.000000 ta-cmi-1.4.0/ta_cmi/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 18:18:40.066926 ta-cmi-1.4.0/ta_cmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7096 2023-01-25 18:18:39.000000 ta-cmi-1.4.0/ta_cmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2023-01-25 18:18:40.000000 ta-cmi-1.4.0/ta_cmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 18:18:39.000000 ta-cmi-1.4.0/ta_cmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-25 18:18:39.000000 ta-cmi-1.4.0/ta_cmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-25 18:18:39.000000 ta-cmi-1.4.0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.693181 ta-cmi-2.0.0.dev1/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 ta-cmi-2.0.0.dev1/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 16:39:08.688911 ta-cmi-2.0.0.dev1/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     5596 2023-01-17 13:17:51.000000 ta-cmi-2.0.0.dev1/README.md
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-04-18 16:39:08.694219 ta-cmi-2.0.0.dev1/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      627 2023-04-18 16:37:21.000000 ta-cmi-2.0.0.dev1/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.342570 ta-cmi-2.0.0.dev1/ta_cmi/
+-rwxrwxrwx   0 user      (1000) user      (1000)      436 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2307 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1122 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      661 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2696 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      610 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1930 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      780 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      494 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3708 2023-01-25 18:14:05.000000 ta-cmi-2.0.0.dev1/ta_cmi/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4459 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/device.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.481565 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      512 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.659793 ta-cmi-2.0.0.dev1/tests/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2854 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      650 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     5036 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      991 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2787 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1074 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    11873 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_device.py
```

### Comparing `ta-cmi-1.4.0/LICENSE` & `ta-cmi-2.0.0.dev1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 DeerMaximum
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 DeerMaximum
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ta-cmi-1.4.0/PKG-INFO` & `ta-cmi-2.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 1.4.0
+Version: 2.0.0.dev1
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `ta-cmi-1.4.0/README.md` & `ta-cmi-2.0.0.dev1/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# TA-CMI
-A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
-
-## How to use package
-
-```python
-import asyncio
-
-from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
-
-
-async def main():
-    try:
-        cmi = CMI("http://192.168.1.101", "admin", "admin")
-
-        devices = await cmi.get_devices()
-
-        device = devices[0]
-
-        # Set type automatically
-        await device.fetch_type()
-
-        # Set type manually
-        device.set_device_type("UVR16x2")
-
-        await device.update()
-
-        print(str(device))
-
-        inputChannels = device.get_channels(ChannelType.INPUT)
-        outputChannels = device.get_channels(ChannelType.OUTPUT)
-        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
-
-        for i in inputChannels:
-            ch = inputChannels.get(i)
-            print(str(ch))
-
-        for o in outputChannels:
-            ch = outputChannels.get(o)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-        for al in analogLogging:
-            ch = analogLogging.get(al)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
-        print(f"Error: {error}")
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-loop.close()
-```
-
-## Supported data types
-
-| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
-|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
-| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
-| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
-| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
-| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-
-> **Note**
+# TA-CMI
+A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+
+## How to use package
+
+```python
+import asyncio
+
+from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
+
+
+async def main():
+    try:
+        cmi = CMI("http://192.168.1.101", "admin", "admin")
+
+        devices = await cmi.get_devices()
+
+        device = devices[0]
+
+        # Set type automatically
+        await device.fetch_type()
+
+        # Set type manually
+        device.set_device_type("UVR16x2")
+
+        await device.update()
+
+        print(str(device))
+
+        inputChannels = device.get_channels(ChannelType.INPUT)
+        outputChannels = device.get_channels(ChannelType.OUTPUT)
+        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
+
+        for i in inputChannels:
+            ch = inputChannels.get(i)
+            print(str(ch))
+
+        for o in outputChannels:
+            ch = outputChannels.get(o)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+        for al in analogLogging:
+            ch = analogLogging.get(al)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
+        print(f"Error: {error}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+loop.close()
+```
+
+## Supported data types
+
+| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
+|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
+| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
+| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
+| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
+| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+
+> **Note**
 > The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
```

### Comparing `ta-cmi-1.4.0/ta_cmi/channel.py` & `ta-cmi-2.0.0.dev1/ta_cmi/channel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-from typing import Any, Dict
-
-from .const import (
-    UNITS_DE,
-    UNITS_EN,
-    ChannelMode,
-    ChannelType,
-    Languages,
-    ReadOnlyClass,
-)
-
-
-class Channel(metaclass=ReadOnlyClass):
-    """Class to display an input or output."""
-
-    def __init__(self, mode: ChannelType, json: Dict[str, Any]) -> None:
-        """Initialize and parse json to get properties."""
-        self.mode: ChannelType = mode
-        self.type: ChannelMode = json["AD"]
-        self.index: int = json["Number"]
-        self.value: float = json["Value"]["Value"]
-        self.unit: str = json["Value"]["Unit"]
-
-    def get_unit(self, language: Languages = Languages.EN) -> str:
-        """Get the unit of the channel."""
-        if language == Languages.EN:
-            return UNITS_EN.get(self.unit, "Unknown")
-        else:
-            return UNITS_DE.get(self.unit, "Unknown")
-
-    def __eq__(self, other) -> bool:
-        return (
-            self.mode == other.mode
-            and self.type == other.type
-            and self.index == other.index
-            and self.value == other.value
-            and self.unit == other.unit
-        )
-
-    def __repr__(self) -> str:
-        return f"Channel {self.index}: Type: {self.type}, Mode: {self.mode}, Value: {self.value} {self.get_unit()}"
+from .const import UNITS_DE, UNITS_EN, ChannelMode, ChannelType, Languages
+
+
+class Channel:
+    """Class to display a data point"""
+
+    def __init__(self) -> None:
+        """Initialize and parse json to get properties."""
+        self.mode: ChannelType | None = None
+        self.type: ChannelMode = ChannelMode.ANALOG
+        self.index: int = 0
+        self.value: float = 0
+        self.unit: str = ""
+
+    def get_unit(self, language: Languages = Languages.EN) -> str:
+        """Get the unit of the channel."""
+        if language == Languages.EN:
+            return UNITS_EN.get(self.unit, "Unknown")
+        else:
+            return UNITS_DE.get(self.unit, "Unknown")
+
+    def __eq__(self, other) -> bool:
+        return (
+            self.mode == other.mode
+            and self.type == other.type
+            and self.index == other.index
+            and self.value == other.value
+            and self.unit == other.unit
+        )
+
+    def __repr__(self) -> str:
+        return f"Channel {self.index}: Type: {self.type}, Mode: {self.mode}, Value: {self.value} {self.get_unit()}"
```

### Comparing `ta-cmi-1.4.0/ta_cmi/device.py` & `ta-cmi-2.0.0.dev1/ta_cmi/device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,149 +1,126 @@
-import asyncio
-from typing import Any, Dict, List
-
-from aiohttp import ClientSession
-
-from .baseApi import BaseAPI
-from .channel import Channel
-from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
-
-
-class Device(BaseAPI):
-    """Class to interact with a device."""
-
-    def __init__(
-        self,
-        node_id: str,
-        host: str,
-        username: str,
-        password: str,
-        session: ClientSession = None,
-    ) -> None:
-        """Initialize."""
-        super().__init__(username, password, session)
-        self.id: str = node_id
-        self.host: str = host
-
-        self.api_version: int = 0
-        self.device_id: str = "00"
-
-        self._channels: Dict[ChannelType, Dict[int, Channel]] = {}
-
-    def _extract_device_info(self, json: Dict[str, Any]) -> None:
-        """Extract device info from request response."""
-        self.api_version: int = json["Header"]["Version"]
-        self.device_id: str = json["Header"]["Device"]
-
-        if self.device_id not in DEVICES.keys():
-            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
-
-    @staticmethod
-    def _extract_channels(
-        mode: ChannelType, raw_channels: List[Dict[str, Any]]
-    ) -> Dict[int, Channel]:
-        """Extract channel info from data array from request."""
-        list_of_channels: Dict[int, Channel] = {}
-        for channel_raw in raw_channels:
-            ch: Channel = Channel(mode, channel_raw)
-            list_of_channels[ch.index] = ch
-
-        return list_of_channels
-
-    def _get_json_params(self) -> str:
-        """Compose json params based on the device type."""
-        default_params = "I,O"
-        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
-
-    async def _make_request_to_device(self) -> Dict[str, Any]:
-        """Make a request to the device."""
-
-        params = self._get_json_params()
-
-        data: dict[str, Any] = {}
-
-        if len(params.split(",")) > 7:
-            first_params = ",".join(params.split(",")[:7])
-            params = ",".join(params.split(",")[7:])
-
-            url_first: str = f"{self.host}/INCLUDE/api.cgi?jsonparam={first_params}&jsonnode={self.id}"
-            _LOGGER.debug(
-                "Make request to device %s from type %s with parameters: %s",
-                self.id,
-                self.device_id,
-                first_params,
-            )
-
-            data = await self._make_request(url_first)
-            await asyncio.sleep(61)
-
-        url: str = f"{self.host}/INCLUDE/api.cgi?jsonparam={params}&jsonnode={self.id}"
-        _LOGGER.debug(
-            "Make request to device %s from type %s with parameters: %s",
-            self.id,
-            self.device_id,
-            params,
-        )
-
-        if len(data.keys()) == 0:
-            return await self._make_request(url)
-
-        data["Data"].update((await self._make_request(url))["Data"])
-
-        return data
-
-    async def fetch_type(self) -> None:
-        """Fetch the device type without parsing the data from the device."""
-        self._extract_device_info(await self._make_request_to_device())
-
-    async def update(self) -> None:
-        """Update data."""
-        _LOGGER.debug("Update device: %s", self.id)
-        res: Dict[str, Any] = await self._make_request_to_device()
-
-        if self.device_id == "00":
-            self._extract_device_info(res)
-            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
-
-        for channel_type_text in res["Data"]:
-            channel_type = ChannelType(channel_type_text)
-            self._channels[channel_type] = self._extract_channels(
-                channel_type, res["Data"][channel_type_text]
-            )
-
-    def get_channels(self, channel_type: ChannelType) -> Dict[int, Channel]:
-        """Get all the fetched channels from a type."""
-        return self._channels[channel_type]
-
-    def has_channel_type(self, channel_type: ChannelType) -> bool:
-        """Check if a channel type was fetched."""
-        return self._channels.get(channel_type, None) is not None
-
-    def set_device_type(self, device_name: str) -> None:
-        """Set the type of the device manually."""
-        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
-
-        if len(type_id) != 1:
-            raise InvalidDeviceError(f"Invalid device name: {device_name}")
-
-        self.device_id = type_id[0]
-
-    def get_device_type(self) -> str:
-        """Get the type of the device."""
-        return DEVICES.get(self.device_id, "Unknown")
-
-    def __repr__(self) -> str:
-        text = f"Node {self.id}: Type: {self.get_device_type()}"
-
-        for channel_type in self._channels:
-            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
-
-        return text
-
-
-class InvalidDeviceError(Exception):
-    """Triggered when an invalid device type is set."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
+import asyncio
+from typing import Any, Dict, List
+
+from .channel import Channel
+from .cmi_api import CMIAPI
+from .cmi_channel import CMIChannel
+from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
+
+
+class Device:
+    """Class to interact with a device."""
+
+    def __init__(self, node_id: str, api: CMIAPI) -> None:
+        """Initialize."""
+        super().__init__()
+
+        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
+
+        self.id = node_id
+        self._api = api
+
+        self.api_version: int = 0
+        self.device_id: str = "00"
+
+    def _extract_device_info(self, json: Dict[str, Any]) -> None:
+        """Extract device info from request response."""
+        self.api_version: int = json["Header"]["Version"]
+        self.device_id: str = json["Header"]["Device"]
+
+        if self.device_id not in DEVICES.keys():
+            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
+
+    @staticmethod
+    def _extract_channels(
+        mode: ChannelType, raw_channels: List[Dict[str, Any]]
+    ) -> Dict[int, CMIChannel]:
+        """Extract channel info from data array from request."""
+        list_of_channels: Dict[int, CMIChannel] = {}
+        for channel_raw in raw_channels:
+            ch: CMIChannel = CMIChannel(mode, channel_raw)
+            list_of_channels[ch.index] = ch
+
+        return list_of_channels
+
+    def _get_json_params(self) -> str:
+        """Compose json params based on the device type."""
+        default_params = "I,O"
+        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
+
+    async def _make_request_to_device(self) -> Dict[str, Any]:
+        """Make a request to the device."""
+        params = self._get_json_params()
+
+        data: dict[str, Any] = {}
+
+        if len(params.split(",")) > 7:
+            first_params = ",".join(params.split(",")[:7])
+            params = ",".join(params.split(",")[7:])
+
+            data = await self._api.get_device_data(self.id, first_params)
+
+            await asyncio.sleep(61)
+
+        if len(data.keys()) == 0:
+            return await self._api.get_device_data(self.id, params)
+
+        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
+
+        return data
+
+    async def fetch_type(self) -> None:
+        """Fetch the device type without parsing the data from the device."""
+        self._extract_device_info(await self._make_request_to_device())
+
+    async def update(self) -> None:
+        """Update data."""
+        _LOGGER.debug("Update device: %s", self.id)
+        res: Dict[str, Any] = await self._make_request_to_device()
+
+        if self.device_id == "00":
+            self._extract_device_info(res)
+            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
+
+        for channel_type_text in res["Data"]:
+            channel_type = ChannelType(channel_type_text)
+            self._channels[channel_type] = self._extract_channels(
+                channel_type, res["Data"][channel_type_text]
+            )
+
+    def set_device_type(self, device_name: str) -> None:
+        """Set the type of the device manually."""
+        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
+
+        if len(type_id) != 1:
+            raise InvalidDeviceError(f"Invalid device name: {device_name}")
+
+        self.device_id = type_id[0]
+
+    def get_device_type(self) -> str:
+        """Get the type of the device."""
+        return DEVICES.get(self.device_id, "Unknown")
+
+    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
+        """Get all the fetched channels from a type."""
+        return self._channels[channel_type]
+
+    def has_channel_type(self, channel_type: ChannelType) -> bool:
+        """Check if a channel type was fetched."""
+        return self._channels.get(channel_type, None) is not None
+
+    def __repr__(self) -> str:
+        text = f"Node {self.id}: Type: {self.get_device_type()}"
+
+        for channel_type in self._channels:
+            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
+
+        return text
+
+
+class InvalidDeviceError(Exception):
+    """Triggered when an invalid device type is set."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
```

### Comparing `ta-cmi-1.4.0/ta_cmi.egg-info/PKG-INFO` & `ta-cmi-2.0.0.dev1/ta_cmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 1.4.0
+Version: 2.0.0.dev1
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

