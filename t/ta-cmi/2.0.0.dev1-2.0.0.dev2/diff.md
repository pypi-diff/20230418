# Comparing `tmp/ta-cmi-2.0.0.dev1.tar.gz` & `tmp/ta-cmi-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-2.0.0.dev1.tar", last modified: Tue Apr 18 16:39:08 2023, max compression
+gzip compressed data, was "ta-cmi-2.0.0.dev2.tar", last modified: Tue Apr 18 18:50:04 2023, max compression
```

## Comparing `ta-cmi-2.0.0.dev1.tar` & `ta-cmi-2.0.0.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.693181 ta-cmi-2.0.0.dev1/
--rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 ta-cmi-2.0.0.dev1/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 16:39:08.688911 ta-cmi-2.0.0.dev1/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     5596 2023-01-17 13:17:51.000000 ta-cmi-2.0.0.dev1/README.md
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-04-18 16:39:08.694219 ta-cmi-2.0.0.dev1/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      627 2023-04-18 16:37:21.000000 ta-cmi-2.0.0.dev1/setup.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.342570 ta-cmi-2.0.0.dev1/ta_cmi/
--rwxrwxrwx   0 user      (1000) user      (1000)      436 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2307 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/api.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1122 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/channel.py
--rwxrwxrwx   0 user      (1000) user      (1000)      661 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2696 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi_api.py
--rwxrwxrwx   0 user      (1000) user      (1000)      610 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/cmi_channel.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1930 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe.py
--rwxrwxrwx   0 user      (1000) user      (1000)      780 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe_api.py
--rwxrwxrwx   0 user      (1000) user      (1000)      494 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/coe_channel.py
--rwxrwxrwx   0 user      (1000) user      (1000)     3708 2023-01-25 18:14:05.000000 ta-cmi-2.0.0.dev1/ta_cmi/const.py
--rwxrwxrwx   0 user      (1000) user      (1000)     4459 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/ta_cmi/device.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.481565 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      512 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-04-18 16:39:07.000000 ta-cmi-2.0.0.dev1/ta_cmi.egg-info/top_level.txt
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 16:39:08.659793 ta-cmi-2.0.0.dev1/tests/
--rwxrwxrwx   0 user      (1000) user      (1000)     2854 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_api.py
--rwxrwxrwx   0 user      (1000) user      (1000)      650 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi.py
--rwxrwxrwx   0 user      (1000) user      (1000)     5036 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi_api.py
--rwxrwxrwx   0 user      (1000) user      (1000)      991 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_cmi_channel.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2787 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_coe.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1074 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_coe_api.py
--rwxrwxrwx   0 user      (1000) user      (1000)    11873 2023-04-17 20:03:15.000000 ta-cmi-2.0.0.dev1/tests/test_device.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 18:50:04.064099 ta-cmi-2.0.0.dev2/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1067 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 18:50:04.059944 ta-cmi-2.0.0.dev2/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     5525 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/README.md
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-04-18 18:50:04.070843 ta-cmi-2.0.0.dev2/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      606 2023-04-18 18:49:54.000000 ta-cmi-2.0.0.dev2/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 18:50:03.079661 ta-cmi-2.0.0.dev2/ta_cmi/
+-rwxrwxrwx   0 user      (1000) user      (1000)      423 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2227 2023-04-18 18:49:25.000000 ta-cmi-2.0.0.dev2/ta_cmi/api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1090 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      638 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2614 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      593 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1867 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      748 2023-04-18 18:49:16.000000 ta-cmi-2.0.0.dev2/ta_cmi/coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      480 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/ta_cmi/coe_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3514 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/ta_cmi/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4333 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/ta_cmi/device.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 18:50:03.340802 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     7101 2023-04-18 18:50:01.000000 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      512 2023-04-18 18:50:02.000000 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-04-18 18:50:02.000000 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-04-18 18:50:02.000000 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-04-18 18:50:02.000000 ta-cmi-2.0.0.dev2/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-18 18:50:03.866808 ta-cmi-2.0.0.dev2/tests/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2761 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      624 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4903 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      967 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2690 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1033 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    11517 2023-04-18 18:49:17.000000 ta-cmi-2.0.0.dev2/tests/test_device.py
```

### Comparing `ta-cmi-2.0.0.dev1/LICENSE` & `ta-cmi-2.0.0.dev2/LICENSE`

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

### Comparing `ta-cmi-2.0.0.dev1/PKG-INFO` & `ta-cmi-2.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `ta-cmi-2.0.0.dev1/README.md` & `ta-cmi-2.0.0.dev2/ta_cmi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,103 @@
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
-> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
+Metadata-Version: 2.1
+Name: ta-cmi
+Version: 2.0.0.dev2
+Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+Home-page: https://gitlab.com/DeerMaximum/ta-cmi
+Author: DeerMaximum
+Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
+License: MIT License
+        
+        Copyright (c) 2021 DeerMaximum
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
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
+> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
```

### Comparing `ta-cmi-2.0.0.dev1/ta_cmi/api.py` & `ta-cmi-2.0.0.dev2/ta_cmi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import json
-from typing import Any, Dict
-
-import yarl
-from aiohttp import BasicAuth, ClientConnectionError, ClientSession
-
-from ta_cmi.const import HTTP_UNAUTHORIZED
-
-
-class API:
-    """Class to perform basic API requests."""
-
-    def __init__(self, session: ClientSession = None, auth: BasicAuth = None) -> None:
-        """Initialize."""
-        self.session = session
-        self._auth = auth
-
-        self._internal_session = False
-
-    async def _make_request(self, url: str) -> Dict[str, Any]:
-        """Retrieve json data from REST endpoint."""
-        raw_response: str = await self._make_request_no_json(url)
-
-        if not len(raw_response):
-            return {}
-
-        return json.loads(raw_response)
-
-    async def _make_request_no_json(self, url: str) -> str:
-        """Retrieve data from REST endpoint."""
-        if self.session is None:
-            self._internal_session = True
-            self.session = ClientSession()
-
-        try:
-            async with self.session.get(url, auth=self._auth) as res:
-                await self._close_session()
-
-                if res.status == HTTP_UNAUTHORIZED:
-                    raise InvalidCredentialsError("Invalid credentials")
-                elif res.status >= 300:
-                    raise ApiError(
-                        f"Invalid response from {res.url.host}: {res.status}"
-                    )
-
-                text = await res.text()
-                return text
-        except ClientConnectionError:
-            await self._close_session()
-            raise ApiError(f"Could not connect to {yarl.URL(url).host}")
-
-    async def _close_session(self) -> None:
-        """Close the internal session."""
-        if self._internal_session:
-            await self.session.close()
-            self.session = None
-
-
-class ApiError(Exception):
-    """Raised when API request ended in error."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
-
-
-class InvalidCredentialsError(Exception):
-    """Triggered when the credentials are invalid."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
+import json
+from typing import Any, Dict
+
+import yarl
+from aiohttp import BasicAuth, ClientConnectionError, ClientSession
+
+from .const import HTTP_UNAUTHORIZED
+
+
+class API:
+    """Class to perform basic API requests."""
+
+    def __init__(self, session: ClientSession = None, auth: BasicAuth = None) -> None:
+        """Initialize."""
+        self.session = session
+        self._auth = auth
+
+        self._internal_session = False
+
+    async def _make_request(self, url: str) -> Dict[str, Any]:
+        """Retrieve json data from REST endpoint."""
+        raw_response: str = await self._make_request_no_json(url)
+
+        if not len(raw_response):
+            return {}
+
+        return json.loads(raw_response)
+
+    async def _make_request_no_json(self, url: str) -> str:
+        """Retrieve data from REST endpoint."""
+        if self.session is None:
+            self._internal_session = True
+            self.session = ClientSession()
+
+        try:
+            async with self.session.get(url, auth=self._auth) as res:
+                await self._close_session()
+
+                if res.status == HTTP_UNAUTHORIZED:
+                    raise InvalidCredentialsError("Invalid credentials")
+                elif res.status >= 300:
+                    raise ApiError(
+                        f"Invalid response from {res.url.host}: {res.status}"
+                    )
+
+                text = await res.text()
+                return text
+        except ClientConnectionError:
+            await self._close_session()
+            raise ApiError(f"Could not connect to {yarl.URL(url).host}")
+
+    async def _close_session(self) -> None:
+        """Close the internal session."""
+        if self._internal_session:
+            await self.session.close()
+            self.session = None
+
+
+class ApiError(Exception):
+    """Raised when API request ended in error."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
+
+
+class InvalidCredentialsError(Exception):
+    """Triggered when the credentials are invalid."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
```

### Comparing `ta-cmi-2.0.0.dev1/ta_cmi/channel.py` & `ta-cmi-2.0.0.dev2/ta_cmi/channel.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from .const import UNITS_DE, UNITS_EN, ChannelMode, ChannelType, Languages
-
-
-class Channel:
-    """Class to display a data point"""
-
-    def __init__(self) -> None:
-        """Initialize and parse json to get properties."""
-        self.mode: ChannelType | None = None
-        self.type: ChannelMode = ChannelMode.ANALOG
-        self.index: int = 0
-        self.value: float = 0
-        self.unit: str = ""
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

### Comparing `ta-cmi-2.0.0.dev1/ta_cmi/cmi_channel.py` & `ta-cmi-2.0.0.dev2/ta_cmi/cmi_channel.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Any, Dict
-
-from . import Channel
-from .const import ChannelMode, ChannelType, ReadOnlyClass
-
-
-class CMIChannel(Channel, metaclass=ReadOnlyClass):
-    """Class to display an input or output."""
-
-    def __init__(self, mode: ChannelType, json: Dict[str, Any]) -> None:
-        """Initialize and parse json to get properties."""
-        super().__init__()
-        self.mode: ChannelType = mode
-        self.type: ChannelMode = json["AD"]
-        self.index: int = json["Number"]
-        self.value: float = json["Value"]["Value"]
-        self.unit: str = json["Value"]["Unit"]
+from typing import Any, Dict
+
+from . import Channel
+from .const import ChannelMode, ChannelType, ReadOnlyClass
+
+
+class CMIChannel(Channel, metaclass=ReadOnlyClass):
+    """Class to display an input or output."""
+
+    def __init__(self, mode: ChannelType, json: Dict[str, Any]) -> None:
+        """Initialize and parse json to get properties."""
+        super().__init__()
+        self.mode: ChannelType = mode
+        self.type: ChannelMode = json["AD"]
+        self.index: int = json["Number"]
+        self.value: float = json["Value"]["Value"]
+        self.unit: str = json["Value"]["Unit"]
```

### Comparing `ta-cmi-2.0.0.dev1/ta_cmi/device.py` & `ta-cmi-2.0.0.dev2/ta_cmi/device.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import asyncio
-from typing import Any, Dict, List
-
-from .channel import Channel
-from .cmi_api import CMIAPI
-from .cmi_channel import CMIChannel
-from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
-
-
-class Device:
-    """Class to interact with a device."""
-
-    def __init__(self, node_id: str, api: CMIAPI) -> None:
-        """Initialize."""
-        super().__init__()
-
-        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
-
-        self.id = node_id
-        self._api = api
-
-        self.api_version: int = 0
-        self.device_id: str = "00"
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
-    ) -> Dict[int, CMIChannel]:
-        """Extract channel info from data array from request."""
-        list_of_channels: Dict[int, CMIChannel] = {}
-        for channel_raw in raw_channels:
-            ch: CMIChannel = CMIChannel(mode, channel_raw)
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
-        params = self._get_json_params()
-
-        data: dict[str, Any] = {}
-
-        if len(params.split(",")) > 7:
-            first_params = ",".join(params.split(",")[:7])
-            params = ",".join(params.split(",")[7:])
-
-            data = await self._api.get_device_data(self.id, first_params)
-
-            await asyncio.sleep(61)
-
-        if len(data.keys()) == 0:
-            return await self._api.get_device_data(self.id, params)
-
-        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
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
-    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
-        """Get all the fetched channels from a type."""
-        return self._channels[channel_type]
-
-    def has_channel_type(self, channel_type: ChannelType) -> bool:
-        """Check if a channel type was fetched."""
-        return self._channels.get(channel_type, None) is not None
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

### Comparing `ta-cmi-2.0.0.dev1/ta_cmi.egg-info/SOURCES.txt` & `ta-cmi-2.0.0.dev2/ta_cmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.0.0.dev1/tests/test_cmi_api.py` & `ta-cmi-2.0.0.dev2/tests/test_cmi_api.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from typing import Any, Dict
-from unittest.mock import patch
-
-import pytest
-
-from ta_cmi import RateLimitError
-from ta_cmi.api import ApiError
-from ta_cmi.cmi_api import CMIAPI
-
-from . import MAKE_REQUEST_PACKAGE
-
-TEST_HOST = "http://localhost"
-TEST_USER = "user"
-TEST_PASS = "pass"
-TEST_NODE_ID = "1"
-TEST_PARAMS = "I,O"
-
-
-def generate_response(status_code: int) -> Dict[str, Any]:
-    """Generate a response with the provided status code."""
-    return {
-        "Header": {"Version": 6, "Device": "8F", "Timestamp": 1670960961},
-        "Data": {"DL-Bus": []},
-        "Status": "OK",
-        "Status code": status_code,
-    }
-
-
-def generate_device_data_url() -> str:
-    """Generate the device data url."""
-    return (
-        f"{TEST_HOST}/INCLUDE/api.cgi?jsonparam={TEST_PARAMS}&jsonnode={TEST_NODE_ID}"
-    )
-
-
-api = CMIAPI(TEST_HOST, TEST_USER, TEST_PASS)
-
-
-@pytest.mark.asyncio
-async def test_get_devices_ids_to_list_conversion():
-    """Test the get_devices_ids method with a valid api response."""
-    with patch(
-        "ta_cmi.api.API._make_request_no_json", return_value="1;2;"
-    ) as request_mock:
-        ids = await api.get_devices_ids()
-
-        assert ids == ["1", "2"]
-
-        request_mock.assert_called_once()
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_successful_request():
-    """Test the get_device_data function with a successful request."""
-    sample_response: Dict[str, Any] = generate_response(0)
-
-    with patch(MAKE_REQUEST_PACKAGE, return_value=sample_response) as request_mock:
-        result = await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert result == sample_response
-
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_node_not_available():
-    """Test the get_device_data function with a successful request but the cmi status code is 1."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(1)) as request_mock:
-        with pytest.raises(ApiError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert str(exc_info.value) == "Node not available"
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_fail_can_bus():
-    """Test the get_device_data function with a successful request but the cmi status code is 2."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(2)) as request_mock:
-        with pytest.raises(ApiError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert (
-            str(exc_info.value)
-            == "Failure during the CAN-request/parameter not available for this device"
-        )
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_rate_limit():
-    """Test the get_device_data function with a successful request but the cmi status code is 4."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(4)) as request_mock:
-        with pytest.raises(RateLimitError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert str(exc_info.value) == "Only one request per minute is permitted"
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_unsupported_device():
-    """Test the get_device_data function with a successful request but the cmi status code is 5."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(5)) as request_mock:
-        with pytest.raises(ApiError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert str(exc_info.value) == "Device not supported"
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_busy_can_bus():
-    """Test the get_device_data function with a successful request but the cmi status code is 7."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(7)) as request_mock:
-        with pytest.raises(ApiError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert str(exc_info.value) == "CAN Bus is busy"
-        request_mock.assert_called_once_with(generate_device_data_url())
-
-
-@pytest.mark.asyncio
-async def test_get_device_data_unknown_status_code():
-    """Test the get_device_data function with a successful request but the cmi status code is unknown."""
-    with patch(
-        MAKE_REQUEST_PACKAGE, return_value=generate_response(55)
-    ) as request_mock:
-        with pytest.raises(ApiError) as exc_info:
-            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
-
-        assert str(exc_info.value) == "Unknown error"
-        request_mock.assert_called_once_with(generate_device_data_url())
+from typing import Any, Dict
+from unittest.mock import patch
+
+import pytest
+
+from ta_cmi import RateLimitError
+from ta_cmi.api import ApiError
+from ta_cmi.cmi_api import CMIAPI
+
+from . import MAKE_REQUEST_PACKAGE
+
+TEST_HOST = "http://localhost"
+TEST_USER = "user"
+TEST_PASS = "pass"
+TEST_NODE_ID = "1"
+TEST_PARAMS = "I,O"
+
+
+def generate_response(status_code: int) -> Dict[str, Any]:
+    """Generate a response with the provided status code."""
+    return {
+        "Header": {"Version": 6, "Device": "8F", "Timestamp": 1670960961},
+        "Data": {"DL-Bus": []},
+        "Status": "OK",
+        "Status code": status_code,
+    }
+
+
+def generate_device_data_url() -> str:
+    """Generate the device data url."""
+    return (
+        f"{TEST_HOST}/INCLUDE/api.cgi?jsonparam={TEST_PARAMS}&jsonnode={TEST_NODE_ID}"
+    )
+
+
+api = CMIAPI(TEST_HOST, TEST_USER, TEST_PASS)
+
+
+@pytest.mark.asyncio
+async def test_get_devices_ids_to_list_conversion():
+    """Test the get_devices_ids method with a valid api response."""
+    with patch(
+        "ta_cmi.api.API._make_request_no_json", return_value="1;2;"
+    ) as request_mock:
+        ids = await api.get_devices_ids()
+
+        assert ids == ["1", "2"]
+
+        request_mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_successful_request():
+    """Test the get_device_data function with a successful request."""
+    sample_response: Dict[str, Any] = generate_response(0)
+
+    with patch(MAKE_REQUEST_PACKAGE, return_value=sample_response) as request_mock:
+        result = await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert result == sample_response
+
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_node_not_available():
+    """Test the get_device_data function with a successful request but the cmi status code is 1."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(1)) as request_mock:
+        with pytest.raises(ApiError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert str(exc_info.value) == "Node not available"
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_fail_can_bus():
+    """Test the get_device_data function with a successful request but the cmi status code is 2."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(2)) as request_mock:
+        with pytest.raises(ApiError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert (
+            str(exc_info.value)
+            == "Failure during the CAN-request/parameter not available for this device"
+        )
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_rate_limit():
+    """Test the get_device_data function with a successful request but the cmi status code is 4."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(4)) as request_mock:
+        with pytest.raises(RateLimitError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert str(exc_info.value) == "Only one request per minute is permitted"
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_unsupported_device():
+    """Test the get_device_data function with a successful request but the cmi status code is 5."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(5)) as request_mock:
+        with pytest.raises(ApiError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert str(exc_info.value) == "Device not supported"
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_busy_can_bus():
+    """Test the get_device_data function with a successful request but the cmi status code is 7."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=generate_response(7)) as request_mock:
+        with pytest.raises(ApiError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert str(exc_info.value) == "CAN Bus is busy"
+        request_mock.assert_called_once_with(generate_device_data_url())
+
+
+@pytest.mark.asyncio
+async def test_get_device_data_unknown_status_code():
+    """Test the get_device_data function with a successful request but the cmi status code is unknown."""
+    with patch(
+        MAKE_REQUEST_PACKAGE, return_value=generate_response(55)
+    ) as request_mock:
+        with pytest.raises(ApiError) as exc_info:
+            await api.get_device_data(TEST_NODE_ID, TEST_PARAMS)
+
+        assert str(exc_info.value) == "Unknown error"
+        request_mock.assert_called_once_with(generate_device_data_url())
```

### Comparing `ta-cmi-2.0.0.dev1/tests/test_cmi_channel.py` & `ta-cmi-2.0.0.dev2/tests/test_cmi_channel.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import pytest
-
-from ta_cmi.cmi_channel import CMIChannel
-from ta_cmi.const import UNITS_DE, UNITS_EN, ChannelType, Languages
-
-
-@pytest.mark.parametrize("unit_number, expected_unit", UNITS_DE.items())
-def test_units_german(unit_number: str, expected_unit: str):
-    """Test the translation from a unit number to a string with german units."""
-    test = {"Number": 1, "AD": "A", "Value": {"Value": 0, "Unit": unit_number}}
-
-    channel: CMIChannel = CMIChannel(ChannelType.INPUT, test)
-
-    assert channel.get_unit(Languages.DE) == expected_unit
-
-
-@pytest.mark.parametrize("unit_number, expected_unit", UNITS_EN.items())
-def test_units_english(unit_number: str, expected_unit: str):
-    """Test the translation from a unit number to a string with english units."""
-    test = {"Number": 1, "AD": "A", "Value": {"Value": 0, "Unit": unit_number}}
-
-    channel: CMIChannel = CMIChannel(ChannelType.INPUT, test)
-
-    assert channel.get_unit(Languages.EN) == expected_unit
+import pytest
+
+from ta_cmi.cmi_channel import CMIChannel
+from ta_cmi.const import UNITS_DE, UNITS_EN, ChannelType, Languages
+
+
+@pytest.mark.parametrize("unit_number, expected_unit", UNITS_DE.items())
+def test_units_german(unit_number: str, expected_unit: str):
+    """Test the translation from a unit number to a string with german units."""
+    test = {"Number": 1, "AD": "A", "Value": {"Value": 0, "Unit": unit_number}}
+
+    channel: CMIChannel = CMIChannel(ChannelType.INPUT, test)
+
+    assert channel.get_unit(Languages.DE) == expected_unit
+
+
+@pytest.mark.parametrize("unit_number, expected_unit", UNITS_EN.items())
+def test_units_english(unit_number: str, expected_unit: str):
+    """Test the translation from a unit number to a string with english units."""
+    test = {"Number": 1, "AD": "A", "Value": {"Value": 0, "Unit": unit_number}}
+
+    channel: CMIChannel = CMIChannel(ChannelType.INPUT, test)
+
+    assert channel.get_unit(Languages.EN) == expected_unit
```

### Comparing `ta-cmi-2.0.0.dev1/tests/test_coe.py` & `ta-cmi-2.0.0.dev2/tests/test_coe.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from unittest.mock import patch
-
-import pytest
-
-from ta_cmi import ChannelMode, ChannelType
-from ta_cmi.coe import CoE
-from ta_cmi.coe_api import CoEAPI
-from ta_cmi.coe_channel import CoEChannel
-from tests import COE_DATA_PACKAGE
-
-TEST_HOST = "http://localhost"
-
-DATA_RESPONSE = {
-    "digital": [{"value": True, "unit": 43}],
-    "analog": [{"value": 34.4, "unit": 1}],
-    "last_update_unix": 1680410064.03764,
-    "last_update": "2023-04-01T12:00:00",
-}
-
-DATA_RESPONSE_WITH_EMPTY_SLOTS = {
-    "digital": [{"value": True, "unit": 43}, {"value": False, "unit": 0}],
-    "analog": [{"value": 34.4, "unit": 1}, {"value": 0.0, "unit": 0}],
-    "last_update_unix": 1680410064.03764,
-    "last_update": "2023-04-01T12:00:00",
-}
-
-
-@pytest.mark.asyncio
-async def test_update_no_data_received():
-    """Test the update method with empty data."""
-    coe = CoE(TEST_HOST)
-
-    coe._channels = {}
-
-    with patch(COE_DATA_PACKAGE, return_value=None) as data_mock:
-        await coe.update()
-
-        assert coe._channels == {}
-
-        data_mock.assert_called_once()
-
-
-@pytest.mark.asyncio
-async def test_update_old_data_received():
-    """Test the update method with old data."""
-    coe = CoE(TEST_HOST)
-
-    coe._channels = {ChannelType.INPUT: {}}
-    coe.last_update = DATA_RESPONSE["last_update_unix"]
-
-    with patch(COE_DATA_PACKAGE, return_value=DATA_RESPONSE) as data_mock:
-        await coe.update()
-
-        assert coe._channels == {ChannelType.INPUT: {}}
-
-        data_mock.assert_called_once()
-
-
-@pytest.mark.asyncio
-async def test_update_data_received():
-    """Test the update method with new data."""
-    coe = CoE(TEST_HOST)
-
-    assert coe._channels == {}
-    assert coe.last_update == 0
-
-    with patch(COE_DATA_PACKAGE, return_value=DATA_RESPONSE) as data_mock:
-        await coe.update()
-
-        assert coe._channels == {
-            ChannelMode.DIGITAL: {0: CoEChannel(ChannelMode.DIGITAL, 0, 1, "43")},
-            ChannelMode.ANALOG: {0: CoEChannel(ChannelMode.ANALOG, 0, 34.4, "1")},
-        }
-
-        assert coe.last_update == 1680410064.03764
-
-        data_mock.assert_called_once()
-
-
-@pytest.mark.asyncio
-async def test_update_data_received_with_empty_slots():
-    """Test the update method with new data with empty slots."""
-    coe = CoE(TEST_HOST)
-
-    assert coe._channels == {}
-
-    with patch(
-        COE_DATA_PACKAGE, return_value=DATA_RESPONSE_WITH_EMPTY_SLOTS
-    ) as data_mock:
-        await coe.update()
-
-        assert coe._channels == {
-            ChannelMode.DIGITAL: {0: CoEChannel(ChannelMode.DIGITAL, 0, 1, "43")},
-            ChannelMode.ANALOG: {0: CoEChannel(ChannelMode.ANALOG, 0, 34.4, "1")},
-        }
-
-        data_mock.assert_called_once()
+from unittest.mock import patch
+
+import pytest
+
+from ta_cmi import ChannelMode, ChannelType
+from ta_cmi.coe import CoE
+from ta_cmi.coe_api import CoEAPI
+from ta_cmi.coe_channel import CoEChannel
+from tests import COE_DATA_PACKAGE
+
+TEST_HOST = "http://localhost"
+
+DATA_RESPONSE = {
+    "digital": [{"value": True, "unit": 43}],
+    "analog": [{"value": 34.4, "unit": 1}],
+    "last_update_unix": 1680410064.03764,
+    "last_update": "2023-04-01T12:00:00",
+}
+
+DATA_RESPONSE_WITH_EMPTY_SLOTS = {
+    "digital": [{"value": True, "unit": 43}, {"value": False, "unit": 0}],
+    "analog": [{"value": 34.4, "unit": 1}, {"value": 0.0, "unit": 0}],
+    "last_update_unix": 1680410064.03764,
+    "last_update": "2023-04-01T12:00:00",
+}
+
+
+@pytest.mark.asyncio
+async def test_update_no_data_received():
+    """Test the update method with empty data."""
+    coe = CoE(TEST_HOST)
+
+    coe._channels = {}
+
+    with patch(COE_DATA_PACKAGE, return_value=None) as data_mock:
+        await coe.update()
+
+        assert coe._channels == {}
+
+        data_mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_update_old_data_received():
+    """Test the update method with old data."""
+    coe = CoE(TEST_HOST)
+
+    coe._channels = {ChannelType.INPUT: {}}
+    coe.last_update = DATA_RESPONSE["last_update_unix"]
+
+    with patch(COE_DATA_PACKAGE, return_value=DATA_RESPONSE) as data_mock:
+        await coe.update()
+
+        assert coe._channels == {ChannelType.INPUT: {}}
+
+        data_mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_update_data_received():
+    """Test the update method with new data."""
+    coe = CoE(TEST_HOST)
+
+    assert coe._channels == {}
+    assert coe.last_update == 0
+
+    with patch(COE_DATA_PACKAGE, return_value=DATA_RESPONSE) as data_mock:
+        await coe.update()
+
+        assert coe._channels == {
+            ChannelMode.DIGITAL: {0: CoEChannel(ChannelMode.DIGITAL, 0, 1, "43")},
+            ChannelMode.ANALOG: {0: CoEChannel(ChannelMode.ANALOG, 0, 34.4, "1")},
+        }
+
+        assert coe.last_update == 1680410064.03764
+
+        data_mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_update_data_received_with_empty_slots():
+    """Test the update method with new data with empty slots."""
+    coe = CoE(TEST_HOST)
+
+    assert coe._channels == {}
+
+    with patch(
+        COE_DATA_PACKAGE, return_value=DATA_RESPONSE_WITH_EMPTY_SLOTS
+    ) as data_mock:
+        await coe.update()
+
+        assert coe._channels == {
+            ChannelMode.DIGITAL: {0: CoEChannel(ChannelMode.DIGITAL, 0, 1, "43")},
+            ChannelMode.ANALOG: {0: CoEChannel(ChannelMode.ANALOG, 0, 34.4, "1")},
+        }
+
+        data_mock.assert_called_once()
```

### Comparing `ta-cmi-2.0.0.dev1/tests/test_coe_api.py` & `ta-cmi-2.0.0.dev2/tests/test_coe_api.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from unittest.mock import patch
-
-import pytest
-
-from ta_cmi.coe_api import CoEAPI
-
-from . import MAKE_REQUEST_PACKAGE
-
-TEST_HOST = "http://localhost"
-
-DATA_RESPONSE = {
-    "digital": [{"value": True, "unit": 43}],
-    "analog": [{"value": 34.4, "unit": 1}],
-    "last_update_unix": 1680410064.03764,
-    "last_update": "2023-04-01T12:00:00",
-}
-
-
-api = CoEAPI(TEST_HOST)
-
-
-@pytest.mark.asyncio
-async def test_get_coe_data_with_data_response():
-    """Test the get_coe_data with a valid data response."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value=DATA_RESPONSE) as request_mock:
-        result = await api.get_coe_data()
-
-        assert result == DATA_RESPONSE
-
-        request_mock.assert_called_once()
-
-
-@pytest.mark.asyncio
-async def test_get_coe_data_with_empty_response():
-    """Test the get_coe_data with a valid empty response."""
-    with patch(MAKE_REQUEST_PACKAGE, return_value={}) as request_mock:
-        result = await api.get_coe_data()
-
-        assert result is None
-
-        request_mock.assert_called_once()
+from unittest.mock import patch
+
+import pytest
+
+from ta_cmi.coe_api import CoEAPI
+
+from . import MAKE_REQUEST_PACKAGE
+
+TEST_HOST = "http://localhost"
+
+DATA_RESPONSE = {
+    "digital": [{"value": True, "unit": 43}],
+    "analog": [{"value": 34.4, "unit": 1}],
+    "last_update_unix": 1680410064.03764,
+    "last_update": "2023-04-01T12:00:00",
+}
+
+
+api = CoEAPI(TEST_HOST)
+
+
+@pytest.mark.asyncio
+async def test_get_coe_data_with_data_response():
+    """Test the get_coe_data with a valid data response."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value=DATA_RESPONSE) as request_mock:
+        result = await api.get_coe_data()
+
+        assert result == DATA_RESPONSE
+
+        request_mock.assert_called_once()
+
+
+@pytest.mark.asyncio
+async def test_get_coe_data_with_empty_response():
+    """Test the get_coe_data with a valid empty response."""
+    with patch(MAKE_REQUEST_PACKAGE, return_value={}) as request_mock:
+        result = await api.get_coe_data()
+
+        assert result is None
+
+        request_mock.assert_called_once()
```

