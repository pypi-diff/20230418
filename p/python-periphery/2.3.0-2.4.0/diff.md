# Comparing `tmp/python-periphery-2.3.0.tar.gz` & `tmp/python-periphery-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-periphery-2.3.0.tar", last modified: Mon Feb 15 04:42:52 2021, max compression
+gzip compressed data, was "python-periphery-2.4.0.tar", last modified: Tue Apr 18 04:09:03 2023, max compression
```

## Comparing `python-periphery-2.3.0.tar` & `python-periphery-2.4.0.tar`

### file list

```diff
@@ -1,20 +1,42 @@
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2021-02-15 04:42:52.131258 python-periphery-2.3.0/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2021-02-14 21:56:02.000000 python-periphery-2.3.0/LICENSE
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1465 2021-02-15 04:42:52.131258 python-periphery-2.3.0/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5561 2020-12-16 07:27:49.000000 python-periphery-2.3.0/README.md
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2021-02-15 04:42:52.131258 python-periphery-2.3.0/periphery/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1030 2021-02-15 04:38:06.000000 python-periphery-2.3.0/periphery/__init__.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    42037 2021-02-04 07:46:50.000000 python-periphery-2.3.0/periphery/gpio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     6769 2019-10-29 03:46:27.000000 python-periphery-2.3.0/periphery/i2c.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5997 2019-10-29 03:46:27.000000 python-periphery-2.3.0/periphery/led.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    10483 2021-02-14 21:52:06.000000 python-periphery-2.3.0/periphery/mmio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    10213 2019-11-09 17:53:20.000000 python-periphery-2.3.0/periphery/pwm.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    25275 2020-05-28 05:33:30.000000 python-periphery-2.3.0/periphery/serial.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    15568 2021-02-04 07:36:15.000000 python-periphery-2.3.0/periphery/spi.py
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2021-02-15 04:42:52.131258 python-periphery-2.3.0/python_periphery.egg-info/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1465 2021-02-15 04:42:52.000000 python-periphery-2.3.0/python_periphery.egg-info/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)      342 2021-02-15 04:42:52.000000 python-periphery-2.3.0/python_periphery.egg-info/SOURCES.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2021-02-15 04:42:52.000000 python-periphery-2.3.0/python_periphery.egg-info/dependency_links.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)       10 2021-02-15 04:42:52.000000 python-periphery-2.3.0/python_periphery.egg-info/top_level.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)      131 2021-02-15 04:42:52.131258 python-periphery-2.3.0/setup.cfg
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1633 2021-02-15 04:38:06.000000 python-periphery-2.3.0/setup.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2023-04-18 04:01:48.000000 python-periphery-2.4.0/LICENSE
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-18 04:09:03.215770 python-periphery-2.4.0/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5634 2023-04-14 08:42:18.000000 python-periphery-2.4.0/README.md
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/periphery/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1030 2023-04-18 04:02:08.000000 python-periphery-2.4.0/periphery/__init__.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      698 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/__init__.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     9960 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1935 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/gpio.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    20665 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_cdev1.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    21051 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_cdev2.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    11903 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_sysfs.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     6769 2019-10-29 03:46:27.000000 python-periphery-2.4.0/periphery/i2c.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      752 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/i2c.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5997 2019-10-29 03:46:27.000000 python-periphery-2.4.0/periphery/led.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      704 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/led.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    10469 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/mmio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1032 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/mmio.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    10220 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/pwm.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      749 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/pwm.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/py.typed
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    25275 2020-05-28 05:33:30.000000 python-periphery-2.4.0/periphery/serial.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1114 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/serial.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    15568 2021-02-04 07:36:15.000000 python-periphery-2.4.0/periphery/spi.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      806 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/spi.pyi
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/python_periphery.egg-info/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      757 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/SOURCES.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/dependency_links.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)       10 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/top_level.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      131 2023-04-18 04:09:03.215770 python-periphery-2.4.0/setup.cfg
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1688 2023-04-18 04:02:08.000000 python-periphery-2.4.0/setup.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/tests/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1258 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    11956 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_gpio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     8499 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_gpio_sysfs.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     3001 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_i2c.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     3592 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_led.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5896 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_mmio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     7312 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_pwm.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     8865 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_serial.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5681 2020-12-10 07:07:56.000000 python-periphery-2.4.0/tests/test_spi.py
```

### Comparing `python-periphery-2.3.0/LICENSE` & `python-periphery-2.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- Copyright (c) 2015-2021 vsergeev / Ivan (Vanya) A. Sergeev
+ Copyright (c) 2015-2023 vsergeev / Ivan (Vanya) A. Sergeev
 
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `python-periphery-2.3.0/PKG-INFO` & `python-periphery-2.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-periphery
-Version: 2.3.0
+Version: 2.4.0
 Summary: A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.
 Home-page: https://github.com/vsergeev/python-periphery
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
-Description: python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.
 Keywords: gpio spi led pwm i2c mmio serial uart embedded linux beaglebone raspberrypi rpi odroid
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
+License-File: LICENSE
+
+python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.
```

### Comparing `python-periphery-2.3.0/README.md` & `python-periphery-2.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# python-periphery [![Build Status](https://travis-ci.org/vsergeev/python-periphery.svg?branch=master)](https://travis-ci.org/vsergeev/python-periphery) [![Docs Status](https://readthedocs.org/projects/python-periphery/badge/)](https://python-periphery.readthedocs.io/en/latest/) [![GitHub release](https://img.shields.io/github/release/vsergeev/python-periphery.svg?maxAge=7200)](https://github.com/vsergeev/python-periphery) [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vsergeev/python-periphery/blob/master/LICENSE)
+# python-periphery [![Build Status](https://app.travis-ci.com/vsergeev/python-periphery.svg?branch=master)](https://app.travis-ci.com/github/vsergeev/python-periphery) [![Docs Status](https://readthedocs.org/projects/python-periphery/badge/)](https://python-periphery.readthedocs.io/en/latest/) [![GitHub release](https://img.shields.io/github/release/vsergeev/python-periphery.svg?maxAge=7200)](https://github.com/vsergeev/python-periphery) [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vsergeev/python-periphery/blob/master/LICENSE)
 
 ## Linux Peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) with Python 2 & 3
 
 python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed.
 
 Using Lua or C? Check out the [lua-periphery](https://github.com/vsergeev/lua-periphery) and [c-periphery](https://github.com/vsergeev/c-periphery) projects.
 
-Contributed libraries: [java-periphery](https://github.com/sgjava/java-periphery)
+Contributed libraries: [java-periphery](https://github.com/sgjava/java-periphery), [dart_periphery](https://github.com/pezi/dart_periphery)
 
 ## Installation
 
 With pip:
 ``` text
 pip install python-periphery
 ```
```

### Comparing `python-periphery-2.3.0/periphery/__init__.py` & `python-periphery-2.4.0/periphery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 "Module version string."
 
-version = (2, 3, 0)
+version = (2, 4, 0)
 "Module version tuple."
 
 
 def sleep(seconds):
     """Sleep for the specified number of seconds.
 
     Args:
```

### Comparing `python-periphery-2.3.0/periphery/i2c.py` & `python-periphery-2.4.0/periphery/i2c.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.3.0/periphery/led.py` & `python-periphery-2.4.0/periphery/led.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.3.0/periphery/mmio.py` & `python-periphery-2.4.0/periphery/mmio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 import os
 import mmap
 import ctypes
-import struct
 
 
 # Alias long to int on Python 3
 if sys.version_info[0] >= 3:
     long = int
```

### Comparing `python-periphery-2.3.0/periphery/pwm.py` & `python-periphery-2.4.0/periphery/pwm.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 class PWMError(IOError):
     """Base class for PWM errors."""
     pass
 
 
 class PWM(object):
     # Number of retries to check for successful PWM export on open
-    PWM_STAT_RETRIES = 10
+    _PWM_STAT_RETRIES = 10
     # Delay between check for scucessful PWM export on open (100ms)
-    PWM_STAT_DELAY = 0.1
+    _PWM_STAT_DELAY = 0.1
 
     def __init__(self, chip, channel):
         """Instantiate a PWM object and open the sysfs PWM corresponding to the
         specified chip and channel.
 
         Args:
             chip (int): PWM chip number.
@@ -65,35 +65,35 @@
                 with open(os.path.join(chip_path, "export"), "w") as f_export:
                     f_export.write("{:d}\n".format(channel))
             except IOError as e:
                 raise PWMError(e.errno, "Exporting PWM channel: " + e.strerror)
 
             # Loop until PWM is exported
             exported = False
-            for i in range(PWM.PWM_STAT_RETRIES):
+            for i in range(PWM._PWM_STAT_RETRIES):
                 if os.path.isdir(channel_path):
                     exported = True
                     break
 
-                time.sleep(PWM.PWM_STAT_DELAY)
+                time.sleep(PWM._PWM_STAT_DELAY)
 
             if not exported:
                 raise TimeoutError("Exporting PWM: waiting for \"{:s}\" timed out".format(channel_path))
 
             # Loop until period is writable. This could take some time after
             # export as application of udev rules after export is asynchronous.
-            for i in range(PWM.PWM_STAT_RETRIES):
+            for i in range(PWM._PWM_STAT_RETRIES):
                 try:
                     with open(os.path.join(channel_path, "period"), 'w'):
                         break
                 except IOError as e:
-                    if e.errno != errno.EACCES or (e.errno == errno.EACCES and i == PWM.PWM_STAT_RETRIES - 1):
+                    if e.errno != errno.EACCES or (e.errno == errno.EACCES and i == PWM._PWM_STAT_RETRIES - 1):
                         raise PWMError(e.errno, "Opening PWM period: " + e.strerror)
 
-                time.sleep(PWM.PWM_STAT_DELAY)
+                time.sleep(PWM._PWM_STAT_DELAY)
 
         self._chip = chip
         self._channel = channel
         self._path = channel_path
 
         # Cache the period for fast duty cycle updates
         self._period_ns = self._get_period_ns()
```

### Comparing `python-periphery-2.3.0/periphery/serial.py` & `python-periphery-2.4.0/periphery/serial.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.3.0/periphery/spi.py` & `python-periphery-2.4.0/periphery/spi.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.3.0/python_periphery.egg-info/PKG-INFO` & `python-periphery-2.4.0/python_periphery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-periphery
-Version: 2.3.0
+Version: 2.4.0
 Summary: A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.
 Home-page: https://github.com/vsergeev/python-periphery
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
-Description: python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.
 Keywords: gpio spi led pwm i2c mmio serial uart embedded linux beaglebone raspberrypi rpi odroid
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
+License-File: LICENSE
+
+python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.
```

### Comparing `python-periphery-2.3.0/setup.py` & `python-periphery-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='python-periphery',
-    version='2.3.0',
+    version='2.4.0',
     description='A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.',
     author='vsergeev',
     author_email='v@sergeev.io',
     url='https://github.com/vsergeev/python-periphery',
     packages=['periphery'],
+    package_data={'periphery': ['*.pyi', 'py.typed']},
     long_description="""python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.""",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
```

