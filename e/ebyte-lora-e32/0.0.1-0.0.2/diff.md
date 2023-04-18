# Comparing `tmp/ebyte-lora-e32-0.0.1.tar.gz` & `tmp/ebyte-lora-e32-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e32-0.0.1.tar", last modified: Fri Mar 31 08:52:54 2023, max compression
+gzip compressed data, was "ebyte-lora-e32-0.0.2.tar", last modified: Tue Apr 18 06:20:28 2023, max compression
```

## Comparing `ebyte-lora-e32-0.0.1.tar` & `ebyte-lora-e32-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:52:54.434264 ebyte-lora-e32-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    22467 2023-03-31 08:52:54.434264 ebyte-lora-e32-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    19512 2023-03-31 08:51:37.000000 ebyte-lora-e32-0.0.1/README.md
--rw-rw-rw-   0        0        0     1571 2023-03-31 08:44:30.000000 ebyte-lora-e32-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      924 2023-03-31 08:52:54.441264 ebyte-lora-e32-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1913 2023-03-31 08:49:19.000000 ebyte-lora-e32-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:52:54.411553 ebyte-lora-e32-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:52:54.432265 ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/
--rw-rw-rw-   0        0        0    22467 2023-03-31 08:52:54.000000 ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-03-31 08:52:54.000000 ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:52:54.000000 ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-31 08:52:54.000000 ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24548 2023-03-31 08:50:56.000000 ebyte-lora-e32-0.0.1/src/lora_e32.py
--rw-rw-rw-   0        0        0    10616 2023-03-21 08:24:44.000000 ebyte-lora-e32-0.0.1/src/lora_e32_constants.py
--rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-0.0.1/src/lora_e32_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:28.204810 ebyte-lora-e32-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    22737 2023-04-18 06:20:28.223810 ebyte-lora-e32-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19782 2023-04-18 06:14:24.000000 ebyte-lora-e32-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1571 2023-04-18 06:19:48.000000 ebyte-lora-e32-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      924 2023-04-18 06:20:28.227808 ebyte-lora-e32-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1913 2023-04-18 06:19:48.000000 ebyte-lora-e32-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:28.165809 ebyte-lora-e32-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:28.202807 ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/
+-rw-rw-rw-   0        0        0    22737 2023-04-18 06:20:28.000000 ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-18 06:20:28.000000 ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:20:28.000000 ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-18 06:20:28.000000 ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    24552 2023-04-18 06:19:48.000000 ebyte-lora-e32-0.0.2/src/lora_e32.py
+-rw-rw-rw-   0        0        0    10641 2023-04-18 06:14:50.000000 ebyte-lora-e32-0.0.2/src/lora_e32_constants.py
+-rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-0.0.2/src/lora_e32_operation_constant.py
```

### Comparing `ebyte-lora-e32-0.0.1/LICENSE.md` & `ebyte-lora-e32-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e32-0.0.1/PKG-INFO` & `ebyte-lora-e32-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -71,20 +71,28 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e32
+```
+
 #### Initialization
 
 ```python
 from lora_e32 import LoRaE32
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.1 Summary: Ebyte E32
+Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.2 Summary: Ebyte E32
 LoRa micropython library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -54,22 +54,26 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-#### Initialization ```python from lora_e32 import LoRaE32 from machine import
-UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print(ResponseStatusCode.get_description(code)) ``` #### Get Configuration
-```python from lora_e32 import LoRaE32, print_configuration, Configuration from
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.2 Distinct
+frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
+forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
+functional library ### Library usage Here an example of constructor, you must
+pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
+and M1. ### Installation To install the library execute the following command:
+```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
+lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
+('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print
+(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e32 import LoRaE32, print_configuration, Configuration from
 lora_e32_operation_constant import ResponseStatusCode code, configuration =
 lora.get_configuration() print(ResponseStatusCode.get_description(code))
 print_configuration(configuration) ``` The result ``` -------------------------
 --------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
 SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
 (default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
 > Fixed transmission (first three bytes can be used a s high/low address and
```

### Comparing `ebyte-lora-e32-0.0.1/README.md` & `ebyte-lora-e32-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,28 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e32
+```
+
 #### Initialization
 
 ```python
 from lora_e32 import LoRaE32
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -18,22 +18,26 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-#### Initialization ```python from lora_e32 import LoRaE32 from machine import
-UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print(ResponseStatusCode.get_description(code)) ``` #### Get Configuration
-```python from lora_e32 import LoRaE32, print_configuration, Configuration from
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.2 Distinct
+frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
+forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
+functional library ### Library usage Here an example of constructor, you must
+pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
+and M1. ### Installation To install the library execute the following command:
+```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
+lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
+('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print
+(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e32 import LoRaE32, print_configuration, Configuration from
 lora_e32_operation_constant import ResponseStatusCode code, configuration =
 lora.get_configuration() print(ResponseStatusCode.get_description(code))
 print_configuration(configuration) ``` The result ``` -------------------------
 --------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
 SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
 (default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
 > Fixed transmission (first three bytes can be used a s high/low address and
```

### Comparing `ebyte-lora-e32-0.0.1/pyproject.toml` & `ebyte-lora-e32-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6533  = "ebyte-lora-e3
 00000020: 3222 0d0a 7665 7273 696f 6e20 3d20 2230  2"..version = "0
-00000030: 2e30 2e31 220d 0a61 7574 686f 7273 203d  .0.1"..authors =
+00000030: 2e30 2e32 220d 0a61 7574 686f 7273 203d  .0.2"..authors =
 00000040: 205b 0d0a 2020 7b20 6e61 6d65 3d22 5265   [..  { name="Re
 00000050: 6e7a 6f20 4d69 7363 6869 616e 7469 222c  nzo Mischianti",
 00000060: 2065 6d61 696c 3d22 7265 6e7a 6f40 6d69   email="renzo@mi
 00000070: 7363 6869 616e 7469 2e6f 7267 2220 7d2c  schianti.org" },
 00000080: 0d0a 5d0d 0a6d 6169 6e74 6169 6e65 7273  ..]..maintainers
 00000090: 203d 205b 0d0a 2020 7b20 6e61 6d65 3d22   = [..  { name="
 000000a0: 5265 6e7a 6f20 4d69 7363 6869 616e 7469  Renzo Mischianti
```

### Comparing `ebyte-lora-e32-0.0.1/setup.cfg` & `ebyte-lora-e32-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6533   = ebyte-lora-e3
 00000020: 320d 0a76 6572 7369 6f6e 203d 2030 2e30  2..version = 0.0
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2052 656e  .1..author = Ren
+00000030: 2e32 0d0a 6175 7468 6f72 203d 2052 656e  .2..author = Ren
 00000040: 7a6f 204d 6973 6368 6961 6e74 690d 0a64  zo Mischianti..d
 00000050: 6573 6372 6970 7469 6f6e 203d 2022 4562  escription = "Eb
 00000060: 7974 6520 4533 3220 4c6f 5261 206d 6963  yte E32 LoRa mic
 00000070: 726f 7079 7468 6f6e 206c 6962 7261 7279  ropython library
 00000080: 2064 6576 6963 6520 7665 7279 2063 6865   device very che
 00000090: 6170 2061 6e64 2076 6572 7920 6c6f 6e67  ap and very long
 000000a0: 2072 616e 6765 2028 6672 6f6d 2033 4b6d   range (from 3Km
```

### Comparing `ebyte-lora-e32-0.0.1/setup.py` & `ebyte-lora-e32-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="ebyte-lora-e32",
     package_dir={'': 'src'},
     py_modules=["lora_e32", "lora_e32_constants", "lora_e32_operation_constant"],
-    version="0.0.1",
+    version="0.0.2",
     description="Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     long_description="Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     keywords="LoRa, UART, EByte, e32, esp32, esp8266, stm32, SAMD, Arduino, Raspberry Pi Pico, MicroPython, sx1278, sx1276",
     url="https://github.com/xreef/EByte_LoRa_E32_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e32-0.0.1/src/ebyte_lora_e32.egg-info/PKG-INFO` & `ebyte-lora-e32-0.0.2/src/ebyte_lora_e32.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -71,20 +71,28 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e32
+```
+
 #### Initialization
 
 ```python
 from lora_e32 import LoRaE32
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.1 Summary: Ebyte E32
+Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.2 Summary: Ebyte E32
 LoRa micropython library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -54,22 +54,26 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-#### Initialization ```python from lora_e32 import LoRaE32 from machine import
-UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print(ResponseStatusCode.get_description(code)) ``` #### Get Configuration
-```python from lora_e32 import LoRaE32, print_configuration, Configuration from
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.2 Distinct
+frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
+forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
+functional library ### Library usage Here an example of constructor, you must
+pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
+and M1. ### Installation To install the library execute the following command:
+```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
+lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
+('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print
+(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e32 import LoRaE32, print_configuration, Configuration from
 lora_e32_operation_constant import ResponseStatusCode code, configuration =
 lora.get_configuration() print(ResponseStatusCode.get_description(code))
 print_configuration(configuration) ``` The result ``` -------------------------
 --------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
 SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
 (default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
 > Fixed transmission (first three bytes can be used a s high/low address and
```

### Comparing `ebyte-lora-e32-0.0.1/src/lora_e32.py` & `ebyte-lora-e32-0.0.2/src/lora_e32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E32 Series for MicroPython
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.1
+# VERSION: 0.0.2
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e32-devices/
 #
 # This library implements the EBYTE LoRa E32 Series for MicroPython.
 #
 # The MIT License (MIT)
@@ -264,15 +264,15 @@
 class LoRaE32:
     # now the constructor that receive directly the UART object
     def __init__(self, model, uart, aux_pin=None, m0_pin=None, m1_pin=None,
                  uart_baudrate=SerialUARTBaudRate.BPS_RATE_9600):
         self.uart = uart
         self.model = model
 
-        pattern = '^(400|433|868|900|915|170)(T|M)(20|27|30)(S|D|C)?..?(\\d)?$'
+        pattern = '^(400|433|868|900|915|170)(T|R|S|M)(20|27|30)(S|D|C)?..?(\\d)?$'
 
         model_regex = ure.compile(pattern)
         if not model_regex.match(model):
             raise ValueError('Invalid model')
 
         self.aux_pin = aux_pin
         self.m0_pin = m0_pin
```

### Comparing `ebyte-lora-e32-0.0.1/src/lora_e32_constants.py` & `ebyte-lora-e32-0.0.2/src/lora_e32_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,15 @@
 # here a class that contains the starting frequency of the different devices
 # the device 433 start with 410 frequency and so on
 class OperatingFrequency:
     FREQUENCY_433 = 410
     FREQUENCY_170 = 130
     FREQUENCY_470 = 370
     FREQUENCY_868 = 862
+    FREQUENCY_900 = 850
     FREQUENCY_915 = 900
 
     @staticmethod
     def get_value_from_frequency(frequency):
         if not isinstance(frequency, str):
             frequency = str(frequency)
```

### Comparing `ebyte-lora-e32-0.0.1/src/lora_e32_operation_constant.py` & `ebyte-lora-e32-0.0.2/src/lora_e32_operation_constant.py`

 * *Files identical despite different names*

