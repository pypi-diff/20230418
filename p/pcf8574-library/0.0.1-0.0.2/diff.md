# Comparing `tmp/pcf8574-library-0.0.1.tar.gz` & `tmp/pcf8574-library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcf8574-library-0.0.1.tar", last modified: Fri Apr 14 16:20:46 2023, max compression
+gzip compressed data, was "pcf8574-library-0.0.2.tar", last modified: Tue Apr 18 20:36:44 2023, max compression
```

## Comparing `pcf8574-library-0.0.1.tar` & `pcf8574-library-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:20:46.290018 pcf8574-library-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 pcf8574-library-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     6826 2023-04-14 16:20:46.290018 pcf8574-library-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3915 2023-04-14 16:12:23.000000 pcf8574-library-0.0.1/README.md
--rw-rw-rw-   0        0        0     1539 2023-04-14 15:55:59.000000 pcf8574-library-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      805 2023-04-14 16:20:46.293021 pcf8574-library-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-04-14 16:00:37.000000 pcf8574-library-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:20:46.278020 pcf8574-library-0.0.1/src/
--rw-rw-rw-   0        0        0    19737 2023-04-14 16:17:03.000000 pcf8574-library-0.0.1/src/PCF8574.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:20:46.288020 pcf8574-library-0.0.1/src/pcf8574_library.egg-info/
--rw-rw-rw-   0        0        0     6826 2023-04-14 16:20:46.000000 pcf8574-library-0.0.1/src/pcf8574_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-14 16:20:46.000000 pcf8574-library-0.0.1/src/pcf8574_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:20:46.000000 pcf8574-library-0.0.1/src/pcf8574_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 16:20:46.000000 pcf8574-library-0.0.1/src/pcf8574_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 20:36:44.958388 pcf8574-library-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 pcf8574-library-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     6887 2023-04-18 20:36:44.958388 pcf8574-library-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3976 2023-04-18 20:35:39.000000 pcf8574-library-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1539 2023-04-18 20:34:51.000000 pcf8574-library-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      805 2023-04-18 20:36:44.961387 pcf8574-library-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-04-18 20:34:51.000000 pcf8574-library-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:36:44.933387 pcf8574-library-0.0.2/src/
+-rw-rw-rw-   0        0        0    19835 2023-04-18 20:34:51.000000 pcf8574-library-0.0.2/src/PCF8574.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:36:44.957388 pcf8574-library-0.0.2/src/pcf8574_library.egg-info/
+-rw-rw-rw-   0        0        0     6887 2023-04-18 20:36:44.000000 pcf8574-library-0.0.2/src/pcf8574_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-18 20:36:44.000000 pcf8574-library-0.0.2/src/pcf8574_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:36:44.000000 pcf8574-library-0.0.2/src/pcf8574_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 20:36:44.000000 pcf8574-library-0.0.2/src/pcf8574_library.egg-info/top_level.txt
```

### Comparing `pcf8574-library-0.0.1/LICENSE.md` & `pcf8574-library-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcf8574-library-0.0.1/PKG-INFO` & `pcf8574-library-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcf8574-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Most starred PCF8574 library. i2c digital expander for Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read write digital values with only 2 wire. Very simple to use
 Home-page: https://github.com/xreef/PCF8574_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -59,14 +59,15 @@
 
 #
 #### www.mischianti.org
 
 # PCF8574 PCF8574AP digital input and output expander with i2c bus.
 
 ## Changelog
+ - 18/04/2023: v0.0.2 Add static declaration for Px constants inside class.
  - 14/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operations.
 
 Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and rp2040 (Raspberry Pi Pico and similar)
 
 PCF8574P address map 0x20-0x27 
@@ -78,43 +79,43 @@
 ```bash
 pip install pcf8574-library
 ```
 
 **Constructor:**
 Pass the address of I2C 
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     pcf = PCF8574(0x38, sda=21, scl=22)
 ```
 To use interrupt you must pass the interrupt pin and the function to call when interrupt raised from PCF8574
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     def keyPressedOnPCF8574(pin):
         # Interrupt called (No Serial no read no wire in this function, and DEBUG disabled on PCF library)
         keyPressed = True
     
     pcf = PCF8574(0x38, sda=21, scl=22, interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18)
 ```
 
 You must set input/output mode:
 ```python
     from machine import Pin
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
 
-    pcf.Pin(P0, Pin.IN)
-    pcf.Pin(P1, Pin.IN, Pin.PULL_UP)
-    pcf.Pin(P2, Pin.IN)
-    pcf.Pin(P3, Pin.IN)
-    
-    pcf.Pin(P7, Pin.OUT)
-    pcf.Pin(P6, Pin.OUT, 1)
-    pcf.Pin(P5, Pin.OUT, 0)
-    pcf.Pin(P4, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P0, Pin.IN)
+    pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+    pcf.Pin(PCF8574.P2, Pin.IN)
+    pcf.Pin(PCF8574.P3, Pin.IN)
+    
+    pcf.Pin(PCF8574.P7, Pin.OUT)
+    pcf.Pin(PCF8574.P6, Pin.OUT, 1)
+    pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P4, Pin.OUT, 0)
 ```
 
 then IC as you can see in the image has 8 digital input/output ports:
 
 ![PCF8574 schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-pins.gif)
 
 To read all analog input in one trasmission you can do (even if I use a 10millis debounce time to prevent too much read from i2c):
@@ -135,21 +136,21 @@
     
     byte_input = pcf.digital_read_all_byte()
     print(bin(byte_input))
 ```
 
 If you want to read a single input:
 ```python
-    digital_input = pcf.digital_read(P1)
+    digital_input = pcf.digital_read(PCF8574.P1)
     print(digital_input)
 ```
 
 If you want to write a digital value:
 ```python
-    pcf.digital_write(P1, 1)
+    pcf.digital_write(PCF8574.P1, 1)
 ```
 
 You can also use an interrupt pin:
 You must initialize the pin and the function to call when interrupt raised from PCF8574
 ```python
     def callback(pin):
         now = utime.ticks_ms()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcf8574-library Version: 0.0.1 Summary: Most
+Metadata-Version: 2.1 Name: pcf8574-library Version: 0.0.2 Summary: Most
 starred PCF8574 library. i2c digital expander for Arduino, Raspberry Pi Pico
 and rp2040 boards, esp32, SMT32 and ESP8266. Can read write digital values with
 only 2 wire. Very simple to use Home-page: https://github.com/xreef/
 PCF8574_micropython_library Author: Renzo Mischianti Author-email: Renzo
 Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -33,46 +33,47 @@
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python :: Implementation :: MicroPython Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
 [Support_forum_pcf8574_English]
 [Forum_supporto_pcf8574_italiano]
 # #### www.mischianti.org # PCF8574 PCF8574AP digital input and output expander
-with i2c bus. ## Changelog - 14/04/2023: v0.0.1 Initial commit of stable
-version. I try to simplify the use of this IC, with a minimal set of
-operations. Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR
-etc.), STM32 and rp2040 (Raspberry Pi Pico and similar) PCF8574P address map
-0x20-0x27 PCF8574AP address map 0x38-0x3f ### Installation To install the
-library execute the following command: ```bash pip install pcf8574-library ```
-**Constructor:** Pass the address of I2C ```python from PCF8574 import PCF8574,
-P0, P7, P6, P1, P2, P3, P5, P4 pcf = PCF8574(0x38, sda=21, scl=22) ``` To use
-interrupt you must pass the interrupt pin and the function to call when
-interrupt raised from PCF8574 ```python from PCF8574 import PCF8574, P0, P7,
-P6, P1, P2, P3, P5, P4 def keyPressedOnPCF8574(pin): # Interrupt called (No
-Serial no read no wire in this function, and DEBUG disabled on PCF library)
-keyPressed = True pcf = PCF8574(0x38, sda=21, scl=22,
+with i2c bus. ## Changelog - 18/04/2023: v0.0.2 Add static declaration for Px
+constants inside class. - 14/04/2023: v0.0.1 Initial commit of stable version.
+I try to simplify the use of this IC, with a minimal set of operations. Tested
+with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and
+rp2040 (Raspberry Pi Pico and similar) PCF8574P address map 0x20-0x27 PCF8574AP
+address map 0x38-0x3f ### Installation To install the library execute the
+following command: ```bash pip install pcf8574-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8574 import PCF8574 pcf = PCF8574
+(0x38, sda=21, scl=22) ``` To use interrupt you must pass the interrupt pin and
+the function to call when interrupt raised from PCF8574 ```python from PCF8574
+import PCF8574 def keyPressedOnPCF8574(pin): # Interrupt called (No Serial no
+read no wire in this function, and DEBUG disabled on PCF library) keyPressed =
+True pcf = PCF8574(0x38, sda=21, scl=22,
 interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18) ``` You must set
 input/output mode: ```python from machine import Pin from PCF8574 import
-PCF8574, P0, P7, P6, P1, P2, P3, P5, P4 pcf.Pin(P0, Pin.IN) pcf.Pin(P1, Pin.IN,
-Pin.PULL_UP) pcf.Pin(P2, Pin.IN) pcf.Pin(P3, Pin.IN) pcf.Pin(P7, Pin.OUT)
-pcf.Pin(P6, Pin.OUT, 1) pcf.Pin(P5, Pin.OUT, 0) pcf.Pin(P4, Pin.OUT, 0) ```
-then IC as you can see in the image has 8 digital input/output ports: ![PCF8574
-schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-
-pins.gif) To read all analog input in one trasmission you can do (even if I use
-a 10millis debounce time to prevent too much read from i2c): ```python
-digital_input = pcf.digital_read_all() print(digital_input.p0) print
-(digital_input.p1) print(digital_input.p2) print(digital_input.p3) print
-(digital_input.p4) print(digital_input.p5) print(digital_input.p6) print
-(digital_input.p7) array_input = pcf.digital_read_all_array() print
-(array_input) byte_input = pcf.digital_read_all_byte() print(bin(byte_input))
-``` If you want to read a single input: ```python digital_input =
-pcf.digital_read(P1) print(digital_input) ``` If you want to write a digital
-value: ```python pcf.digital_write(P1, 1) ``` You can also use an interrupt
-pin: You must initialize the pin and the function to call when interrupt raised
-from PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count
-count += 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18,
-callback) ``` For the examples I use this wire schema on breadboard: !
-[Breadboard](https://www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-
-esp8266-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https://
-www.mischianti.org/wp-content/uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-
-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/uploads/2022/08/
+PCF8574 pcf.Pin(PCF8574.P0, Pin.IN) pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+pcf.Pin(PCF8574.P2, Pin.IN) pcf.Pin(PCF8574.P3, Pin.IN) pcf.Pin(PCF8574.P7,
+Pin.OUT) pcf.Pin(PCF8574.P6, Pin.OUT, 1) pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+pcf.Pin(PCF8574.P4, Pin.OUT, 0) ``` then IC as you can see in the image has 8
+digital input/output ports: ![PCF8574 schema](https://github.com/xreef/
+PCF8574_library/raw/master/resources/PCF8574-pins.gif) To read all analog input
+in one trasmission you can do (even if I use a 10millis debounce time to
+prevent too much read from i2c): ```python digital_input = pcf.digital_read_all
+() print(digital_input.p0) print(digital_input.p1) print(digital_input.p2)
+print(digital_input.p3) print(digital_input.p4) print(digital_input.p5) print
+(digital_input.p6) print(digital_input.p7) array_input =
+pcf.digital_read_all_array() print(array_input) byte_input =
+pcf.digital_read_all_byte() print(bin(byte_input)) ``` If you want to read a
+single input: ```python digital_input = pcf.digital_read(PCF8574.P1) print
+(digital_input) ``` If you want to write a digital value: ```python
+pcf.digital_write(PCF8574.P1, 1) ``` You can also use an interrupt pin: You
+must initialize the pin and the function to call when interrupt raised from
+PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count count
++= 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18, callback)
+``` For the examples I use this wire schema on breadboard: ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-esp8266-pcf8574-IC-
+wiring-schema-8-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/
+uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2022/08/
 stm32_pcf8574_wiring_4_Led_4_Buttons_bb.jpg)
```

### Comparing `pcf8574-library-0.0.1/README.md` & `pcf8574-library-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 #
 #### www.mischianti.org
 
 # PCF8574 PCF8574AP digital input and output expander with i2c bus.
 
 ## Changelog
+ - 18/04/2023: v0.0.2 Add static declaration for Px constants inside class.
  - 14/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operations.
 
 Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and rp2040 (Raspberry Pi Pico and similar)
 
 PCF8574P address map 0x20-0x27 
@@ -30,43 +31,43 @@
 ```bash
 pip install pcf8574-library
 ```
 
 **Constructor:**
 Pass the address of I2C 
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     pcf = PCF8574(0x38, sda=21, scl=22)
 ```
 To use interrupt you must pass the interrupt pin and the function to call when interrupt raised from PCF8574
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     def keyPressedOnPCF8574(pin):
         # Interrupt called (No Serial no read no wire in this function, and DEBUG disabled on PCF library)
         keyPressed = True
     
     pcf = PCF8574(0x38, sda=21, scl=22, interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18)
 ```
 
 You must set input/output mode:
 ```python
     from machine import Pin
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
 
-    pcf.Pin(P0, Pin.IN)
-    pcf.Pin(P1, Pin.IN, Pin.PULL_UP)
-    pcf.Pin(P2, Pin.IN)
-    pcf.Pin(P3, Pin.IN)
-    
-    pcf.Pin(P7, Pin.OUT)
-    pcf.Pin(P6, Pin.OUT, 1)
-    pcf.Pin(P5, Pin.OUT, 0)
-    pcf.Pin(P4, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P0, Pin.IN)
+    pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+    pcf.Pin(PCF8574.P2, Pin.IN)
+    pcf.Pin(PCF8574.P3, Pin.IN)
+    
+    pcf.Pin(PCF8574.P7, Pin.OUT)
+    pcf.Pin(PCF8574.P6, Pin.OUT, 1)
+    pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P4, Pin.OUT, 0)
 ```
 
 then IC as you can see in the image has 8 digital input/output ports:
 
 ![PCF8574 schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-pins.gif)
 
 To read all analog input in one trasmission you can do (even if I use a 10millis debounce time to prevent too much read from i2c):
@@ -87,21 +88,21 @@
     
     byte_input = pcf.digital_read_all_byte()
     print(bin(byte_input))
 ```
 
 If you want to read a single input:
 ```python
-    digital_input = pcf.digital_read(P1)
+    digital_input = pcf.digital_read(PCF8574.P1)
     print(digital_input)
 ```
 
 If you want to write a digital value:
 ```python
-    pcf.digital_write(P1, 1)
+    pcf.digital_write(PCF8574.P1, 1)
 ```
 
 You can also use an interrupt pin:
 You must initialize the pin and the function to call when interrupt raised from PCF8574
 ```python
     def callback(pin):
         now = utime.ticks_ms()
```

#### html2text {}

```diff
@@ -1,42 +1,43 @@
 [Support_forum_pcf8574_English]
 [Forum_supporto_pcf8574_italiano]
 # #### www.mischianti.org # PCF8574 PCF8574AP digital input and output expander
-with i2c bus. ## Changelog - 14/04/2023: v0.0.1 Initial commit of stable
-version. I try to simplify the use of this IC, with a minimal set of
-operations. Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR
-etc.), STM32 and rp2040 (Raspberry Pi Pico and similar) PCF8574P address map
-0x20-0x27 PCF8574AP address map 0x38-0x3f ### Installation To install the
-library execute the following command: ```bash pip install pcf8574-library ```
-**Constructor:** Pass the address of I2C ```python from PCF8574 import PCF8574,
-P0, P7, P6, P1, P2, P3, P5, P4 pcf = PCF8574(0x38, sda=21, scl=22) ``` To use
-interrupt you must pass the interrupt pin and the function to call when
-interrupt raised from PCF8574 ```python from PCF8574 import PCF8574, P0, P7,
-P6, P1, P2, P3, P5, P4 def keyPressedOnPCF8574(pin): # Interrupt called (No
-Serial no read no wire in this function, and DEBUG disabled on PCF library)
-keyPressed = True pcf = PCF8574(0x38, sda=21, scl=22,
+with i2c bus. ## Changelog - 18/04/2023: v0.0.2 Add static declaration for Px
+constants inside class. - 14/04/2023: v0.0.1 Initial commit of stable version.
+I try to simplify the use of this IC, with a minimal set of operations. Tested
+with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and
+rp2040 (Raspberry Pi Pico and similar) PCF8574P address map 0x20-0x27 PCF8574AP
+address map 0x38-0x3f ### Installation To install the library execute the
+following command: ```bash pip install pcf8574-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8574 import PCF8574 pcf = PCF8574
+(0x38, sda=21, scl=22) ``` To use interrupt you must pass the interrupt pin and
+the function to call when interrupt raised from PCF8574 ```python from PCF8574
+import PCF8574 def keyPressedOnPCF8574(pin): # Interrupt called (No Serial no
+read no wire in this function, and DEBUG disabled on PCF library) keyPressed =
+True pcf = PCF8574(0x38, sda=21, scl=22,
 interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18) ``` You must set
 input/output mode: ```python from machine import Pin from PCF8574 import
-PCF8574, P0, P7, P6, P1, P2, P3, P5, P4 pcf.Pin(P0, Pin.IN) pcf.Pin(P1, Pin.IN,
-Pin.PULL_UP) pcf.Pin(P2, Pin.IN) pcf.Pin(P3, Pin.IN) pcf.Pin(P7, Pin.OUT)
-pcf.Pin(P6, Pin.OUT, 1) pcf.Pin(P5, Pin.OUT, 0) pcf.Pin(P4, Pin.OUT, 0) ```
-then IC as you can see in the image has 8 digital input/output ports: ![PCF8574
-schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-
-pins.gif) To read all analog input in one trasmission you can do (even if I use
-a 10millis debounce time to prevent too much read from i2c): ```python
-digital_input = pcf.digital_read_all() print(digital_input.p0) print
-(digital_input.p1) print(digital_input.p2) print(digital_input.p3) print
-(digital_input.p4) print(digital_input.p5) print(digital_input.p6) print
-(digital_input.p7) array_input = pcf.digital_read_all_array() print
-(array_input) byte_input = pcf.digital_read_all_byte() print(bin(byte_input))
-``` If you want to read a single input: ```python digital_input =
-pcf.digital_read(P1) print(digital_input) ``` If you want to write a digital
-value: ```python pcf.digital_write(P1, 1) ``` You can also use an interrupt
-pin: You must initialize the pin and the function to call when interrupt raised
-from PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count
-count += 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18,
-callback) ``` For the examples I use this wire schema on breadboard: !
-[Breadboard](https://www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-
-esp8266-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https://
-www.mischianti.org/wp-content/uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-
-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/uploads/2022/08/
+PCF8574 pcf.Pin(PCF8574.P0, Pin.IN) pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+pcf.Pin(PCF8574.P2, Pin.IN) pcf.Pin(PCF8574.P3, Pin.IN) pcf.Pin(PCF8574.P7,
+Pin.OUT) pcf.Pin(PCF8574.P6, Pin.OUT, 1) pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+pcf.Pin(PCF8574.P4, Pin.OUT, 0) ``` then IC as you can see in the image has 8
+digital input/output ports: ![PCF8574 schema](https://github.com/xreef/
+PCF8574_library/raw/master/resources/PCF8574-pins.gif) To read all analog input
+in one trasmission you can do (even if I use a 10millis debounce time to
+prevent too much read from i2c): ```python digital_input = pcf.digital_read_all
+() print(digital_input.p0) print(digital_input.p1) print(digital_input.p2)
+print(digital_input.p3) print(digital_input.p4) print(digital_input.p5) print
+(digital_input.p6) print(digital_input.p7) array_input =
+pcf.digital_read_all_array() print(array_input) byte_input =
+pcf.digital_read_all_byte() print(bin(byte_input)) ``` If you want to read a
+single input: ```python digital_input = pcf.digital_read(PCF8574.P1) print
+(digital_input) ``` If you want to write a digital value: ```python
+pcf.digital_write(PCF8574.P1, 1) ``` You can also use an interrupt pin: You
+must initialize the pin and the function to call when interrupt raised from
+PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count count
++= 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18, callback)
+``` For the examples I use this wire schema on breadboard: ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-esp8266-pcf8574-IC-
+wiring-schema-8-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/
+uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2022/08/
 stm32_pcf8574_wiring_4_Led_4_Buttons_bb.jpg)
```

### Comparing `pcf8574-library-0.0.1/pyproject.toml` & `pcf8574-library-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 6366 3835 3734 2d6c 6962 7261  = "pcf8574-libra
 00000020: 7279 220d 0a76 6572 7369 6f6e 203d 2022  ry"..version = "
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

### Comparing `pcf8574-library-0.0.1/setup.cfg` & `pcf8574-library-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6366 3835 3734 2d6c 6962 7261   = pcf8574-libra
 00000020: 7279 0d0a 7665 7273 696f 6e20 3d20 302e  ry..version = 0.
-00000030: 302e 310d 0a61 7574 686f 7220 3d20 5265  0.1..author = Re
+00000030: 302e 320d 0a61 7574 686f 7220 3d20 5265  0.2..author = Re
 00000040: 6e7a 6f20 4d69 7363 6869 616e 7469 0d0a  nzo Mischianti..
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 5043  description = PC
 00000060: 4638 3537 3420 6d69 6372 6f70 7974 686f  F8574 micropytho
 00000070: 6e20 6c69 6272 6172 792e 2069 3263 2064  n library. i2c d
 00000080: 6967 6974 616c 2065 7870 616e 6465 7220  igital expander 
 00000090: 666f 7220 4172 6475 696e 6f2c 2052 6173  for Arduino, Ras
 000000a0: 7062 6572 7279 2050 6920 5069 636f 2061  pberry Pi Pico a
```

### Comparing `pcf8574-library-0.0.1/setup.py` & `pcf8574-library-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="pcf8574-library",
     package_dir={'': 'src'},
     py_modules=["PCF8574"],
-    version="0.0.1",
+    version="0.0.2",
     description="PCF8574 micropython library. i2c digital expander for Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266",
     long_description="PCF8574 micropython library. i2c digital expander for Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read write digital values with only 2 wire. Very simple to use",
     keywords="micropython, digital, i2c, expander, pcf8574, pcf8574a, esp32, esp8266, stm32, SAMD, Arduino, wire, rp2040, Raspberry",
     url="https://github.com/xreef/PCF8574_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `pcf8574-library-0.0.1/src/PCF8574.py` & `pcf8574-library-0.0.2/src/PCF8574.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # PCF8574 GPIO Port Expand
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.1
+# VERSION: 0.0.2
 #
 #           _____
 #     A0  |1    16| Vcc
 #     A1  |2    15| SDA
 #     A2  |3    14| SCL
 #  P0/IO0 |4    13| INT
 #  P1/IO1 |5    12| P7/IO7
@@ -69,26 +69,35 @@
         return Logger(self.enable_debug)
 
 
 logging = Logger(False)
 
 logger = logging.getLogger(__name__)
 
+DEBOUNCE_LATENCY = 100
+
 P0 = 0
 P1 = 1
 P2 = 2
 P3 = 3
 P4 = 4
 P5 = 5
 P6 = 6
 P7 = 7
 
-DEBOUNCE_LATENCY = 100
-
 class PCF8574:
+    P0 = 0
+    P1 = 1
+    P2 = 2
+    P3 = 3
+    P4 = 4
+    P5 = 5
+    P6 = 6
+    P7 = 7
+
     def __init__(self, address, i2c=None, i2c_id=0, sda=None, scl=None, interrupt_pin=None, interrupt_callback=None):
         if i2c:
             self._i2c = i2c
         elif sda and scl:
             self._i2c = I2C(i2c_id, scl=Pin(scl), sda=Pin(sda))
         else:
             raise ValueError('Either i2c or sda and scl must be provided')
```

### Comparing `pcf8574-library-0.0.1/src/pcf8574_library.egg-info/PKG-INFO` & `pcf8574-library-0.0.2/src/pcf8574_library.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcf8574-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Most starred PCF8574 library. i2c digital expander for Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read write digital values with only 2 wire. Very simple to use
 Home-page: https://github.com/xreef/PCF8574_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -59,14 +59,15 @@
 
 #
 #### www.mischianti.org
 
 # PCF8574 PCF8574AP digital input and output expander with i2c bus.
 
 ## Changelog
+ - 18/04/2023: v0.0.2 Add static declaration for Px constants inside class.
  - 14/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operations.
 
 Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and rp2040 (Raspberry Pi Pico and similar)
 
 PCF8574P address map 0x20-0x27 
@@ -78,43 +79,43 @@
 ```bash
 pip install pcf8574-library
 ```
 
 **Constructor:**
 Pass the address of I2C 
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     pcf = PCF8574(0x38, sda=21, scl=22)
 ```
 To use interrupt you must pass the interrupt pin and the function to call when interrupt raised from PCF8574
 ```python
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
     
     def keyPressedOnPCF8574(pin):
         # Interrupt called (No Serial no read no wire in this function, and DEBUG disabled on PCF library)
         keyPressed = True
     
     pcf = PCF8574(0x38, sda=21, scl=22, interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18)
 ```
 
 You must set input/output mode:
 ```python
     from machine import Pin
-    from PCF8574 import PCF8574, P0, P7, P6, P1, P2, P3, P5, P4
+    from PCF8574 import PCF8574
 
-    pcf.Pin(P0, Pin.IN)
-    pcf.Pin(P1, Pin.IN, Pin.PULL_UP)
-    pcf.Pin(P2, Pin.IN)
-    pcf.Pin(P3, Pin.IN)
-    
-    pcf.Pin(P7, Pin.OUT)
-    pcf.Pin(P6, Pin.OUT, 1)
-    pcf.Pin(P5, Pin.OUT, 0)
-    pcf.Pin(P4, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P0, Pin.IN)
+    pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+    pcf.Pin(PCF8574.P2, Pin.IN)
+    pcf.Pin(PCF8574.P3, Pin.IN)
+    
+    pcf.Pin(PCF8574.P7, Pin.OUT)
+    pcf.Pin(PCF8574.P6, Pin.OUT, 1)
+    pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+    pcf.Pin(PCF8574.P4, Pin.OUT, 0)
 ```
 
 then IC as you can see in the image has 8 digital input/output ports:
 
 ![PCF8574 schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-pins.gif)
 
 To read all analog input in one trasmission you can do (even if I use a 10millis debounce time to prevent too much read from i2c):
@@ -135,21 +136,21 @@
     
     byte_input = pcf.digital_read_all_byte()
     print(bin(byte_input))
 ```
 
 If you want to read a single input:
 ```python
-    digital_input = pcf.digital_read(P1)
+    digital_input = pcf.digital_read(PCF8574.P1)
     print(digital_input)
 ```
 
 If you want to write a digital value:
 ```python
-    pcf.digital_write(P1, 1)
+    pcf.digital_write(PCF8574.P1, 1)
 ```
 
 You can also use an interrupt pin:
 You must initialize the pin and the function to call when interrupt raised from PCF8574
 ```python
     def callback(pin):
         now = utime.ticks_ms()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcf8574-library Version: 0.0.1 Summary: Most
+Metadata-Version: 2.1 Name: pcf8574-library Version: 0.0.2 Summary: Most
 starred PCF8574 library. i2c digital expander for Arduino, Raspberry Pi Pico
 and rp2040 boards, esp32, SMT32 and ESP8266. Can read write digital values with
 only 2 wire. Very simple to use Home-page: https://github.com/xreef/
 PCF8574_micropython_library Author: Renzo Mischianti Author-email: Renzo
 Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -33,46 +33,47 @@
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python :: Implementation :: MicroPython Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
 [Support_forum_pcf8574_English]
 [Forum_supporto_pcf8574_italiano]
 # #### www.mischianti.org # PCF8574 PCF8574AP digital input and output expander
-with i2c bus. ## Changelog - 14/04/2023: v0.0.1 Initial commit of stable
-version. I try to simplify the use of this IC, with a minimal set of
-operations. Tested with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR
-etc.), STM32 and rp2040 (Raspberry Pi Pico and similar) PCF8574P address map
-0x20-0x27 PCF8574AP address map 0x38-0x3f ### Installation To install the
-library execute the following command: ```bash pip install pcf8574-library ```
-**Constructor:** Pass the address of I2C ```python from PCF8574 import PCF8574,
-P0, P7, P6, P1, P2, P3, P5, P4 pcf = PCF8574(0x38, sda=21, scl=22) ``` To use
-interrupt you must pass the interrupt pin and the function to call when
-interrupt raised from PCF8574 ```python from PCF8574 import PCF8574, P0, P7,
-P6, P1, P2, P3, P5, P4 def keyPressedOnPCF8574(pin): # Interrupt called (No
-Serial no read no wire in this function, and DEBUG disabled on PCF library)
-keyPressed = True pcf = PCF8574(0x38, sda=21, scl=22,
+with i2c bus. ## Changelog - 18/04/2023: v0.0.2 Add static declaration for Px
+constants inside class. - 14/04/2023: v0.0.1 Initial commit of stable version.
+I try to simplify the use of this IC, with a minimal set of operations. Tested
+with esp8266, esp32, Arduino, Arduino SAMD (Nano 33 IoT, MKR etc.), STM32 and
+rp2040 (Raspberry Pi Pico and similar) PCF8574P address map 0x20-0x27 PCF8574AP
+address map 0x38-0x3f ### Installation To install the library execute the
+following command: ```bash pip install pcf8574-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8574 import PCF8574 pcf = PCF8574
+(0x38, sda=21, scl=22) ``` To use interrupt you must pass the interrupt pin and
+the function to call when interrupt raised from PCF8574 ```python from PCF8574
+import PCF8574 def keyPressedOnPCF8574(pin): # Interrupt called (No Serial no
+read no wire in this function, and DEBUG disabled on PCF library) keyPressed =
+True pcf = PCF8574(0x38, sda=21, scl=22,
 interrupt_callback=keyPressedOnPCF8574, interrupt_pin=18) ``` You must set
 input/output mode: ```python from machine import Pin from PCF8574 import
-PCF8574, P0, P7, P6, P1, P2, P3, P5, P4 pcf.Pin(P0, Pin.IN) pcf.Pin(P1, Pin.IN,
-Pin.PULL_UP) pcf.Pin(P2, Pin.IN) pcf.Pin(P3, Pin.IN) pcf.Pin(P7, Pin.OUT)
-pcf.Pin(P6, Pin.OUT, 1) pcf.Pin(P5, Pin.OUT, 0) pcf.Pin(P4, Pin.OUT, 0) ```
-then IC as you can see in the image has 8 digital input/output ports: ![PCF8574
-schema](https://github.com/xreef/PCF8574_library/raw/master/resources/PCF8574-
-pins.gif) To read all analog input in one trasmission you can do (even if I use
-a 10millis debounce time to prevent too much read from i2c): ```python
-digital_input = pcf.digital_read_all() print(digital_input.p0) print
-(digital_input.p1) print(digital_input.p2) print(digital_input.p3) print
-(digital_input.p4) print(digital_input.p5) print(digital_input.p6) print
-(digital_input.p7) array_input = pcf.digital_read_all_array() print
-(array_input) byte_input = pcf.digital_read_all_byte() print(bin(byte_input))
-``` If you want to read a single input: ```python digital_input =
-pcf.digital_read(P1) print(digital_input) ``` If you want to write a digital
-value: ```python pcf.digital_write(P1, 1) ``` You can also use an interrupt
-pin: You must initialize the pin and the function to call when interrupt raised
-from PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count
-count += 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18,
-callback) ``` For the examples I use this wire schema on breadboard: !
-[Breadboard](https://www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-
-esp8266-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https://
-www.mischianti.org/wp-content/uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-
-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/uploads/2022/08/
+PCF8574 pcf.Pin(PCF8574.P0, Pin.IN) pcf.Pin(PCF8574.P1, Pin.IN, Pin.PULL_UP)
+pcf.Pin(PCF8574.P2, Pin.IN) pcf.Pin(PCF8574.P3, Pin.IN) pcf.Pin(PCF8574.P7,
+Pin.OUT) pcf.Pin(PCF8574.P6, Pin.OUT, 1) pcf.Pin(PCF8574.P5, Pin.OUT, 0)
+pcf.Pin(PCF8574.P4, Pin.OUT, 0) ``` then IC as you can see in the image has 8
+digital input/output ports: ![PCF8574 schema](https://github.com/xreef/
+PCF8574_library/raw/master/resources/PCF8574-pins.gif) To read all analog input
+in one trasmission you can do (even if I use a 10millis debounce time to
+prevent too much read from i2c): ```python digital_input = pcf.digital_read_all
+() print(digital_input.p0) print(digital_input.p1) print(digital_input.p2)
+print(digital_input.p3) print(digital_input.p4) print(digital_input.p5) print
+(digital_input.p6) print(digital_input.p7) array_input =
+pcf.digital_read_all_array() print(array_input) byte_input =
+pcf.digital_read_all_byte() print(bin(byte_input)) ``` If you want to read a
+single input: ```python digital_input = pcf.digital_read(PCF8574.P1) print
+(digital_input) ``` If you want to write a digital value: ```python
+pcf.digital_write(PCF8574.P1, 1) ``` You can also use an interrupt pin: You
+must initialize the pin and the function to call when interrupt raised from
+PCF8574 ```python def callback(pin): now = utime.ticks_ms() global count count
++= 1 print("Time: {} {}".format(now, count)) pcf.attach_interrupt(18, callback)
+``` For the examples I use this wire schema on breadboard: ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2021/04/WeMos-D1-esp8266-pcf8574-IC-
+wiring-schema-8-leds.jpg) ![Breadboard](https://www.mischianti.org/wp-content/
+uploads/2021/04/esp32-pcf8574-IC-wiring-schema-8-leds.jpg) ![Breadboard](https:
+//www.mischianti.org/wp-content/uploads/2022/08/
 stm32_pcf8574_wiring_4_Led_4_Buttons_bb.jpg)
```

