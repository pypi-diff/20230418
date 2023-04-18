# Comparing `tmp/ebyte-lora-e22-0.0.1.tar.gz` & `tmp/ebyte-lora-e22-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e22-0.0.1.tar", last modified: Fri Mar 31 09:03:21 2023, max compression
+gzip compressed data, was "ebyte-lora-e22-0.0.2.tar", last modified: Tue Apr 18 14:12:54 2023, max compression
```

## Comparing `ebyte-lora-e22-0.0.1.tar` & `ebyte-lora-e22-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:21.445222 ebyte-lora-e22-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e22-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    28006 2023-03-31 09:03:21.446221 ebyte-lora-e22-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    25102 2023-03-31 09:02:12.000000 ebyte-lora-e22-0.0.1/README.md
--rw-rw-rw-   0        0        0     1521 2023-03-31 09:00:49.000000 ebyte-lora-e22-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      844 2023-03-31 09:03:21.449226 ebyte-lora-e22-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1514 2023-03-31 09:00:14.000000 ebyte-lora-e22-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:19.829398 ebyte-lora-e22-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:19.861393 ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/
--rw-rw-rw-   0        0        0    28006 2023-03-31 09:03:19.000000 ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-03-31 09:03:19.000000 ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 09:03:19.000000 ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-31 09:03:19.000000 ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    28657 2023-03-22 21:59:40.000000 ebyte-lora-e22-0.0.1/src/lora_e22.py
--rw-rw-rw-   0        0        0    11501 2023-03-22 16:17:49.000000 ebyte-lora-e22-0.0.1/src/lora_e22_constants.py
--rw-rw-rw-   0        0        0     3615 2023-03-22 16:19:56.000000 ebyte-lora-e22-0.0.1/src/lora_e22_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.829271 ebyte-lora-e22-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e22-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    28200 2023-04-18 14:12:54.830234 ebyte-lora-e22-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25296 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1521 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      844 2023-04-18 14:12:54.833238 ebyte-lora-e22-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1514 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.800404 ebyte-lora-e22-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.816160 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/
+-rw-rw-rw-   0        0        0    28200 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28688 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/src/lora_e22.py
+-rw-rw-rw-   0        0        0    12924 2023-04-18 14:04:15.000000 ebyte-lora-e22-0.0.2/src/lora_e22_constants.py
+-rw-rw-rw-   0        0        0     3615 2023-03-22 16:19:56.000000 ebyte-lora-e22-0.0.2/src/lora_e22_operation_constant.py
```

### Comparing `ebyte-lora-e22-0.0.1/LICENSE.md` & `ebyte-lora-e22-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e22-0.0.1/PKG-INFO` & `ebyte-lora-e22-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e22
-Version: 0.0.1
+Version: 0.0.2
 Summary: MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268
 Home-page: https://github.com/xreef/EByte_LoRa_E22_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -58,20 +58,28 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e22
+```
+
 #### Initialization
 
 ```python
 from lora_e22 import LoRaE22
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.1 Summary: MicroPython
+Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.2 Summary: MicroPython
 LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266,
 esp32, Raspberry, rp2040 and STM32. sx1262/sx1268 Home-page: https://
 github.com/xreef/EByte_LoRa_E22_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,24 +33,26 @@
 Pico,rp2040,MicroPython,sx1262,sx1268,e22 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: Implementation
 :: MicroPython Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-03-21 0.0.1 Fully functional library ### Library usage Here an example of
+2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
+03-21 0.0.1 Fully functional library ### Library usage Here an example of
 constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e22 import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
-('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e22 import LoRaE22, print_configuration from
-lora_e22_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+reccomended) the AUX pin, M0 and M1. ### Installation To install the library
+execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
+Initialization ```python from lora_e22 import LoRaE22 from machine import UART
+uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
+m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
+print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
+Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
+from lora_e22_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.1/README.md` & `ebyte-lora-e22-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,28 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e22
+```
+
 #### Initialization
 
 ```python
 from lora_e22 import LoRaE22
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-03-21 0.0.1 Fully functional library ### Library usage Here an example of
+2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
+03-21 0.0.1 Fully functional library ### Library usage Here an example of
 constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e22 import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
-('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e22 import LoRaE22, print_configuration from
-lora_e22_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+reccomended) the AUX pin, M0 and M1. ### Installation To install the library
+execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
+Initialization ```python from lora_e22 import LoRaE22 from machine import UART
+uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
+m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
+print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
+Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
+from lora_e22_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.1/pyproject.toml` & `ebyte-lora-e22-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6532  = "ebyte-lora-e2
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

### Comparing `ebyte-lora-e22-0.0.1/setup.cfg` & `ebyte-lora-e22-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6532   = ebyte-lora-e2
 00000020: 320d 0a76 6572 7369 6f6e 203d 2030 2e30  2..version = 0.0
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2052 656e  .1..author = Ren
+00000030: 2e32 0d0a 6175 7468 6f72 203d 2052 656e  .2..author = Ren
 00000040: 7a6f 204d 6973 6368 6961 6e74 690d 0a64  zo Mischianti..d
 00000050: 6573 6372 6970 7469 6f6e 203d 2022 4d69  escription = "Mi
 00000060: 6372 6f50 7974 686f 6e20 4c6f 5261 2045  croPython LoRa E
 00000070: 4259 5445 2045 3232 2064 6576 6963 6520  BYTE E22 device 
 00000080: 6c69 6272 6172 7920 636f 6d70 6c65 7465  library complete
 00000090: 2061 6e64 2074 6573 7465 6420 7769 7468   and tested with
 000000a0: 2041 7264 7569 6e6f 2053 414d 442c 2065   Arduino SAMD, e
```

### Comparing `ebyte-lora-e22-0.0.1/setup.py` & `ebyte-lora-e22-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="micropython-lora-e22",
     package_dir={'': 'src'},
     py_modules=["lora_e22", "lora_e22_constants", "lora_e22_operation_constant"],
-    version="0.0.1",
+    version="0.0.2",
     description="MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268",
     long_description="MicroPython Ebyte E22 LoRa (Long Range) library device very cheap and very long range (from 4Km to 10Km). LoRa EBYTE E22 device library complete and tested with  Arduino SAMD, esp8266, esp32 and STM32. sx1262/sx1268",
     keywords="LoRa, UART, EByte, esp32, esp8266, stm32, SAMD, Arduino, Raspberry Pi Pico, rp2040, MicroPython,sx1262, sx1268, e22",
     url="https://github.com/xreef/EByte_LoRa_E22_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e22-0.0.1/src/ebyte_lora_e22.egg-info/PKG-INFO` & `ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e22
-Version: 0.0.1
+Version: 0.0.2
 Summary: MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268
 Home-page: https://github.com/xreef/EByte_LoRa_E22_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -58,20 +58,28 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
+### Installation
+To install the library execute the following command:
+
+```bash
+pip install ebyte-lora-e22
+```
+
 #### Initialization
 
 ```python
 from lora_e22 import LoRaE22
 from machine import UART
 
 uart2 = UART(2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.1 Summary: MicroPython
+Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.2 Summary: MicroPython
 LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266,
 esp32, Raspberry, rp2040 and STM32. sx1262/sx1268 Home-page: https://
 github.com/xreef/EByte_LoRa_E22_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,24 +33,26 @@
 Pico,rp2040,MicroPython,sx1262,sx1268,e22 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: Implementation
 :: MicroPython Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-03-21 0.0.1 Fully functional library ### Library usage Here an example of
+2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
+03-21 0.0.1 Fully functional library ### Library usage Here an example of
 constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. #### Initialization ```python from
-lora_e22 import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
-('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print("Initialization: {}",
-ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e22 import LoRaE22, print_configuration from
-lora_e22_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print("Retrieve configuration: {}",
+reccomended) the AUX pin, M0 and M1. ### Installation To install the library
+execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
+Initialization ```python from lora_e22 import LoRaE22 from machine import UART
+uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
+m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
+print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
+Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
+from lora_e22_operation_constant import ResponseStatusCode code, configuration
+= lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.1/src/lora_e22.py` & `ebyte-lora-e22-0.0.2/src/lora_e22.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E22 Series for MicroPython
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.1
+# VERSION: 0.0.2
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e22-devices/
 #
 # This library implements the EBYTE LoRa E22 Series for MicroPython.
 #
 # The MIT License (MIT)
@@ -339,15 +339,15 @@
 class LoRaE22:
     # now the constructor that receive directly the UART object
     def __init__(self, model, uart, aux_pin=None, m0_pin=None, m1_pin=None,
                  uart_baudrate=SerialUARTBaudRate.BPS_RATE_9600):
         self.uart = uart
         self.model = model
 
-        pattern = "^((400|900|230)T(22|30)(S(1)?(B|C)|D))$"
+        pattern = '^(230|400|433|900|915)(T|S|M|MM)(22|27|30|33|37)(S|D|C|U|E)?..?(\\d)?$'
 
         model_regex = ure.compile(pattern)
         if not model_regex.match(model):
             raise ValueError('Invalid model')
 
         self.aux_pin = aux_pin
         self.m0_pin = m0_pin
```

### Comparing `ebyte-lora-e22-0.0.1/src/lora_e22_constants.py` & `ebyte-lora-e22-0.0.2/src/lora_e22_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -275,14 +275,62 @@
             return "Invalid transmission power param"
 
     @staticmethod
     def get_default_value():
         return TransmissionPower30.POWER_30
 
 
+class TransmissionPower33:
+    POWER_33 = 0b00
+    POWER_30 = 0b01
+    POWER_27 = 0b10
+    POWER_24 = 0b11
+
+    @staticmethod
+    def get_description(transmission_power):
+        if transmission_power == TransmissionPower33.POWER_33:
+            return "33dBm (Default)"
+        elif transmission_power == TransmissionPower33.POWER_30:
+            return "30dBm"
+        elif transmission_power == TransmissionPower33.POWER_27:
+            return "27dBm"
+        elif transmission_power == TransmissionPower33.POWER_24:
+            return "24dBm"
+        else:
+            return "Invalid transmission power param"
+
+    @staticmethod
+    def get_default_value():
+        return TransmissionPower33.POWER_33
+
+
+class TransmissionPower37:
+    POWER_37_00 = 0b00
+    POWER_37_01 = 0b01
+    POWER_37_10 = 0b10
+    POWER_37_11 = 0b11
+
+    @staticmethod
+    def get_description(transmission_power):
+        if transmission_power == TransmissionPower37.POWER_37_00:
+            return "37dBm (Default)"
+        elif transmission_power == TransmissionPower37.POWER_37_01:
+            return "37dBm"
+        elif transmission_power == TransmissionPower37.POWER_37_10:
+            return "37dBm"
+        elif transmission_power == TransmissionPower37.POWER_37_11:
+            return "37dBm"
+        else:
+            return "Invalid transmission power param"
+
+    @staticmethod
+    def get_default_value():
+        return TransmissionPower37.POWER_37_00
+
+
 # here a class that contains the starting frequency of the different devices
 # the device 433 start with 410 frequency and so on
 class OperatingFrequency:
     FREQUENCY_433 = 410
     FREQUENCY_400 = 410
     FREQUENCY_170 = 130
     FREQUENCY_230 = 220
@@ -323,21 +371,20 @@
 
         if model is not None:
             self.package_type = model[6]
             self.frequency = int(model[0:3])
             self.transmission_power = int(model[4:6])
 
     def get_transmission_power(self):
-        if self.transmission_power == self.transmission_power:
+        if self.transmission_power == 22:
             return TransmissionPower22
-        elif self.transmission_power == self.transmission_power:
+        elif self.transmission_power == 30:
             return TransmissionPower30
+        elif self.transmission_power == 33:
+            return TransmissionPower33
+        elif self.transmission_power == 37:
+            return TransmissionPower37
         else:
-            return None
+            return "Invalid transmission power param"
 
     def get_transmission_power_description(self, transmission_power):
-        if self.transmission_power == 22:
-            return TransmissionPower22.get_description(transmission_power)
-        elif self.transmission_power == 30:
-            return TransmissionPower30.get_description(transmission_power)
-        else:
-            return "Invalid transmission power param"
+        return self.get_transmission_power().get_description(transmission_power)
```

### Comparing `ebyte-lora-e22-0.0.1/src/lora_e22_operation_constant.py` & `ebyte-lora-e22-0.0.2/src/lora_e22_operation_constant.py`

 * *Files identical despite different names*

