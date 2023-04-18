# Comparing `tmp/ebyte-lora-e220-0.0.1.tar.gz` & `tmp/ebyte-lora-e220-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e220-0.0.1.tar", last modified: Fri Mar 31 08:16:24 2023, max compression
+gzip compressed data, was "ebyte-lora-e220-0.0.2.tar", last modified: Tue Apr 18 06:17:51 2023, max compression
```

## Comparing `ebyte-lora-e220-0.0.1.tar` & `ebyte-lora-e220-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:16:24.197403 ebyte-lora-e220-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e220-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    35589 2023-03-31 08:16:24.198413 ebyte-lora-e220-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    32715 2023-03-22 21:43:48.000000 ebyte-lora-e220-0.0.1/README.md
--rw-rw-rw-   0        0        0     1487 2023-03-31 08:15:42.000000 ebyte-lora-e220-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      793 2023-03-31 08:16:24.200750 ebyte-lora-e220-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-03-31 08:15:58.000000 ebyte-lora-e220-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:16:23.870203 ebyte-lora-e220-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:16:23.896203 ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/
--rw-rw-rw-   0        0        0    35589 2023-03-31 08:16:23.000000 ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-03-31 08:16:23.000000 ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:16:23.000000 ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-31 08:16:23.000000 ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27408 2023-03-22 15:36:09.000000 ebyte-lora-e220-0.0.1/src/lora_e220.py
--rw-rw-rw-   0        0        0    10582 2023-03-22 13:53:14.000000 ebyte-lora-e220-0.0.1/src/lora_e220_constants.py
--rw-rw-rw-   0        0        0     3771 2023-03-22 07:57:47.000000 ebyte-lora-e220-0.0.1/src/lora_e220_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:17:51.874411 ebyte-lora-e220-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e220-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    35799 2023-04-18 06:17:51.875347 ebyte-lora-e220-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    32925 2023-04-18 06:07:17.000000 ebyte-lora-e220-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1487 2023-04-18 06:07:46.000000 ebyte-lora-e220-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      793 2023-04-18 06:17:51.882346 ebyte-lora-e220-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-18 06:07:46.000000 ebyte-lora-e220-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:17:51.847348 ebyte-lora-e220-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:17:51.872387 ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/
+-rw-rw-rw-   0        0        0    35799 2023-04-18 06:17:51.000000 ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-18 06:17:51.000000 ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:17:51.000000 ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-18 06:17:51.000000 ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27619 2023-04-18 06:16:19.000000 ebyte-lora-e220-0.0.2/src/lora_e220.py
+-rw-rw-rw-   0        0        0    10607 2023-04-18 06:06:03.000000 ebyte-lora-e220-0.0.2/src/lora_e220_constants.py
+-rw-rw-rw-   0        0        0     3771 2023-03-22 07:57:47.000000 ebyte-lora-e220-0.0.2/src/lora_e220_operation_constant.py
```

### Comparing `ebyte-lora-e220-0.0.1/LICENSE.md` & `ebyte-lora-e220-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e220-0.0.1/PKG-INFO` & `ebyte-lora-e220-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e220
-Version: 0.0.1
+Version: 0.0.2
 Summary: LoRa EBYTE E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. LLCC68
 Home-page: https://github.com/xreef/EByte_LoRa_E220_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -60,16 +60,24 @@
 
 </br></br>
 
 # EBYTE LoRa E220 devices micropython library (LLCC68)   
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e220
+```
+
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 #### Initialization
 
 ```python
@@ -251,19 +259,14 @@
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2022/04/19/ebyte-lora-e220-llcc68-device-for-arduino-esp32-or-esp8266-configuration-3/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: fixed transmission, broadcast, monitor, and RSSI](https://www.mischianti.org/2022/04/27/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/)
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and WeMos D1 shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and esp32 dev v1 shield
 
-## CHANGELOG
-- 2023-03-22 0.0.1 First stable release
-
-
-
 
 
 <h2>LLCC68 </h2>
 
 
 
 <p>LoRa Smart Home (LLCC68) is a sub-GHz LoRa® RF Transceiver for medium-range indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for long battery life with just 4.2 mA of active receive current consumption. The SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can transmit up to +22 dBm with highly efficient integrated power&nbsp;amplifiers.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e220 Version: 0.0.1 Summary: LoRa EBYTE
+Metadata-Version: 2.1 Name: ebyte-lora-e220 Version: 0.0.2 Summary: LoRa EBYTE
 E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and
 Raspberry Pi Pico. LLCC68 Home-page: https://github.com/xreef/
 EByte_LoRa_E220_micropython_library Author: Renzo Mischianti Author-email:
 Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,24 +33,27 @@
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python :: Implementation :: MicroPython Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
 [Support_forum_EByte_e220_English]
 [Forum_supporto_EByte_e220_italiano]
  # EBYTE LoRa E220 devices micropython library (LLCC68) ### Changelog - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e220 import LoRaE220 from machine import UART uart2 = UART(2) lora =
-LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the
-module transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e220 import LoRaE220, print_configuration from
-lora_e220_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://
+www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21
+0.0.1 Fully functional library ### Installation To install the library execute
+the following command: ```bash pip install ebyte-lora-e220 ``` ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. #### Initialization
+```python from lora_e220 import LoRaE220 from machine import UART uart2 = UART
+(2) lora = LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ```
+#### Start the module transmission ```python code = lora.begin() print
+("Initialization: {}", ResponseStatusCode.get_description(code)) ``` #### Get
+Configuration ```python from lora_e220 import LoRaE220, print_configuration
+from lora_e220_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` ---------------------------------------- Initialization: {}
 Success Retrieve configuration: {} Success ------------------------------------
 ---- HEAD : 0xc1 0x0 0x8 AddH : 0x0 AddL : 0x0 Chan : 23 -> 433 SpeedParityBit
 : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps (default)
 SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionSubPacketSett: 0b0 -
 > 200bytes (default) OptionTranPower : 0b0 -> 22dBm (Default)
@@ -117,16 +120,15 @@
 esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/) - [Ebyte LoRa E220
 device for Arduino, esp32 or esp8266: power saving and sending structured data]
 (https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-
 esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/) - Ebyte
 LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino
 shield - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR
 microcontroller and WeMos D1 shield - Ebyte LoRa E220 device for Arduino, esp32
-or esp8266: WOR microcontroller and esp32 dev v1 shield ## CHANGELOG - 2023-03-
-22 0.0.1 First stable release
+or esp8266: WOR microcontroller and esp32 dev v1 shield
 ***** LLCC68 *****
 LoRa Smart Home (LLCC68) is a sub-GHz LoRaÂ® RF Transceiver for medium-range
 indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin
 is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for
 long battery life with just 4.2 mA of active receive current consumption. The
 SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can
 transmit up to +22 dBm with highly efficient integrated power amplifiers.
```

### Comparing `ebyte-lora-e220-0.0.1/README.md` & `ebyte-lora-e220-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,24 @@
 
 </br></br>
 
 # EBYTE LoRa E220 devices micropython library (LLCC68)   
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e220
+```
+
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 #### Initialization
 
 ```python
@@ -203,19 +211,14 @@
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2022/04/19/ebyte-lora-e220-llcc68-device-for-arduino-esp32-or-esp8266-configuration-3/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: fixed transmission, broadcast, monitor, and RSSI](https://www.mischianti.org/2022/04/27/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/)
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and WeMos D1 shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and esp32 dev v1 shield
 
-## CHANGELOG
-- 2023-03-22 0.0.1 First stable release
-
-
-
 
 
 <h2>LLCC68 </h2>
 
 
 
 <p>LoRa Smart Home (LLCC68) is a sub-GHz LoRa® RF Transceiver for medium-range indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for long battery life with just 4.2 mA of active receive current consumption. The SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can transmit up to +22 dBm with highly efficient integrated power&nbsp;amplifiers.</p>
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
 [Support_forum_EByte_e220_English]
 [Forum_supporto_EByte_e220_italiano]
  # EBYTE LoRa E220 devices micropython library (LLCC68) ### Changelog - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e220 import LoRaE220 from machine import UART uart2 = UART(2) lora =
-LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the
-module transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e220 import LoRaE220, print_configuration from
-lora_e220_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://
+www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21
+0.0.1 Fully functional library ### Installation To install the library execute
+the following command: ```bash pip install ebyte-lora-e220 ``` ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. #### Initialization
+```python from lora_e220 import LoRaE220 from machine import UART uart2 = UART
+(2) lora = LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ```
+#### Start the module transmission ```python code = lora.begin() print
+("Initialization: {}", ResponseStatusCode.get_description(code)) ``` #### Get
+Configuration ```python from lora_e220 import LoRaE220, print_configuration
+from lora_e220_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` ---------------------------------------- Initialization: {}
 Success Retrieve configuration: {} Success ------------------------------------
 ---- HEAD : 0xc1 0x0 0x8 AddH : 0x0 AddL : 0x0 Chan : 23 -> 433 SpeedParityBit
 : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps (default)
 SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionSubPacketSett: 0b0 -
 > 200bytes (default) OptionTranPower : 0b0 -> 22dBm (Default)
@@ -81,16 +84,15 @@
 esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/) - [Ebyte LoRa E220
 device for Arduino, esp32 or esp8266: power saving and sending structured data]
 (https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-
 esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/) - Ebyte
 LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino
 shield - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR
 microcontroller and WeMos D1 shield - Ebyte LoRa E220 device for Arduino, esp32
-or esp8266: WOR microcontroller and esp32 dev v1 shield ## CHANGELOG - 2023-03-
-22 0.0.1 First stable release
+or esp8266: WOR microcontroller and esp32 dev v1 shield
 ***** LLCC68 *****
 LoRa Smart Home (LLCC68) is a sub-GHz LoRaÂ® RF Transceiver for medium-range
 indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin
 is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for
 long battery life with just 4.2 mA of active receive current consumption. The
 SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can
 transmit up to +22 dBm with highly efficient integrated power amplifiers.
```

### Comparing `ebyte-lora-e220-0.0.1/pyproject.toml` & `ebyte-lora-e220-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6532  = "ebyte-lora-e2
 00000020: 3230 220d 0a76 6572 7369 6f6e 203d 2022  20"..version = "
-00000030: 302e 302e 3122 0d0a 6175 7468 6f72 7320  0.0.1"..authors 
+00000030: 302e 302e 3222 0d0a 6175 7468 6f72 7320  0.0.2"..authors 
 00000040: 3d20 5b0d 0a20 207b 206e 616d 653d 2252  = [..  { name="R
 00000050: 656e 7a6f 204d 6973 6368 6961 6e74 6922  enzo Mischianti"
 00000060: 2c20 656d 6169 6c3d 2272 656e 7a6f 406d  , email="renzo@m
 00000070: 6973 6368 6961 6e74 692e 6f72 6722 207d  ischianti.org" }
 00000080: 2c0d 0a5d 0d0a 6d61 696e 7461 696e 6572  ,..]..maintainer
 00000090: 7320 3d20 5b0d 0a20 207b 206e 616d 653d  s = [..  { name=
 000000a0: 2252 656e 7a6f 204d 6973 6368 6961 6e74  "Renzo Mischiant
```

### Comparing `ebyte-lora-e220-0.0.1/setup.cfg` & `ebyte-lora-e220-0.0.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6532   = ebyte-lora-e2
 00000020: 3230 0d0a 7665 7273 696f 6e20 3d20 302e  20..version = 0.
-00000030: 302e 310d 0a61 7574 686f 7220 3d20 5265  0.1..author = Re
+00000030: 302e 320d 0a61 7574 686f 7220 3d20 5265  0.2..author = Re
 00000040: 6e7a 6f20 4d69 7363 6869 616e 7469 0d0a  nzo Mischianti..
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 4c6f  description = Lo
 00000060: 5261 2045 4259 5445 2045 3232 3020 6465  Ra EBYTE E220 de
 00000070: 7669 6365 206c 6962 7261 7279 2063 6f6d  vice library com
 00000080: 706c 6574 6520 616e 6420 7465 7374 6564  plete and tested
 00000090: 2077 6974 6820 4172 6475 696e 6f2c 2065   with Arduino, e
 000000a0: 7370 3832 3636 2c20 6573 7033 322c 2053  sp8266, esp32, S
```

### Comparing `ebyte-lora-e220-0.0.1/setup.py` & `ebyte-lora-e220-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import sys
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="ebyte-lora-e220",
     package_dir={'': 'src'},
-    # packages=["src-lora-e220"],
     py_modules=["lora_e220", "lora_e220_constants", "lora_e220_operation_constant"],
-    version="0.0.1",
+    version="0.0.2",
     description="LoRa EBYTE E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. LLCC68",
     long_description="Ebyte E220 LoRa (Long Range) library device very cheap and very long range (from 5Km to 10Km). Arduino LoRa EBYTE E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. LLCC68",
     keywords="LoRa, UART, EByte, esp32, esp8266, stm32, SAMD, Arduino, Raspberry Pi Pico, MicroPython",
     url="https://github.com/xreef/EByte_LoRa_E220_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e220-0.0.1/src/ebyte_lora_e220.egg-info/PKG-INFO` & `ebyte-lora-e220-0.0.2/src/ebyte_lora_e220.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e220
-Version: 0.0.1
+Version: 0.0.2
 Summary: LoRa EBYTE E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. LLCC68
 Home-page: https://github.com/xreef/EByte_LoRa_E220_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -60,16 +60,24 @@
 
 </br></br>
 
 # EBYTE LoRa E220 devices micropython library (LLCC68)   
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e220
+```
+
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 #### Initialization
 
 ```python
@@ -251,19 +259,14 @@
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2022/04/19/ebyte-lora-e220-llcc68-device-for-arduino-esp32-or-esp8266-configuration-3/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: fixed transmission, broadcast, monitor, and RSSI](https://www.mischianti.org/2022/04/27/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/)
 - [Ebyte LoRa E220 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/)
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and WeMos D1 shield
 - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and esp32 dev v1 shield
 
-## CHANGELOG
-- 2023-03-22 0.0.1 First stable release
-
-
-
 
 
 <h2>LLCC68 </h2>
 
 
 
 <p>LoRa Smart Home (LLCC68) is a sub-GHz LoRa® RF Transceiver for medium-range indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for long battery life with just 4.2 mA of active receive current consumption. The SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can transmit up to +22 dBm with highly efficient integrated power&nbsp;amplifiers.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e220 Version: 0.0.1 Summary: LoRa EBYTE
+Metadata-Version: 2.1 Name: ebyte-lora-e220 Version: 0.0.2 Summary: LoRa EBYTE
 E220 device library complete and tested with Arduino, esp8266, esp32, STM32 and
 Raspberry Pi Pico. LLCC68 Home-page: https://github.com/xreef/
 EByte_LoRa_E220_micropython_library Author: Renzo Mischianti Author-email:
 Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,24 +33,27 @@
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python :: Implementation :: MicroPython Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
 [Support_forum_EByte_e220_English]
 [Forum_supporto_EByte_e220_italiano]
  # EBYTE LoRa E220 devices micropython library (LLCC68) ### Changelog - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e220 import LoRaE220 from machine import UART uart2 = UART(2) lora =
-LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the
-module transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e220 import LoRaE220, print_configuration from
-lora_e220_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://
+www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21
+0.0.1 Fully functional library ### Installation To install the library execute
+the following command: ```bash pip install ebyte-lora-e220 ``` ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. #### Initialization
+```python from lora_e220 import LoRaE220 from machine import UART uart2 = UART
+(2) lora = LoRaE220('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ```
+#### Start the module transmission ```python code = lora.begin() print
+("Initialization: {}", ResponseStatusCode.get_description(code)) ``` #### Get
+Configuration ```python from lora_e220 import LoRaE220, print_configuration
+from lora_e220_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` ---------------------------------------- Initialization: {}
 Success Retrieve configuration: {} Success ------------------------------------
 ---- HEAD : 0xc1 0x0 0x8 AddH : 0x0 AddL : 0x0 Chan : 23 -> 433 SpeedParityBit
 : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps (default)
 SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionSubPacketSett: 0b0 -
 > 200bytes (default) OptionTranPower : 0b0 -> 22dBm (Default)
@@ -117,16 +120,15 @@
 esp8266-fixed-transmission-broadcast-monitor-and-rssi-4/) - [Ebyte LoRa E220
 device for Arduino, esp32 or esp8266: power saving and sending structured data]
 (https://www.mischianti.org/2022/05/06/ebyte-lora-e220-device-for-arduino-
 esp32-or-esp8266-manage-wake-on-radio-and-sends-structured-data-5/) - Ebyte
 LoRa E220 device for Arduino, esp32 or esp8266: WOR microcontroller and Arduino
 shield - Ebyte LoRa E220 device for Arduino, esp32 or esp8266: WOR
 microcontroller and WeMos D1 shield - Ebyte LoRa E220 device for Arduino, esp32
-or esp8266: WOR microcontroller and esp32 dev v1 shield ## CHANGELOG - 2023-03-
-22 0.0.1 First stable release
+or esp8266: WOR microcontroller and esp32 dev v1 shield
 ***** LLCC68 *****
 LoRa Smart Home (LLCC68) is a sub-GHz LoRaÂ® RF Transceiver for medium-range
 indoor and indoor to outdoor wireless applications. SPI interface. Pin-to-pin
 is compatible with SX1262. SX1261, SX1262, SX1268, and LLCC68 are designed for
 long battery life with just 4.2 mA of active receive current consumption. The
 SX1261 can transmit up to +15 dBm, and the SX1262, SX1268, and LLCC68 can
 transmit up to +22 dBm with highly efficient integrated power amplifiers.
```

### Comparing `ebyte-lora-e220-0.0.1/src/lora_e220.py` & `ebyte-lora-e220-0.0.2/src/lora_e220.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E220 Series for MicroPython
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.1
+# VERSION: 0.0.2
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e220-devices/
 #
 # This library implements the EBYTE LoRa E220 Series for MicroPython.
 #
 # The MIT License (MIT)
@@ -319,15 +319,15 @@
 class LoRaE220:
     # now the constructor that receive directly the UART object
     def __init__(self, model, uart, aux_pin=None, m0_pin=None, m1_pin=None,
                  uart_baudrate=SerialUARTBaudRate.BPS_RATE_9600):
         self.uart = uart
         self.model = model
 
-        pattern = '^(400|900)[TRS](22|30)[SD]$'
+        pattern = '^(400|433|868|900|915|170)(T|R|S|M)(20|27|30)(S|D|C)?..?(\\d)?$'
 
         model_regex = ure.compile(pattern)
         if not model_regex.match(model):
             raise ValueError('Invalid model')
 
         self.aux_pin = aux_pin
         self.m0_pin = m0_pin
@@ -522,14 +522,18 @@
 
         self.write_program_command(
             ProgramCommand.READ_CONFIGURATION,
             RegisterAddress.REG_ADDRESS_CFG,
             PacketLength.PL_CONFIGURATION)
 
         data = self.uart.read()
+        if data is None or len(data) != PacketLength.PL_CONFIGURATION+3:
+            code = ResponseStatusCode.ERR_E220_DATA_SIZE_NOT_MATCH
+            return code, None
+
         logger.debug("data: {}".format(data))
         logger.debug("data len: {}".format(len(data)))
 
         logger.debug("model: {}".format(self.model))
         configuration = Configuration(self.model)
         configuration.from_bytes(data)
         code = self.set_mode(prev_mode)
```

### Comparing `ebyte-lora-e220-0.0.1/src/lora_e220_constants.py` & `ebyte-lora-e220-0.0.2/src/lora_e220_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,16 @@
 class OperatingFrequency:
     FREQUENCY_433 = 410
     FREQUENCY_400 = 410
     FREQUENCY_170 = 130
     FREQUENCY_230 = 220
     FREQUENCY_470 = 370
     FREQUENCY_868 = 850
-    FREQUENCY_915 = 850
+    FREQUENCY_900 = 850
+    FREQUENCY_915 = 900
 
     @staticmethod
     def get_value_from_frequency(frequency):
         if not isinstance(frequency, str):
             frequency = str(frequency)
 
         freq_attr_name = 'FREQUENCY_' + frequency
```

### Comparing `ebyte-lora-e220-0.0.1/src/lora_e220_operation_constant.py` & `ebyte-lora-e220-0.0.2/src/lora_e220_operation_constant.py`

 * *Files identical despite different names*

