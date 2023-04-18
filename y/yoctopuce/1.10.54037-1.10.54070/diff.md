# Comparing `tmp/yoctopuce-1.10.54037.tar.gz` & `tmp/yoctopuce-1.10.54070.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yoctopuce-1.10.54037.tar", last modified: Fri Apr 14 07:22:34 2023, max compression
+gzip compressed data, was "dist/yoctopuce-1.10.54070.tar", last modified: Tue Apr 18 06:55:05 2023, max compression
```

## Comparing `yoctopuce-1.10.54037.tar` & `yoctopuce-1.10.54070.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:34.000000 yoctopuce-1.10.54037/
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Documentation/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)  1648958 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Documentation/yoctolib-python-EN.html
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)  1962920 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Documentation/yoctolib-python-FR.html
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:28.000000 yoctopuce-1.10.54037/Examples/
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2063 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2063 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-3D/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2535 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-3D/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2068 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1977 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Altimeter/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2147 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Altimeter/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Amp/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1954 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Amp/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Bridge/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1850 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Bridge/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Buzzer/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2467 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Buzzer/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-CO2/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1730 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-CO2/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2351 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color-V2/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2490 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color-V2/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Demo/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2013 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Demo/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Display/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2474 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Display/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-GPS/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1636 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-GPS/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-I2C/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2295 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-I2C/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-IO/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2505 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-IO/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Inclinometer/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2159 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Inclinometer/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Knob/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2417 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Knob/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-LatchedRelay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1714 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-LatchedRelay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Light/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1655 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Light/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Maxi-IO/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2524 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Maxi-IO/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBridge/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1924 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBridge/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2556 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1965 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2486 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiKnob/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2640 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiKnob/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2049 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:29.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1973 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2501 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Meteo/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2046 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Meteo/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MiniDisplay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2485 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MiniDisplay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Motor-DC/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2650 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Motor-DC/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PT100/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1660 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PT100/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Rx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1909 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Rx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Tx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2379 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Tx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerColor/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1929 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerColor/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerRelay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1708 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerRelay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Pressure/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1615 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Pressure/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Proximity/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1932 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Proximity/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS232/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1686 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS232/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS485/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2530 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS485/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RangeFinder/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2008 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RangeFinder/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Relay/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1855 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Relay/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-SPI/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2544 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-SPI/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Serial/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1858 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Serial/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Servo/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1784 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Servo/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1678 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature-IR/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1967 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature-IR/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermistor-C/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2495 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermistor-C/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermocouple/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1994 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermocouple/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-VOC/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1659 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-VOC/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Volt/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1794 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Volt/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-WatchdogDC/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1824 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-WatchdogDC/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Watt/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1612 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Watt/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1898 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1910 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/helloworld.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-Inventory/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)      889 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-Inventory/inventory.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-ModuleControl/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1598 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-ModuleControl/modulecontrol.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Doc-SaveSettings/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1230 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Doc-SaveSettings/savesettings.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Prog-ConfigureYoctoHub/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8915 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-ConfigureYoctoHub/hubconfig.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Prog-DataLogger/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2035 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-DataLogger/datalogger.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Prog-DevicesTree/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     4092 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-DevicesTree/demo.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Prog-Display-DoubleBuffering/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2407 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Display-DoubleBuffering/doubleBuffering.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:30.000000 yoctopuce-1.10.54037/Examples/Prog-Display-DrawBitmap/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2294 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Display-DrawBitmap/drawbitmap.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-Display-Sequence/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2071 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Display-Sequence/DisplaySequence.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-EventBased-Programming/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2628 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-EventBased-Programming/demo.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-ExportCSV/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1076 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-ExportCSV/exportcsv.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-FirmwareUpdate/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2855 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-FirmwareUpdate/firmwareupdate.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-GetDeviceLogs/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)      862 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-GetDeviceLogs/devicelog.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method1/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1608 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method1/demo.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method2/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1452 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method2/demo.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-Modbus/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1990 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Modbus/modbus.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-PyQt6/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     7916 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-PyQt6/demo.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-SensorMonitor/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     4798 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-SensorMonitor/SensorMonitor.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-YFiles-Example/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1694 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-YFiles-Example/YFilesExample.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-Blink/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1518 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-Blink/yocto-color-blink.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-V2-Blink/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2288 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-V2-Blink/yocto-color-blink.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:31.000000 yoctopuce-1.10.54037/Examples/Prog-YoctoHubSettings/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)      883 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/Examples/Prog-YoctoHubSettings/savesettings.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:33.000000 yoctopuce-1.10.54037/yoctopuce/
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:33.000000 yoctopuce-1.10.54037/yoctopuce/cdll/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   287528 2023-04-13 18:11:15.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-aarch64.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   300000 2023-04-13 18:11:03.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-amd64.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   625664 2023-04-13 18:11:13.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-armel.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   294116 2023-04-13 18:11:12.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-armhf.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   281688 2023-04-13 18:11:03.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-i386.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   693166 2023-04-13 18:11:03.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-mips.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   691271 2023-04-13 18:11:03.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-mipsel.so
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   573168 2023-04-13 18:11:14.000000 yoctopuce-1.10.54037/yoctopuce/cdll/libyapi.dylib
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   333048 2023-04-13 18:11:10.000000 yoctopuce-1.10.54037/yoctopuce/cdll/yapi.dll
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   391928 2023-04-13 18:11:10.000000 yoctopuce-1.10.54037/yoctopuce/cdll/yapi64.dll
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/__init__.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11364 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_accelerometer.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9700 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_altitude.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21608 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_anbutton.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   337587 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_api.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13804 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_arithmeticsensor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11027 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_audioin.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11122 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_audioout.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18314 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_bluetoothlink.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    22199 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_buzzer.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11714 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_carbondioxide.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)   214576 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_cellular.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18695 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_colorled.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45054 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_colorledcluster.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9135 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_compass.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8108 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_current.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    12206 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_currentloopoutput.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9933 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_daisychain.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1936 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_datalogger.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    25504 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_digitalio.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45888 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_display.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10237 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_dualpower.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13395 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_files.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19336 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_genericsensor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21726 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_gps.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6705 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_groundspeed.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    26593 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_gyro.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9791 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_hubport.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8790 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_humidity.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45638 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_i2cport.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    34172 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_inputcapture.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    27291 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_inputchain.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6510 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_latitude.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10038 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_led.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9757 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_lightsensor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6570 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_longitude.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10822 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_magnetometer.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    61656 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_messagebox.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    23078 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_motor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14465 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_multiaxiscontroller.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    22846 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_multicellweighscale.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14697 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_multisenscontroller.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    50421 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_network.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     7949 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_oscontrol.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    12966 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_power.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8200 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_poweroutput.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    20619 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_powersupply.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6515 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_pressure.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21586 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_proximity.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19181 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_pwminput.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    23078 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_pwmoutput.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8859 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_pwmpowersource.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11138 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_quadraturedecoder.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18202 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_rangefinder.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13174 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_realtimeclock.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    36403 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_refframe.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19457 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_relay.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8684 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_segmenteddisplay.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    68213 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_serialport.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16087 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_servo.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    48849 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_spiport.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    29819 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_steppermotor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19198 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_temperature.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9645 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_tilt.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6688 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_tvoc.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6545 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_voc.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8107 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_voltage.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10741 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_voltageoutput.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16134 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_wakeupmonitor.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16040 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_wakeupschedule.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    26764 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_watchdog.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    29068 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_weighscale.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    20011 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/yoctopuce/yocto_wireless.py
-drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-14 07:22:33.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     3715 2023-04-14 07:22:26.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/PKG-INFO
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6939 2023-04-14 07:22:27.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/SOURCES.txt
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)        1 2023-04-14 07:22:26.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/dependency_links.txt
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)        1 2023-04-14 07:22:26.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/not-zip-safe
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)       10 2023-04-14 07:22:26.000000 yoctopuce-1.10.54037/yoctopuce.egg-info/top_level.txt
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14231 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/FILES.txt
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1321 2018-12-17 09:44:09.000000 yoctopuce-1.10.54037/LICENSE.txt
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)      156 2023-04-13 19:00:23.000000 yoctopuce-1.10.54037/MANIFEST.in
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1422 2018-12-17 15:52:10.000000 yoctopuce-1.10.54037/README.md
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2334 2023-04-13 17:01:42.000000 yoctopuce-1.10.54037/setup.py
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)     3715 2023-04-14 07:22:34.000000 yoctopuce-1.10.54037/PKG-INFO
--rwxrwxrwx   0 yocto     (1000) yocto     (1000)       38 2023-04-14 07:22:34.000000 yoctopuce-1.10.54037/setup.cfg
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Documentation/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)  1648958 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Documentation/yoctolib-python-EN.html
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)  1962920 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Documentation/yoctolib-python-FR.html
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:54:59.000000 yoctopuce-1.10.54070/Examples/
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2063 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2063 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-3D/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2535 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-3D/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2068 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1977 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Altimeter/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2147 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Altimeter/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Amp/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1954 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Amp/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Bridge/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1850 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Bridge/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Buzzer/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2467 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Buzzer/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-CO2/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1730 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-CO2/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2351 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color-V2/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2490 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color-V2/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Demo/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2013 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Demo/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Display/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2474 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Display/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-GPS/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1636 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-GPS/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-I2C/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2295 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-I2C/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-IO/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2505 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-IO/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Inclinometer/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2159 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Inclinometer/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Knob/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2417 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Knob/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-LatchedRelay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1714 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-LatchedRelay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Light/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1655 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Light/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Maxi-IO/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2524 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Maxi-IO/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBridge/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1924 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBridge/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2556 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1965 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2486 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiKnob/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2640 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiKnob/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:00.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2049 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1973 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2501 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Meteo/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2046 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Meteo/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MiniDisplay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2485 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MiniDisplay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Motor-DC/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2650 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Motor-DC/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PT100/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1660 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PT100/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Rx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1909 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Rx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Tx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2379 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Tx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerColor/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1929 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerColor/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerRelay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1708 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerRelay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Pressure/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1615 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Pressure/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Proximity/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1932 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Proximity/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS232/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1686 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS232/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS485/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2530 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS485/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RangeFinder/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2008 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RangeFinder/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Relay/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1855 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Relay/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-SPI/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2544 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-SPI/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Serial/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1858 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Serial/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Servo/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1784 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Servo/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1678 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature-IR/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1967 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature-IR/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermistor-C/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2495 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermistor-C/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermocouple/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1994 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermocouple/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-VOC/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1659 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-VOC/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Volt/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1794 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Volt/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-WatchdogDC/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1824 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-WatchdogDC/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Watt/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1612 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Watt/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1898 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1910 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/helloworld.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-Inventory/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)      889 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-Inventory/inventory.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-ModuleControl/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1598 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-ModuleControl/modulecontrol.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Doc-SaveSettings/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1230 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Doc-SaveSettings/savesettings.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Prog-ConfigureYoctoHub/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8915 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-ConfigureYoctoHub/hubconfig.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Prog-DataLogger/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2035 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-DataLogger/datalogger.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Prog-DevicesTree/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     4092 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-DevicesTree/demo.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:01.000000 yoctopuce-1.10.54070/Examples/Prog-Display-DoubleBuffering/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2407 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Display-DoubleBuffering/doubleBuffering.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-Display-DrawBitmap/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2294 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Display-DrawBitmap/drawbitmap.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-Display-Sequence/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2071 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Display-Sequence/DisplaySequence.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-EventBased-Programming/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2628 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-EventBased-Programming/demo.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-ExportCSV/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1076 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-ExportCSV/exportcsv.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-FirmwareUpdate/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2855 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-FirmwareUpdate/firmwareupdate.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-GetDeviceLogs/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)      862 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-GetDeviceLogs/devicelog.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method1/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1608 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method1/demo.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method2/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1452 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method2/demo.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-Modbus/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1990 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Modbus/modbus.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-PyQt6/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     7916 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-PyQt6/demo.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-SensorMonitor/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     4798 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-SensorMonitor/SensorMonitor.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-YFiles-Example/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1694 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-YFiles-Example/YFilesExample.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-Blink/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1518 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-Blink/yocto-color-blink.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-V2-Blink/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2288 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-V2-Blink/yocto-color-blink.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:02.000000 yoctopuce-1.10.54070/Examples/Prog-YoctoHubSettings/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)      883 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/Examples/Prog-YoctoHubSettings/savesettings.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/yoctopuce/
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/yoctopuce/cdll/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   287528 2023-04-17 22:02:30.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-aarch64.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   300000 2023-04-17 22:02:16.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-amd64.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   625664 2023-04-17 22:02:27.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-armel.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   294116 2023-04-17 22:02:26.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-armhf.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   281688 2023-04-17 22:02:16.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-i386.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   693166 2023-04-17 22:02:16.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-mips.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   691271 2023-04-17 22:02:16.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-mipsel.so
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   573168 2023-04-17 22:02:28.000000 yoctopuce-1.10.54070/yoctopuce/cdll/libyapi.dylib
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   333048 2023-04-17 22:02:23.000000 yoctopuce-1.10.54070/yoctopuce/cdll/yapi.dll
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   391928 2023-04-17 22:02:23.000000 yoctopuce-1.10.54070/yoctopuce/cdll/yapi64.dll
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/__init__.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11364 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_accelerometer.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9700 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_altitude.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21608 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_anbutton.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   337401 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_api.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13804 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_arithmeticsensor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11027 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_audioin.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11122 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_audioout.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18314 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_bluetoothlink.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    22199 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_buzzer.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11714 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_carbondioxide.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)   214576 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_cellular.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18695 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_colorled.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45054 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_colorledcluster.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9135 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_compass.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8108 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_current.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    12206 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_currentloopoutput.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9933 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_daisychain.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1936 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_datalogger.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    25504 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_digitalio.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45888 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_display.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10237 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_dualpower.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13395 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_files.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19336 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_genericsensor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21726 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_gps.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6705 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_groundspeed.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    26593 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_gyro.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9791 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_hubport.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8790 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_humidity.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    45638 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_i2cport.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    34172 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_inputcapture.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    27291 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_inputchain.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6510 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_latitude.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10038 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_led.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9757 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_lightsensor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6570 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_longitude.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10822 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_magnetometer.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    61656 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_messagebox.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    23078 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_motor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14465 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_multiaxiscontroller.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    22846 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_multicellweighscale.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14697 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_multisenscontroller.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    50421 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_network.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     7949 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_oscontrol.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    12966 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_power.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8200 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_poweroutput.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    20619 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_powersupply.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6515 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_pressure.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    21586 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_proximity.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19181 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_pwminput.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    23078 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_pwmoutput.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8859 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_pwmpowersource.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    11138 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_quadraturedecoder.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    18202 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_rangefinder.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    13174 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_realtimeclock.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    36403 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_refframe.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19457 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_relay.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8684 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_segmenteddisplay.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    68213 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_serialport.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16087 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_servo.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    48849 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_spiport.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    29819 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_steppermotor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    19198 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_temperature.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     9645 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_tilt.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6688 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_tvoc.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6545 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_voc.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     8107 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_voltage.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    10741 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_voltageoutput.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16134 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_wakeupmonitor.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    16040 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_wakeupschedule.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    26764 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_watchdog.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    29068 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_weighscale.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    20011 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/yoctopuce/yocto_wireless.py
+drwxrwxrwx   0 yocto     (1000) yocto     (1000)        0 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     3715 2023-04-18 06:54:55.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/PKG-INFO
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     6939 2023-04-18 06:54:57.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)        1 2023-04-18 06:54:55.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)        1 2023-04-18 06:54:55.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/not-zip-safe
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)       10 2023-04-18 06:54:55.000000 yoctopuce-1.10.54070/yoctopuce.egg-info/top_level.txt
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)    14231 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/FILES.txt
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1321 2018-12-17 09:44:09.000000 yoctopuce-1.10.54070/LICENSE.txt
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)      156 2023-04-17 22:51:37.000000 yoctopuce-1.10.54070/MANIFEST.in
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     1422 2018-12-17 15:52:10.000000 yoctopuce-1.10.54070/README.md
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     2334 2023-04-17 20:53:02.000000 yoctopuce-1.10.54070/setup.py
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)     3715 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/PKG-INFO
+-rwxrwxrwx   0 yocto     (1000) yocto     (1000)       38 2023-04-18 06:55:04.000000 yoctopuce-1.10.54070/setup.cfg
```

### Comparing `yoctopuce-1.10.54037/Documentation/yoctolib-python-EN.html` & `yoctopuce-1.10.54070/Documentation/yoctolib-python-EN.html`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Documentation/yoctolib-python-FR.html` & `yoctopuce-1.10.54070/Documentation/yoctolib-python-FR.html`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Rx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-0-10V-Tx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-3D/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-3D/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Rx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-4-20mA-Tx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Altimeter/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Altimeter/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Amp/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Amp/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Bridge/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Bridge/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Buzzer/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Buzzer/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-CO2/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-CO2/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Color-V2/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Color-V2/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Demo/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Demo/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Display/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Display/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-GPS/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-GPS/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-I2C/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-I2C/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-IO/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-IO/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Inclinometer/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Inclinometer/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Knob/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Knob/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-LatchedRelay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-LatchedRelay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Light/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Light/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Maxi-IO/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Maxi-IO/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBridge/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBridge/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiBuzzer/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiCoupler/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiDisplay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiKnob/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiKnob/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiMicroVolt-Rx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiPowerRelay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MaxiThermistor/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Meteo/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Meteo/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-MiniDisplay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-MiniDisplay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Motor-DC/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Motor-DC/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PT100/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PT100/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Rx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Rx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PWM-Tx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PWM-Tx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerColor/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerColor/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-PowerRelay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-PowerRelay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Pressure/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Pressure/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Proximity/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Proximity/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS232/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS232/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RS485/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RS485/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-RangeFinder/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-RangeFinder/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Relay/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Relay/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-SPI/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-SPI/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Serial/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Serial/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Servo/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Servo/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Temperature-IR/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Temperature-IR/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermistor-C/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermistor-C/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Thermocouple/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Thermocouple/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-VOC/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-VOC/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Volt/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Volt/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-WatchdogDC/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-WatchdogDC/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-Watt/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-Watt/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/helloworld.py` & `yoctopuce-1.10.54070/Examples/Doc-GettingStarted-Yocto-milliVolt-Rx-BNC/helloworld.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-Inventory/inventory.py` & `yoctopuce-1.10.54070/Examples/Doc-Inventory/inventory.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-ModuleControl/modulecontrol.py` & `yoctopuce-1.10.54070/Examples/Doc-ModuleControl/modulecontrol.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Doc-SaveSettings/savesettings.py` & `yoctopuce-1.10.54070/Examples/Doc-SaveSettings/savesettings.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-ConfigureYoctoHub/hubconfig.py` & `yoctopuce-1.10.54070/Examples/Prog-ConfigureYoctoHub/hubconfig.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-DataLogger/datalogger.py` & `yoctopuce-1.10.54070/Examples/Prog-DataLogger/datalogger.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-DevicesTree/demo.py` & `yoctopuce-1.10.54070/Examples/Prog-DevicesTree/demo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Display-DoubleBuffering/doubleBuffering.py` & `yoctopuce-1.10.54070/Examples/Prog-Display-DoubleBuffering/doubleBuffering.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Display-DrawBitmap/drawbitmap.py` & `yoctopuce-1.10.54070/Examples/Prog-Display-DrawBitmap/drawbitmap.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Display-Sequence/DisplaySequence.py` & `yoctopuce-1.10.54070/Examples/Prog-Display-Sequence/DisplaySequence.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-EventBased-Programming/demo.py` & `yoctopuce-1.10.54070/Examples/Prog-EventBased-Programming/demo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-ExportCSV/exportcsv.py` & `yoctopuce-1.10.54070/Examples/Prog-ExportCSV/exportcsv.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-FirmwareUpdate/firmwareupdate.py` & `yoctopuce-1.10.54070/Examples/Prog-FirmwareUpdate/firmwareupdate.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-GetDeviceLogs/devicelog.py` & `yoctopuce-1.10.54070/Examples/Prog-GetDeviceLogs/devicelog.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method1/demo.py` & `yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method1/demo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-HubDiscovery-method2/demo.py` & `yoctopuce-1.10.54070/Examples/Prog-HubDiscovery-method2/demo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Modbus/modbus.py` & `yoctopuce-1.10.54070/Examples/Prog-Modbus/modbus.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-PyQt6/demo.py` & `yoctopuce-1.10.54070/Examples/Prog-PyQt6/demo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-SensorMonitor/SensorMonitor.py` & `yoctopuce-1.10.54070/Examples/Prog-SensorMonitor/SensorMonitor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-YFiles-Example/YFilesExample.py` & `yoctopuce-1.10.54070/Examples/Prog-YFiles-Example/YFilesExample.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-Blink/yocto-color-blink.py` & `yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-Blink/yocto-color-blink.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-Yocto-Color-V2-Blink/yocto-color-blink.py` & `yoctopuce-1.10.54070/Examples/Prog-Yocto-Color-V2-Blink/yocto-color-blink.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/Examples/Prog-YoctoHubSettings/savesettings.py` & `yoctopuce-1.10.54070/Examples/Prog-YoctoHubSettings/savesettings.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-aarch64.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-aarch64.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 1e5132027f1d9c68c9e9b0fafdfebfb772d68dc3
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7c883571258bee8197448fc7e91253ddd9116c8e
```

#### strings --all --bytes=8 {}

```diff
@@ -452,16 +452,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:18:31
+1.10.54070
+Apr 17 2023 23:09:08
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -178,16 +178,16 @@
   0x00041520 6520636f 6e6e6563 74696f6e 00000000 e connection....
   0x00041530 47455420 2f617069 2f6d6f64 756c652f GET /api/module/
   0x00041540 6669726d 77617265 52656c65 6173652e firmwareRelease.
   0x00041550 6a736f6e 200d0a0d 0a000000 00000000 json ...........
   0x00041560 456e756d 65726174 696f6e20 6661696c Enumeration fail
   0x00041570 65642066 6f722025 733a2564 20282573 ed for %s:%d (%s
   0x00041580 29000000 00000000 312e3130 2e353430 ).......1.10.540
-  0x00041590 33370000 00000000 41707220 31332032 37......Apr 13 2
-  0x000415a0 30323320 31393a31 383a3331 00000000 023 19:18:31....
+  0x00041590 37300000 00000000 41707220 31372032 70......Apr 17 2
+  0x000415a0 30323320 32333a30 393a3038 00000000 023 23:09:08....
   0x000415b0 596f6374 6f707563 65000000 00000000 Yoctopuce.......
   0x000415c0 25733a2f 2f25733a 25642573 25730000 %s://%s:%d%s%s..
   0x000415d0 4e6f2066 756e6374 696f6e20 6f662074 No function of t
   0x000415e0 68617420 636c6173 73000000 00000000 hat class.......
   0x000415f0 200d0a0d 0a000000 41636365 73732064  .......Access d
   0x00041600 656e6965 643a2061 646d696e 20637265 enied: admin cre
   0x00041610 64656e74 69616c73 20726571 75697265 dentials require
@@ -442,15 +442,15 @@
   0x000425a0 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
   0x000425b0 696c6500 00000000 496e636f 72726563 ile.....Incorrec
   0x000425c0 74206669 6c652073 697a6520 6f722063 t file size or c
   0x000425d0 6f727275 70742066 696c6500 00000000 orrupt file.....
   0x000425e0 496e7661 6c696420 70726f67 72616d6d Invalid programm
   0x000425f0 696e6720 746f6f6c 73207265 76697369 ing tools revisi
   0x00042600 6f6e206f 7220636f 72727570 74206669 on or corrupt fi
-  0x00042610 6c650000 00000000 35343033 37000000 le......54037...
+  0x00042610 6c650000 00000000 35343037 30000000 le......54070...
   0x00042620 54686973 20666972 6d776172 65206973 This firmware is
   0x00042630 20746f6f 20726563 656e742c 20706c65  too recent, ple
   0x00042640 61736520 75706772 61646520 796f7572 ase upgrade your
   0x00042650 20566972 7475616c 48756220 6f722059  VirtualHub or Y
   0x00042660 6f63746f 70756365 206c6962 72617279 octopuce library
   0x00042670 00000000 00000000 546f6f20 6d616e79 ........Too many
   0x00042680 20524f4d 207a6f6e 65732069 6e202e62  ROM zones in .b
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-amd64.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-amd64.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: dfb55254b1e8b00642b410ffc9d2f29cfadba427
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0e48d433771b16a78d3b762eea97a505cf9ff17d
```

#### strings --all --bytes=8 {}

```diff
@@ -454,16 +454,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:02:27
+1.10.54070
+Apr 17 2023 22:53:42
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -167,17 +167,17 @@
   0x0003e7f0 6f737420 68617320 636c6f73 65207468 ost has close th
   0x0003e800 6520636f 6e6e6563 74696f6e 00000000 e connection....
   0x0003e810 47455420 2f617069 2f6d6f64 756c652f GET /api/module/
   0x0003e820 6669726d 77617265 52656c65 6173652e firmwareRelease.
   0x0003e830 6a736f6e 200d0a0d 0a000000 00000000 json ...........
   0x0003e840 456e756d 65726174 696f6e20 6661696c Enumeration fail
   0x0003e850 65642066 6f722025 733a2564 20282573 ed for %s:%d (%s
-  0x0003e860 2900312e 31302e35 34303337 00417072 ).1.10.54037.Apr
-  0x0003e870 20313320 32303233 2031393a 30323a32  13 2023 19:02:2
-  0x0003e880 3700596f 63746f70 75636500 25733a2f 7.Yoctopuce.%s:/
+  0x0003e860 2900312e 31302e35 34303730 00417072 ).1.10.54070.Apr
+  0x0003e870 20313720 32303233 2032323a 35333a34  17 2023 22:53:4
+  0x0003e880 3200596f 63746f70 75636500 25733a2f 2.Yoctopuce.%s:/
   0x0003e890 2f25733a 25642573 2573004e 6f206675 /%s:%d%s%s.No fu
   0x0003e8a0 6e637469 6f6e206f 66207468 61742063 nction of that c
   0x0003e8b0 6c617373 00200d0a 0d0a0000 00000000 lass. ..........
   0x0003e8c0 41636365 73732064 656e6965 643a2061 Access denied: a
   0x0003e8d0 646d696e 20637265 64656e74 69616c73 dmin credentials
   0x0003e8e0 20726571 75697265 64006875 62202573  required.hub %s
   0x0003e8f0 20697320 6e6f7420 72656164 79006875  is not ready.hu
@@ -433,15 +433,15 @@
   0x0003f890 6d616e79 207a6f6e 65732069 6e202e62 many zones in .b
   0x0003f8a0 796e2066 696c6500 496e636f 72726563 yn file.Incorrec
   0x0003f8b0 74206669 6c652073 697a6520 6f722063 t file size or c
   0x0003f8c0 6f727275 70742066 696c6500 00000000 orrupt file.....
   0x0003f8d0 496e7661 6c696420 70726f67 72616d6d Invalid programm
   0x0003f8e0 696e6720 746f6f6c 73207265 76697369 ing tools revisi
   0x0003f8f0 6f6e206f 7220636f 72727570 74206669 on or corrupt fi
-  0x0003f900 6c650035 34303337 00000000 00000000 le.54037........
+  0x0003f900 6c650035 34303730 00000000 00000000 le.54070........
   0x0003f910 54686973 20666972 6d776172 65206973 This firmware is
   0x0003f920 20746f6f 20726563 656e742c 20706c65  too recent, ple
   0x0003f930 61736520 75706772 61646520 796f7572 ase upgrade your
   0x0003f940 20566972 7475616c 48756220 6f722059  VirtualHub or Y
   0x0003f950 6f63746f 70756365 206c6962 72617279 octopuce library
   0x0003f960 00000000 00000000 546f6f20 6d616e79 ........Too many
   0x0003f970 20524f4d 207a6f6e 65732069 6e202e62  ROM zones in .b
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-armel.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-armel.so`

 * *Files 0% similar despite different names*

#### strings --all --bytes=8 {}

```diff
@@ -439,16 +439,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:18:03
+1.10.54070
+Apr 17 2023 23:09:13
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -148,16 +148,16 @@
   0x0004bdc8 68617320 636c6f73 65207468 6520636f has close the co
   0x0004bdd8 6e6e6563 74696f6e 00000000 47455420 nnection....GET 
   0x0004bde8 2f617069 2f6d6f64 756c652f 6669726d /api/module/firm
   0x0004bdf8 77617265 52656c65 6173652e 6a736f6e wareRelease.json
   0x0004be08 200d0a0d 0a000000 456e756d 65726174  .......Enumerat
   0x0004be18 696f6e20 6661696c 65642066 6f722025 ion failed for %
   0x0004be28 733a2564 20282573 29000000 312e3130 s:%d (%s)...1.10
-  0x0004be38 2e353430 33370000 41707220 31332032 .54037..Apr 13 2
-  0x0004be48 30323320 31393a31 383a3033 00000000 023 19:18:03....
+  0x0004be38 2e353430 37300000 41707220 31372032 .54070..Apr 17 2
+  0x0004be48 30323320 32333a30 393a3133 00000000 023 23:09:13....
   0x0004be58 596f6374 6f707563 65000000 25733a2f Yoctopuce...%s:/
   0x0004be68 2f25733a 25642573 25730000 4e6f2066 /%s:%d%s%s..No f
   0x0004be78 756e6374 696f6e20 6f662074 68617420 unction of that 
   0x0004be88 636c6173 73000000 200d0a0d 0a000000 class... .......
   0x0004be98 41636365 73732064 656e6965 643a2061 Access denied: a
   0x0004bea8 646d696e 20637265 64656e74 69616c73 dmin credentials
   0x0004beb8 20726571 75697265 64000000 68756220  required...hub 
@@ -393,16 +393,16 @@
   0x0004cd18 6973696f 6e000000 546f6f20 6d616e79 ision...Too many
   0x0004cd28 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
   0x0004cd38 696c6500 496e636f 72726563 74206669 ile.Incorrect fi
   0x0004cd48 6c652073 697a6520 6f722063 6f727275 le size or corru
   0x0004cd58 70742066 696c6500 496e7661 6c696420 pt file.Invalid 
   0x0004cd68 70726f67 72616d6d 696e6720 746f6f6c programming tool
   0x0004cd78 73207265 76697369 6f6e206f 7220636f s revision or co
-  0x0004cd88 72727570 74206669 6c650000 35343033 rrupt file..5403
-  0x0004cd98 37000000 54686973 20666972 6d776172 7...This firmwar
+  0x0004cd88 72727570 74206669 6c650000 35343037 rrupt file..5407
+  0x0004cd98 30000000 54686973 20666972 6d776172 0...This firmwar
   0x0004cda8 65206973 20746f6f 20726563 656e742c e is too recent,
   0x0004cdb8 20706c65 61736520 75706772 61646520  please upgrade 
   0x0004cdc8 796f7572 20566972 7475616c 48756220 your VirtualHub 
   0x0004cdd8 6f722059 6f63746f 70756365 206c6962 or Yoctopuce lib
   0x0004cde8 72617279 00000000 546f6f20 6d616e79 rary....Too many
   0x0004cdf8 20524f4d 207a6f6e 65732069 6e202e62  ROM zones in .b
   0x0004ce08 796e2066 696c6500 546f6f20 6d616e79 yn file.Too many
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-armhf.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-armhf.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5356b990b054c5d9f4d1c641c361b2c71decf9b5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d7ccad47b1b86691c738f0ce984b55bf07f6f7fb
```

#### strings --all --bytes=8 {}

```diff
@@ -450,16 +450,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:18:06
+1.10.54070
+Apr 17 2023 23:09:25
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -148,16 +148,16 @@
   0x00043a24 68617320 636c6f73 65207468 6520636f has close the co
   0x00043a34 6e6e6563 74696f6e 00000000 47455420 nnection....GET 
   0x00043a44 2f617069 2f6d6f64 756c652f 6669726d /api/module/firm
   0x00043a54 77617265 52656c65 6173652e 6a736f6e wareRelease.json
   0x00043a64 200d0a0d 0a000000 456e756d 65726174  .......Enumerat
   0x00043a74 696f6e20 6661696c 65642066 6f722025 ion failed for %
   0x00043a84 733a2564 20282573 29000000 312e3130 s:%d (%s)...1.10
-  0x00043a94 2e353430 33370000 41707220 31332032 .54037..Apr 13 2
-  0x00043aa4 30323320 31393a31 383a3036 00000000 023 19:18:06....
+  0x00043a94 2e353430 37300000 41707220 31372032 .54070..Apr 17 2
+  0x00043aa4 30323320 32333a30 393a3235 00000000 023 23:09:25....
   0x00043ab4 596f6374 6f707563 65000000 25733a2f Yoctopuce...%s:/
   0x00043ac4 2f25733a 25642573 25730000 4e6f2066 /%s:%d%s%s..No f
   0x00043ad4 756e6374 696f6e20 6f662074 68617420 unction of that 
   0x00043ae4 636c6173 73000000 200d0a0d 0a000000 class... .......
   0x00043af4 41636365 73732064 656e6965 643a2061 Access denied: a
   0x00043b04 646d696e 20637265 64656e74 69616c73 dmin credentials
   0x00043b14 20726571 75697265 64000000 68756220  required...hub 
@@ -393,16 +393,16 @@
   0x00044974 6973696f 6e000000 546f6f20 6d616e79 ision...Too many
   0x00044984 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
   0x00044994 696c6500 496e636f 72726563 74206669 ile.Incorrect fi
   0x000449a4 6c652073 697a6520 6f722063 6f727275 le size or corru
   0x000449b4 70742066 696c6500 496e7661 6c696420 pt file.Invalid 
   0x000449c4 70726f67 72616d6d 696e6720 746f6f6c programming tool
   0x000449d4 73207265 76697369 6f6e206f 7220636f s revision or co
-  0x000449e4 72727570 74206669 6c650000 35343033 rrupt file..5403
-  0x000449f4 37000000 54686973 20666972 6d776172 7...This firmwar
+  0x000449e4 72727570 74206669 6c650000 35343037 rrupt file..5407
+  0x000449f4 30000000 54686973 20666972 6d776172 0...This firmwar
   0x00044a04 65206973 20746f6f 20726563 656e742c e is too recent,
   0x00044a14 20706c65 61736520 75706772 61646520  please upgrade 
   0x00044a24 796f7572 20566972 7475616c 48756220 your VirtualHub 
   0x00044a34 6f722059 6f63746f 70756365 206c6962 or Yoctopuce lib
   0x00044a44 72617279 00000000 546f6f20 6d616e79 rary....Too many
   0x00044a54 20524f4d 207a6f6e 65732069 6e202e62  ROM zones in .b
   0x00044a64 796e2066 696c6500 546f6f20 6d616e79 yn file.Too many
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-i386.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-i386.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 157fe58324384adcb8183c803f7e6351983c7b27
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3f80851997501a805c00bc99c8e7769084d1d2e9
```

#### strings --all --bytes=8 {}

```diff
@@ -453,16 +453,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:03:31
+1.10.54070
+Apr 17 2023 22:54:45
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -163,17 +163,17 @@
   0x0003a1d0 74652068 6f737420 68617320 636c6f73 te host has clos
   0x0003a1e0 65207468 6520636f 6e6e6563 74696f6e e the connection
   0x0003a1f0 00000000 47455420 2f617069 2f6d6f64 ....GET /api/mod
   0x0003a200 756c652f 6669726d 77617265 52656c65 ule/firmwareRele
   0x0003a210 6173652e 6a736f6e 200d0a0d 0a000000 ase.json .......
   0x0003a220 456e756d 65726174 696f6e20 6661696c Enumeration fail
   0x0003a230 65642066 6f722025 733a2564 20282573 ed for %s:%d (%s
-  0x0003a240 2900312e 31302e35 34303337 00417072 ).1.10.54037.Apr
-  0x0003a250 20313320 32303233 2031393a 30333a33  13 2023 19:03:3
-  0x0003a260 3100596f 63746f70 75636500 25733a2f 1.Yoctopuce.%s:/
+  0x0003a240 2900312e 31302e35 34303730 00417072 ).1.10.54070.Apr
+  0x0003a250 20313720 32303233 2032323a 35343a34  17 2023 22:54:4
+  0x0003a260 3500596f 63746f70 75636500 25733a2f 5.Yoctopuce.%s:/
   0x0003a270 2f25733a 25642573 2573004e 6f206675 /%s:%d%s%s.No fu
   0x0003a280 6e637469 6f6e206f 66207468 61742063 nction of that c
   0x0003a290 6c617373 00200d0a 0d0a0000 41636365 lass. ......Acce
   0x0003a2a0 73732064 656e6965 643a2061 646d696e ss denied: admin
   0x0003a2b0 20637265 64656e74 69616c73 20726571  credentials req
   0x0003a2c0 75697265 64006875 62202573 20697320 uired.hub %s is 
   0x0003a2d0 6e6f7420 72656164 79006875 62206973 not ready.hub is
@@ -423,15 +423,15 @@
   0x0003b210 65766973 696f6e00 546f6f20 6d616e79 evision.Too many
   0x0003b220 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
   0x0003b230 696c6500 496e636f 72726563 74206669 ile.Incorrect fi
   0x0003b240 6c652073 697a6520 6f722063 6f727275 le size or corru
   0x0003b250 70742066 696c6500 496e7661 6c696420 pt file.Invalid 
   0x0003b260 70726f67 72616d6d 696e6720 746f6f6c programming tool
   0x0003b270 73207265 76697369 6f6e206f 7220636f s revision or co
-  0x0003b280 72727570 74206669 6c650035 34303337 rrupt file.54037
+  0x0003b280 72727570 74206669 6c650035 34303730 rrupt file.54070
   0x0003b290 00000000 54686973 20666972 6d776172 ....This firmwar
   0x0003b2a0 65206973 20746f6f 20726563 656e742c e is too recent,
   0x0003b2b0 20706c65 61736520 75706772 61646520  please upgrade 
   0x0003b2c0 796f7572 20566972 7475616c 48756220 your VirtualHub 
   0x0003b2d0 6f722059 6f63746f 70756365 206c6962 or Yoctopuce lib
   0x0003b2e0 72617279 00000000 546f6f20 6d616e79 rary....Too many
   0x0003b2f0 20524f4d 207a6f6e 65732069 6e202e62  ROM zones in .b
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-mips.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-mips.so`

 * *Files 0% similar despite different names*

#### strings --all --bytes=8 {}

```diff
@@ -462,16 +462,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:04:28
+1.10.54070
+Apr 17 2023 22:55:41
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -171,17 +171,17 @@
   0x00060c50 74652068 6f737420 68617320 636c6f73 te host has clos
   0x00060c60 65207468 6520636f 6e6e6563 74696f6e e the connection
   0x00060c70 00000000 47455420 2f617069 2f6d6f64 ....GET /api/mod
   0x00060c80 756c652f 6669726d 77617265 52656c65 ule/firmwareRele
   0x00060c90 6173652e 6a736f6e 200d0a0d 0a000000 ase.json .......
   0x00060ca0 456e756d 65726174 696f6e20 6661696c Enumeration fail
   0x00060cb0 65642066 6f722025 733a2564 20282573 ed for %s:%d (%s
-  0x00060cc0 29000000 312e3130 2e353430 33370000 )...1.10.54037..
-  0x00060cd0 41707220 31332032 30323320 31393a30 Apr 13 2023 19:0
-  0x00060ce0 343a3238 00000000 596f6374 6f707563 4:28....Yoctopuc
+  0x00060cc0 29000000 312e3130 2e353430 37300000 )...1.10.54070..
+  0x00060cd0 41707220 31372032 30323320 32323a35 Apr 17 2023 22:5
+  0x00060ce0 353a3431 00000000 596f6374 6f707563 5:41....Yoctopuc
   0x00060cf0 65000000 25733a2f 2f25733a 25642573 e...%s://%s:%d%s
   0x00060d00 25730000 4e6f2066 756e6374 696f6e20 %s..No function 
   0x00060d10 6f662074 68617420 636c6173 73000000 of that class...
   0x00060d20 200d0a0d 0a000000 41636365 73732064  .......Access d
   0x00060d30 656e6965 643a2061 646d696e 20637265 enied: admin cre
   0x00060d40 64656e74 69616c73 20726571 75697265 dentials require
   0x00060d50 64000000 68756220 25732069 73206e6f d...hub %s is no
@@ -439,15 +439,15 @@
   0x00061d10 6e000000 546f6f20 6d616e79 207a6f6e n...Too many zon
   0x00061d20 65732069 6e202e62 796e2066 696c6500 es in .byn file.
   0x00061d30 496e636f 72726563 74206669 6c652073 Incorrect file s
   0x00061d40 697a6520 6f722063 6f727275 70742066 ize or corrupt f
   0x00061d50 696c6500 496e7661 6c696420 70726f67 ile.Invalid prog
   0x00061d60 72616d6d 696e6720 746f6f6c 73207265 ramming tools re
   0x00061d70 76697369 6f6e206f 7220636f 72727570 vision or corrup
-  0x00061d80 74206669 6c650000 35343033 37000000 t file..54037...
+  0x00061d80 74206669 6c650000 35343037 30000000 t file..54070...
   0x00061d90 54686973 20666972 6d776172 65206973 This firmware is
   0x00061da0 20746f6f 20726563 656e742c 20706c65  too recent, ple
   0x00061db0 61736520 75706772 61646520 796f7572 ase upgrade your
   0x00061dc0 20566972 7475616c 48756220 6f722059  VirtualHub or Y
   0x00061dd0 6f63746f 70756365 206c6962 72617279 octopuce library
   0x00061de0 00000000 546f6f20 6d616e79 20524f4d ....Too many ROM
   0x00061df0 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi-mipsel.so` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi-mipsel.so`

 * *Files 0% similar despite different names*

#### strings --all --bytes=8 {}

```diff
@@ -461,16 +461,16 @@
 Too many network hub registered
 hub not ready
 http://%s
 GET /api/module/serial?serial=&. 
 Remote host has close the connection
 GET /api/module/firmwareRelease.json 
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:05:18
+1.10.54070
+Apr 17 2023 22:56:31
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 Access denied: admin credentials required
 hub %s is not ready
 hub is not ready
 Preloading of URL is only supported for HTTP callback.
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -171,17 +171,17 @@
   0x0005f850 74652068 6f737420 68617320 636c6f73 te host has clos
   0x0005f860 65207468 6520636f 6e6e6563 74696f6e e the connection
   0x0005f870 00000000 47455420 2f617069 2f6d6f64 ....GET /api/mod
   0x0005f880 756c652f 6669726d 77617265 52656c65 ule/firmwareRele
   0x0005f890 6173652e 6a736f6e 200d0a0d 0a000000 ase.json .......
   0x0005f8a0 456e756d 65726174 696f6e20 6661696c Enumeration fail
   0x0005f8b0 65642066 6f722025 733a2564 20282573 ed for %s:%d (%s
-  0x0005f8c0 29000000 312e3130 2e353430 33370000 )...1.10.54037..
-  0x0005f8d0 41707220 31332032 30323320 31393a30 Apr 13 2023 19:0
-  0x0005f8e0 353a3138 00000000 596f6374 6f707563 5:18....Yoctopuc
+  0x0005f8c0 29000000 312e3130 2e353430 37300000 )...1.10.54070..
+  0x0005f8d0 41707220 31372032 30323320 32323a35 Apr 17 2023 22:5
+  0x0005f8e0 363a3331 00000000 596f6374 6f707563 6:31....Yoctopuc
   0x0005f8f0 65000000 25733a2f 2f25733a 25642573 e...%s://%s:%d%s
   0x0005f900 25730000 4e6f2066 756e6374 696f6e20 %s..No function 
   0x0005f910 6f662074 68617420 636c6173 73000000 of that class...
   0x0005f920 200d0a0d 0a000000 41636365 73732064  .......Access d
   0x0005f930 656e6965 643a2061 646d696e 20637265 enied: admin cre
   0x0005f940 64656e74 69616c73 20726571 75697265 dentials require
   0x0005f950 64000000 68756220 25732069 73206e6f d...hub %s is no
@@ -439,15 +439,15 @@
   0x00060910 6e000000 546f6f20 6d616e79 207a6f6e n...Too many zon
   0x00060920 65732069 6e202e62 796e2066 696c6500 es in .byn file.
   0x00060930 496e636f 72726563 74206669 6c652073 Incorrect file s
   0x00060940 697a6520 6f722063 6f727275 70742066 ize or corrupt f
   0x00060950 696c6500 496e7661 6c696420 70726f67 ile.Invalid prog
   0x00060960 72616d6d 696e6720 746f6f6c 73207265 ramming tools re
   0x00060970 76697369 6f6e206f 7220636f 72727570 vision or corrup
-  0x00060980 74206669 6c650000 35343033 37000000 t file..54037...
+  0x00060980 74206669 6c650000 35343037 30000000 t file..54070...
   0x00060990 54686973 20666972 6d776172 65206973 This firmware is
   0x000609a0 20746f6f 20726563 656e742c 20706c65  too recent, ple
   0x000609b0 61736520 75706772 61646520 796f7572 ase upgrade your
   0x000609c0 20566972 7475616c 48756220 6f722059  VirtualHub or Y
   0x000609d0 6f63746f 70756365 206c6962 72617279 octopuce library
   0x000609e0 00000000 546f6f20 6d616e79 20524f4d ....Too many ROM
   0x000609f0 207a6f6e 65732069 6e202e62 796e2066  zones in .byn f
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/libyapi.dylib` & `yoctopuce-1.10.54070/yoctopuce/cdll/libyapi.dylib`

 * *Files 0% similar despite different names*

#### strings -a -n 8 {}

```diff
@@ -7,15 +7,14 @@
 __DATA_CONST
 __common
 __LINKEDIT
 /usr/local/lib/libyapi.dylib
 /usr/lib/libSystem.B.dylib
 /System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
 /System/Library/Frameworks/IOKit.framework/Versions/A/IOKit
-/usr/lib/libobjc.A.dylib
 AWAVAUATSH
 [A\A]A^A_]
 https://H9
 AWAVAUATSH
 [A\A]A^A_]
 AWAVAUATSH
 [A\A]A^A_]
@@ -800,16 +799,16 @@
 productId
 networkUrl
 baseType
 hardwareId
 advertisedValue
 Disable JZON encoding for hub %
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:02:00
+1.10.54070
+Apr 17 2023 22:53:19
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 ASync request for %s failed. Retrying after yapiUpdateDeviceList
 yapiUpdateDeviceList failled too with %s
 %s"%s/%s=
 Transfer-Encoding
@@ -1400,15 +1399,14 @@
 _getsockopt
 _gettimeofday
 _inet_addr
 _kCFAllocatorDefault
 _kCFRunLoopDefaultMode
 _kCFTypeDictionaryKeyCallBacks
 _kCFTypeDictionaryValueCallBacks
-_objc_msgSend
 _opendir$INODE64
 _pthread_attr_destroy
 _pthread_attr_init
 _pthread_attr_setdetachstate
 _pthread_cancel
 _pthread_cond_destroy
 _pthread_cond_init
@@ -1953,17 +1951,16 @@
 _yTryEnterCriticalSection
 _yLeaveCriticalSection
 _yDeleteCriticalSection
 _initTsdKey
 _yInitKeyOnce
 _yNextThreadIdx
 _yTsdKey
-libyapi-55554944af3f5f9a013e3c5fbce4367b642b2035
-pJO#>eB6d
-pJEU(\hV
+libyapi-555549445e7e2953b18a3407bb0cb69f5766f7f7
+JO#>eB6d
 <?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
 <plist version="1.0">
 	<key>com.apple.application-identifier</key>
 	<string></string>
 </plist>
 __cstring
@@ -2365,16 +2362,16 @@
 productId
 networkUrl
 baseType
 hardwareId
 advertisedValue
 Disable JZON encoding for hub %
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:02:01
+1.10.54070
+Apr 17 2023 22:53:20
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 ASync request for %s failed. Retrying after yapiUpdateDeviceList
 yapiUpdateDeviceList failled too with %s
 %s"%s/%s=
 !;invalid
@@ -3505,15 +3502,15 @@
 _yTryEnterCriticalSection
 _yLeaveCriticalSection
 _yDeleteCriticalSection
 _initTsdKey
 _yInitKeyOnce
 _yNextThreadIdx
 _yTsdKey
-libyapi-55554944af3f5f9a013e3c5fbce4367b642b2035
+libyapi-555549445e7e2953b18a3407bb0cb69f5766f7f7
 gHYMr,HL,
 <?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
 <plist version="1.0">
 	<key>com.apple.application-identifier</key>
 	<string></string>
 </plist>
```

#### llvm-readobj --file-headers {}

```diff
@@ -3,16 +3,16 @@
 Arch: x86_64
 AddressSize: 64bit
 MachHeader {
   Magic: Magic64 (0xFEEDFACF)
   CpuType: X86-64 (0x1000007)
   CpuSubType: CPU_SUBTYPE_X86_64_ALL (0x3)
   FileType: DynamicLibrary (0x6)
-  NumOfLoadCommands: 19
-  SizeOfLoadCommands: 1784
+  NumOfLoadCommands: 18
+  SizeOfLoadCommands: 1728
   Flags [ (0x100085)
     MH_DYLDLINK (0x4)
     MH_NOUNDEFS (0x1)
     MH_NO_REEXPORTED_DYLIBS (0x100000)
     MH_TWOLEVEL (0x80)
   ]
   Reserved: 0x0
```

#### llvm-readobj --needed-libs {}

```diff
@@ -2,15 +2,14 @@
 Format: Mach-O 64-bit x86-64
 Arch: x86_64
 AddressSize: 64bit
 NeededLibraries [
   /System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
   /System/Library/Frameworks/IOKit.framework/Versions/A/IOKit
   /usr/lib/libSystem.B.dylib
-  /usr/lib/libobjc.A.dylib
   /usr/local/lib/libyapi.dylib
 ]
 
 Format: Mach-O arm64
 Arch: aarch64
 AddressSize: 64bit
 NeededLibraries [
```

#### llvm-readobj --symbols {}

```diff
@@ -1,968 +1,968 @@
 
 Format: Mach-O 64-bit x86-64
 Arch: x86_64
 AddressSize: 64bit
 Symbols [
   Symbol {
-    Name: _yTcpOpen (7085)
+    Name: _yTcpOpen (7071)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4E45
   }
   Symbol {
-    Name: _yTcpWrite (7095)
+    Name: _yTcpWrite (7081)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x52C7
   }
   Symbol {
-    Name: _yTcpRead (7106)
+    Name: _yTcpRead (7092)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5470
   }
   Symbol {
-    Name: _yHTTPOpenReqEx (7116)
+    Name: _yHTTPOpenReqEx (7102)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5C08
   }
   Symbol {
-    Name: _yHTTPMultiSelectReq (7132)
+    Name: _yHTTPMultiSelectReq (7118)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6719
   }
   Symbol {
-    Name: _yTcpCheckReqTimeout (7153)
+    Name: _yTcpCheckReqTimeout (7139)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6E4B
   }
   Symbol {
-    Name: _yHTTPCloseReqEx (7174)
+    Name: _yHTTPCloseReqEx (7160)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x708A
   }
   Symbol {
-    Name: _yWSCloseReq (7191)
+    Name: _yWSCloseReq (7177)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x712F
   }
   Symbol {
-    Name: _yWSRemoveReq (7204)
+    Name: _yWSRemoveReq (7190)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x723B
   }
   Symbol {
-    Name: _closeAllReq (7218)
+    Name: _closeAllReq (7204)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x95B4
   }
   Symbol {
-    Name: _ySSDP_thread (7231)
+    Name: _ySSDP_thread (7217)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9B9A
   }
   Symbol {
-    Name: _resolveDNSCache (7245)
+    Name: _resolveDNSCache (7231)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA017
   }
   Symbol {
-    Name: _Base64Encode (7262)
+    Name: _Base64Encode (7248)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA141
   }
   Symbol {
-    Name: _ws_appendTCPData (7276)
+    Name: _ws_appendTCPData (7262)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA255
   }
   Symbol {
-    Name: _ws_sendFrame (7294)
+    Name: _ws_sendFrame (7280)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA304
   }
   Symbol {
-    Name: _ySSDP_parseSSPDMessage (7308)
+    Name: _ySSDP_parseSSPDMessage (7294)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA44A
   }
   Symbol {
-    Name: _ypUpdateUSB (7332)
+    Name: _ypUpdateUSB (7318)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAE0D
   }
   Symbol {
-    Name: _yPktQueuePushEx (7345)
+    Name: _yPktQueuePushEx (7331)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB0D0
   }
   Symbol {
-    Name: _yPktQueuePop (7362)
+    Name: _yPktQueuePop (7348)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB224
   }
   Symbol {
-    Name: _enuUpdateDStatus (7376)
+    Name: _enuUpdateDStatus (7362)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB495
   }
   Symbol {
-    Name: _yDispatchReceive (7394)
+    Name: _yDispatchReceive (7380)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC2FC
   }
   Symbol {
-    Name: _yStreamTransmit (7412)
+    Name: _yStreamTransmit (7398)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC7E4
   }
   Symbol {
-    Name: _yStreamFlush (7429)
+    Name: _yStreamFlush (7415)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC903
   }
   Symbol {
-    Name: _devReportError (7443)
+    Name: _devReportError (7429)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC987
   }
   Symbol {
-    Name: _devStopIO (7459)
+    Name: _devStopIO (7445)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCA1A
   }
   Symbol {
-    Name: _devPauseIO (7470)
+    Name: _devPauseIO (7456)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCBB4
   }
   Symbol {
-    Name: _devCheckIO (7482)
+    Name: _devCheckIO (7468)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD1A4
   }
   Symbol {
-    Name: _devStartEnum (7494)
+    Name: _devStartEnum (7480)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDC5D
   }
   Symbol {
-    Name: _StartDevice (7508)
+    Name: _StartDevice (7494)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDD40
   }
   Symbol {
-    Name: _yStreamShutdown (7521)
+    Name: _yStreamShutdown (7507)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE3F0
   }
   Symbol {
-    Name: _yyWaitOnlyConfPkt (7538)
+    Name: _yyWaitOnlyConfPkt (7524)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE42A
   }
   Symbol {
-    Name: _yStreamReceived (7557)
+    Name: _yStreamReceived (7543)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE575
   }
   Symbol {
-    Name: _yDispatchNotice (7574)
+    Name: _yDispatchNotice (7560)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE9D2
   }
   Symbol {
-    Name: _yProgLogProgress (7591)
+    Name: _yProgLogProgress (7577)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108B0
   }
   Symbol {
-    Name: _uGetDeviceInfo (7609)
+    Name: _uGetDeviceInfo (7595)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108E9
   }
   Symbol {
-    Name: _yGetFirmware (7625)
+    Name: _yGetFirmware (7611)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10B58
   }
   Symbol {
-    Name: _isWebPath (7639)
+    Name: _isWebPath (7625)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x112F4
   }
   Symbol {
-    Name: _yapiCheckFirmware_r (7650)
+    Name: _yapiCheckFirmware_r (7636)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11338
   }
   Symbol {
-    Name: _yStartFirmwareUpdate (7671)
+    Name: _yStartFirmwareUpdate (7657)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x117C0
   }
   Symbol {
-    Name: _yapiCheckFirmwareFile (7693)
+    Name: _yapiCheckFirmwareFile (7679)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1195A
   }
   Symbol {
-    Name: _yLoadFirmwareFile (7716)
+    Name: _yLoadFirmwareFile (7702)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11A21
   }
   Symbol {
-    Name: _yFirmwareUpdate_thread (7735)
+    Name: _yFirmwareUpdate_thread (7721)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11B63
   }
   Symbol {
-    Name: _osProgLogProgressEx (7759)
+    Name: _osProgLogProgressEx (7745)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A02
   }
   Symbol {
-    Name: _sendHubFlashCmd (7780)
+    Name: _sendHubFlashCmd (7766)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A65
   }
   Symbol {
-    Name: _upload (7797)
+    Name: _upload (7783)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1315C
   }
   Symbol {
-    Name: _checkHTTPHeader (7805)
+    Name: _checkHTTPHeader (7791)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x133C6
   }
   Symbol {
-    Name: _initshaw (7822)
+    Name: _initshaw (7808)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14987
   }
   Symbol {
-    Name: _itershaw (7832)
+    Name: _itershaw (7818)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14ACF
   }
   Symbol {
-    Name: _MD5Transform (7842)
+    Name: _MD5Transform (7828)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14EE9
   }
   Symbol {
-    Name: _yBlkAlloc (7856)
+    Name: _yBlkAlloc (7842)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x158BB
   }
   Symbol {
-    Name: _yHashPut (7867)
+    Name: _yHashPut (7853)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15A23
   }
   Symbol {
-    Name: _yBlkFree (7877)
+    Name: _yBlkFree (7863)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18912
   }
   Symbol {
-    Name: _event_thread (7887)
+    Name: _event_thread (7873)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18BA0
   }
   Symbol {
-    Name: _setupHIDManager (7901)
+    Name: _setupHIDManager (7887)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18C57
   }
   Symbol {
-    Name: _stopHIDManager (7918)
+    Name: _stopHIDManager (7904)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18E62
   }
   Symbol {
-    Name: _getDevRef (7934)
+    Name: _getDevRef (7920)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1900F
   }
   Symbol {
-    Name: _get_int_property (7945)
+    Name: _get_int_property (7931)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1907F
   }
   Symbol {
-    Name: _get_txt_property (7963)
+    Name: _get_txt_property (7949)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x190D8
   }
   Symbol {
-    Name: _Handle_IOHIDDeviceIOHIDReportCallback (7981)
+    Name: _Handle_IOHIDDeviceIOHIDReportCallback (7967)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19523
   }
   Symbol {
-    Name: _yapiRequestOpenUSB (8020)
+    Name: _yapiRequestOpenUSB (8006)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19D50
   }
   Symbol {
-    Name: _logResult (8040)
+    Name: _logResult (8026)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19FB8
   }
   Symbol {
-    Name: _yapiRequestOpenWS (8051)
+    Name: _yapiRequestOpenWS (8037)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A242
   }
   Symbol {
-    Name: _yapiRequestOpenHTTP (8070)
+    Name: _yapiRequestOpenHTTP (8056)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A4EF
   }
   Symbol {
-    Name: _unregisterNetDevice (8091)
+    Name: _unregisterNetDevice (8077)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B898
   }
   Symbol {
-    Name: _unpackHTTPRequest (8112)
+    Name: _unpackHTTPRequest (8098)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C2F6
   }
   Symbol {
-    Name: _yapiRequestClose (8131)
+    Name: _yapiRequestClose (8117)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C607
   }
   Symbol {
-    Name: _yapiJsonValueParseStruct (8149)
+    Name: _yapiJsonValueParseStruct (8135)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CA1F
   }
   Symbol {
-    Name: _yapiInitAPI_internal (8175)
+    Name: _yapiInitAPI_internal (8161)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CEAD
   }
   Symbol {
-    Name: _yapiFreeAPI_internal (8197)
+    Name: _yapiFreeAPI_internal (8183)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D07F
   }
   Symbol {
-    Name: _yapiUnregisterHub_internal (8219)
+    Name: _yapiUnregisterHub_internal (8205)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DD00
   }
   Symbol {
-    Name: _yapiUpdateDeviceList_internal (8247)
+    Name: _yapiUpdateDeviceList_internal (8233)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DE55
   }
   Symbol {
-    Name: _yapiHandleEvents_internal (8278)
+    Name: _yapiHandleEvents_internal (8264)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DFF7
   }
   Symbol {
-    Name: _yapiGetFunctionInfoEx_internal (8305)
+    Name: _yapiGetFunctionInfoEx_internal (8291)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E8E2
   }
   Symbol {
-    Name: _yapiHTTPRequestAsyncEx_internal (8337)
+    Name: _yapiHTTPRequestAsyncEx_internal (8323)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA59
   }
   Symbol {
-    Name: _deleteAllCS (8370)
+    Name: _deleteAllCS (8356)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FB82
   }
   Symbol {
-    Name: _ssdpEntryUpdate (8383)
+    Name: _ssdpEntryUpdate (8369)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FBDE
   }
   Symbol {
-    Name: _unregisterNetHub (8400)
+    Name: _unregisterNetHub (8386)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FC80
   }
   Symbol {
-    Name: _isSameHub (8418)
+    Name: _isSameHub (8404)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF13
   }
   Symbol {
-    Name: _yapiFreeHub (8429)
+    Name: _yapiFreeHub (8415)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF6A
   }
   Symbol {
-    Name: _yFreeParsedURL (8442)
+    Name: _yFreeParsedURL (8428)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x200E6
   }
   Symbol {
-    Name: _yapiAllocHub (8458)
+    Name: _yapiAllocHub (8444)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2014C
   }
   Symbol {
-    Name: _pingURLOnhub (8472)
+    Name: _pingURLOnhub (8458)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20986
   }
   Symbol {
-    Name: _yParseHubURL (8486)
+    Name: _yParseHubURL (8472)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20C50
   }
   Symbol {
-    Name: _yapiRegisterHubEx (8500)
+    Name: _yapiRegisterHubEx (8486)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20F2D
   }
   Symbol {
-    Name: _yhelper_thread (8519)
+    Name: _yhelper_thread (8505)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x216D4
   }
   Symbol {
-    Name: _yNetHubEnum (8535)
+    Name: _yNetHubEnum (8521)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x21F6E
   }
   Symbol {
-    Name: _yNetHubEnumEx (8548)
+    Name: _yNetHubEnumEx (8534)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x22341
   }
   Symbol {
-    Name: _disable_jzon (8563)
+    Name: _disable_jzon (8549)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23CD8
   }
   Symbol {
-    Name: _parseNetWpEntry (8577)
+    Name: _parseNetWpEntry (8563)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23D1E
   }
   Symbol {
-    Name: _ypUpdateNet (8594)
+    Name: _ypUpdateNet (8580)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23DAA
   }
   Symbol {
-    Name: _asyncDrop (8607)
+    Name: _asyncDrop (8593)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E09
   }
   Symbol {
-    Name: _yCreateDetachedThreadEx (8618)
+    Name: _yCreateDetachedThreadEx (8604)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2498E
   }
   Symbol {
-    Name: _initTsdKey (8643)
+    Name: _initTsdKey (8629)
     Type: Section (0xE)
     Section: __text (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24C1A
   }
   Symbol {
-    Name: _dayofs (8655)
+    Name: _dayofs (8641)
     Type: Section (0xE)
     Section: __const (0x4)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x27A30
   }
   Symbol {
-    Name: _wpak (8663)
+    Name: _wpak (8649)
     Type: Section (0xE)
     Section: __data (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C000
   }
   Symbol {
-    Name: _nextCatYdx (8669)
+    Name: _nextCatYdx (8655)
     Type: Section (0xE)
     Section: __data (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1A6
   }
   Symbol {
-    Name: _nextHashEntry (8681)
+    Name: _nextHashEntry (8667)
     Type: Section (0xE)
     Section: __data (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1A8
   }
   Symbol {
-    Name: _yInitKeyOnce (8696)
+    Name: _yInitKeyOnce (8682)
     Type: Section (0xE)
     Section: __data (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1C0
   }
   Symbol {
-    Name: _yNextThreadIdx (8710)
+    Name: _yNextThreadIdx (8696)
     Type: Section (0xE)
     Section: __data (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1D0
   }
   Symbol {
-    Name: _yHashTable (8726)
+    Name: _yHashTable (8712)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2CED0
   }
   Symbol {
-    Name: _devYdxPtr (8738)
+    Name: _devYdxPtr (8724)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6CED0
   }
   Symbol {
-    Name: _funYdxPtr (8749)
+    Name: _funYdxPtr (8735)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D0D0
   }
   Symbol {
-    Name: _nextDevYdx (8760)
+    Name: _nextDevYdx (8746)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D2D0
   }
   Symbol {
-    Name: _usedDevYdx (8772)
+    Name: _usedDevYdx (8758)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D2E0
   }
   Symbol {
-    Name: _wpLockCount (8784)
+    Name: _wpLockCount (8770)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D300
   }
   Symbol {
-    Name: _wpSomethingUnregistered (8797)
+    Name: _wpSomethingUnregistered (8783)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D304
   }
   Symbol {
-    Name: _yTsdKey (8822)
+    Name: _yTsdKey (8808)
     Type: Section (0xE)
     Section: __bss (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D308
   }
@@ -972,51 +972,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ymemory.c (8903)
+    Name: ymemory.c (8889)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ymemory.o (8913)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ymemory.o (8899)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BE
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3CE8
   }
   Symbol {
-    Name: _ystrcpy_s (9062)
+    Name: _ystrcpy_s (9048)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3CE8
   }
@@ -1044,15 +1044,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3CF4
   }
   Symbol {
-    Name: _ystrncpy_s (9073)
+    Name: _ystrncpy_s (9059)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3CF4
   }
@@ -1080,15 +1080,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3DE2
   }
   Symbol {
-    Name: _ystrdup_s (9085)
+    Name: _ystrdup_s (9071)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3DE2
   }
@@ -1116,15 +1116,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E20
   }
   Symbol {
-    Name: _ystrndup_s (9096)
+    Name: _ystrndup_s (9082)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E20
   }
@@ -1152,15 +1152,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E60
   }
   Symbol {
-    Name: _ystrcat_s (9108)
+    Name: _ystrcat_s (9094)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E60
   }
@@ -1188,15 +1188,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E6C
   }
   Symbol {
-    Name: _ystrncat_s (9119)
+    Name: _ystrncat_s (9105)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3E6C
   }
@@ -1224,15 +1224,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3F13
   }
   Symbol {
-    Name: _ysprintf_s (9131)
+    Name: _ysprintf_s (9117)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3F13
   }
@@ -1260,15 +1260,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3FA9
   }
   Symbol {
-    Name: _yvsprintf_s (9143)
+    Name: _yvsprintf_s (9129)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x3FA9
   }
@@ -1296,15 +1296,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x400A
   }
   Symbol {
-    Name: _ymemfind (9156)
+    Name: _ymemfind (9142)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x400A
   }
@@ -1332,51 +1332,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ytcp.c (9166)
+    Name: ytcp.c (9152)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ytcp.o (9173)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ytcp.o (9159)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4070
   }
   Symbol {
-    Name: _yDupSet (9319)
+    Name: _yDupSet (9305)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4070
   }
@@ -1404,15 +1404,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x40D5
   }
   Symbol {
-    Name: _yNetSetErrEx (9328)
+    Name: _yNetSetErrEx (9314)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x40D5
   }
@@ -1440,15 +1440,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x413A
   }
   Symbol {
-    Name: _yInitWakeUpSocket (9342)
+    Name: _yInitWakeUpSocket (9328)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x413A
   }
@@ -1476,15 +1476,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4147
   }
   Symbol {
-    Name: _yStartWakeUpSocket (9361)
+    Name: _yStartWakeUpSocket (9347)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4147
   }
@@ -1512,15 +1512,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4305
   }
   Symbol {
-    Name: _yDringWakeUpSocket (9381)
+    Name: _yDringWakeUpSocket (9367)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4305
   }
@@ -1548,15 +1548,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x435B
   }
   Symbol {
-    Name: _yConsumeWakeUpSocket (9401)
+    Name: _yConsumeWakeUpSocket (9387)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x435B
   }
@@ -1584,15 +1584,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x43AB
   }
   Symbol {
-    Name: _yFreeWakeUpSocket (9423)
+    Name: _yFreeWakeUpSocket (9409)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x43AB
   }
@@ -1620,15 +1620,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x43E1
   }
   Symbol {
-    Name: _yResolveDNS (9442)
+    Name: _yResolveDNS (9428)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x43E1
   }
@@ -1656,15 +1656,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x445B
   }
   Symbol {
-    Name: _yTcpInit (9455)
+    Name: _yTcpInit (9441)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x445B
   }
@@ -1692,15 +1692,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4474
   }
   Symbol {
-    Name: _yTcpShutdown (9465)
+    Name: _yTcpShutdown (9451)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4474
   }
@@ -1728,15 +1728,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x44AC
   }
   Symbol {
-    Name: _decodeHex (9479)
+    Name: _decodeHex (9465)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x44AC
   }
@@ -1764,15 +1764,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x450C
   }
   Symbol {
-    Name: _yTcpDownload (9490)
+    Name: _yTcpDownload (9476)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x450C
   }
@@ -1800,15 +1800,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4E45
   }
   Symbol {
-    Name: _yTcpOpen (9504)
+    Name: _yTcpOpen (9490)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x4E45
   }
@@ -1836,15 +1836,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x52C7
   }
   Symbol {
-    Name: _yTcpWrite (9514)
+    Name: _yTcpWrite (9500)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x52C7
   }
@@ -1872,15 +1872,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5470
   }
   Symbol {
-    Name: _yTcpRead (9525)
+    Name: _yTcpRead (9511)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5470
   }
@@ -1908,15 +1908,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x54EA
   }
   Symbol {
-    Name: _yReqAlloc (9535)
+    Name: _yReqAlloc (9521)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x54EA
   }
@@ -1944,15 +1944,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5568
   }
   Symbol {
-    Name: _yReqOpen (9546)
+    Name: _yReqOpen (9532)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5568
   }
@@ -1980,15 +1980,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5C08
   }
   Symbol {
-    Name: _yHTTPOpenReqEx (9556)
+    Name: _yHTTPOpenReqEx (9542)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x5C08
   }
@@ -2016,15 +2016,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x66C7
   }
   Symbol {
-    Name: _yReqSelect (9572)
+    Name: _yReqSelect (9558)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x66C7
   }
@@ -2052,15 +2052,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6719
   }
   Symbol {
-    Name: _yHTTPMultiSelectReq (9584)
+    Name: _yHTTPMultiSelectReq (9570)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6719
   }
@@ -2088,15 +2088,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D9D
   }
   Symbol {
-    Name: _yReqMultiSelect (9605)
+    Name: _yReqMultiSelect (9591)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D9D
   }
@@ -2124,15 +2124,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6DA7
   }
   Symbol {
-    Name: _yReqIsEof (9622)
+    Name: _yReqIsEof (9608)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6DA7
   }
@@ -2160,15 +2160,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6E4B
   }
   Symbol {
-    Name: _yTcpCheckReqTimeout (9633)
+    Name: _yTcpCheckReqTimeout (9619)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6E4B
   }
@@ -2196,15 +2196,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6EF1
   }
   Symbol {
-    Name: _yReqGet (9654)
+    Name: _yReqGet (9640)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6EF1
   }
@@ -2232,15 +2232,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6F59
   }
   Symbol {
-    Name: _yReqRead (9663)
+    Name: _yReqRead (9649)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6F59
   }
@@ -2268,15 +2268,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x7025
   }
   Symbol {
-    Name: _yReqClose (9673)
+    Name: _yReqClose (9659)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x7025
   }
@@ -2304,15 +2304,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x708A
   }
   Symbol {
-    Name: _yHTTPCloseReqEx (9684)
+    Name: _yHTTPCloseReqEx (9670)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x708A
   }
@@ -2340,15 +2340,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x712F
   }
   Symbol {
-    Name: _yWSCloseReq (9701)
+    Name: _yWSCloseReq (9687)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x712F
   }
@@ -2376,15 +2376,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x723B
   }
   Symbol {
-    Name: _yWSRemoveReq (9714)
+    Name: _yWSRemoveReq (9700)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x723B
   }
@@ -2412,15 +2412,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x730B
   }
   Symbol {
-    Name: _yReqIsAsync (9728)
+    Name: _yReqIsAsync (9714)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x730B
   }
@@ -2448,15 +2448,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x7355
   }
   Symbol {
-    Name: _yReqFree (9741)
+    Name: _yReqFree (9727)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x7355
   }
@@ -2484,15 +2484,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x73ED
   }
   Symbol {
-    Name: _yReqHasPending (9751)
+    Name: _yReqHasPending (9737)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x73ED
   }
@@ -2520,15 +2520,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x74A3
   }
   Symbol {
-    Name: _ws_cleanup (9767)
+    Name: _ws_cleanup (9753)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x74A3
   }
@@ -2556,15 +2556,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x74D6
   }
   Symbol {
-    Name: _ws_thread (9779)
+    Name: _ws_thread (9765)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x74D6
   }
@@ -2592,15 +2592,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x95B4
   }
   Symbol {
-    Name: _closeAllReq (9790)
+    Name: _closeAllReq (9776)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x95B4
   }
@@ -2628,15 +2628,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9680
   }
   Symbol {
-    Name: _ySSDPDiscover (9803)
+    Name: _ySSDPDiscover (9789)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9680
   }
@@ -2664,15 +2664,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9759
   }
   Symbol {
-    Name: _ySSDPStart (9818)
+    Name: _ySSDPStart (9804)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9759
   }
@@ -2700,15 +2700,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9B9A
   }
   Symbol {
-    Name: _ySSDP_thread (9830)
+    Name: _ySSDP_thread (9816)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9B9A
   }
@@ -2736,15 +2736,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9F09
   }
   Symbol {
-    Name: _ySSDPStop (9844)
+    Name: _ySSDPStop (9830)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x9F09
   }
@@ -2772,15 +2772,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA017
   }
   Symbol {
-    Name: _resolveDNSCache (9855)
+    Name: _resolveDNSCache (9841)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA017
   }
@@ -2808,15 +2808,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA141
   }
   Symbol {
-    Name: _Base64Encode (9872)
+    Name: _Base64Encode (9858)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA141
   }
@@ -2844,15 +2844,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA255
   }
   Symbol {
-    Name: _ws_appendTCPData (9886)
+    Name: _ws_appendTCPData (9872)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA255
   }
@@ -2880,15 +2880,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA304
   }
   Symbol {
-    Name: _ws_sendFrame (9904)
+    Name: _ws_sendFrame (9890)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA304
   }
@@ -2916,15 +2916,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA44A
   }
   Symbol {
-    Name: _ySSDP_parseSSPDMessage (9918)
+    Name: _ySSDP_parseSSPDMessage (9904)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA44A
   }
@@ -2943,33 +2943,33 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA44A
   }
   Symbol {
-    Name: _dnsCache (9942)
+    Name: _dnsCache (9928)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _nbDetectedIfaces (9952)
+    Name: _nbDetectedIfaces (9938)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _detectedIfaces (9970)
+    Name: _detectedIfaces (9956)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
@@ -2979,51 +2979,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ystream.c (9986)
+    Name: ystream.c (9972)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ystream.o (9996)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ystream.o (9982)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BE
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA97C
   }
   Symbol {
-    Name: _ySetErr (10145)
+    Name: _ySetErr (10131)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA97C
   }
@@ -3051,15 +3051,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA9EB
   }
   Symbol {
-    Name: _FusionErrmsg (10154)
+    Name: _FusionErrmsg (10140)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xA9EB
   }
@@ -3087,15 +3087,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAA59
   }
   Symbol {
-    Name: _YFOPEN (10168)
+    Name: _YFOPEN (10154)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAA59
   }
@@ -3123,15 +3123,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAA7D
   }
   Symbol {
-    Name: _vdbglogf (10176)
+    Name: _vdbglogf (10162)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAA7D
   }
@@ -3159,15 +3159,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAD10
   }
   Symbol {
-    Name: _dbglogf (10186)
+    Name: _dbglogf (10172)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAD10
   }
@@ -3195,15 +3195,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xADA6
   }
   Symbol {
-    Name: _ypUpdateTCP (10195)
+    Name: _ypUpdateTCP (10181)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xADA6
   }
@@ -3231,15 +3231,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAE0D
   }
   Symbol {
-    Name: _ypUpdateUSB (10208)
+    Name: _ypUpdateUSB (10194)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAE0D
   }
@@ -3267,15 +3267,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAF18
   }
   Symbol {
-    Name: _ypUpdateYdx (10221)
+    Name: _ypUpdateYdx (10207)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAF18
   }
@@ -3303,15 +3303,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAF89
   }
   Symbol {
-    Name: _yPktQueueInit (10234)
+    Name: _yPktQueueInit (10220)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAF89
   }
@@ -3339,15 +3339,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAFD4
   }
   Symbol {
-    Name: _yPktQueueFree (10249)
+    Name: _yPktQueueFree (10235)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xAFD4
   }
@@ -3375,15 +3375,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB04E
   }
   Symbol {
-    Name: _yPktQueueSetError (10264)
+    Name: _yPktQueueSetError (10250)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB04E
   }
@@ -3411,15 +3411,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB0B1
   }
   Symbol {
-    Name: _yPktQueuePushD2H (10283)
+    Name: _yPktQueuePushD2H (10269)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB0B1
   }
@@ -3447,15 +3447,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB0D0
   }
   Symbol {
-    Name: _yPktQueuePushEx (10301)
+    Name: _yPktQueuePushEx (10287)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB0D0
   }
@@ -3483,15 +3483,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB1A6
   }
   Symbol {
-    Name: _yPktQueueWaitAndPopD2H (10318)
+    Name: _yPktQueueWaitAndPopD2H (10304)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB1A6
   }
@@ -3519,15 +3519,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB224
   }
   Symbol {
-    Name: _yPktQueuePop (10342)
+    Name: _yPktQueuePop (10328)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB224
   }
@@ -3555,15 +3555,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB2D3
   }
   Symbol {
-    Name: _yPktQueuePushH2D (10356)
+    Name: _yPktQueuePushH2D (10342)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB2D3
   }
@@ -3591,15 +3591,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB2E4
   }
   Symbol {
-    Name: _yPktQueuePeekH2D (10374)
+    Name: _yPktQueuePeekH2D (10360)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB2E4
   }
@@ -3627,15 +3627,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB332
   }
   Symbol {
-    Name: _yPktQueuePopH2D (10392)
+    Name: _yPktQueuePopH2D (10378)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB332
   }
@@ -3663,15 +3663,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB345
   }
   Symbol {
-    Name: _yyySendPacket (10409)
+    Name: _yyySendPacket (10395)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB345
   }
@@ -3699,15 +3699,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB437
   }
   Symbol {
-    Name: _yUSBReleaseAllDevices (10424)
+    Name: _yUSBReleaseAllDevices (10410)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB437
   }
@@ -3735,15 +3735,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB495
   }
   Symbol {
-    Name: _enuUpdateDStatus (10447)
+    Name: _enuUpdateDStatus (10433)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB495
   }
@@ -3771,15 +3771,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB72C
   }
   Symbol {
-    Name: _yUSBUpdateDeviceList (10465)
+    Name: _yUSBUpdateDeviceList (10451)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB72C
   }
@@ -3807,15 +3807,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB98F
   }
   Symbol {
-    Name: _findDev (10487)
+    Name: _findDev (10473)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xB98F
   }
@@ -3843,15 +3843,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA2F
   }
   Symbol {
-    Name: _findDevHdlFromStr (10496)
+    Name: _findDevHdlFromStr (10482)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA2F
   }
@@ -3879,15 +3879,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA4E
   }
   Symbol {
-    Name: _findDevFromIOHdl (10515)
+    Name: _findDevFromIOHdl (10501)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA4E
   }
@@ -3915,15 +3915,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA86
   }
   Symbol {
-    Name: _devHdlInfo (10533)
+    Name: _devHdlInfo (10519)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBA86
   }
@@ -3951,15 +3951,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB2C
   }
   Symbol {
-    Name: _dumpYPerfEntry (10545)
+    Name: _dumpYPerfEntry (10531)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB2C
   }
@@ -3987,15 +3987,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB77
   }
   Symbol {
-    Name: _yUsbInit (10561)
+    Name: _yUsbInit (10547)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB77
   }
@@ -4023,15 +4023,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB81
   }
   Symbol {
-    Name: _yUsbFree (10571)
+    Name: _yUsbFree (10557)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBB81
   }
@@ -4059,15 +4059,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBC6F
   }
   Symbol {
-    Name: _yUsbIdle (10581)
+    Name: _yUsbIdle (10567)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xBC6F
   }
@@ -4095,15 +4095,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC2FC
   }
   Symbol {
-    Name: _yDispatchReceive (10591)
+    Name: _yDispatchReceive (10577)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC2FC
   }
@@ -4131,15 +4131,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC7E4
   }
   Symbol {
-    Name: _yStreamTransmit (10609)
+    Name: _yStreamTransmit (10595)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC7E4
   }
@@ -4167,15 +4167,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC903
   }
   Symbol {
-    Name: _yStreamFlush (10626)
+    Name: _yStreamFlush (10612)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC903
   }
@@ -4203,15 +4203,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC987
   }
   Symbol {
-    Name: _devReportError (10640)
+    Name: _devReportError (10626)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xC987
   }
@@ -4239,15 +4239,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCA1A
   }
   Symbol {
-    Name: _devStopIO (10656)
+    Name: _devStopIO (10642)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCA1A
   }
@@ -4275,15 +4275,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCBB4
   }
   Symbol {
-    Name: _devPauseIO (10667)
+    Name: _devPauseIO (10653)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCBB4
   }
@@ -4311,15 +4311,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCD70
   }
   Symbol {
-    Name: _yUsbTrafficPending (10679)
+    Name: _yUsbTrafficPending (10665)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCD70
   }
@@ -4347,15 +4347,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCDB2
   }
   Symbol {
-    Name: _yUsbOpenDevDescr (10699)
+    Name: _yUsbOpenDevDescr (10685)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCDB2
   }
@@ -4383,15 +4383,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCE14
   }
   Symbol {
-    Name: _yUsbOpen (10717)
+    Name: _yUsbOpen (10703)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xCE14
   }
@@ -4419,15 +4419,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD0D8
   }
   Symbol {
-    Name: _yUsbSetIOAsync (10727)
+    Name: _yUsbSetIOAsync (10713)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD0D8
   }
@@ -4455,15 +4455,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD1A4
   }
   Symbol {
-    Name: _devCheckIO (10743)
+    Name: _devCheckIO (10729)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD1A4
   }
@@ -4491,15 +4491,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD3DC
   }
   Symbol {
-    Name: _yUsbWrite (10755)
+    Name: _yUsbWrite (10741)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD3DC
   }
@@ -4527,15 +4527,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD5D3
   }
   Symbol {
-    Name: _yUsbReadNonBlock (10766)
+    Name: _yUsbReadNonBlock (10752)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD5D3
   }
@@ -4563,15 +4563,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD720
   }
   Symbol {
-    Name: _yUsbReadBlock (10784)
+    Name: _yUsbReadBlock (10770)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD720
   }
@@ -4599,15 +4599,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD88C
   }
   Symbol {
-    Name: _yUsbEOF (10799)
+    Name: _yUsbEOF (10785)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD88C
   }
@@ -4635,15 +4635,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD9CB
   }
   Symbol {
-    Name: _yUsbClose (10808)
+    Name: _yUsbClose (10794)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xD9CB
   }
@@ -4671,15 +4671,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDC5D
   }
   Symbol {
-    Name: _devStartEnum (10819)
+    Name: _devStartEnum (10805)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDC5D
   }
@@ -4707,15 +4707,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDD40
   }
   Symbol {
-    Name: _StartDevice (10833)
+    Name: _StartDevice (10819)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xDD40
   }
@@ -4743,15 +4743,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE3F0
   }
   Symbol {
-    Name: _yStreamShutdown (10846)
+    Name: _yStreamShutdown (10832)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE3F0
   }
@@ -4779,15 +4779,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE42A
   }
   Symbol {
-    Name: _yyWaitOnlyConfPkt (10863)
+    Name: _yyWaitOnlyConfPkt (10849)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE42A
   }
@@ -4815,15 +4815,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE575
   }
   Symbol {
-    Name: _yStreamReceived (10882)
+    Name: _yStreamReceived (10868)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE575
   }
@@ -4851,15 +4851,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE9D2
   }
   Symbol {
-    Name: _yDispatchNotice (10899)
+    Name: _yDispatchNotice (10885)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE9D2
   }
@@ -4878,33 +4878,33 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xE9D2
   }
   Symbol {
-    Name: _dayofs (10916)
+    Name: _dayofs (10902)
     Type: SymDebugTable (0x26)
     Section:  (0x4)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x27A30
   }
   Symbol {
-    Name: _yContext (10924)
+    Name: _yContext (10910)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _ytracefile (10934)
+    Name: _ytracefile (10920)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
@@ -4914,51 +4914,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: yprog.c (10946)
+    Name: yprog.c (10932)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yprog.o (10954)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yprog.o (10940)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BE
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xEF58
   }
   Symbol {
-    Name: _yProgInit (11101)
+    Name: _yProgInit (11087)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xEF58
   }
@@ -4986,15 +4986,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xEFA9
   }
   Symbol {
-    Name: _yProgFree (11112)
+    Name: _yProgFree (11098)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xEFA9
   }
@@ -5022,15 +5022,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF06F
   }
   Symbol {
-    Name: _prog_GetCPUName (11123)
+    Name: _prog_GetCPUName (11109)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF06F
   }
@@ -5058,15 +5058,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF0EA
   }
   Symbol {
-    Name: _IsValidBynHead (11140)
+    Name: _IsValidBynHead (11126)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF0EA
   }
@@ -5094,15 +5094,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF3F7
   }
   Symbol {
-    Name: _ValidateBynCompat (11156)
+    Name: _ValidateBynCompat (11142)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF3F7
   }
@@ -5130,15 +5130,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF4E9
   }
   Symbol {
-    Name: _IsValidBynFile (11175)
+    Name: _IsValidBynFile (11161)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF4E9
   }
@@ -5166,15 +5166,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5B7
   }
   Symbol {
-    Name: _ypIsSendBootloaderBusy (11191)
+    Name: _ypIsSendBootloaderBusy (11177)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5B7
   }
@@ -5202,15 +5202,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5BF
   }
   Symbol {
-    Name: _ypSendBootloaderCmd (11215)
+    Name: _ypSendBootloaderCmd (11201)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5BF
   }
@@ -5238,15 +5238,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5C9
   }
   Symbol {
-    Name: _ypGetBootloaderReply (11236)
+    Name: _ypGetBootloaderReply (11222)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF5C9
   }
@@ -5274,15 +5274,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF639
   }
   Symbol {
-    Name: _BlockingRead (11258)
+    Name: _BlockingRead (11244)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF639
   }
@@ -5310,15 +5310,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF6B0
   }
   Symbol {
-    Name: _SendDataPacket (11272)
+    Name: _SendDataPacket (11258)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF6B0
   }
@@ -5346,15 +5346,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF757
   }
   Symbol {
-    Name: _yUSBGetBooloader (11288)
+    Name: _yUSBGetBooloader (11274)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF757
   }
@@ -5382,15 +5382,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF834
   }
   Symbol {
-    Name: _uFlashDevice (11306)
+    Name: _uFlashDevice (11292)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0xF834
   }
@@ -5418,15 +5418,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108B0
   }
   Symbol {
-    Name: _yProgLogProgress (11320)
+    Name: _yProgLogProgress (11306)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108B0
   }
@@ -5454,15 +5454,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108E9
   }
   Symbol {
-    Name: _uGetDeviceInfo (11338)
+    Name: _uGetDeviceInfo (11324)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x108E9
   }
@@ -5490,15 +5490,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10B58
   }
   Symbol {
-    Name: _yGetFirmware (11354)
+    Name: _yGetFirmware (11340)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10B58
   }
@@ -5526,15 +5526,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10BE9
   }
   Symbol {
-    Name: _yNetHubGetBootloaders (11368)
+    Name: _yNetHubGetBootloaders (11354)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10BE9
   }
@@ -5562,15 +5562,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10EF5
   }
   Symbol {
-    Name: _yapiCheckFirmware_internal (11391)
+    Name: _yapiCheckFirmware_internal (11377)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x10EF5
   }
@@ -5598,15 +5598,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x112F4
   }
   Symbol {
-    Name: _isWebPath (11419)
+    Name: _isWebPath (11405)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x112F4
   }
@@ -5634,15 +5634,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11338
   }
   Symbol {
-    Name: _yapiCheckFirmware_r (11430)
+    Name: _yapiCheckFirmware_r (11416)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11338
   }
@@ -5670,15 +5670,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11696
   }
   Symbol {
-    Name: _yapiUpdateFirmware_internal (11451)
+    Name: _yapiUpdateFirmware_internal (11437)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11696
   }
@@ -5706,15 +5706,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x117C0
   }
   Symbol {
-    Name: _yStartFirmwareUpdate (11480)
+    Name: _yStartFirmwareUpdate (11466)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x117C0
   }
@@ -5742,15 +5742,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1195A
   }
   Symbol {
-    Name: _yapiCheckFirmwareFile (11502)
+    Name: _yapiCheckFirmwareFile (11488)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1195A
   }
@@ -5778,15 +5778,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11A21
   }
   Symbol {
-    Name: _yLoadFirmwareFile (11525)
+    Name: _yLoadFirmwareFile (11511)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11A21
   }
@@ -5814,15 +5814,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11B63
   }
   Symbol {
-    Name: _yFirmwareUpdate_thread (11544)
+    Name: _yFirmwareUpdate_thread (11530)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x11B63
   }
@@ -5850,15 +5850,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A02
   }
   Symbol {
-    Name: _osProgLogProgressEx (11568)
+    Name: _osProgLogProgressEx (11554)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A02
   }
@@ -5886,15 +5886,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A65
   }
   Symbol {
-    Name: _sendHubFlashCmd (11589)
+    Name: _sendHubFlashCmd (11575)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x12A65
   }
@@ -5922,15 +5922,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1315C
   }
   Symbol {
-    Name: _upload (11606)
+    Name: _upload (11592)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1315C
   }
@@ -5958,15 +5958,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x133C6
   }
   Symbol {
-    Name: _checkHTTPHeader (11614)
+    Name: _checkHTTPHeader (11600)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x133C6
   }
@@ -5985,33 +5985,33 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x133C6
   }
   Symbol {
-    Name: _fctx (11631)
+    Name: _fctx (11617)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _firm_dev (11637)
+    Name: _firm_dev (11623)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _firm_pkt (11647)
+    Name: _firm_pkt (11633)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
@@ -6021,51 +6021,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: yjson.c (11657)
+    Name: yjson.c (11643)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yjson.o (11665)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yjson.o (11651)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1347C
   }
   Symbol {
-    Name: _yJsonParse (11812)
+    Name: _yJsonParse (11798)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1347C
   }
@@ -6093,15 +6093,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13D44
   }
   Symbol {
-    Name: _yJsonSkip (11824)
+    Name: _yJsonSkip (11810)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13D44
   }
@@ -6129,51 +6129,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ykey.c (11835)
+    Name: ykey.c (11821)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ykey.o (11842)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ykey.o (11828)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13D50
   }
   Symbol {
-    Name: _bin2str (11988)
+    Name: _bin2str (11974)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13D50
   }
@@ -6201,15 +6201,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13DB3
   }
   Symbol {
-    Name: _ComputeAuthHA1 (11997)
+    Name: _ComputeAuthHA1 (11983)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13DB3
   }
@@ -6237,15 +6237,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13E68
   }
   Symbol {
-    Name: _MD5Initialize (12013)
+    Name: _MD5Initialize (11999)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13E68
   }
@@ -6273,15 +6273,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13E80
   }
   Symbol {
-    Name: _MD5AddData (12028)
+    Name: _MD5AddData (12014)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13E80
   }
@@ -6309,15 +6309,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13F5E
   }
   Symbol {
-    Name: _MD5Calculate (12040)
+    Name: _MD5Calculate (12026)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x13F5E
   }
@@ -6345,15 +6345,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1400C
   }
   Symbol {
-    Name: _ComputeAuthHA2 (12054)
+    Name: _ComputeAuthHA2 (12040)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1400C
   }
@@ -6381,15 +6381,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14093
   }
   Symbol {
-    Name: _ComputeAuthResponse (12070)
+    Name: _ComputeAuthResponse (12056)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14093
   }
@@ -6417,15 +6417,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x142C4
   }
   Symbol {
-    Name: _CheckWSAuth (12091)
+    Name: _CheckWSAuth (12077)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x142C4
   }
@@ -6453,15 +6453,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1442D
   }
   Symbol {
-    Name: _ySHA1 (12104)
+    Name: _ySHA1 (12090)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1442D
   }
@@ -6489,15 +6489,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x144D3
   }
   Symbol {
-    Name: _yParseWWWAuthenticate (12111)
+    Name: _yParseWWWAuthenticate (12097)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x144D3
   }
@@ -6525,15 +6525,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1477D
   }
   Symbol {
-    Name: _yDigestAuthorization (12134)
+    Name: _yDigestAuthorization (12120)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1477D
   }
@@ -6561,15 +6561,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14987
   }
   Symbol {
-    Name: _initshaw (12156)
+    Name: _initshaw (12142)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14987
   }
@@ -6597,15 +6597,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14ACF
   }
   Symbol {
-    Name: _itershaw (12166)
+    Name: _itershaw (12152)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14ACF
   }
@@ -6633,15 +6633,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14C7C
   }
   Symbol {
-    Name: _yInitPsk (12176)
+    Name: _yInitPsk (12162)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14C7C
   }
@@ -6669,15 +6669,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14D30
   }
   Symbol {
-    Name: _yIterPsk (12186)
+    Name: _yIterPsk (12172)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14D30
   }
@@ -6705,15 +6705,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14EE9
   }
   Symbol {
-    Name: _MD5Transform (12196)
+    Name: _MD5Transform (12182)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14EE9
   }
@@ -6732,24 +6732,24 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x14EE9
   }
   Symbol {
-    Name: _sha1_init (12210)
+    Name: _sha1_init (12196)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _wpak (12221)
+    Name: _wpak (12207)
     Type: SymDebugTable (0x26)
     Section:  (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C000
   }
@@ -6759,51 +6759,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: yhash.c (12227)
+    Name: yhash.c (12213)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yhash.o (12235)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yhash.o (12221)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15620
   }
   Symbol {
-    Name: _yBlkListLength (12382)
+    Name: _yBlkListLength (12368)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15620
   }
@@ -6831,15 +6831,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15657
   }
   Symbol {
-    Name: _yBlkListSeek (12398)
+    Name: _yBlkListSeek (12384)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15657
   }
@@ -6867,15 +6867,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1569C
   }
   Symbol {
-    Name: _yHashInit (12412)
+    Name: _yHashInit (12398)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1569C
   }
@@ -6903,15 +6903,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15887
   }
   Symbol {
-    Name: _yHashPutStr (12423)
+    Name: _yHashPutStr (12409)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15887
   }
@@ -6939,15 +6939,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x158BB
   }
   Symbol {
-    Name: _yBlkAlloc (12436)
+    Name: _yBlkAlloc (12422)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x158BB
   }
@@ -6975,15 +6975,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x159D6
   }
   Symbol {
-    Name: _yHashFree (12447)
+    Name: _yHashFree (12433)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x159D6
   }
@@ -7011,15 +7011,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15A0B
   }
   Symbol {
-    Name: _yHashPutBuf (12458)
+    Name: _yHashPutBuf (12444)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15A0B
   }
@@ -7047,15 +7047,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15A23
   }
   Symbol {
-    Name: _yHashPut (12471)
+    Name: _yHashPut (12457)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15A23
   }
@@ -7083,15 +7083,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15CF1
   }
   Symbol {
-    Name: _yHashTestBuf (12481)
+    Name: _yHashTestBuf (12467)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15CF1
   }
@@ -7119,15 +7119,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15D0C
   }
   Symbol {
-    Name: _yHashTestStr (12495)
+    Name: _yHashTestStr (12481)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15D0C
   }
@@ -7155,15 +7155,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15D43
   }
   Symbol {
-    Name: _yHashGetBuf (12509)
+    Name: _yHashGetBuf (12495)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15D43
   }
@@ -7191,15 +7191,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15E2C
   }
   Symbol {
-    Name: _yHashGetStr (12522)
+    Name: _yHashGetStr (12508)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15E2C
   }
@@ -7227,15 +7227,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15E4A
   }
   Symbol {
-    Name: _yHashGetStrLen (12535)
+    Name: _yHashGetStrLen (12521)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15E4A
   }
@@ -7263,15 +7263,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15EF9
   }
   Symbol {
-    Name: _yHashGetStrPtr (12551)
+    Name: _yHashGetStrPtr (12537)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15EF9
   }
@@ -7299,15 +7299,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15FA0
   }
   Symbol {
-    Name: _wpPreventUnregisterEx (12567)
+    Name: _wpPreventUnregisterEx (12553)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15FA0
   }
@@ -7335,15 +7335,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15FFB
   }
   Symbol {
-    Name: _wpAllowUnregisterEx (12590)
+    Name: _wpAllowUnregisterEx (12576)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x15FFB
   }
@@ -7371,15 +7371,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x163A9
   }
   Symbol {
-    Name: _wpRegister (12611)
+    Name: _wpRegister (12597)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x163A9
   }
@@ -7407,15 +7407,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x166F1
   }
   Symbol {
-    Name: _wpGetAttribute (12623)
+    Name: _wpGetAttribute (12609)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x166F1
   }
@@ -7443,15 +7443,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x167C0
   }
   Symbol {
-    Name: _wpGetSerial (12639)
+    Name: _wpGetSerial (12625)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x167C0
   }
@@ -7479,15 +7479,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16820
   }
   Symbol {
-    Name: _wpGetLogicalName (12652)
+    Name: _wpGetLogicalName (12638)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16820
   }
@@ -7515,15 +7515,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16880
   }
   Symbol {
-    Name: _wpMarkForUnregister (12670)
+    Name: _wpMarkForUnregister (12656)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16880
   }
@@ -7551,15 +7551,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1690A
   }
   Symbol {
-    Name: _wpEntryCount (12691)
+    Name: _wpEntryCount (12677)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1690A
   }
@@ -7587,15 +7587,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16949
   }
   Symbol {
-    Name: _wpGetDevYdx (12705)
+    Name: _wpGetDevYdx (12691)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16949
   }
@@ -7623,15 +7623,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16A00
   }
   Symbol {
-    Name: _wpSearchEx (12718)
+    Name: _wpSearchEx (12704)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16A00
   }
@@ -7659,15 +7659,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16AFA
   }
   Symbol {
-    Name: _wpSearch (12730)
+    Name: _wpSearch (12716)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16AFA
   }
@@ -7695,15 +7695,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16B4B
   }
   Symbol {
-    Name: _wpSearchByNameHash (12740)
+    Name: _wpSearchByNameHash (12726)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16B4B
   }
@@ -7731,15 +7731,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16C16
   }
   Symbol {
-    Name: _wpGetDeviceInfo (12760)
+    Name: _wpGetDeviceInfo (12746)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16C16
   }
@@ -7767,15 +7767,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16D81
   }
   Symbol {
-    Name: _ypRegister (12777)
+    Name: _ypRegister (12763)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x16D81
   }
@@ -7803,15 +7803,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17287
   }
   Symbol {
-    Name: _ypRegisterByYdx (12789)
+    Name: _ypRegisterByYdx (12775)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17287
   }
@@ -7839,15 +7839,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17461
   }
   Symbol {
-    Name: _ypGetAttributesByYdx (12806)
+    Name: _ypGetAttributesByYdx (12792)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17461
   }
@@ -7875,15 +7875,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17668
   }
   Symbol {
-    Name: _ypGetCategory (12828)
+    Name: _ypGetCategory (12814)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17668
   }
@@ -7911,15 +7911,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x176E4
   }
   Symbol {
-    Name: _ypGetAttributes (12843)
+    Name: _ypGetAttributes (12829)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x176E4
   }
@@ -7947,15 +7947,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x177F4
   }
   Symbol {
-    Name: _ypGetType (12860)
+    Name: _ypGetType (12846)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x177F4
   }
@@ -7983,15 +7983,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1784C
   }
   Symbol {
-    Name: _ypSearch (12871)
+    Name: _ypSearch (12857)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1784C
   }
@@ -8019,15 +8019,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17FF7
   }
   Symbol {
-    Name: _ypGetFunctions (12881)
+    Name: _ypGetFunctions (12867)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x17FF7
   }
@@ -8055,15 +8055,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x182B2
   }
   Symbol {
-    Name: _ypGetFunctionInfo (12897)
+    Name: _ypGetFunctionInfo (12883)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x182B2
   }
@@ -8091,15 +8091,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18532
   }
   Symbol {
-    Name: _ypGetFunctionsEx (12916)
+    Name: _ypGetFunctionsEx (12902)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18532
   }
@@ -8127,15 +8127,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1876B
   }
   Symbol {
-    Name: _ypFindBootloaders (12934)
+    Name: _ypFindBootloaders (12920)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1876B
   }
@@ -8163,15 +8163,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18880
   }
   Symbol {
-    Name: _decodeNetFuncValV2 (12953)
+    Name: _decodeNetFuncValV2 (12939)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18880
   }
@@ -8199,15 +8199,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18912
   }
   Symbol {
-    Name: _yBlkFree (12973)
+    Name: _yBlkFree (12959)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18912
   }
@@ -8226,168 +8226,168 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18912
   }
   Symbol {
-    Name: _SerialRef (12983)
+    Name: _SerialRef (12969)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _nextCatYdx (12994)
+    Name: _nextCatYdx (12980)
     Type: SymDebugTable (0x26)
     Section:  (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1A6
   }
   Symbol {
-    Name: _nextHashEntry (13006)
+    Name: _nextHashEntry (12992)
     Type: SymDebugTable (0x26)
     Section:  (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1A8
   }
   Symbol {
-    Name: _SerialNumberStr (13021)
+    Name: _SerialNumberStr (13007)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yWpListHead (13038)
+    Name: _yWpListHead (13024)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yYpListHead (13051)
+    Name: _yYpListHead (13037)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _freeBlks (13064)
+    Name: _freeBlks (13050)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yHashMutex (13074)
+    Name: _yHashMutex (13060)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yFreeMutex (13086)
+    Name: _yFreeMutex (13072)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yWpMutex (13098)
+    Name: _yWpMutex (13084)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yYpMutex (13108)
+    Name: _yYpMutex (13094)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _yHashTable (13118)
+    Name: _yHashTable (13104)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2CED0
   }
   Symbol {
-    Name: _devYdxPtr (13130)
+    Name: _devYdxPtr (13116)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6CED0
   }
   Symbol {
-    Name: _funYdxPtr (13141)
+    Name: _funYdxPtr (13127)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D0D0
   }
   Symbol {
-    Name: _nextDevYdx (13152)
+    Name: _nextDevYdx (13138)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D2D0
   }
   Symbol {
-    Name: _usedDevYdx (13164)
+    Name: _usedDevYdx (13150)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D2E0
   }
   Symbol {
-    Name: _wpLockCount (13176)
+    Name: _wpLockCount (13162)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D300
   }
   Symbol {
-    Name: _wpSomethingUnregistered (13189)
+    Name: _wpSomethingUnregistered (13175)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D304
   }
@@ -8397,51 +8397,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ypkt_osx.c (13214)
+    Name: ypkt_osx.c (13200)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ypkt_osx.o (13225)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ypkt_osx.o (13211)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BE
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1896A
   }
   Symbol {
-    Name: _yyyUSB_init (13375)
+    Name: _yyyUSB_init (13361)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1896A
   }
@@ -8469,15 +8469,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18BA0
   }
   Symbol {
-    Name: _event_thread (13388)
+    Name: _event_thread (13374)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18BA0
   }
@@ -8505,15 +8505,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18C57
   }
   Symbol {
-    Name: _setupHIDManager (13402)
+    Name: _setupHIDManager (13388)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18C57
   }
@@ -8541,15 +8541,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18D77
   }
   Symbol {
-    Name: _yyyUSB_stop (13419)
+    Name: _yyyUSB_stop (13405)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18D77
   }
@@ -8577,15 +8577,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18E62
   }
   Symbol {
-    Name: _stopHIDManager (13432)
+    Name: _stopHIDManager (13418)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18E62
   }
@@ -8613,15 +8613,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18EA2
   }
   Symbol {
-    Name: _yyyUSBGetInterfaces (13448)
+    Name: _yyyUSBGetInterfaces (13434)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x18EA2
   }
@@ -8649,15 +8649,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1900F
   }
   Symbol {
-    Name: _getDevRef (13469)
+    Name: _getDevRef (13455)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1900F
   }
@@ -8685,15 +8685,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1907F
   }
   Symbol {
-    Name: _get_int_property (13480)
+    Name: _get_int_property (13466)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1907F
   }
@@ -8721,15 +8721,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x190D8
   }
   Symbol {
-    Name: _get_txt_property (13498)
+    Name: _get_txt_property (13484)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x190D8
   }
@@ -8757,15 +8757,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x191F6
   }
   Symbol {
-    Name: _yyyOShdlCompare (13516)
+    Name: _yyyOShdlCompare (13502)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x191F6
   }
@@ -8793,15 +8793,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19209
   }
   Symbol {
-    Name: _yyySetup (13533)
+    Name: _yyySetup (13519)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19209
   }
@@ -8829,15 +8829,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19523
   }
   Symbol {
-    Name: _Handle_IOHIDDeviceIOHIDReportCallback (13543)
+    Name: _Handle_IOHIDDeviceIOHIDReportCallback (13529)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19523
   }
@@ -8865,15 +8865,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19565
   }
   Symbol {
-    Name: _yyySignalOutPkt (13582)
+    Name: _yyySignalOutPkt (13568)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19565
   }
@@ -8901,15 +8901,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19642
   }
   Symbol {
-    Name: _yyyPacketShutdown (13599)
+    Name: _yyyPacketShutdown (13585)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19642
   }
@@ -8937,51 +8937,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: yapi.c (13618)
+    Name: yapi.c (13604)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yapi.o (13625)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yapi.o (13611)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383589
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19734
   }
   Symbol {
-    Name: _yapiAddUdevRulesForYocto (13771)
+    Name: _yapiAddUdevRulesForYocto (13757)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19734
   }
@@ -9009,15 +9009,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19757
   }
   Symbol {
-    Name: _yFunctionUpdate (13797)
+    Name: _yFunctionUpdate (13783)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19757
   }
@@ -9045,15 +9045,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x197B7
   }
   Symbol {
-    Name: _yFunctionTimedUpdate (13814)
+    Name: _yFunctionTimedUpdate (13800)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x197B7
   }
@@ -9081,15 +9081,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19886
   }
   Symbol {
-    Name: _initDevYdxInfos (13836)
+    Name: _initDevYdxInfos (13822)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19886
   }
@@ -9117,15 +9117,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19927
   }
   Symbol {
-    Name: _freeDevYdxInfos (13853)
+    Name: _freeDevYdxInfos (13839)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19927
   }
@@ -9153,15 +9153,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x199A5
   }
   Symbol {
-    Name: _yapiPullDeviceLogEx (13870)
+    Name: _yapiPullDeviceLogEx (13856)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x199A5
   }
@@ -9189,15 +9189,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19C5C
   }
   Symbol {
-    Name: _yapiGetDevicePath (13891)
+    Name: _yapiGetDevicePath (13877)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19C5C
   }
@@ -9225,15 +9225,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19CF0
   }
   Symbol {
-    Name: _ywpGetDeviceHub (13910)
+    Name: _ywpGetDeviceHub (13896)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19CF0
   }
@@ -9261,15 +9261,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19D50
   }
   Symbol {
-    Name: _yapiRequestOpenUSB (13927)
+    Name: _yapiRequestOpenUSB (13913)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19D50
   }
@@ -9297,15 +9297,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19FB8
   }
   Symbol {
-    Name: _logResult (13947)
+    Name: _logResult (13933)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x19FB8
   }
@@ -9333,15 +9333,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A242
   }
   Symbol {
-    Name: _yapiRequestOpenWS (13958)
+    Name: _yapiRequestOpenWS (13944)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A242
   }
@@ -9369,15 +9369,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A4EF
   }
   Symbol {
-    Name: _yapiRequestOpenHTTP (13977)
+    Name: _yapiRequestOpenHTTP (13963)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A4EF
   }
@@ -9405,15 +9405,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A71E
   }
   Symbol {
-    Name: _yapiPullDeviceLog (13998)
+    Name: _yapiPullDeviceLog (13984)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A71E
   }
@@ -9441,15 +9441,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A742
   }
   Symbol {
-    Name: _checkForSameHubAccess (14017)
+    Name: _checkForSameHubAccess (14003)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A742
   }
@@ -9477,15 +9477,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A887
   }
   Symbol {
-    Name: _ywpSafeUnregister (14040)
+    Name: _ywpSafeUnregister (14026)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A887
   }
@@ -9513,15 +9513,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A97D
   }
   Symbol {
-    Name: _ywpSafeRegister (14059)
+    Name: _ywpSafeRegister (14045)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1A97D
   }
@@ -9549,15 +9549,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1AB25
   }
   Symbol {
-    Name: _ywpSafeUpdate (14076)
+    Name: _ywpSafeUpdate (14062)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1AB25
   }
@@ -9585,15 +9585,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1AC96
   }
   Symbol {
-    Name: _ywpGetDeviceUrl (14091)
+    Name: _ywpGetDeviceUrl (14077)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1AC96
   }
@@ -9621,15 +9621,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1ADF3
   }
   Symbol {
-    Name: _handleNetNotification (14108)
+    Name: _handleNetNotification (14094)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1ADF3
   }
@@ -9657,15 +9657,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B898
   }
   Symbol {
-    Name: _unregisterNetDevice (14131)
+    Name: _unregisterNetDevice (14117)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B898
   }
@@ -9693,15 +9693,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B8FB
   }
   Symbol {
-    Name: _request_pending_logs (14152)
+    Name: _request_pending_logs (14138)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B8FB
   }
@@ -9729,15 +9729,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B92E
   }
   Symbol {
-    Name: _yapiGetDLLPath (14174)
+    Name: _yapiGetDLLPath (14160)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B92E
   }
@@ -9765,15 +9765,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B94F
   }
   Symbol {
-    Name: _WakeUpAllSleep (14190)
+    Name: _WakeUpAllSleep (14176)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B94F
   }
@@ -9801,15 +9801,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B982
   }
   Symbol {
-    Name: _yapiGetTickCount (14206)
+    Name: _yapiGetTickCount (14192)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B982
   }
@@ -9837,15 +9837,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B9C4
   }
   Symbol {
-    Name: _yapiGetCNonce (14224)
+    Name: _yapiGetCNonce (14210)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1B9C4
   }
@@ -9873,15 +9873,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1BA5C
   }
   Symbol {
-    Name: _yapiRequestOpen (14239)
+    Name: _yapiRequestOpen (14225)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1BA5C
   }
@@ -9909,15 +9909,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1BDAA
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncStartEx_internal (14256)
+    Name: _yapiHTTPRequestSyncStartEx_internal (14242)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1BDAA
   }
@@ -9945,15 +9945,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C2F6
   }
   Symbol {
-    Name: _unpackHTTPRequest (14293)
+    Name: _unpackHTTPRequest (14279)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C2F6
   }
@@ -9981,15 +9981,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C607
   }
   Symbol {
-    Name: _yapiRequestClose (14312)
+    Name: _yapiRequestClose (14298)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C607
   }
@@ -10017,15 +10017,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C663
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncDone_internal (14330)
+    Name: _yapiHTTPRequestSyncDone_internal (14316)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C663
   }
@@ -10053,15 +10053,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C74B
   }
   Symbol {
-    Name: _yapiGetBootloadersDevs (14364)
+    Name: _yapiGetBootloadersDevs (14350)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C74B
   }
@@ -10089,15 +10089,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C895
   }
   Symbol {
-    Name: _yapiJsonGetPath_internal (14388)
+    Name: _yapiJsonGetPath_internal (14374)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1C895
   }
@@ -10125,15 +10125,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CA1F
   }
   Symbol {
-    Name: _yapiJsonValueParseStruct (14414)
+    Name: _yapiJsonValueParseStruct (14400)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CA1F
   }
@@ -10161,15 +10161,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CDB0
   }
   Symbol {
-    Name: _yapiRegisterRawNotificationCb (14440)
+    Name: _yapiRegisterRawNotificationCb (14426)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CDB0
   }
@@ -10197,15 +10197,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CE01
   }
   Symbol {
-    Name: _yapiRegisterRawReportCb (14471)
+    Name: _yapiRegisterRawReportCb (14457)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CE01
   }
@@ -10233,15 +10233,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CE52
   }
   Symbol {
-    Name: _yapiRegisterRawReportV2Cb (14496)
+    Name: _yapiRegisterRawReportV2Cb (14482)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CE52
   }
@@ -10269,15 +10269,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CEA3
   }
   Symbol {
-    Name: _yapiInitAPI (14523)
+    Name: _yapiInitAPI (14509)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CEA3
   }
@@ -10305,15 +10305,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CEAD
   }
   Symbol {
-    Name: _yapiInitAPI_internal (14536)
+    Name: _yapiInitAPI_internal (14522)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1CEAD
   }
@@ -10341,15 +10341,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D075
   }
   Symbol {
-    Name: _yapiFreeAPI (14558)
+    Name: _yapiFreeAPI (14544)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D075
   }
@@ -10377,15 +10377,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D07F
   }
   Symbol {
-    Name: _yapiFreeAPI_internal (14571)
+    Name: _yapiFreeAPI_internal (14557)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D07F
   }
@@ -10413,15 +10413,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2A9
   }
   Symbol {
-    Name: _yapiSetNetworkTimeout (14593)
+    Name: _yapiSetNetworkTimeout (14579)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2A9
   }
@@ -10449,15 +10449,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2B5
   }
   Symbol {
-    Name: _yapiGetNetworkTimeout (14616)
+    Name: _yapiGetNetworkTimeout (14602)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2B5
   }
@@ -10485,15 +10485,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2C1
   }
   Symbol {
-    Name: _yapiSetNetDevListValidity (14639)
+    Name: _yapiSetNetDevListValidity (14625)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2C1
   }
@@ -10521,15 +10521,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2D6
   }
   Symbol {
-    Name: _yapiGetNetDevListValidity (14666)
+    Name: _yapiGetNetDevListValidity (14652)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2D6
   }
@@ -10557,15 +10557,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2FB
   }
   Symbol {
-    Name: _yapiRegisterLogFunction (14693)
+    Name: _yapiRegisterLogFunction (14679)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D2FB
   }
@@ -10593,15 +10593,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D383
   }
   Symbol {
-    Name: _yapiRegisterDeviceLogCallback (14718)
+    Name: _yapiRegisterDeviceLogCallback (14704)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D383
   }
@@ -10629,15 +10629,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D40B
   }
   Symbol {
-    Name: _yapiStartStopDeviceLogCallback (14749)
+    Name: _yapiStartStopDeviceLogCallback (14735)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D40B
   }
@@ -10665,15 +10665,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D48C
   }
   Symbol {
-    Name: _yapiRegisterDeviceArrivalCallback (14781)
+    Name: _yapiRegisterDeviceArrivalCallback (14767)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D48C
   }
@@ -10701,15 +10701,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D514
   }
   Symbol {
-    Name: _yapiRegisterDeviceRemovalCallback (14816)
+    Name: _yapiRegisterDeviceRemovalCallback (14802)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D514
   }
@@ -10737,15 +10737,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D59C
   }
   Symbol {
-    Name: _yapiRegisterDeviceChangeCallback (14851)
+    Name: _yapiRegisterDeviceChangeCallback (14837)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D59C
   }
@@ -10773,15 +10773,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D608
   }
   Symbol {
-    Name: _yapiRegisterBeaconCallback (14885)
+    Name: _yapiRegisterBeaconCallback (14871)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D608
   }
@@ -10809,15 +10809,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D674
   }
   Symbol {
-    Name: _yapiRegisterDeviceConfigChangeCallback (14913)
+    Name: _yapiRegisterDeviceConfigChangeCallback (14899)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D674
   }
@@ -10845,15 +10845,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D6E0
   }
   Symbol {
-    Name: _yapiRegisterFunctionUpdateCallback (14953)
+    Name: _yapiRegisterFunctionUpdateCallback (14939)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D6E0
   }
@@ -10881,15 +10881,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D74C
   }
   Symbol {
-    Name: _yapiRegisterTimedReportCallback (14989)
+    Name: _yapiRegisterTimedReportCallback (14975)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D74C
   }
@@ -10917,15 +10917,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D7B8
   }
   Symbol {
-    Name: _yapiLockFunctionCallBack (15022)
+    Name: _yapiLockFunctionCallBack (15008)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D7B8
   }
@@ -10953,15 +10953,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D7F8
   }
   Symbol {
-    Name: _yapiUnlockFunctionCallBack (15048)
+    Name: _yapiUnlockFunctionCallBack (15034)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D7F8
   }
@@ -10989,15 +10989,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D838
   }
   Symbol {
-    Name: _yapiLockDeviceCallBack (15076)
+    Name: _yapiLockDeviceCallBack (15062)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D838
   }
@@ -11025,15 +11025,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D878
   }
   Symbol {
-    Name: _yapiUnlockDeviceCallBack (15100)
+    Name: _yapiUnlockDeviceCallBack (15086)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D878
   }
@@ -11061,15 +11061,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D8B8
   }
   Symbol {
-    Name: _yapiTestHub (15126)
+    Name: _yapiTestHub (15112)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1D8B8
   }
@@ -11097,15 +11097,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCD5
   }
   Symbol {
-    Name: _yapiRegisterHub (15139)
+    Name: _yapiRegisterHub (15125)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCD5
   }
@@ -11133,15 +11133,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCE7
   }
   Symbol {
-    Name: _yapiPreregisterHub (15156)
+    Name: _yapiPreregisterHub (15142)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCE7
   }
@@ -11169,15 +11169,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCF6
   }
   Symbol {
-    Name: _yapiUnregisterHub (15176)
+    Name: _yapiUnregisterHub (15162)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DCF6
   }
@@ -11205,15 +11205,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DD00
   }
   Symbol {
-    Name: _yapiUnregisterHub_internal (15195)
+    Name: _yapiUnregisterHub_internal (15181)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DD00
   }
@@ -11241,15 +11241,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DE4B
   }
   Symbol {
-    Name: _yapiUpdateDeviceList (15223)
+    Name: _yapiUpdateDeviceList (15209)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DE4B
   }
@@ -11277,15 +11277,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DE55
   }
   Symbol {
-    Name: _yapiUpdateDeviceList_internal (15245)
+    Name: _yapiUpdateDeviceList_internal (15231)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DE55
   }
@@ -11313,15 +11313,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DFED
   }
   Symbol {
-    Name: _yapiHandleEvents (15276)
+    Name: _yapiHandleEvents (15262)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DFED
   }
@@ -11349,15 +11349,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DFF7
   }
   Symbol {
-    Name: _yapiHandleEvents_internal (15294)
+    Name: _yapiHandleEvents_internal (15280)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1DFF7
   }
@@ -11385,15 +11385,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E05A
   }
   Symbol {
-    Name: _yapiSleep (15321)
+    Name: _yapiSleep (15307)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E05A
   }
@@ -11421,15 +11421,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E188
   }
   Symbol {
-    Name: _yapiCheckLogicalName (15332)
+    Name: _yapiCheckLogicalName (15318)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E188
   }
@@ -11457,15 +11457,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E20F
   }
   Symbol {
-    Name: _yapiGetAPIVersion (15354)
+    Name: _yapiGetAPIVersion (15340)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E20F
   }
@@ -11493,15 +11493,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E238
   }
   Symbol {
-    Name: _yapiSetTraceFile (15373)
+    Name: _yapiSetTraceFile (15359)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E238
   }
@@ -11529,15 +11529,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E283
   }
   Symbol {
-    Name: _yapiGetDevice (15391)
+    Name: _yapiGetDevice (15377)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E283
   }
@@ -11565,15 +11565,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E2E5
   }
   Symbol {
-    Name: _yapiGetAllDevices (15406)
+    Name: _yapiGetAllDevices (15392)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E2E5
   }
@@ -11601,15 +11601,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E3F4
   }
   Symbol {
-    Name: _yapiGetDeviceInfo (15425)
+    Name: _yapiGetDeviceInfo (15411)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E3F4
   }
@@ -11637,15 +11637,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E504
   }
   Symbol {
-    Name: _yapiGetDevicePathEx (15444)
+    Name: _yapiGetDevicePathEx (15430)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E504
   }
@@ -11673,15 +11673,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E71F
   }
   Symbol {
-    Name: _yapiGetFunction (15465)
+    Name: _yapiGetFunction (15451)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E71F
   }
@@ -11709,15 +11709,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E7A3
   }
   Symbol {
-    Name: _yapiGetFunctionsByClass (15482)
+    Name: _yapiGetFunctionsByClass (15468)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E7A3
   }
@@ -11745,15 +11745,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E835
   }
   Symbol {
-    Name: _yapiGetFunctionsByDevice (15507)
+    Name: _yapiGetFunctionsByDevice (15493)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E835
   }
@@ -11781,15 +11781,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E8C6
   }
   Symbol {
-    Name: _yapiGetFunctionInfo (15533)
+    Name: _yapiGetFunctionInfo (15519)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E8C6
   }
@@ -11817,15 +11817,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E8E2
   }
   Symbol {
-    Name: _yapiGetFunctionInfoEx_internal (15554)
+    Name: _yapiGetFunctionInfoEx_internal (15540)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E8E2
   }
@@ -11853,15 +11853,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E975
   }
   Symbol {
-    Name: _yapiGetFunctionInfoEx (15586)
+    Name: _yapiGetFunctionInfoEx (15572)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E975
   }
@@ -11889,15 +11889,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E97F
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncStartEx (15609)
+    Name: _yapiHTTPRequestSyncStartEx (15595)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E97F
   }
@@ -11925,15 +11925,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E9B8
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncStart (15637)
+    Name: _yapiHTTPRequestSyncStart (15623)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1E9B8
   }
@@ -11961,15 +11961,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA1B
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncStartOutOfBand (15663)
+    Name: _yapiHTTPRequestSyncStartOutOfBand (15649)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA1B
   }
@@ -11997,15 +11997,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA25
   }
   Symbol {
-    Name: _yapiHTTPRequestSyncDone (15698)
+    Name: _yapiHTTPRequestSyncDone (15684)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA25
   }
@@ -12033,15 +12033,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA2F
   }
   Symbol {
-    Name: _yapiHTTPRequestAsyncEx (15723)
+    Name: _yapiHTTPRequestAsyncEx (15709)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA2F
   }
@@ -12069,15 +12069,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA59
   }
   Symbol {
-    Name: _yapiHTTPRequestAsyncEx_internal (15747)
+    Name: _yapiHTTPRequestAsyncEx_internal (15733)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EA59
   }
@@ -12105,15 +12105,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EBFE
   }
   Symbol {
-    Name: _yapiHTTPRequestAsync (15780)
+    Name: _yapiHTTPRequestAsync (15766)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EBFE
   }
@@ -12141,15 +12141,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EC4B
   }
   Symbol {
-    Name: _yapiHTTPRequestAsyncOutOfBand (15802)
+    Name: _yapiHTTPRequestAsyncOutOfBand (15788)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EC4B
   }
@@ -12177,15 +12177,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EC94
   }
   Symbol {
-    Name: _yapiHTTPRequest (15833)
+    Name: _yapiHTTPRequest (15819)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EC94
   }
@@ -12213,15 +12213,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1ED91
   }
   Symbol {
-    Name: _yapiRegisterHubDiscoveryCallback (15850)
+    Name: _yapiRegisterHubDiscoveryCallback (15836)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1ED91
   }
@@ -12249,15 +12249,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EDFD
   }
   Symbol {
-    Name: _yapiRegisterWakeUpCb (15884)
+    Name: _yapiRegisterWakeUpCb (15870)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EDFD
   }
@@ -12285,15 +12285,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EE22
   }
   Symbol {
-    Name: _yapiTriggerHubDiscovery (15906)
+    Name: _yapiTriggerHubDiscovery (15892)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EE22
   }
@@ -12321,15 +12321,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EE8E
   }
   Symbol {
-    Name: _yapiGetBootloaders (15931)
+    Name: _yapiGetBootloaders (15917)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1EE8E
   }
@@ -12357,15 +12357,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F214
   }
   Symbol {
-    Name: _yapiIsModuleWritable (15951)
+    Name: _yapiIsModuleWritable (15937)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F214
   }
@@ -12393,15 +12393,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F2A2
   }
   Symbol {
-    Name: _yapiJsonDecodeString (15973)
+    Name: _yapiJsonDecodeString (15959)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F2A2
   }
@@ -12429,15 +12429,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F369
   }
   Symbol {
-    Name: _yapiJsonGetPath (15995)
+    Name: _yapiJsonGetPath (15981)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F369
   }
@@ -12465,15 +12465,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F3B4
   }
   Symbol {
-    Name: _yapiGetAllJsonKeys (16012)
+    Name: _yapiGetAllJsonKeys (15998)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F3B4
   }
@@ -12501,15 +12501,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8E8
   }
   Symbol {
-    Name: _yapiGetMem (16032)
+    Name: _yapiGetMem (16018)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8E8
   }
@@ -12537,15 +12537,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8F5
   }
   Symbol {
-    Name: _yapiFreeMem (16044)
+    Name: _yapiFreeMem (16030)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8F5
   }
@@ -12573,15 +12573,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8FF
   }
   Symbol {
-    Name: _yapiCheckFirmware (16057)
+    Name: _yapiCheckFirmware (16043)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F8FF
   }
@@ -12609,15 +12609,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F920
   }
   Symbol {
-    Name: _yapiUpdateFirmware (16076)
+    Name: _yapiUpdateFirmware (16062)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F920
   }
@@ -12645,15 +12645,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F932
   }
   Symbol {
-    Name: _yapiUpdateFirmwareEx (16096)
+    Name: _yapiUpdateFirmwareEx (16082)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F932
   }
@@ -12681,15 +12681,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F93C
   }
   Symbol {
-    Name: _yapiGetSubdevices (16118)
+    Name: _yapiGetSubdevices (16104)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1F93C
   }
@@ -12717,15 +12717,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FB82
   }
   Symbol {
-    Name: _deleteAllCS (16137)
+    Name: _deleteAllCS (16123)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FB82
   }
@@ -12753,15 +12753,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FBDE
   }
   Symbol {
-    Name: _ssdpEntryUpdate (16150)
+    Name: _ssdpEntryUpdate (16136)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FBDE
   }
@@ -12789,15 +12789,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FC80
   }
   Symbol {
-    Name: _unregisterNetHub (16167)
+    Name: _unregisterNetHub (16153)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FC80
   }
@@ -12825,15 +12825,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF13
   }
   Symbol {
-    Name: _isSameHub (16185)
+    Name: _isSameHub (16171)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF13
   }
@@ -12861,15 +12861,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF6A
   }
   Symbol {
-    Name: _yapiFreeHub (16196)
+    Name: _yapiFreeHub (16182)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x1FF6A
   }
@@ -12897,15 +12897,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x200E6
   }
   Symbol {
-    Name: _yFreeParsedURL (16209)
+    Name: _yFreeParsedURL (16195)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x200E6
   }
@@ -12933,15 +12933,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2014C
   }
   Symbol {
-    Name: _yapiAllocHub (16225)
+    Name: _yapiAllocHub (16211)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2014C
   }
@@ -12969,15 +12969,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20986
   }
   Symbol {
-    Name: _pingURLOnhub (16239)
+    Name: _pingURLOnhub (16225)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20986
   }
@@ -13005,15 +13005,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20C50
   }
   Symbol {
-    Name: _yParseHubURL (16253)
+    Name: _yParseHubURL (16239)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20C50
   }
@@ -13041,15 +13041,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20F2D
   }
   Symbol {
-    Name: _yapiRegisterHubEx (16267)
+    Name: _yapiRegisterHubEx (16253)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x20F2D
   }
@@ -13077,15 +13077,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x216D4
   }
   Symbol {
-    Name: _yhelper_thread (16286)
+    Name: _yhelper_thread (16272)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x216D4
   }
@@ -13113,15 +13113,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x21F6E
   }
   Symbol {
-    Name: _yNetHubEnum (16302)
+    Name: _yNetHubEnum (16288)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x21F6E
   }
@@ -13149,15 +13149,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x22341
   }
   Symbol {
-    Name: _yNetHubEnumEx (16315)
+    Name: _yNetHubEnumEx (16301)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x22341
   }
@@ -13185,15 +13185,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23CD8
   }
   Symbol {
-    Name: _disable_jzon (16330)
+    Name: _disable_jzon (16316)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23CD8
   }
@@ -13221,15 +13221,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23D1E
   }
   Symbol {
-    Name: _parseNetWpEntry (16344)
+    Name: _parseNetWpEntry (16330)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23D1E
   }
@@ -13257,15 +13257,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23DAA
   }
   Symbol {
-    Name: _ypUpdateNet (16361)
+    Name: _ypUpdateNet (16347)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23DAA
   }
@@ -13293,15 +13293,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E09
   }
   Symbol {
-    Name: _asyncDrop (16374)
+    Name: _asyncDrop (16360)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E09
   }
@@ -13320,24 +13320,24 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E09
   }
   Symbol {
-    Name: _YctxDeviceListValidityMs (16385)
+    Name: _YctxDeviceListValidityMs (16371)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _YctxNetworkTimeout (16411)
+    Name: _YctxNetworkTimeout (16397)
     Type: SymDebugTable (0x20)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
@@ -13347,51 +13347,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: yfifo.c (16431)
+    Name: yfifo.c (16417)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yfifo.o (16439)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/yfifo.o (16425)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E10
   }
   Symbol {
-    Name: _yFifoInitEx (16586)
+    Name: _yFifoInitEx (16572)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E10
   }
@@ -13419,15 +13419,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E42
   }
   Symbol {
-    Name: _yFifoCleanup (16599)
+    Name: _yFifoCleanup (16585)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E42
   }
@@ -13455,15 +13455,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E6D
   }
   Symbol {
-    Name: _yFifoEnterCS (16613)
+    Name: _yFifoEnterCS (16599)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E6D
   }
@@ -13491,15 +13491,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E7B
   }
   Symbol {
-    Name: _yFifoLeaveCS (16627)
+    Name: _yFifoLeaveCS (16613)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E7B
   }
@@ -13527,15 +13527,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E89
   }
   Symbol {
-    Name: _yFifoEmptyEx (16641)
+    Name: _yFifoEmptyEx (16627)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23E89
   }
@@ -13563,15 +13563,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23EA1
   }
   Symbol {
-    Name: _yFifoEmpty (16655)
+    Name: _yFifoEmpty (16641)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23EA1
   }
@@ -13599,15 +13599,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23ED5
   }
   Symbol {
-    Name: _yPushFifoEx (16667)
+    Name: _yPushFifoEx (16653)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23ED5
   }
@@ -13635,15 +13635,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23F6D
   }
   Symbol {
-    Name: _yPushFifo (16680)
+    Name: _yPushFifo (16666)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23F6D
   }
@@ -13671,15 +13671,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23FB1
   }
   Symbol {
-    Name: _yPopFifoEx (16691)
+    Name: _yPopFifoEx (16677)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x23FB1
   }
@@ -13707,15 +13707,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2407A
   }
   Symbol {
-    Name: _yPopFifo (16703)
+    Name: _yPopFifo (16689)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2407A
   }
@@ -13743,15 +13743,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x240BE
   }
   Symbol {
-    Name: _yForceFifo (16713)
+    Name: _yForceFifo (16699)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x240BE
   }
@@ -13779,15 +13779,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2413B
   }
   Symbol {
-    Name: _yPeekFifoEx (16725)
+    Name: _yPeekFifoEx (16711)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2413B
   }
@@ -13815,15 +13815,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x241E7
   }
   Symbol {
-    Name: _yPeekFifo (16738)
+    Name: _yPeekFifo (16724)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x241E7
   }
@@ -13851,15 +13851,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2423A
   }
   Symbol {
-    Name: _yPeekContinuousFifoEx (16749)
+    Name: _yPeekContinuousFifoEx (16735)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2423A
   }
@@ -13887,15 +13887,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2428F
   }
   Symbol {
-    Name: _yPeekContinuousFifo (16772)
+    Name: _yPeekContinuousFifo (16758)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2428F
   }
@@ -13923,15 +13923,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x242D3
   }
   Symbol {
-    Name: _ySeekFifoEx (16793)
+    Name: _ySeekFifoEx (16779)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x242D3
   }
@@ -13959,15 +13959,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24422
   }
   Symbol {
-    Name: _ySeekFifo (16806)
+    Name: _ySeekFifo (16792)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24422
   }
@@ -13995,15 +13995,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24485
   }
   Symbol {
-    Name: _yFifoGetUsedEx (16817)
+    Name: _yFifoGetUsedEx (16803)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24485
   }
@@ -14031,15 +14031,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2448F
   }
   Symbol {
-    Name: _yFifoGetUsed (16833)
+    Name: _yFifoGetUsed (16819)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2448F
   }
@@ -14067,15 +14067,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x244B8
   }
   Symbol {
-    Name: _yFifoGetFreeEx (16847)
+    Name: _yFifoGetFreeEx (16833)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x244B8
   }
@@ -14103,15 +14103,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x244C8
   }
   Symbol {
-    Name: _yFifoGetFree (16863)
+    Name: _yFifoGetFree (16849)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x244C8
   }
@@ -14139,15 +14139,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24500
   }
   Symbol {
-    Name: _yxtoa (16877)
+    Name: _yxtoa (16863)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24500
   }
@@ -14175,15 +14175,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24535
   }
   Symbol {
-    Name: _decodePubVal (16884)
+    Name: _decodePubVal (16870)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24535
   }
@@ -14211,51 +14211,51 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8831)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Sources/yapi/ (8817)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: ythread.c (16898)
+    Name: ythread.c (16884)
     Type: SymDebugTable (0x64)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ythread.o (16908)
+    Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/x86_64/ythread.o (16894)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383587
+    Value: 0x643DB1BE
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24768
   }
   Symbol {
-    Name: _yCreateEvent (17057)
+    Name: _yCreateEvent (17043)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24768
   }
@@ -14283,15 +14283,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24798
   }
   Symbol {
-    Name: _yCreateManualEvent (17071)
+    Name: _yCreateManualEvent (17057)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24798
   }
@@ -14319,15 +14319,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x247CE
   }
   Symbol {
-    Name: _ySetEvent (17091)
+    Name: _ySetEvent (17077)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x247CE
   }
@@ -14355,15 +14355,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x247FF
   }
   Symbol {
-    Name: _yResetEvent (17102)
+    Name: _yResetEvent (17088)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x247FF
   }
@@ -14391,15 +14391,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24828
   }
   Symbol {
-    Name: _yWaitForEvent (17115)
+    Name: _yWaitForEvent (17101)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24828
   }
@@ -14427,15 +14427,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24901
   }
   Symbol {
-    Name: _yCloseEvent (17130)
+    Name: _yCloseEvent (17116)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24901
   }
@@ -14463,15 +14463,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24921
   }
   Symbol {
-    Name: _yThreadIndex (17143)
+    Name: _yThreadIndex (17129)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24921
   }
@@ -14499,15 +14499,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24974
   }
   Symbol {
-    Name: _yCreateDetachedThreadNamed (17157)
+    Name: _yCreateDetachedThreadNamed (17143)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24974
   }
@@ -14535,15 +14535,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2498E
   }
   Symbol {
-    Name: _yCreateDetachedThreadEx (17185)
+    Name: _yCreateDetachedThreadEx (17171)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2498E
   }
@@ -14571,15 +14571,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24A0E
   }
   Symbol {
-    Name: _yThreadCreateNamed (17210)
+    Name: _yThreadCreateNamed (17196)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24A0E
   }
@@ -14607,15 +14607,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24ABB
   }
   Symbol {
-    Name: _yThreadIsRunning (17230)
+    Name: _yThreadIsRunning (17216)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24ABB
   }
@@ -14643,15 +14643,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AD1
   }
   Symbol {
-    Name: _yThreadSignalStart (17248)
+    Name: _yThreadSignalStart (17234)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AD1
   }
@@ -14679,15 +14679,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AE9
   }
   Symbol {
-    Name: _yThreadSignalEnd (17268)
+    Name: _yThreadSignalEnd (17254)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AE9
   }
@@ -14715,15 +14715,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AF9
   }
   Symbol {
-    Name: _yThreadRequestEnd (17286)
+    Name: _yThreadRequestEnd (17272)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24AF9
   }
@@ -14751,15 +14751,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B12
   }
   Symbol {
-    Name: _yThreadMustEnd (17305)
+    Name: _yThreadMustEnd (17291)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B12
   }
@@ -14787,15 +14787,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B24
   }
   Symbol {
-    Name: _yThreadKill (17321)
+    Name: _yThreadKill (17307)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B24
   }
@@ -14823,15 +14823,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B4A
   }
   Symbol {
-    Name: _yInitializeCriticalSection (17334)
+    Name: _yInitializeCriticalSection (17320)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24B4A
   }
@@ -14859,15 +14859,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BC1
   }
   Symbol {
-    Name: _yEnterCriticalSection (17362)
+    Name: _yEnterCriticalSection (17348)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BC1
   }
@@ -14895,15 +14895,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BCE
   }
   Symbol {
-    Name: _yTryEnterCriticalSection (17385)
+    Name: _yTryEnterCriticalSection (17371)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BCE
   }
@@ -14931,15 +14931,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BE6
   }
   Symbol {
-    Name: _yLeaveCriticalSection (17411)
+    Name: _yLeaveCriticalSection (17397)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BE6
   }
@@ -14967,15 +14967,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BF3
   }
   Symbol {
-    Name: _yDeleteCriticalSection (17434)
+    Name: _yDeleteCriticalSection (17420)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24BF3
   }
@@ -15003,15 +15003,15 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24C1A
   }
   Symbol {
-    Name: _initTsdKey (17458)
+    Name: _initTsdKey (17444)
     Type: SymDebugTable (0x24)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24C1A
   }
@@ -15030,33 +15030,33 @@
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x24C1A
   }
   Symbol {
-    Name: _yInitKeyOnce (17470)
+    Name: _yInitKeyOnce (17456)
     Type: SymDebugTable (0x26)
     Section:  (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1C0
   }
   Symbol {
-    Name: _yNextThreadIdx (17484)
+    Name: _yNextThreadIdx (17470)
     Type: SymDebugTable (0x26)
     Section:  (0x9)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x2C1D0
   }
   Symbol {
-    Name: _yTsdKey (17500)
+    Name: _yTsdKey (17486)
     Type: SymDebugTable (0x26)
     Section:  (0xB)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
     ]
     Value: 0x6D308
   }
@@ -18883,543 +18883,532 @@
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _objc_msgSend (6366)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x400)
-      ColdFunc (0x400)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _open (6380)
+    Name: _open (6366)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _opendir$INODE64 (6386)
+    Name: _opendir$INODE64 (6372)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_attr_destroy (6403)
+    Name: _pthread_attr_destroy (6389)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_attr_init (6425)
+    Name: _pthread_attr_init (6411)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_attr_setdetachstate (6444)
+    Name: _pthread_attr_setdetachstate (6430)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cancel (6473)
+    Name: _pthread_cancel (6459)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cond_destroy (6489)
+    Name: _pthread_cond_destroy (6475)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cond_init (6511)
+    Name: _pthread_cond_init (6497)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cond_signal (6530)
+    Name: _pthread_cond_signal (6516)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cond_timedwait (6551)
+    Name: _pthread_cond_timedwait (6537)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_cond_wait (6575)
+    Name: _pthread_cond_wait (6561)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_create (6594)
+    Name: _pthread_create (6580)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_getspecific (6610)
+    Name: _pthread_getspecific (6596)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_join (6631)
+    Name: _pthread_join (6617)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_key_create (6645)
+    Name: _pthread_key_create (6631)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutex_destroy (6665)
+    Name: _pthread_mutex_destroy (6651)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutex_init (6688)
+    Name: _pthread_mutex_init (6674)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutex_lock (6708)
+    Name: _pthread_mutex_lock (6694)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutex_trylock (6728)
+    Name: _pthread_mutex_trylock (6714)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutex_unlock (6751)
+    Name: _pthread_mutex_unlock (6737)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutexattr_init (6773)
+    Name: _pthread_mutexattr_init (6759)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_mutexattr_settype (6797)
+    Name: _pthread_mutexattr_settype (6783)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_once (6824)
+    Name: _pthread_once (6810)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _pthread_setspecific (6838)
+    Name: _pthread_setspecific (6824)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _rand (6859)
+    Name: _rand (6845)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _read (6865)
+    Name: _read (6851)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _readdir$INODE64 (6871)
+    Name: _readdir$INODE64 (6857)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _recv (6888)
+    Name: _recv (6874)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _select$1050 (6894)
+    Name: _select$1050 (6880)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _send (6907)
+    Name: _send (6893)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _sendto (6913)
+    Name: _sendto (6899)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _setsockopt (6921)
+    Name: _setsockopt (6907)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _socket (6933)
+    Name: _socket (6919)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _stat$INODE64 (6941)
+    Name: _stat$INODE64 (6927)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strcasecmp (6955)
+    Name: _strcasecmp (6941)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strchr (6967)
+    Name: _strchr (6953)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strcmp (6975)
+    Name: _strcmp (6961)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strcpy (6983)
+    Name: _strcpy (6969)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strerror (6991)
+    Name: _strerror (6977)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strlen (7001)
+    Name: _strlen (6987)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strncasecmp (7009)
+    Name: _strncasecmp (6995)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strncmp (7022)
+    Name: _strncmp (7008)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _strstr (7031)
+    Name: _strstr (7017)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _sysctlbyname (7039)
+    Name: _sysctlbyname (7025)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _time (7053)
+    Name: _time (7039)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _usleep (7059)
+    Name: _usleep (7045)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _vsnprintf (7067)
+    Name: _vsnprintf (7053)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
     Value: 0x0
   }
   Symbol {
-    Name: _write (7078)
+    Name: _write (7064)
     Extern
     Type: Undef (0x0)
     Section:  (0x0)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x100)
       SymbolResolver (0x100)
     ]
@@ -20424,15 +20413,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ymemory.o (8867)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -20784,15 +20773,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ytcp.o (9126)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -22431,15 +22420,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ystream.o (9948)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -24366,15 +24355,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/yprog.o (10905)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -25473,15 +25462,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/yjson.o (11615)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -25581,15 +25570,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ykey.o (11791)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383589
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -26211,15 +26200,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/yhash.o (12183)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383589
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -27849,15 +27838,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ypkt_osx.o (13172)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -28389,15 +28378,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/yapi.o (13571)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383589
+    Value: 0x643DB1C1
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -32799,15 +32788,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/yfifo.o (16384)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383589
+    Value: 0x643DB1C0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
@@ -33663,15 +33652,15 @@
   Symbol {
     Name: /Users/yocto/tmp_build/yoctoprod/yoctolib/v1.0/Public/cpp/Binaries/xcode_as/yapi/build/yapi.build/Release/yapi.build/Objects-normal/arm64/ythread.o (16852)
     Type: SymDebugTable (0x66)
     Section:  (0x0)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64383588
+    Value: 0x643DB1BF
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

##### llvm-objdump --arch=x86_64 --section=__TEXT,__text --macho --demangle --no-leading-addr --no-show-raw-insn {}

```diff
@@ -11554,29 +11554,29 @@
 	jmp	0xf281
 	testb	$1, %r12b
 	jne	0xf33b
 	cmpb	$0, (%r15)
 	je	0xf33b
 	movq	%r15, %rdi
 	callq	0x24d18 ## symbol stub for: _atoi
-	cmpl	$54038, %eax
+	cmpl	$54071, %eax
 	jl	0xf33b
 	leaq	94250(%rip), %rdx ## literal pool for: "This firmware is too recent, please upgrade your VirtualHub or Yoctopuce library"
 	leaq	94060(%rip), %rcx ## literal pool for: "yprog"
 	movl	$4294967291, %edi
 	movq	%r14, %rsi
 	movl	$251, %r8d
 	jmp	0xf281
 	testb	$1, %r12b
 	jne	0xf365
 	cmpb	$0, (%r13)
 	je	0xf365
 	movq	%r13, %rdi
 	callq	0x24d18 ## symbol stub for: _atoi
-	cmpl	$54038, %eax
+	cmpl	$54071, %eax
 	jl	0xf365
 	leaq	94192(%rip), %rdx ## literal pool for: "This firmware is too recent, please upgrade your VirtualHub or Yoctopuce library"
 	leaq	94002(%rip), %rcx ## literal pool for: "yprog"
 	movl	$4294967291, %edi
 	movq	%r14, %rsi
 	movl	$231, %r8d
 	jmp	0xf281
@@ -27576,19 +27576,19 @@
 	popq	%rbp
 	retq
 _yapiGetAPIVersion:
 	pushq	%rbp
 	movq	%rsp, %rbp
 	testq	%rdi, %rdi
 	je	0x1e222
-	leaq	38550(%rip), %rax ## literal pool for: "1.10.54037"
+	leaq	38550(%rip), %rax ## literal pool for: "1.10.54070"
 	movq	%rax, (%rdi)
 	testq	%rsi, %rsi
 	je	0x1e231
-	leaq	38546(%rip), %rax ## literal pool for: "Apr 13 2023 19:02:00"
+	leaq	38546(%rip), %rax ## literal pool for: "Apr 17 2023 22:53:19"
 	movq	%rax, (%rsi)
 	movl	$272, %eax
 	popq	%rbp
 	retq
 _yapiSetTraceFile:
 	pushq	%rbp
 	movq	%rsp, %rbp
```

##### llvm-objdump --arch=x86_64 --section=__TEXT,__cstring --macho --demangle --no-leading-addr --no-show-raw-insn {}

```diff
@@ -443,16 +443,16 @@
 beacon
 index
 baseType
 hardwareId
 advertisedValue
 Disable JZON encoding for hub %\n
 Enumeration failed for %s:%d (%s)
-1.10.54037
-Apr 13 2023 19:02:00
+1.10.54070
+Apr 17 2023 22:53:19
 Yoctopuce
 %s://%s:%d%s%s
 No function of that class
 ASync request for %s failed. Retrying after yapiUpdateDeviceList\n
 yapiUpdateDeviceList failled too with %s\n
 %s\"%s/%s=
 \"
```

#### aarch64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O universal binary with 2 architectures: [x86_64:\012- Mach-O 64-bit x86_64 dynamically linked shared library, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|NO_REEXPORTED_DYLIBS>] [\012- arm64:\012- Mach-O 64-bit arm64 dynamically linked shared library, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|NO_REEXPORTED_DYLIBS>]*

```diff
@@ -1,9 +1,9 @@
 00000000: cafe babe 0000 0002 0100 0007 0000 0003  ................
-00000010: 0000 4000 0004 3fd0 0000 000e 0100 000c  ..@...?.........
+00000010: 0000 4000 0004 3fb0 0000 000e 0100 000c  ..@...?.........
 00000020: 0000 0000 0004 8000 0004 3ef0 0000 000e  ..........>.....
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1019,15 +1019,15 @@
 00003fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004000: cffa edfe 0700 0001 0300 0000 0600 0000  ................
-00004010: 1300 0000 f806 0000 8500 1000 0000 0000  ................
+00004010: 1200 0000 c006 0000 8500 1000 0000 0000  ................
 00004020: 1900 0000 d801 0000 5f5f 5445 5854 0000  ........__TEXT..
 00004030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004040: 0080 0200 0000 0000 0000 0000 0000 0000  ................
 00004050: 0080 0200 0000 0000 0500 0000 0500 0000  ................
 00004060: 0500 0000 0000 0000 5f5f 7465 7874 0000  ........__text..
 00004070: 0000 0000 0000 0000 5f5f 5445 5854 0000  ........__TEXT..
 00004080: 0000 0000 0000 0000 e83c 0000 0000 0000  .........<......
@@ -1091,30 +1091,30 @@
 00004420: 0000 0000 0000 0000 5f5f 4441 5441 0000  ........__DATA..
 00004430: 0000 0000 0000 0000 d0ce 0200 0000 0000  ................
 00004440: 4004 0400 0000 0000 0000 0000 0400 0000  @...............
 00004450: 0000 0000 0000 0000 0100 0000 0000 0000  ................
 00004460: 0000 0000 0000 0000 1900 0000 4800 0000  ............H...
 00004470: 5f5f 4c49 4e4b 4544 4954 0000 0000 0000  __LINKEDIT......
 00004480: 0000 0700 0000 0000 0040 0100 0000 0000  .........@......
-00004490: 0000 0300 0000 0000 d03f 0100 0000 0000  .........?......
+00004490: 0000 0300 0000 0000 b03f 0100 0000 0000  .........?......
 000044a0: 0100 0000 0100 0000 0000 0000 0000 0000  ................
 000044b0: 0d00 0000 3800 0000 1800 0000 0100 0000  ....8...........
 000044c0: 0000 0100 0000 0100 2f75 7372 2f6c 6f63  ......../usr/loc
 000044d0: 616c 2f6c 6962 2f6c 6962 7961 7069 2e64  al/lib/libyapi.d
 000044e0: 796c 6962 0000 0000 3400 0080 1000 0000  ylib....4.......
 000044f0: 0000 0300 c009 0000 3300 0080 1000 0000  ........3.......
 00004500: c009 0300 8817 0000 0200 0000 1800 0000  ................
-00004510: 1024 0300 3008 0000 c0aa 0300 6844 0000  .$..0.......hD..
+00004510: 1024 0300 2f08 0000 b0aa 0300 5844 0000  .$../.......XD..
 00004520: 0b00 0000 5000 0000 0000 0000 8a06 0000  ....P...........
-00004530: 8a06 0000 2b01 0000 b507 0000 7b00 0000  ....+.......{...
+00004530: 8a06 0000 2b01 0000 b507 0000 7a00 0000  ....+.......z...
 00004540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004550: 0000 0000 0000 0000 10a7 0300 ec00 0000  ................
+00004550: 0000 0000 0000 0000 00a7 0300 ec00 0000  ................
 00004560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004570: 1b00 0000 1800 0000 af3f 5f9a 013e 3c5f  .........?_..><_
-00004580: bce4 367b 642b 2035 3200 0000 2000 0000  ..6{d+ 52... ...
+00004570: 1b00 0000 1800 0000 5e7e 2953 b18a 3407  ........^~)S..4.
+00004580: bb0c b69f 5766 f7f7 3200 0000 2000 0000  ....Wf..2... ...
 00004590: 0100 0000 0001 0c00 0001 0d00 0100 0000  ................
 000045a0: 0300 0000 0001 3403 2a00 0000 1000 0000  ......4.*.......
 000045b0: 0000 0000 0000 0000 0c00 0000 3800 0000  ............8...
 000045c0: 1800 0000 0200 0000 0000 2705 0000 0100  ..........'.....
 000045d0: 2f75 7372 2f6c 6962 2f6c 6962 5379 7374  /usr/lib/libSyst
 000045e0: 656d 2e42 2e64 796c 6962 0000 0000 0000  em.B.dylib......
 000045f0: 0c00 0000 6800 0000 1800 0000 0200 0000  ....h...........
@@ -1125,21 +1125,21 @@
 00004640: 696f 6e73 2f41 2f43 6f72 6546 6f75 6e64  ions/A/CoreFound
 00004650: 6174 696f 6e00 0000 0c00 0000 5800 0000  ation.......X...
 00004660: 1800 0000 0200 0000 0000 1301 0000 0100  ................
 00004670: 2f53 7973 7465 6d2f 4c69 6272 6172 792f  /System/Library/
 00004680: 4672 616d 6577 6f72 6b73 2f49 4f4b 6974  Frameworks/IOKit
 00004690: 2e66 7261 6d65 776f 726b 2f56 6572 7369  .framework/Versi
 000046a0: 6f6e 732f 412f 494f 4b69 7400 0000 0000  ons/A/IOKit.....
-000046b0: 0c00 0000 3800 0000 1800 0000 0200 0000  ....8...........
-000046c0: 0000 e400 0000 0100 2f75 7372 2f6c 6962  ......../usr/lib
-000046d0: 2f6c 6962 6f62 6a63 2e41 2e64 796c 6962  /libobjc.A.dylib
-000046e0: 0000 0000 0000 0000 2600 0000 1000 0000  ........&.......
-000046f0: 4821 0300 4002 0000 2900 0000 1000 0000  H!..@...).......
-00004700: 8823 0300 8800 0000 1d00 0000 1000 0000  .#..............
-00004710: 30ef 0300 a050 0000 0000 0000 0000 0000  0....P..........
+000046b0: 2600 0000 1000 0000 4821 0300 4002 0000  &.......H!..@...
+000046c0: 2900 0000 1000 0000 8823 0300 8800 0000  )........#......
+000046d0: 1d00 0000 1000 0000 10ef 0300 a050 0000  .............P..
+000046e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000046f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -4903,19 +4903,19 @@
 00013260: 0000 00eb 1c48 8d15 3871 0100 488d 0de7  .....H..8q..H...
 00013270: 6f01 00bf feff ffff 4c89 f641 b809 0100  o.......L..A....
 00013280: 0048 83c4 085b 415c 415d 415e 415f 5de9  .H...[A\A]A^A_].
 00013290: e8b6 ffff 8b43 6444 89f9 4883 c198 4839  .....CdD..H...H9
 000132a0: c10f 841e 0100 0048 8d15 0c70 0100 488d  .......H...p..H.
 000132b0: 0da5 6f01 00bf feff ffff 4c89 f641 b8db  ..o.......L..A..
 000132c0: 0000 00eb bc41 f6c4 0175 7041 803f 0074  .....A...upA.?.t
-000132d0: 6a4c 89ff e83f 5a01 003d 16d3 0000 7c5b  jL...?Z..=....|[
+000132d0: 6a4c 89ff e83f 5a01 003d 37d3 0000 7c5b  jL...?Z..=7...|[
 000132e0: 488d 152a 7001 0048 8d0d 6c6f 0100 bffb  H..*p..H..lo....
 000132f0: ffff ff4c 89f6 41b8 fb00 0000 eb83 41f6  ...L..A.......A.
 00013300: c401 7561 4180 7d00 0074 5a4c 89ef e805  ..uaA.}..tZL....
-00013310: 5a01 003d 16d3 0000 7c4b 488d 15f0 6f01  Z..=....|KH...o.
+00013310: 5a01 003d 37d3 0000 7c4b 488d 15f0 6f01  Z..=7...|KH...o.
 00013320: 0048 8d0d 326f 0100 bffb ffff ff4c 89f6  .H..2o.......L..
 00013330: 41b8 e700 0000 e946 ffff ff80 bb86 0000  A......F........
 00013340: 0011 7248 488d 1517 7001 0048 8d0d 086f  ..rHH...p..H...o
 00013350: 0100 bffe ffff ff4c 89f6 41b8 0001 0000  .......L..A.....
 00013360: e91c ffff ff83 7b78 1172 4b48 8d15 2c6f  ......{x.rKH..,o
 00013370: 0100 488d 0de1 6e01 00bf feff ffff 4c89  ..H...n.......L.
 00013380: f641 b8ec 0000 00e9 f5fe ffff 80bb 8700  .A..............
@@ -11141,17 +11141,17 @@
 0002b840: 0062 6561 636f 6e00 696e 6465 7800 6261  .beacon.index.ba
 0002b850: 7365 5479 7065 0068 6172 6477 6172 6549  seType.hardwareI
 0002b860: 6400 6164 7665 7274 6973 6564 5661 6c75  d.advertisedValu
 0002b870: 6500 4469 7361 626c 6520 4a5a 4f4e 2065  e.Disable JZON e
 0002b880: 6e63 6f64 696e 6720 666f 7220 6875 6220  ncoding for hub 
 0002b890: 250a 0045 6e75 6d65 7261 7469 6f6e 2066  %..Enumeration f
 0002b8a0: 6169 6c65 6420 666f 7220 2573 3a25 6420  ailed for %s:%d 
-0002b8b0: 2825 7329 0031 2e31 302e 3534 3033 3700  (%s).1.10.54037.
-0002b8c0: 4170 7220 3133 2032 3032 3320 3139 3a30  Apr 13 2023 19:0
-0002b8d0: 323a 3030 0059 6f63 746f 7075 6365 0025  2:00.Yoctopuce.%
+0002b8b0: 2825 7329 0031 2e31 302e 3534 3037 3000  (%s).1.10.54070.
+0002b8c0: 4170 7220 3137 2032 3032 3320 3232 3a35  Apr 17 2023 22:5
+0002b8d0: 333a 3139 0059 6f63 746f 7075 6365 0025  3:19.Yoctopuce.%
 0002b8e0: 733a 2f2f 2573 3a25 6425 7325 7300 4e6f  s://%s:%d%s%s.No
 0002b8f0: 2066 756e 6374 696f 6e20 6f66 2074 6861   function of tha
 0002b900: 7420 636c 6173 7300 4153 796e 6320 7265  t class.ASync re
 0002b910: 7175 6573 7420 666f 7220 2573 2066 6169  quest for %s fai
 0002b920: 6c65 642e 2052 6574 7279 696e 6720 6166  led. Retrying af
 0002b930: 7465 7220 7961 7069 5570 6461 7465 4465  ter yapiUpdateDe
 0002b940: 7669 6365 4c69 7374 0a00 7961 7069 5570  viceList..yapiUp
@@ -13883,1687 +13883,1687 @@
 000363a0: 9ccb 0000 1800 0400 58cd 0000 1800 0400  ........X.......
 000363b0: c0d0 0000 1800 0400 c4d3 0000 1800 0400  ................
 000363c0: 2cef 0000 2c00 0400 6808 0100 4800 0400  ,...,...h...H...
 000363d0: 480b 0100 1000 0400 4c31 0100 1000 0400  H.......L1......
 000363e0: f43c 0100 5000 0400 a467 0100 1c00 0400  .<..P....g......
 000363f0: 54b8 0100 4400 0400 94cd 0100 1c00 0400  T...D...........
 00036400: a83b 0200 3001 0400 4047 0200 2800 0400  .;..0...@G..(...
-00036410: ad1b 0000 0e01 0000 454e 0000 0000 0000  ........EN......
-00036420: b71b 0000 0e01 0000 c752 0000 0000 0000  .........R......
-00036430: c21b 0000 0e01 0000 7054 0000 0000 0000  ........pT......
-00036440: cc1b 0000 0e01 0000 085c 0000 0000 0000  .........\......
-00036450: dc1b 0000 0e01 0000 1967 0000 0000 0000  .........g......
-00036460: f11b 0000 0e01 0000 4b6e 0000 0000 0000  ........Kn......
-00036470: 061c 0000 0e01 0000 8a70 0000 0000 0000  .........p......
-00036480: 171c 0000 0e01 0000 2f71 0000 0000 0000  ......../q......
-00036490: 241c 0000 0e01 0000 3b72 0000 0000 0000  $.......;r......
-000364a0: 321c 0000 0e01 0000 b495 0000 0000 0000  2...............
-000364b0: 3f1c 0000 0e01 0000 9a9b 0000 0000 0000  ?...............
-000364c0: 4d1c 0000 0e01 0000 17a0 0000 0000 0000  M...............
-000364d0: 5e1c 0000 0e01 0000 41a1 0000 0000 0000  ^.......A.......
-000364e0: 6c1c 0000 0e01 0000 55a2 0000 0000 0000  l.......U.......
-000364f0: 7e1c 0000 0e01 0000 04a3 0000 0000 0000  ~...............
-00036500: 8c1c 0000 0e01 0000 4aa4 0000 0000 0000  ........J.......
-00036510: a41c 0000 0e01 0000 0dae 0000 0000 0000  ................
-00036520: b11c 0000 0e01 0000 d0b0 0000 0000 0000  ................
-00036530: c21c 0000 0e01 0000 24b2 0000 0000 0000  ........$.......
-00036540: d01c 0000 0e01 0000 95b4 0000 0000 0000  ................
-00036550: e21c 0000 0e01 0000 fcc2 0000 0000 0000  ................
-00036560: f41c 0000 0e01 0000 e4c7 0000 0000 0000  ................
-00036570: 051d 0000 0e01 0000 03c9 0000 0000 0000  ................
-00036580: 131d 0000 0e01 0000 87c9 0000 0000 0000  ................
-00036590: 231d 0000 0e01 0000 1aca 0000 0000 0000  #...............
-000365a0: 2e1d 0000 0e01 0000 b4cb 0000 0000 0000  ................
-000365b0: 3a1d 0000 0e01 0000 a4d1 0000 0000 0000  :...............
-000365c0: 461d 0000 0e01 0000 5ddc 0000 0000 0000  F.......].......
-000365d0: 541d 0000 0e01 0000 40dd 0000 0000 0000  T.......@.......
-000365e0: 611d 0000 0e01 0000 f0e3 0000 0000 0000  a...............
-000365f0: 721d 0000 0e01 0000 2ae4 0000 0000 0000  r.......*.......
-00036600: 851d 0000 0e01 0000 75e5 0000 0000 0000  ........u.......
-00036610: 961d 0000 0e01 0000 d2e9 0000 0000 0000  ................
-00036620: a71d 0000 0e01 0000 b008 0100 0000 0000  ................
-00036630: b91d 0000 0e01 0000 e908 0100 0000 0000  ................
-00036640: c91d 0000 0e01 0000 580b 0100 0000 0000  ........X.......
-00036650: d71d 0000 0e01 0000 f412 0100 0000 0000  ................
-00036660: e21d 0000 0e01 0000 3813 0100 0000 0000  ........8.......
-00036670: f71d 0000 0e01 0000 c017 0100 0000 0000  ................
-00036680: 0d1e 0000 0e01 0000 5a19 0100 0000 0000  ........Z.......
-00036690: 241e 0000 0e01 0000 211a 0100 0000 0000  $.......!.......
-000366a0: 371e 0000 0e01 0000 631b 0100 0000 0000  7.......c.......
-000366b0: 4f1e 0000 0e01 0000 022a 0100 0000 0000  O........*......
-000366c0: 641e 0000 0e01 0000 652a 0100 0000 0000  d.......e*......
-000366d0: 751e 0000 0e01 0000 5c31 0100 0000 0000  u.......\1......
-000366e0: 7d1e 0000 0e01 0000 c633 0100 0000 0000  }........3......
-000366f0: 8e1e 0000 0e01 0000 8749 0100 0000 0000  .........I......
-00036700: 981e 0000 0e01 0000 cf4a 0100 0000 0000  .........J......
-00036710: a21e 0000 0e01 0000 e94e 0100 0000 0000  .........N......
-00036720: b01e 0000 0e01 0000 bb58 0100 0000 0000  .........X......
-00036730: bb1e 0000 0e01 0000 235a 0100 0000 0000  ........#Z......
-00036740: c51e 0000 0e01 0000 1289 0100 0000 0000  ................
-00036750: cf1e 0000 0e01 0000 a08b 0100 0000 0000  ................
-00036760: dd1e 0000 0e01 0000 578c 0100 0000 0000  ........W.......
-00036770: ee1e 0000 0e01 0000 628e 0100 0000 0000  ........b.......
-00036780: fe1e 0000 0e01 0000 0f90 0100 0000 0000  ................
-00036790: 091f 0000 0e01 0000 7f90 0100 0000 0000  ................
-000367a0: 1b1f 0000 0e01 0000 d890 0100 0000 0000  ................
-000367b0: 2d1f 0000 0e01 0000 2395 0100 0000 0000  -.......#.......
-000367c0: 541f 0000 0e01 0000 509d 0100 0000 0000  T.......P.......
-000367d0: 681f 0000 0e01 0000 b89f 0100 0000 0000  h...............
-000367e0: 731f 0000 0e01 0000 42a2 0100 0000 0000  s.......B.......
-000367f0: 861f 0000 0e01 0000 efa4 0100 0000 0000  ................
-00036800: 9b1f 0000 0e01 0000 98b8 0100 0000 0000  ................
-00036810: b01f 0000 0e01 0000 f6c2 0100 0000 0000  ................
-00036820: c31f 0000 0e01 0000 07c6 0100 0000 0000  ................
-00036830: d51f 0000 0e01 0000 1fca 0100 0000 0000  ................
-00036840: ef1f 0000 0e01 0000 adce 0100 0000 0000  ................
-00036850: 0520 0000 0e01 0000 7fd0 0100 0000 0000  . ..............
-00036860: 1b20 0000 0e01 0000 00dd 0100 0000 0000  . ..............
-00036870: 3720 0000 0e01 0000 55de 0100 0000 0000  7 ......U.......
-00036880: 5620 0000 0e01 0000 f7df 0100 0000 0000  V ..............
-00036890: 7120 0000 0e01 0000 e2e8 0100 0000 0000  q ..............
-000368a0: 9120 0000 0e01 0000 59ea 0100 0000 0000  . ......Y.......
-000368b0: b220 0000 0e01 0000 82fb 0100 0000 0000  . ..............
-000368c0: bf20 0000 0e01 0000 defb 0100 0000 0000  . ..............
-000368d0: d020 0000 0e01 0000 80fc 0100 0000 0000  . ..............
-000368e0: e220 0000 0e01 0000 13ff 0100 0000 0000  . ..............
-000368f0: ed20 0000 0e01 0000 6aff 0100 0000 0000  . ......j.......
-00036900: fa20 0000 0e01 0000 e600 0200 0000 0000  . ..............
-00036910: 0a21 0000 0e01 0000 4c01 0200 0000 0000  .!......L.......
-00036920: 1821 0000 0e01 0000 8609 0200 0000 0000  .!..............
-00036930: 2621 0000 0e01 0000 500c 0200 0000 0000  &!......P.......
-00036940: 3421 0000 0e01 0000 2d0f 0200 0000 0000  4!......-.......
-00036950: 4721 0000 0e01 0000 d416 0200 0000 0000  G!..............
-00036960: 5721 0000 0e01 0000 6e1f 0200 0000 0000  W!......n.......
-00036970: 6421 0000 0e01 0000 4123 0200 0000 0000  d!......A#......
-00036980: 7321 0000 0e01 0000 d83c 0200 0000 0000  s!.......<......
-00036990: 8121 0000 0e01 0000 1e3d 0200 0000 0000  .!.......=......
-000369a0: 9221 0000 0e01 0000 aa3d 0200 0000 0000  .!.......=......
-000369b0: 9f21 0000 0e01 0000 093e 0200 0000 0000  .!.......>......
-000369c0: aa21 0000 0e01 0000 8e49 0200 0000 0000  .!.......I......
-000369d0: c321 0000 0e01 0000 1a4c 0200 0000 0000  .!.......L......
-000369e0: cf21 0000 0e04 0000 307a 0200 0000 0000  .!......0z......
-000369f0: d721 0000 0e09 0000 00c0 0200 0000 0000  .!..............
-00036a00: dd21 0000 0e09 0000 a6c1 0200 0000 0000  .!..............
-00036a10: e921 0000 0e09 0000 a8c1 0200 0000 0000  .!..............
-00036a20: f821 0000 0e09 0000 c0c1 0200 0000 0000  .!..............
-00036a30: 0622 0000 0e09 0000 d0c1 0200 0000 0000  ."..............
-00036a40: 1622 0000 0e0b 0000 d0ce 0200 0000 0000  ."..............
-00036a50: 2222 0000 0e0b 0000 d0ce 0600 0000 0000  ""..............
-00036a60: 2d22 0000 0e0b 0000 d0d0 0600 0000 0000  -"..............
-00036a70: 3822 0000 0e0b 0000 d0d2 0600 0000 0000  8"..............
-00036a80: 4422 0000 0e0b 0000 e0d2 0600 0000 0000  D"..............
-00036a90: 5022 0000 0e0b 0000 00d3 0600 0000 0000  P"..............
-00036aa0: 5d22 0000 0e0b 0000 04d3 0600 0000 0000  ]"..............
-00036ab0: 7622 0000 0e0b 0000 08d3 0600 0000 0000  v"..............
+00036410: 9f1b 0000 0e01 0000 454e 0000 0000 0000  ........EN......
+00036420: a91b 0000 0e01 0000 c752 0000 0000 0000  .........R......
+00036430: b41b 0000 0e01 0000 7054 0000 0000 0000  ........pT......
+00036440: be1b 0000 0e01 0000 085c 0000 0000 0000  .........\......
+00036450: ce1b 0000 0e01 0000 1967 0000 0000 0000  .........g......
+00036460: e31b 0000 0e01 0000 4b6e 0000 0000 0000  ........Kn......
+00036470: f81b 0000 0e01 0000 8a70 0000 0000 0000  .........p......
+00036480: 091c 0000 0e01 0000 2f71 0000 0000 0000  ......../q......
+00036490: 161c 0000 0e01 0000 3b72 0000 0000 0000  ........;r......
+000364a0: 241c 0000 0e01 0000 b495 0000 0000 0000  $...............
+000364b0: 311c 0000 0e01 0000 9a9b 0000 0000 0000  1...............
+000364c0: 3f1c 0000 0e01 0000 17a0 0000 0000 0000  ?...............
+000364d0: 501c 0000 0e01 0000 41a1 0000 0000 0000  P.......A.......
+000364e0: 5e1c 0000 0e01 0000 55a2 0000 0000 0000  ^.......U.......
+000364f0: 701c 0000 0e01 0000 04a3 0000 0000 0000  p...............
+00036500: 7e1c 0000 0e01 0000 4aa4 0000 0000 0000  ~.......J.......
+00036510: 961c 0000 0e01 0000 0dae 0000 0000 0000  ................
+00036520: a31c 0000 0e01 0000 d0b0 0000 0000 0000  ................
+00036530: b41c 0000 0e01 0000 24b2 0000 0000 0000  ........$.......
+00036540: c21c 0000 0e01 0000 95b4 0000 0000 0000  ................
+00036550: d41c 0000 0e01 0000 fcc2 0000 0000 0000  ................
+00036560: e61c 0000 0e01 0000 e4c7 0000 0000 0000  ................
+00036570: f71c 0000 0e01 0000 03c9 0000 0000 0000  ................
+00036580: 051d 0000 0e01 0000 87c9 0000 0000 0000  ................
+00036590: 151d 0000 0e01 0000 1aca 0000 0000 0000  ................
+000365a0: 201d 0000 0e01 0000 b4cb 0000 0000 0000   ...............
+000365b0: 2c1d 0000 0e01 0000 a4d1 0000 0000 0000  ,...............
+000365c0: 381d 0000 0e01 0000 5ddc 0000 0000 0000  8.......].......
+000365d0: 461d 0000 0e01 0000 40dd 0000 0000 0000  F.......@.......
+000365e0: 531d 0000 0e01 0000 f0e3 0000 0000 0000  S...............
+000365f0: 641d 0000 0e01 0000 2ae4 0000 0000 0000  d.......*.......
+00036600: 771d 0000 0e01 0000 75e5 0000 0000 0000  w.......u.......
+00036610: 881d 0000 0e01 0000 d2e9 0000 0000 0000  ................
+00036620: 991d 0000 0e01 0000 b008 0100 0000 0000  ................
+00036630: ab1d 0000 0e01 0000 e908 0100 0000 0000  ................
+00036640: bb1d 0000 0e01 0000 580b 0100 0000 0000  ........X.......
+00036650: c91d 0000 0e01 0000 f412 0100 0000 0000  ................
+00036660: d41d 0000 0e01 0000 3813 0100 0000 0000  ........8.......
+00036670: e91d 0000 0e01 0000 c017 0100 0000 0000  ................
+00036680: ff1d 0000 0e01 0000 5a19 0100 0000 0000  ........Z.......
+00036690: 161e 0000 0e01 0000 211a 0100 0000 0000  ........!.......
+000366a0: 291e 0000 0e01 0000 631b 0100 0000 0000  ).......c.......
+000366b0: 411e 0000 0e01 0000 022a 0100 0000 0000  A........*......
+000366c0: 561e 0000 0e01 0000 652a 0100 0000 0000  V.......e*......
+000366d0: 671e 0000 0e01 0000 5c31 0100 0000 0000  g.......\1......
+000366e0: 6f1e 0000 0e01 0000 c633 0100 0000 0000  o........3......
+000366f0: 801e 0000 0e01 0000 8749 0100 0000 0000  .........I......
+00036700: 8a1e 0000 0e01 0000 cf4a 0100 0000 0000  .........J......
+00036710: 941e 0000 0e01 0000 e94e 0100 0000 0000  .........N......
+00036720: a21e 0000 0e01 0000 bb58 0100 0000 0000  .........X......
+00036730: ad1e 0000 0e01 0000 235a 0100 0000 0000  ........#Z......
+00036740: b71e 0000 0e01 0000 1289 0100 0000 0000  ................
+00036750: c11e 0000 0e01 0000 a08b 0100 0000 0000  ................
+00036760: cf1e 0000 0e01 0000 578c 0100 0000 0000  ........W.......
+00036770: e01e 0000 0e01 0000 628e 0100 0000 0000  ........b.......
+00036780: f01e 0000 0e01 0000 0f90 0100 0000 0000  ................
+00036790: fb1e 0000 0e01 0000 7f90 0100 0000 0000  ................
+000367a0: 0d1f 0000 0e01 0000 d890 0100 0000 0000  ................
+000367b0: 1f1f 0000 0e01 0000 2395 0100 0000 0000  ........#.......
+000367c0: 461f 0000 0e01 0000 509d 0100 0000 0000  F.......P.......
+000367d0: 5a1f 0000 0e01 0000 b89f 0100 0000 0000  Z...............
+000367e0: 651f 0000 0e01 0000 42a2 0100 0000 0000  e.......B.......
+000367f0: 781f 0000 0e01 0000 efa4 0100 0000 0000  x...............
+00036800: 8d1f 0000 0e01 0000 98b8 0100 0000 0000  ................
+00036810: a21f 0000 0e01 0000 f6c2 0100 0000 0000  ................
+00036820: b51f 0000 0e01 0000 07c6 0100 0000 0000  ................
+00036830: c71f 0000 0e01 0000 1fca 0100 0000 0000  ................
+00036840: e11f 0000 0e01 0000 adce 0100 0000 0000  ................
+00036850: f71f 0000 0e01 0000 7fd0 0100 0000 0000  ................
+00036860: 0d20 0000 0e01 0000 00dd 0100 0000 0000  . ..............
+00036870: 2920 0000 0e01 0000 55de 0100 0000 0000  ) ......U.......
+00036880: 4820 0000 0e01 0000 f7df 0100 0000 0000  H ..............
+00036890: 6320 0000 0e01 0000 e2e8 0100 0000 0000  c ..............
+000368a0: 8320 0000 0e01 0000 59ea 0100 0000 0000  . ......Y.......
+000368b0: a420 0000 0e01 0000 82fb 0100 0000 0000  . ..............
+000368c0: b120 0000 0e01 0000 defb 0100 0000 0000  . ..............
+000368d0: c220 0000 0e01 0000 80fc 0100 0000 0000  . ..............
+000368e0: d420 0000 0e01 0000 13ff 0100 0000 0000  . ..............
+000368f0: df20 0000 0e01 0000 6aff 0100 0000 0000  . ......j.......
+00036900: ec20 0000 0e01 0000 e600 0200 0000 0000  . ..............
+00036910: fc20 0000 0e01 0000 4c01 0200 0000 0000  . ......L.......
+00036920: 0a21 0000 0e01 0000 8609 0200 0000 0000  .!..............
+00036930: 1821 0000 0e01 0000 500c 0200 0000 0000  .!......P.......
+00036940: 2621 0000 0e01 0000 2d0f 0200 0000 0000  &!......-.......
+00036950: 3921 0000 0e01 0000 d416 0200 0000 0000  9!..............
+00036960: 4921 0000 0e01 0000 6e1f 0200 0000 0000  I!......n.......
+00036970: 5621 0000 0e01 0000 4123 0200 0000 0000  V!......A#......
+00036980: 6521 0000 0e01 0000 d83c 0200 0000 0000  e!.......<......
+00036990: 7321 0000 0e01 0000 1e3d 0200 0000 0000  s!.......=......
+000369a0: 8421 0000 0e01 0000 aa3d 0200 0000 0000  .!.......=......
+000369b0: 9121 0000 0e01 0000 093e 0200 0000 0000  .!.......>......
+000369c0: 9c21 0000 0e01 0000 8e49 0200 0000 0000  .!.......I......
+000369d0: b521 0000 0e01 0000 1a4c 0200 0000 0000  .!.......L......
+000369e0: c121 0000 0e04 0000 307a 0200 0000 0000  .!......0z......
+000369f0: c921 0000 0e09 0000 00c0 0200 0000 0000  .!..............
+00036a00: cf21 0000 0e09 0000 a6c1 0200 0000 0000  .!..............
+00036a10: db21 0000 0e09 0000 a8c1 0200 0000 0000  .!..............
+00036a20: ea21 0000 0e09 0000 c0c1 0200 0000 0000  .!..............
+00036a30: f821 0000 0e09 0000 d0c1 0200 0000 0000  .!..............
+00036a40: 0822 0000 0e0b 0000 d0ce 0200 0000 0000  ."..............
+00036a50: 1422 0000 0e0b 0000 d0ce 0600 0000 0000  ."..............
+00036a60: 1f22 0000 0e0b 0000 d0d0 0600 0000 0000  ."..............
+00036a70: 2a22 0000 0e0b 0000 d0d2 0600 0000 0000  *"..............
+00036a80: 3622 0000 0e0b 0000 e0d2 0600 0000 0000  6"..............
+00036a90: 4222 0000 0e0b 0000 00d3 0600 0000 0000  B"..............
+00036aa0: 4f22 0000 0e0b 0000 04d3 0600 0000 0000  O"..............
+00036ab0: 6822 0000 0e0b 0000 08d3 0600 0000 0000  h"..............
 00036ac0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00036ad0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00036ae0: c722 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00036af0: d122 0000 6603 0100 8735 3864 0000 0000  ."..f....58d....
+00036ad0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00036ae0: b922 0000 6400 0000 0000 0000 0000 0000  ."..d...........
+00036af0: c322 0000 6603 0100 beb1 3d64 0000 0000  ."..f.....=d....
 00036b00: 0100 0000 2e01 0000 e83c 0000 0000 0000  .........<......
-00036b10: 6623 0000 2401 0000 e83c 0000 0000 0000  f#..$....<......
+00036b10: 5823 0000 2401 0000 e83c 0000 0000 0000  X#..$....<......
 00036b20: 0100 0000 2400 0000 0c00 0000 0000 0000  ....$...........
 00036b30: 0100 0000 4e01 0000 e83c 0000 0000 0000  ....N....<......
 00036b40: 0100 0000 2e01 0000 f43c 0000 0000 0000  .........<......
-00036b50: 7123 0000 2401 0000 f43c 0000 0000 0000  q#..$....<......
+00036b50: 6323 0000 2401 0000 f43c 0000 0000 0000  c#..$....<......
 00036b60: 0100 0000 2400 0000 ee00 0000 0000 0000  ....$...........
 00036b70: 0100 0000 4e01 0000 f43c 0000 0000 0000  ....N....<......
 00036b80: 0100 0000 2e01 0000 e23d 0000 0000 0000  .........=......
-00036b90: 7d23 0000 2401 0000 e23d 0000 0000 0000  }#..$....=......
+00036b90: 6f23 0000 2401 0000 e23d 0000 0000 0000  o#..$....=......
 00036ba0: 0100 0000 2400 0000 3e00 0000 0000 0000  ....$...>.......
 00036bb0: 0100 0000 4e01 0000 e23d 0000 0000 0000  ....N....=......
 00036bc0: 0100 0000 2e01 0000 203e 0000 0000 0000  ........ >......
-00036bd0: 8823 0000 2401 0000 203e 0000 0000 0000  .#..$... >......
+00036bd0: 7a23 0000 2401 0000 203e 0000 0000 0000  z#..$... >......
 00036be0: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 00036bf0: 0100 0000 4e01 0000 203e 0000 0000 0000  ....N... >......
 00036c00: 0100 0000 2e01 0000 603e 0000 0000 0000  ........`>......
-00036c10: 9423 0000 2401 0000 603e 0000 0000 0000  .#..$...`>......
+00036c10: 8623 0000 2401 0000 603e 0000 0000 0000  .#..$...`>......
 00036c20: 0100 0000 2400 0000 0c00 0000 0000 0000  ....$...........
 00036c30: 0100 0000 4e01 0000 603e 0000 0000 0000  ....N...`>......
 00036c40: 0100 0000 2e01 0000 6c3e 0000 0000 0000  ........l>......
-00036c50: 9f23 0000 2401 0000 6c3e 0000 0000 0000  .#..$...l>......
+00036c50: 9123 0000 2401 0000 6c3e 0000 0000 0000  .#..$...l>......
 00036c60: 0100 0000 2400 0000 a700 0000 0000 0000  ....$...........
 00036c70: 0100 0000 4e01 0000 6c3e 0000 0000 0000  ....N...l>......
 00036c80: 0100 0000 2e01 0000 133f 0000 0000 0000  .........?......
-00036c90: ab23 0000 2401 0000 133f 0000 0000 0000  .#..$....?......
+00036c90: 9d23 0000 2401 0000 133f 0000 0000 0000  .#..$....?......
 00036ca0: 0100 0000 2400 0000 9600 0000 0000 0000  ....$...........
 00036cb0: 0100 0000 4e01 0000 133f 0000 0000 0000  ....N....?......
 00036cc0: 0100 0000 2e01 0000 a93f 0000 0000 0000  .........?......
-00036cd0: b723 0000 2401 0000 a93f 0000 0000 0000  .#..$....?......
+00036cd0: a923 0000 2401 0000 a93f 0000 0000 0000  .#..$....?......
 00036ce0: 0100 0000 2400 0000 6100 0000 0000 0000  ....$...a.......
 00036cf0: 0100 0000 4e01 0000 a93f 0000 0000 0000  ....N....?......
 00036d00: 0100 0000 2e01 0000 0a40 0000 0000 0000  .........@......
-00036d10: c423 0000 2401 0000 0a40 0000 0000 0000  .#..$....@......
+00036d10: b623 0000 2401 0000 0a40 0000 0000 0000  .#..$....@......
 00036d20: 0100 0000 2400 0000 6400 0000 0000 0000  ....$...d.......
 00036d30: 0100 0000 4e01 0000 0a40 0000 0000 0000  ....N....@......
 00036d40: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00036d50: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00036d60: ce23 0000 6400 0000 0000 0000 0000 0000  .#..d...........
-00036d70: d523 0000 6603 0100 8735 3864 0000 0000  .#..f....58d....
+00036d50: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00036d60: c023 0000 6400 0000 0000 0000 0000 0000  .#..d...........
+00036d70: c723 0000 6603 0100 bfb1 3d64 0000 0000  .#..f.....=d....
 00036d80: 0100 0000 2e01 0000 7040 0000 0000 0000  ........p@......
-00036d90: 6724 0000 2401 0000 7040 0000 0000 0000  g$..$...p@......
+00036d90: 5924 0000 2401 0000 7040 0000 0000 0000  Y$..$...p@......
 00036da0: 0100 0000 2400 0000 6500 0000 0000 0000  ....$...e.......
 00036db0: 0100 0000 4e01 0000 7040 0000 0000 0000  ....N...p@......
 00036dc0: 0100 0000 2e01 0000 d540 0000 0000 0000  .........@......
-00036dd0: 7024 0000 2401 0000 d540 0000 0000 0000  p$..$....@......
+00036dd0: 6224 0000 2401 0000 d540 0000 0000 0000  b$..$....@......
 00036de0: 0100 0000 2400 0000 6500 0000 0000 0000  ....$...e.......
 00036df0: 0100 0000 4e01 0000 d540 0000 0000 0000  ....N....@......
 00036e00: 0100 0000 2e01 0000 3a41 0000 0000 0000  ........:A......
-00036e10: 7e24 0000 2401 0000 3a41 0000 0000 0000  ~$..$...:A......
+00036e10: 7024 0000 2401 0000 3a41 0000 0000 0000  p$..$...:A......
 00036e20: 0100 0000 2400 0000 0d00 0000 0000 0000  ....$...........
 00036e30: 0100 0000 4e01 0000 3a41 0000 0000 0000  ....N...:A......
 00036e40: 0100 0000 2e01 0000 4741 0000 0000 0000  ........GA......
-00036e50: 9124 0000 2401 0000 4741 0000 0000 0000  .$..$...GA......
+00036e50: 8324 0000 2401 0000 4741 0000 0000 0000  .$..$...GA......
 00036e60: 0100 0000 2400 0000 be01 0000 0000 0000  ....$...........
 00036e70: 0100 0000 4e01 0000 4741 0000 0000 0000  ....N...GA......
 00036e80: 0100 0000 2e01 0000 0543 0000 0000 0000  .........C......
-00036e90: a524 0000 2401 0000 0543 0000 0000 0000  .$..$....C......
+00036e90: 9724 0000 2401 0000 0543 0000 0000 0000  .$..$....C......
 00036ea0: 0100 0000 2400 0000 5600 0000 0000 0000  ....$...V.......
 00036eb0: 0100 0000 4e01 0000 0543 0000 0000 0000  ....N....C......
 00036ec0: 0100 0000 2e01 0000 5b43 0000 0000 0000  ........[C......
-00036ed0: b924 0000 2401 0000 5b43 0000 0000 0000  .$..$...[C......
+00036ed0: ab24 0000 2401 0000 5b43 0000 0000 0000  .$..$...[C......
 00036ee0: 0100 0000 2400 0000 5000 0000 0000 0000  ....$...P.......
 00036ef0: 0100 0000 4e01 0000 5b43 0000 0000 0000  ....N...[C......
 00036f00: 0100 0000 2e01 0000 ab43 0000 0000 0000  .........C......
-00036f10: cf24 0000 2401 0000 ab43 0000 0000 0000  .$..$....C......
+00036f10: c124 0000 2401 0000 ab43 0000 0000 0000  .$..$....C......
 00036f20: 0100 0000 2400 0000 3600 0000 0000 0000  ....$...6.......
 00036f30: 0100 0000 4e01 0000 ab43 0000 0000 0000  ....N....C......
 00036f40: 0100 0000 2e01 0000 e143 0000 0000 0000  .........C......
-00036f50: e224 0000 2401 0000 e143 0000 0000 0000  .$..$....C......
+00036f50: d424 0000 2401 0000 e143 0000 0000 0000  .$..$....C......
 00036f60: 0100 0000 2400 0000 7a00 0000 0000 0000  ....$...z.......
 00036f70: 0100 0000 4e01 0000 e143 0000 0000 0000  ....N....C......
 00036f80: 0100 0000 2e01 0000 5b44 0000 0000 0000  ........[D......
-00036f90: ef24 0000 2401 0000 5b44 0000 0000 0000  .$..$...[D......
+00036f90: e124 0000 2401 0000 5b44 0000 0000 0000  .$..$...[D......
 00036fa0: 0100 0000 2400 0000 1900 0000 0000 0000  ....$...........
 00036fb0: 0100 0000 4e01 0000 5b44 0000 0000 0000  ....N...[D......
 00036fc0: 0100 0000 2e01 0000 7444 0000 0000 0000  ........tD......
-00036fd0: f924 0000 2401 0000 7444 0000 0000 0000  .$..$...tD......
+00036fd0: eb24 0000 2401 0000 7444 0000 0000 0000  .$..$...tD......
 00036fe0: 0100 0000 2400 0000 3800 0000 0000 0000  ....$...8.......
 00036ff0: 0100 0000 4e01 0000 7444 0000 0000 0000  ....N...tD......
 00037000: 0100 0000 2e01 0000 ac44 0000 0000 0000  .........D......
-00037010: 0725 0000 2401 0000 ac44 0000 0000 0000  .%..$....D......
+00037010: f924 0000 2401 0000 ac44 0000 0000 0000  .$..$....D......
 00037020: 0100 0000 2400 0000 6000 0000 0000 0000  ....$...`.......
 00037030: 0100 0000 4e01 0000 ac44 0000 0000 0000  ....N....D......
 00037040: 0100 0000 2e01 0000 0c45 0000 0000 0000  .........E......
-00037050: 1225 0000 2401 0000 0c45 0000 0000 0000  .%..$....E......
+00037050: 0425 0000 2401 0000 0c45 0000 0000 0000  .%..$....E......
 00037060: 0100 0000 2400 0000 3909 0000 0000 0000  ....$...9.......
 00037070: 0100 0000 4e01 0000 0c45 0000 0000 0000  ....N....E......
 00037080: 0100 0000 2e01 0000 454e 0000 0000 0000  ........EN......
-00037090: 2025 0000 2401 0000 454e 0000 0000 0000   %..$...EN......
+00037090: 1225 0000 2401 0000 454e 0000 0000 0000  .%..$...EN......
 000370a0: 0100 0000 2400 0000 8204 0000 0000 0000  ....$...........
 000370b0: 0100 0000 4e01 0000 454e 0000 0000 0000  ....N...EN......
 000370c0: 0100 0000 2e01 0000 c752 0000 0000 0000  .........R......
-000370d0: 2a25 0000 2401 0000 c752 0000 0000 0000  *%..$....R......
+000370d0: 1c25 0000 2401 0000 c752 0000 0000 0000  .%..$....R......
 000370e0: 0100 0000 2400 0000 a901 0000 0000 0000  ....$...........
 000370f0: 0100 0000 4e01 0000 c752 0000 0000 0000  ....N....R......
 00037100: 0100 0000 2e01 0000 7054 0000 0000 0000  ........pT......
-00037110: 3525 0000 2401 0000 7054 0000 0000 0000  5%..$...pT......
+00037110: 2725 0000 2401 0000 7054 0000 0000 0000  '%..$...pT......
 00037120: 0100 0000 2400 0000 7a00 0000 0000 0000  ....$...z.......
 00037130: 0100 0000 4e01 0000 7054 0000 0000 0000  ....N...pT......
 00037140: 0100 0000 2e01 0000 ea54 0000 0000 0000  .........T......
-00037150: 3f25 0000 2401 0000 ea54 0000 0000 0000  ?%..$....T......
+00037150: 3125 0000 2401 0000 ea54 0000 0000 0000  1%..$....T......
 00037160: 0100 0000 2400 0000 7e00 0000 0000 0000  ....$...~.......
 00037170: 0100 0000 4e01 0000 ea54 0000 0000 0000  ....N....T......
 00037180: 0100 0000 2e01 0000 6855 0000 0000 0000  ........hU......
-00037190: 4a25 0000 2401 0000 6855 0000 0000 0000  J%..$...hU......
+00037190: 3c25 0000 2401 0000 6855 0000 0000 0000  <%..$...hU......
 000371a0: 0100 0000 2400 0000 a006 0000 0000 0000  ....$...........
 000371b0: 0100 0000 4e01 0000 6855 0000 0000 0000  ....N...hU......
 000371c0: 0100 0000 2e01 0000 085c 0000 0000 0000  .........\......
-000371d0: 5425 0000 2401 0000 085c 0000 0000 0000  T%..$....\......
+000371d0: 4625 0000 2401 0000 085c 0000 0000 0000  F%..$....\......
 000371e0: 0100 0000 2400 0000 bf0a 0000 0000 0000  ....$...........
 000371f0: 0100 0000 4e01 0000 085c 0000 0000 0000  ....N....\......
 00037200: 0100 0000 2e01 0000 c766 0000 0000 0000  .........f......
-00037210: 6425 0000 2401 0000 c766 0000 0000 0000  d%..$....f......
+00037210: 5625 0000 2401 0000 c766 0000 0000 0000  V%..$....f......
 00037220: 0100 0000 2400 0000 5200 0000 0000 0000  ....$...R.......
 00037230: 0100 0000 4e01 0000 c766 0000 0000 0000  ....N....f......
 00037240: 0100 0000 2e01 0000 1967 0000 0000 0000  .........g......
-00037250: 7025 0000 2401 0000 1967 0000 0000 0000  p%..$....g......
+00037250: 6225 0000 2401 0000 1967 0000 0000 0000  b%..$....g......
 00037260: 0100 0000 2400 0000 8406 0000 0000 0000  ....$...........
 00037270: 0100 0000 4e01 0000 1967 0000 0000 0000  ....N....g......
 00037280: 0100 0000 2e01 0000 9d6d 0000 0000 0000  .........m......
-00037290: 8525 0000 2401 0000 9d6d 0000 0000 0000  .%..$....m......
+00037290: 7725 0000 2401 0000 9d6d 0000 0000 0000  w%..$....m......
 000372a0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 000372b0: 0100 0000 4e01 0000 9d6d 0000 0000 0000  ....N....m......
 000372c0: 0100 0000 2e01 0000 a76d 0000 0000 0000  .........m......
-000372d0: 9625 0000 2401 0000 a76d 0000 0000 0000  .%..$....m......
+000372d0: 8825 0000 2401 0000 a76d 0000 0000 0000  .%..$....m......
 000372e0: 0100 0000 2400 0000 a400 0000 0000 0000  ....$...........
 000372f0: 0100 0000 4e01 0000 a76d 0000 0000 0000  ....N....m......
 00037300: 0100 0000 2e01 0000 4b6e 0000 0000 0000  ........Kn......
-00037310: a125 0000 2401 0000 4b6e 0000 0000 0000  .%..$...Kn......
+00037310: 9325 0000 2401 0000 4b6e 0000 0000 0000  .%..$...Kn......
 00037320: 0100 0000 2400 0000 a600 0000 0000 0000  ....$...........
 00037330: 0100 0000 4e01 0000 4b6e 0000 0000 0000  ....N...Kn......
 00037340: 0100 0000 2e01 0000 f16e 0000 0000 0000  .........n......
-00037350: b625 0000 2401 0000 f16e 0000 0000 0000  .%..$....n......
+00037350: a825 0000 2401 0000 f16e 0000 0000 0000  .%..$....n......
 00037360: 0100 0000 2400 0000 6800 0000 0000 0000  ....$...h.......
 00037370: 0100 0000 4e01 0000 f16e 0000 0000 0000  ....N....n......
 00037380: 0100 0000 2e01 0000 596f 0000 0000 0000  ........Yo......
-00037390: bf25 0000 2401 0000 596f 0000 0000 0000  .%..$...Yo......
+00037390: b125 0000 2401 0000 596f 0000 0000 0000  .%..$...Yo......
 000373a0: 0100 0000 2400 0000 cc00 0000 0000 0000  ....$...........
 000373b0: 0100 0000 4e01 0000 596f 0000 0000 0000  ....N...Yo......
 000373c0: 0100 0000 2e01 0000 2570 0000 0000 0000  ........%p......
-000373d0: c925 0000 2401 0000 2570 0000 0000 0000  .%..$...%p......
+000373d0: bb25 0000 2401 0000 2570 0000 0000 0000  .%..$...%p......
 000373e0: 0100 0000 2400 0000 6500 0000 0000 0000  ....$...e.......
 000373f0: 0100 0000 4e01 0000 2570 0000 0000 0000  ....N...%p......
 00037400: 0100 0000 2e01 0000 8a70 0000 0000 0000  .........p......
-00037410: d425 0000 2401 0000 8a70 0000 0000 0000  .%..$....p......
+00037410: c625 0000 2401 0000 8a70 0000 0000 0000  .%..$....p......
 00037420: 0100 0000 2400 0000 a500 0000 0000 0000  ....$...........
 00037430: 0100 0000 4e01 0000 8a70 0000 0000 0000  ....N....p......
 00037440: 0100 0000 2e01 0000 2f71 0000 0000 0000  ......../q......
-00037450: e525 0000 2401 0000 2f71 0000 0000 0000  .%..$.../q......
+00037450: d725 0000 2401 0000 2f71 0000 0000 0000  .%..$.../q......
 00037460: 0100 0000 2400 0000 0c01 0000 0000 0000  ....$...........
 00037470: 0100 0000 4e01 0000 2f71 0000 0000 0000  ....N.../q......
 00037480: 0100 0000 2e01 0000 3b72 0000 0000 0000  ........;r......
-00037490: f225 0000 2401 0000 3b72 0000 0000 0000  .%..$...;r......
+00037490: e425 0000 2401 0000 3b72 0000 0000 0000  .%..$...;r......
 000374a0: 0100 0000 2400 0000 d000 0000 0000 0000  ....$...........
 000374b0: 0100 0000 4e01 0000 3b72 0000 0000 0000  ....N...;r......
 000374c0: 0100 0000 2e01 0000 0b73 0000 0000 0000  .........s......
-000374d0: 0026 0000 2401 0000 0b73 0000 0000 0000  .&..$....s......
+000374d0: f225 0000 2401 0000 0b73 0000 0000 0000  .%..$....s......
 000374e0: 0100 0000 2400 0000 4a00 0000 0000 0000  ....$...J.......
 000374f0: 0100 0000 4e01 0000 0b73 0000 0000 0000  ....N....s......
 00037500: 0100 0000 2e01 0000 5573 0000 0000 0000  ........Us......
-00037510: 0d26 0000 2401 0000 5573 0000 0000 0000  .&..$...Us......
+00037510: ff25 0000 2401 0000 5573 0000 0000 0000  .%..$...Us......
 00037520: 0100 0000 2400 0000 9800 0000 0000 0000  ....$...........
 00037530: 0100 0000 4e01 0000 5573 0000 0000 0000  ....N...Us......
 00037540: 0100 0000 2e01 0000 ed73 0000 0000 0000  .........s......
-00037550: 1726 0000 2401 0000 ed73 0000 0000 0000  .&..$....s......
+00037550: 0926 0000 2401 0000 ed73 0000 0000 0000  .&..$....s......
 00037560: 0100 0000 2400 0000 b600 0000 0000 0000  ....$...........
 00037570: 0100 0000 4e01 0000 ed73 0000 0000 0000  ....N....s......
 00037580: 0100 0000 2e01 0000 a374 0000 0000 0000  .........t......
-00037590: 2726 0000 2401 0000 a374 0000 0000 0000  '&..$....t......
+00037590: 1926 0000 2401 0000 a374 0000 0000 0000  .&..$....t......
 000375a0: 0100 0000 2400 0000 3300 0000 0000 0000  ....$...3.......
 000375b0: 0100 0000 4e01 0000 a374 0000 0000 0000  ....N....t......
 000375c0: 0100 0000 2e01 0000 d674 0000 0000 0000  .........t......
-000375d0: 3326 0000 2401 0000 d674 0000 0000 0000  3&..$....t......
+000375d0: 2526 0000 2401 0000 d674 0000 0000 0000  %&..$....t......
 000375e0: 0100 0000 2400 0000 de20 0000 0000 0000  ....$.... ......
 000375f0: 0100 0000 4e01 0000 d674 0000 0000 0000  ....N....t......
 00037600: 0100 0000 2e01 0000 b495 0000 0000 0000  ................
-00037610: 3e26 0000 2401 0000 b495 0000 0000 0000  >&..$...........
+00037610: 3026 0000 2401 0000 b495 0000 0000 0000  0&..$...........
 00037620: 0100 0000 2400 0000 cc00 0000 0000 0000  ....$...........
 00037630: 0100 0000 4e01 0000 b495 0000 0000 0000  ....N...........
 00037640: 0100 0000 2e01 0000 8096 0000 0000 0000  ................
-00037650: 4b26 0000 2401 0000 8096 0000 0000 0000  K&..$...........
+00037650: 3d26 0000 2401 0000 8096 0000 0000 0000  =&..$...........
 00037660: 0100 0000 2400 0000 d900 0000 0000 0000  ....$...........
 00037670: 0100 0000 4e01 0000 8096 0000 0000 0000  ....N...........
 00037680: 0100 0000 2e01 0000 5997 0000 0000 0000  ........Y.......
-00037690: 5a26 0000 2401 0000 5997 0000 0000 0000  Z&..$...Y.......
+00037690: 4c26 0000 2401 0000 5997 0000 0000 0000  L&..$...Y.......
 000376a0: 0100 0000 2400 0000 4104 0000 0000 0000  ....$...A.......
 000376b0: 0100 0000 4e01 0000 5997 0000 0000 0000  ....N...Y.......
 000376c0: 0100 0000 2e01 0000 9a9b 0000 0000 0000  ................
-000376d0: 6626 0000 2401 0000 9a9b 0000 0000 0000  f&..$...........
+000376d0: 5826 0000 2401 0000 9a9b 0000 0000 0000  X&..$...........
 000376e0: 0100 0000 2400 0000 6f03 0000 0000 0000  ....$...o.......
 000376f0: 0100 0000 4e01 0000 9a9b 0000 0000 0000  ....N...........
 00037700: 0100 0000 2e01 0000 099f 0000 0000 0000  ................
-00037710: 7426 0000 2401 0000 099f 0000 0000 0000  t&..$...........
+00037710: 6626 0000 2401 0000 099f 0000 0000 0000  f&..$...........
 00037720: 0100 0000 2400 0000 0e01 0000 0000 0000  ....$...........
 00037730: 0100 0000 4e01 0000 099f 0000 0000 0000  ....N...........
 00037740: 0100 0000 2e01 0000 17a0 0000 0000 0000  ................
-00037750: 7f26 0000 2401 0000 17a0 0000 0000 0000  .&..$...........
+00037750: 7126 0000 2401 0000 17a0 0000 0000 0000  q&..$...........
 00037760: 0100 0000 2400 0000 2a01 0000 0000 0000  ....$...*.......
 00037770: 0100 0000 4e01 0000 17a0 0000 0000 0000  ....N...........
 00037780: 0100 0000 2e01 0000 41a1 0000 0000 0000  ........A.......
-00037790: 9026 0000 2401 0000 41a1 0000 0000 0000  .&..$...A.......
+00037790: 8226 0000 2401 0000 41a1 0000 0000 0000  .&..$...A.......
 000377a0: 0100 0000 2400 0000 1401 0000 0000 0000  ....$...........
 000377b0: 0100 0000 4e01 0000 41a1 0000 0000 0000  ....N...A.......
 000377c0: 0100 0000 2e01 0000 55a2 0000 0000 0000  ........U.......
-000377d0: 9e26 0000 2401 0000 55a2 0000 0000 0000  .&..$...U.......
+000377d0: 9026 0000 2401 0000 55a2 0000 0000 0000  .&..$...U.......
 000377e0: 0100 0000 2400 0000 af00 0000 0000 0000  ....$...........
 000377f0: 0100 0000 4e01 0000 55a2 0000 0000 0000  ....N...U.......
 00037800: 0100 0000 2e01 0000 04a3 0000 0000 0000  ................
-00037810: b026 0000 2401 0000 04a3 0000 0000 0000  .&..$...........
+00037810: a226 0000 2401 0000 04a3 0000 0000 0000  .&..$...........
 00037820: 0100 0000 2400 0000 4601 0000 0000 0000  ....$...F.......
 00037830: 0100 0000 4e01 0000 04a3 0000 0000 0000  ....N...........
 00037840: 0100 0000 2e01 0000 4aa4 0000 0000 0000  ........J.......
-00037850: be26 0000 2401 0000 4aa4 0000 0000 0000  .&..$...J.......
+00037850: b026 0000 2401 0000 4aa4 0000 0000 0000  .&..$...J.......
 00037860: 0100 0000 2400 0000 3105 0000 0000 0000  ....$...1.......
 00037870: 0100 0000 4e01 0000 4aa4 0000 0000 0000  ....N...J.......
-00037880: d626 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
-00037890: e026 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
-000378a0: f226 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
+00037880: c826 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
+00037890: d226 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
+000378a0: e426 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
 000378b0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-000378c0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-000378d0: 0227 0000 6400 0000 0000 0000 0000 0000  .'..d...........
-000378e0: 0c27 0000 6603 0100 8735 3864 0000 0000  .'..f....58d....
+000378c0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+000378d0: f426 0000 6400 0000 0000 0000 0000 0000  .&..d...........
+000378e0: fe26 0000 6603 0100 beb1 3d64 0000 0000  .&..f.....=d....
 000378f0: 0100 0000 2e01 0000 7ca9 0000 0000 0000  ........|.......
-00037900: a127 0000 2401 0000 7ca9 0000 0000 0000  .'..$...|.......
+00037900: 9327 0000 2401 0000 7ca9 0000 0000 0000  .'..$...|.......
 00037910: 0100 0000 2400 0000 6f00 0000 0000 0000  ....$...o.......
 00037920: 0100 0000 4e01 0000 7ca9 0000 0000 0000  ....N...|.......
 00037930: 0100 0000 2e01 0000 eba9 0000 0000 0000  ................
-00037940: aa27 0000 2401 0000 eba9 0000 0000 0000  .'..$...........
+00037940: 9c27 0000 2401 0000 eba9 0000 0000 0000  .'..$...........
 00037950: 0100 0000 2400 0000 6e00 0000 0000 0000  ....$...n.......
 00037960: 0100 0000 4e01 0000 eba9 0000 0000 0000  ....N...........
 00037970: 0100 0000 2e01 0000 59aa 0000 0000 0000  ........Y.......
-00037980: b827 0000 2401 0000 59aa 0000 0000 0000  .'..$...Y.......
+00037980: aa27 0000 2401 0000 59aa 0000 0000 0000  .'..$...Y.......
 00037990: 0100 0000 2400 0000 2400 0000 0000 0000  ....$...$.......
 000379a0: 0100 0000 4e01 0000 59aa 0000 0000 0000  ....N...Y.......
 000379b0: 0100 0000 2e01 0000 7daa 0000 0000 0000  ........}.......
-000379c0: c027 0000 2401 0000 7daa 0000 0000 0000  .'..$...}.......
+000379c0: b227 0000 2401 0000 7daa 0000 0000 0000  .'..$...}.......
 000379d0: 0100 0000 2400 0000 9302 0000 0000 0000  ....$...........
 000379e0: 0100 0000 4e01 0000 7daa 0000 0000 0000  ....N...}.......
 000379f0: 0100 0000 2e01 0000 10ad 0000 0000 0000  ................
-00037a00: ca27 0000 2401 0000 10ad 0000 0000 0000  .'..$...........
+00037a00: bc27 0000 2401 0000 10ad 0000 0000 0000  .'..$...........
 00037a10: 0100 0000 2400 0000 9600 0000 0000 0000  ....$...........
 00037a20: 0100 0000 4e01 0000 10ad 0000 0000 0000  ....N...........
 00037a30: 0100 0000 2e01 0000 a6ad 0000 0000 0000  ................
-00037a40: d327 0000 2401 0000 a6ad 0000 0000 0000  .'..$...........
+00037a40: c527 0000 2401 0000 a6ad 0000 0000 0000  .'..$...........
 00037a50: 0100 0000 2400 0000 6700 0000 0000 0000  ....$...g.......
 00037a60: 0100 0000 4e01 0000 a6ad 0000 0000 0000  ....N...........
 00037a70: 0100 0000 2e01 0000 0dae 0000 0000 0000  ................
-00037a80: e027 0000 2401 0000 0dae 0000 0000 0000  .'..$...........
+00037a80: d227 0000 2401 0000 0dae 0000 0000 0000  .'..$...........
 00037a90: 0100 0000 2400 0000 0b01 0000 0000 0000  ....$...........
 00037aa0: 0100 0000 4e01 0000 0dae 0000 0000 0000  ....N...........
 00037ab0: 0100 0000 2e01 0000 18af 0000 0000 0000  ................
-00037ac0: ed27 0000 2401 0000 18af 0000 0000 0000  .'..$...........
+00037ac0: df27 0000 2401 0000 18af 0000 0000 0000  .'..$...........
 00037ad0: 0100 0000 2400 0000 7100 0000 0000 0000  ....$...q.......
 00037ae0: 0100 0000 4e01 0000 18af 0000 0000 0000  ....N...........
 00037af0: 0100 0000 2e01 0000 89af 0000 0000 0000  ................
-00037b00: fa27 0000 2401 0000 89af 0000 0000 0000  .'..$...........
+00037b00: ec27 0000 2401 0000 89af 0000 0000 0000  .'..$...........
 00037b10: 0100 0000 2400 0000 4b00 0000 0000 0000  ....$...K.......
 00037b20: 0100 0000 4e01 0000 89af 0000 0000 0000  ....N...........
 00037b30: 0100 0000 2e01 0000 d4af 0000 0000 0000  ................
-00037b40: 0928 0000 2401 0000 d4af 0000 0000 0000  .(..$...........
+00037b40: fb27 0000 2401 0000 d4af 0000 0000 0000  .'..$...........
 00037b50: 0100 0000 2400 0000 7a00 0000 0000 0000  ....$...z.......
 00037b60: 0100 0000 4e01 0000 d4af 0000 0000 0000  ....N...........
 00037b70: 0100 0000 2e01 0000 4eb0 0000 0000 0000  ........N.......
-00037b80: 1828 0000 2401 0000 4eb0 0000 0000 0000  .(..$...N.......
+00037b80: 0a28 0000 2401 0000 4eb0 0000 0000 0000  .(..$...N.......
 00037b90: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 00037ba0: 0100 0000 4e01 0000 4eb0 0000 0000 0000  ....N...N.......
 00037bb0: 0100 0000 2e01 0000 b1b0 0000 0000 0000  ................
-00037bc0: 2b28 0000 2401 0000 b1b0 0000 0000 0000  +(..$...........
+00037bc0: 1d28 0000 2401 0000 b1b0 0000 0000 0000  .(..$...........
 00037bd0: 0100 0000 2400 0000 1f00 0000 0000 0000  ....$...........
 00037be0: 0100 0000 4e01 0000 b1b0 0000 0000 0000  ....N...........
 00037bf0: 0100 0000 2e01 0000 d0b0 0000 0000 0000  ................
-00037c00: 3d28 0000 2401 0000 d0b0 0000 0000 0000  =(..$...........
+00037c00: 2f28 0000 2401 0000 d0b0 0000 0000 0000  /(..$...........
 00037c10: 0100 0000 2400 0000 d600 0000 0000 0000  ....$...........
 00037c20: 0100 0000 4e01 0000 d0b0 0000 0000 0000  ....N...........
 00037c30: 0100 0000 2e01 0000 a6b1 0000 0000 0000  ................
-00037c40: 4e28 0000 2401 0000 a6b1 0000 0000 0000  N(..$...........
+00037c40: 4028 0000 2401 0000 a6b1 0000 0000 0000  @(..$...........
 00037c50: 0100 0000 2400 0000 7e00 0000 0000 0000  ....$...~.......
 00037c60: 0100 0000 4e01 0000 a6b1 0000 0000 0000  ....N...........
 00037c70: 0100 0000 2e01 0000 24b2 0000 0000 0000  ........$.......
-00037c80: 6628 0000 2401 0000 24b2 0000 0000 0000  f(..$...$.......
+00037c80: 5828 0000 2401 0000 24b2 0000 0000 0000  X(..$...$.......
 00037c90: 0100 0000 2400 0000 af00 0000 0000 0000  ....$...........
 00037ca0: 0100 0000 4e01 0000 24b2 0000 0000 0000  ....N...$.......
 00037cb0: 0100 0000 2e01 0000 d3b2 0000 0000 0000  ................
-00037cc0: 7428 0000 2401 0000 d3b2 0000 0000 0000  t(..$...........
+00037cc0: 6628 0000 2401 0000 d3b2 0000 0000 0000  f(..$...........
 00037cd0: 0100 0000 2400 0000 1100 0000 0000 0000  ....$...........
 00037ce0: 0100 0000 4e01 0000 d3b2 0000 0000 0000  ....N...........
 00037cf0: 0100 0000 2e01 0000 e4b2 0000 0000 0000  ................
-00037d00: 8628 0000 2401 0000 e4b2 0000 0000 0000  .(..$...........
+00037d00: 7828 0000 2401 0000 e4b2 0000 0000 0000  x(..$...........
 00037d10: 0100 0000 2400 0000 4e00 0000 0000 0000  ....$...N.......
 00037d20: 0100 0000 4e01 0000 e4b2 0000 0000 0000  ....N...........
 00037d30: 0100 0000 2e01 0000 32b3 0000 0000 0000  ........2.......
-00037d40: 9828 0000 2401 0000 32b3 0000 0000 0000  .(..$...2.......
+00037d40: 8a28 0000 2401 0000 32b3 0000 0000 0000  .(..$...2.......
 00037d50: 0100 0000 2400 0000 1300 0000 0000 0000  ....$...........
 00037d60: 0100 0000 4e01 0000 32b3 0000 0000 0000  ....N...2.......
 00037d70: 0100 0000 2e01 0000 45b3 0000 0000 0000  ........E.......
-00037d80: a928 0000 2401 0000 45b3 0000 0000 0000  .(..$...E.......
+00037d80: 9b28 0000 2401 0000 45b3 0000 0000 0000  .(..$...E.......
 00037d90: 0100 0000 2400 0000 f200 0000 0000 0000  ....$...........
 00037da0: 0100 0000 4e01 0000 45b3 0000 0000 0000  ....N...E.......
 00037db0: 0100 0000 2e01 0000 37b4 0000 0000 0000  ........7.......
-00037dc0: b828 0000 2401 0000 37b4 0000 0000 0000  .(..$...7.......
+00037dc0: aa28 0000 2401 0000 37b4 0000 0000 0000  .(..$...7.......
 00037dd0: 0100 0000 2400 0000 5e00 0000 0000 0000  ....$...^.......
 00037de0: 0100 0000 4e01 0000 37b4 0000 0000 0000  ....N...7.......
 00037df0: 0100 0000 2e01 0000 95b4 0000 0000 0000  ................
-00037e00: cf28 0000 2401 0000 95b4 0000 0000 0000  .(..$...........
+00037e00: c128 0000 2401 0000 95b4 0000 0000 0000  .(..$...........
 00037e10: 0100 0000 2400 0000 9702 0000 0000 0000  ....$...........
 00037e20: 0100 0000 4e01 0000 95b4 0000 0000 0000  ....N...........
 00037e30: 0100 0000 2e01 0000 2cb7 0000 0000 0000  ........,.......
-00037e40: e128 0000 2401 0000 2cb7 0000 0000 0000  .(..$...,.......
+00037e40: d328 0000 2401 0000 2cb7 0000 0000 0000  .(..$...,.......
 00037e50: 0100 0000 2400 0000 6302 0000 0000 0000  ....$...c.......
 00037e60: 0100 0000 4e01 0000 2cb7 0000 0000 0000  ....N...,.......
 00037e70: 0100 0000 2e01 0000 8fb9 0000 0000 0000  ................
-00037e80: f728 0000 2401 0000 8fb9 0000 0000 0000  .(..$...........
+00037e80: e928 0000 2401 0000 8fb9 0000 0000 0000  .(..$...........
 00037e90: 0100 0000 2400 0000 a000 0000 0000 0000  ....$...........
 00037ea0: 0100 0000 4e01 0000 8fb9 0000 0000 0000  ....N...........
 00037eb0: 0100 0000 2e01 0000 2fba 0000 0000 0000  ......../.......
-00037ec0: 0029 0000 2401 0000 2fba 0000 0000 0000  .)..$.../.......
+00037ec0: f228 0000 2401 0000 2fba 0000 0000 0000  .(..$.../.......
 00037ed0: 0100 0000 2400 0000 1f00 0000 0000 0000  ....$...........
 00037ee0: 0100 0000 4e01 0000 2fba 0000 0000 0000  ....N.../.......
 00037ef0: 0100 0000 2e01 0000 4eba 0000 0000 0000  ........N.......
-00037f00: 1329 0000 2401 0000 4eba 0000 0000 0000  .)..$...N.......
+00037f00: 0529 0000 2401 0000 4eba 0000 0000 0000  .)..$...N.......
 00037f10: 0100 0000 2400 0000 3800 0000 0000 0000  ....$...8.......
 00037f20: 0100 0000 4e01 0000 4eba 0000 0000 0000  ....N...N.......
 00037f30: 0100 0000 2e01 0000 86ba 0000 0000 0000  ................
-00037f40: 2529 0000 2401 0000 86ba 0000 0000 0000  %)..$...........
+00037f40: 1729 0000 2401 0000 86ba 0000 0000 0000  .)..$...........
 00037f50: 0100 0000 2400 0000 a600 0000 0000 0000  ....$...........
 00037f60: 0100 0000 4e01 0000 86ba 0000 0000 0000  ....N...........
 00037f70: 0100 0000 2e01 0000 2cbb 0000 0000 0000  ........,.......
-00037f80: 3129 0000 2401 0000 2cbb 0000 0000 0000  1)..$...,.......
+00037f80: 2329 0000 2401 0000 2cbb 0000 0000 0000  #)..$...,.......
 00037f90: 0100 0000 2400 0000 4b00 0000 0000 0000  ....$...K.......
 00037fa0: 0100 0000 4e01 0000 2cbb 0000 0000 0000  ....N...,.......
 00037fb0: 0100 0000 2e01 0000 77bb 0000 0000 0000  ........w.......
-00037fc0: 4129 0000 2401 0000 77bb 0000 0000 0000  A)..$...w.......
+00037fc0: 3329 0000 2401 0000 77bb 0000 0000 0000  3)..$...w.......
 00037fd0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 00037fe0: 0100 0000 4e01 0000 77bb 0000 0000 0000  ....N...w.......
 00037ff0: 0100 0000 2e01 0000 81bb 0000 0000 0000  ................
-00038000: 4b29 0000 2401 0000 81bb 0000 0000 0000  K)..$...........
+00038000: 3d29 0000 2401 0000 81bb 0000 0000 0000  =)..$...........
 00038010: 0100 0000 2400 0000 ee00 0000 0000 0000  ....$...........
 00038020: 0100 0000 4e01 0000 81bb 0000 0000 0000  ....N...........
 00038030: 0100 0000 2e01 0000 6fbc 0000 0000 0000  ........o.......
-00038040: 5529 0000 2401 0000 6fbc 0000 0000 0000  U)..$...o.......
+00038040: 4729 0000 2401 0000 6fbc 0000 0000 0000  G)..$...o.......
 00038050: 0100 0000 2400 0000 8d06 0000 0000 0000  ....$...........
 00038060: 0100 0000 4e01 0000 6fbc 0000 0000 0000  ....N...o.......
 00038070: 0100 0000 2e01 0000 fcc2 0000 0000 0000  ................
-00038080: 5f29 0000 2401 0000 fcc2 0000 0000 0000  _)..$...........
+00038080: 5129 0000 2401 0000 fcc2 0000 0000 0000  Q)..$...........
 00038090: 0100 0000 2400 0000 e804 0000 0000 0000  ....$...........
 000380a0: 0100 0000 4e01 0000 fcc2 0000 0000 0000  ....N...........
 000380b0: 0100 0000 2e01 0000 e4c7 0000 0000 0000  ................
-000380c0: 7129 0000 2401 0000 e4c7 0000 0000 0000  q)..$...........
+000380c0: 6329 0000 2401 0000 e4c7 0000 0000 0000  c)..$...........
 000380d0: 0100 0000 2400 0000 1f01 0000 0000 0000  ....$...........
 000380e0: 0100 0000 4e01 0000 e4c7 0000 0000 0000  ....N...........
 000380f0: 0100 0000 2e01 0000 03c9 0000 0000 0000  ................
-00038100: 8229 0000 2401 0000 03c9 0000 0000 0000  .)..$...........
+00038100: 7429 0000 2401 0000 03c9 0000 0000 0000  t)..$...........
 00038110: 0100 0000 2400 0000 8400 0000 0000 0000  ....$...........
 00038120: 0100 0000 4e01 0000 03c9 0000 0000 0000  ....N...........
 00038130: 0100 0000 2e01 0000 87c9 0000 0000 0000  ................
-00038140: 9029 0000 2401 0000 87c9 0000 0000 0000  .)..$...........
+00038140: 8229 0000 2401 0000 87c9 0000 0000 0000  .)..$...........
 00038150: 0100 0000 2400 0000 9300 0000 0000 0000  ....$...........
 00038160: 0100 0000 4e01 0000 87c9 0000 0000 0000  ....N...........
 00038170: 0100 0000 2e01 0000 1aca 0000 0000 0000  ................
-00038180: a029 0000 2401 0000 1aca 0000 0000 0000  .)..$...........
+00038180: 9229 0000 2401 0000 1aca 0000 0000 0000  .)..$...........
 00038190: 0100 0000 2400 0000 9a01 0000 0000 0000  ....$...........
 000381a0: 0100 0000 4e01 0000 1aca 0000 0000 0000  ....N...........
 000381b0: 0100 0000 2e01 0000 b4cb 0000 0000 0000  ................
-000381c0: ab29 0000 2401 0000 b4cb 0000 0000 0000  .)..$...........
+000381c0: 9d29 0000 2401 0000 b4cb 0000 0000 0000  .)..$...........
 000381d0: 0100 0000 2400 0000 bc01 0000 0000 0000  ....$...........
 000381e0: 0100 0000 4e01 0000 b4cb 0000 0000 0000  ....N...........
 000381f0: 0100 0000 2e01 0000 70cd 0000 0000 0000  ........p.......
-00038200: b729 0000 2401 0000 70cd 0000 0000 0000  .)..$...p.......
+00038200: a929 0000 2401 0000 70cd 0000 0000 0000  .)..$...p.......
 00038210: 0100 0000 2400 0000 4200 0000 0000 0000  ....$...B.......
 00038220: 0100 0000 4e01 0000 70cd 0000 0000 0000  ....N...p.......
 00038230: 0100 0000 2e01 0000 b2cd 0000 0000 0000  ................
-00038240: cb29 0000 2401 0000 b2cd 0000 0000 0000  .)..$...........
+00038240: bd29 0000 2401 0000 b2cd 0000 0000 0000  .)..$...........
 00038250: 0100 0000 2400 0000 6200 0000 0000 0000  ....$...b.......
 00038260: 0100 0000 4e01 0000 b2cd 0000 0000 0000  ....N...........
 00038270: 0100 0000 2e01 0000 14ce 0000 0000 0000  ................
-00038280: dd29 0000 2401 0000 14ce 0000 0000 0000  .)..$...........
+00038280: cf29 0000 2401 0000 14ce 0000 0000 0000  .)..$...........
 00038290: 0100 0000 2400 0000 c402 0000 0000 0000  ....$...........
 000382a0: 0100 0000 4e01 0000 14ce 0000 0000 0000  ....N...........
 000382b0: 0100 0000 2e01 0000 d8d0 0000 0000 0000  ................
-000382c0: e729 0000 2401 0000 d8d0 0000 0000 0000  .)..$...........
+000382c0: d929 0000 2401 0000 d8d0 0000 0000 0000  .)..$...........
 000382d0: 0100 0000 2400 0000 cc00 0000 0000 0000  ....$...........
 000382e0: 0100 0000 4e01 0000 d8d0 0000 0000 0000  ....N...........
 000382f0: 0100 0000 2e01 0000 a4d1 0000 0000 0000  ................
-00038300: f729 0000 2401 0000 a4d1 0000 0000 0000  .)..$...........
+00038300: e929 0000 2401 0000 a4d1 0000 0000 0000  .)..$...........
 00038310: 0100 0000 2400 0000 3802 0000 0000 0000  ....$...8.......
 00038320: 0100 0000 4e01 0000 a4d1 0000 0000 0000  ....N...........
 00038330: 0100 0000 2e01 0000 dcd3 0000 0000 0000  ................
-00038340: 032a 0000 2401 0000 dcd3 0000 0000 0000  .*..$...........
+00038340: f529 0000 2401 0000 dcd3 0000 0000 0000  .)..$...........
 00038350: 0100 0000 2400 0000 f701 0000 0000 0000  ....$...........
 00038360: 0100 0000 4e01 0000 dcd3 0000 0000 0000  ....N...........
 00038370: 0100 0000 2e01 0000 d3d5 0000 0000 0000  ................
-00038380: 0e2a 0000 2401 0000 d3d5 0000 0000 0000  .*..$...........
+00038380: 002a 0000 2401 0000 d3d5 0000 0000 0000  .*..$...........
 00038390: 0100 0000 2400 0000 4d01 0000 0000 0000  ....$...M.......
 000383a0: 0100 0000 4e01 0000 d3d5 0000 0000 0000  ....N...........
 000383b0: 0100 0000 2e01 0000 20d7 0000 0000 0000  ........ .......
-000383c0: 202a 0000 2401 0000 20d7 0000 0000 0000   *..$... .......
+000383c0: 122a 0000 2401 0000 20d7 0000 0000 0000  .*..$... .......
 000383d0: 0100 0000 2400 0000 6c01 0000 0000 0000  ....$...l.......
 000383e0: 0100 0000 4e01 0000 20d7 0000 0000 0000  ....N... .......
 000383f0: 0100 0000 2e01 0000 8cd8 0000 0000 0000  ................
-00038400: 2f2a 0000 2401 0000 8cd8 0000 0000 0000  /*..$...........
+00038400: 212a 0000 2401 0000 8cd8 0000 0000 0000  !*..$...........
 00038410: 0100 0000 2400 0000 3f01 0000 0000 0000  ....$...?.......
 00038420: 0100 0000 4e01 0000 8cd8 0000 0000 0000  ....N...........
 00038430: 0100 0000 2e01 0000 cbd9 0000 0000 0000  ................
-00038440: 382a 0000 2401 0000 cbd9 0000 0000 0000  8*..$...........
+00038440: 2a2a 0000 2401 0000 cbd9 0000 0000 0000  **..$...........
 00038450: 0100 0000 2400 0000 9202 0000 0000 0000  ....$...........
 00038460: 0100 0000 4e01 0000 cbd9 0000 0000 0000  ....N...........
 00038470: 0100 0000 2e01 0000 5ddc 0000 0000 0000  ........].......
-00038480: 432a 0000 2401 0000 5ddc 0000 0000 0000  C*..$...].......
+00038480: 352a 0000 2401 0000 5ddc 0000 0000 0000  5*..$...].......
 00038490: 0100 0000 2400 0000 e300 0000 0000 0000  ....$...........
 000384a0: 0100 0000 4e01 0000 5ddc 0000 0000 0000  ....N...].......
 000384b0: 0100 0000 2e01 0000 40dd 0000 0000 0000  ........@.......
-000384c0: 512a 0000 2401 0000 40dd 0000 0000 0000  Q*..$...@.......
+000384c0: 432a 0000 2401 0000 40dd 0000 0000 0000  C*..$...@.......
 000384d0: 0100 0000 2400 0000 b006 0000 0000 0000  ....$...........
 000384e0: 0100 0000 4e01 0000 40dd 0000 0000 0000  ....N...@.......
 000384f0: 0100 0000 2e01 0000 f0e3 0000 0000 0000  ................
-00038500: 5e2a 0000 2401 0000 f0e3 0000 0000 0000  ^*..$...........
+00038500: 502a 0000 2401 0000 f0e3 0000 0000 0000  P*..$...........
 00038510: 0100 0000 2400 0000 3a00 0000 0000 0000  ....$...:.......
 00038520: 0100 0000 4e01 0000 f0e3 0000 0000 0000  ....N...........
 00038530: 0100 0000 2e01 0000 2ae4 0000 0000 0000  ........*.......
-00038540: 6f2a 0000 2401 0000 2ae4 0000 0000 0000  o*..$...*.......
+00038540: 612a 0000 2401 0000 2ae4 0000 0000 0000  a*..$...*.......
 00038550: 0100 0000 2400 0000 4b01 0000 0000 0000  ....$...K.......
 00038560: 0100 0000 4e01 0000 2ae4 0000 0000 0000  ....N...*.......
 00038570: 0100 0000 2e01 0000 75e5 0000 0000 0000  ........u.......
-00038580: 822a 0000 2401 0000 75e5 0000 0000 0000  .*..$...u.......
+00038580: 742a 0000 2401 0000 75e5 0000 0000 0000  t*..$...u.......
 00038590: 0100 0000 2400 0000 5d04 0000 0000 0000  ....$...].......
 000385a0: 0100 0000 4e01 0000 75e5 0000 0000 0000  ....N...u.......
 000385b0: 0100 0000 2e01 0000 d2e9 0000 0000 0000  ................
-000385c0: 932a 0000 2401 0000 d2e9 0000 0000 0000  .*..$...........
+000385c0: 852a 0000 2401 0000 d2e9 0000 0000 0000  .*..$...........
 000385d0: 0100 0000 2400 0000 8605 0000 0000 0000  ....$...........
 000385e0: 0100 0000 4e01 0000 d2e9 0000 0000 0000  ....N...........
-000385f0: a42a 0000 2604 0000 307a 0200 0000 0000  .*..&...0z......
-00038600: ac2a 0000 2000 0000 0000 0000 0000 0000  .*.. ...........
-00038610: b62a 0000 2000 0000 0000 0000 0000 0000  .*.. ...........
+000385f0: 962a 0000 2604 0000 307a 0200 0000 0000  .*..&...0z......
+00038600: 9e2a 0000 2000 0000 0000 0000 0000 0000  .*.. ...........
+00038610: a82a 0000 2000 0000 0000 0000 0000 0000  .*.. ...........
 00038620: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00038630: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00038640: c22a 0000 6400 0000 0000 0000 0000 0000  .*..d...........
-00038650: ca2a 0000 6603 0100 8735 3864 0000 0000  .*..f....58d....
+00038630: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00038640: b42a 0000 6400 0000 0000 0000 0000 0000  .*..d...........
+00038650: bc2a 0000 6603 0100 beb1 3d64 0000 0000  .*..f.....=d....
 00038660: 0100 0000 2e01 0000 58ef 0000 0000 0000  ........X.......
-00038670: 5d2b 0000 2401 0000 58ef 0000 0000 0000  ]+..$...X.......
+00038670: 4f2b 0000 2401 0000 58ef 0000 0000 0000  O+..$...X.......
 00038680: 0100 0000 2400 0000 5100 0000 0000 0000  ....$...Q.......
 00038690: 0100 0000 4e01 0000 58ef 0000 0000 0000  ....N...X.......
 000386a0: 0100 0000 2e01 0000 a9ef 0000 0000 0000  ................
-000386b0: 682b 0000 2401 0000 a9ef 0000 0000 0000  h+..$...........
+000386b0: 5a2b 0000 2401 0000 a9ef 0000 0000 0000  Z+..$...........
 000386c0: 0100 0000 2400 0000 c600 0000 0000 0000  ....$...........
 000386d0: 0100 0000 4e01 0000 a9ef 0000 0000 0000  ....N...........
 000386e0: 0100 0000 2e01 0000 6ff0 0000 0000 0000  ........o.......
-000386f0: 732b 0000 2401 0000 6ff0 0000 0000 0000  s+..$...o.......
+000386f0: 652b 0000 2401 0000 6ff0 0000 0000 0000  e+..$...o.......
 00038700: 0100 0000 2400 0000 7b00 0000 0000 0000  ....$...{.......
 00038710: 0100 0000 4e01 0000 6ff0 0000 0000 0000  ....N...o.......
 00038720: 0100 0000 2e01 0000 eaf0 0000 0000 0000  ................
-00038730: 842b 0000 2401 0000 eaf0 0000 0000 0000  .+..$...........
+00038730: 762b 0000 2401 0000 eaf0 0000 0000 0000  v+..$...........
 00038740: 0100 0000 2400 0000 0d03 0000 0000 0000  ....$...........
 00038750: 0100 0000 4e01 0000 eaf0 0000 0000 0000  ....N...........
 00038760: 0100 0000 2e01 0000 f7f3 0000 0000 0000  ................
-00038770: 942b 0000 2401 0000 f7f3 0000 0000 0000  .+..$...........
+00038770: 862b 0000 2401 0000 f7f3 0000 0000 0000  .+..$...........
 00038780: 0100 0000 2400 0000 f200 0000 0000 0000  ....$...........
 00038790: 0100 0000 4e01 0000 f7f3 0000 0000 0000  ....N...........
 000387a0: 0100 0000 2e01 0000 e9f4 0000 0000 0000  ................
-000387b0: a72b 0000 2401 0000 e9f4 0000 0000 0000  .+..$...........
+000387b0: 992b 0000 2401 0000 e9f4 0000 0000 0000  .+..$...........
 000387c0: 0100 0000 2400 0000 ce00 0000 0000 0000  ....$...........
 000387d0: 0100 0000 4e01 0000 e9f4 0000 0000 0000  ....N...........
 000387e0: 0100 0000 2e01 0000 b7f5 0000 0000 0000  ................
-000387f0: b72b 0000 2401 0000 b7f5 0000 0000 0000  .+..$...........
+000387f0: a92b 0000 2401 0000 b7f5 0000 0000 0000  .+..$...........
 00038800: 0100 0000 2400 0000 0800 0000 0000 0000  ....$...........
 00038810: 0100 0000 4e01 0000 b7f5 0000 0000 0000  ....N...........
 00038820: 0100 0000 2e01 0000 bff5 0000 0000 0000  ................
-00038830: cf2b 0000 2401 0000 bff5 0000 0000 0000  .+..$...........
+00038830: c12b 0000 2401 0000 bff5 0000 0000 0000  .+..$...........
 00038840: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 00038850: 0100 0000 4e01 0000 bff5 0000 0000 0000  ....N...........
 00038860: 0100 0000 2e01 0000 c9f5 0000 0000 0000  ................
-00038870: e42b 0000 2401 0000 c9f5 0000 0000 0000  .+..$...........
+00038870: d62b 0000 2401 0000 c9f5 0000 0000 0000  .+..$...........
 00038880: 0100 0000 2400 0000 7000 0000 0000 0000  ....$...p.......
 00038890: 0100 0000 4e01 0000 c9f5 0000 0000 0000  ....N...........
 000388a0: 0100 0000 2e01 0000 39f6 0000 0000 0000  ........9.......
-000388b0: fa2b 0000 2401 0000 39f6 0000 0000 0000  .+..$...9.......
+000388b0: ec2b 0000 2401 0000 39f6 0000 0000 0000  .+..$...9.......
 000388c0: 0100 0000 2400 0000 7700 0000 0000 0000  ....$...w.......
 000388d0: 0100 0000 4e01 0000 39f6 0000 0000 0000  ....N...9.......
 000388e0: 0100 0000 2e01 0000 b0f6 0000 0000 0000  ................
-000388f0: 082c 0000 2401 0000 b0f6 0000 0000 0000  .,..$...........
+000388f0: fa2b 0000 2401 0000 b0f6 0000 0000 0000  .+..$...........
 00038900: 0100 0000 2400 0000 a700 0000 0000 0000  ....$...........
 00038910: 0100 0000 4e01 0000 b0f6 0000 0000 0000  ....N...........
 00038920: 0100 0000 2e01 0000 57f7 0000 0000 0000  ........W.......
-00038930: 182c 0000 2401 0000 57f7 0000 0000 0000  .,..$...W.......
+00038930: 0a2c 0000 2401 0000 57f7 0000 0000 0000  .,..$...W.......
 00038940: 0100 0000 2400 0000 dd00 0000 0000 0000  ....$...........
 00038950: 0100 0000 4e01 0000 57f7 0000 0000 0000  ....N...W.......
 00038960: 0100 0000 2e01 0000 34f8 0000 0000 0000  ........4.......
-00038970: 2a2c 0000 2401 0000 34f8 0000 0000 0000  *,..$...4.......
+00038970: 1c2c 0000 2401 0000 34f8 0000 0000 0000  .,..$...4.......
 00038980: 0100 0000 2400 0000 7c10 0000 0000 0000  ....$...|.......
 00038990: 0100 0000 4e01 0000 34f8 0000 0000 0000  ....N...4.......
 000389a0: 0100 0000 2e01 0000 b008 0100 0000 0000  ................
-000389b0: 382c 0000 2401 0000 b008 0100 0000 0000  8,..$...........
+000389b0: 2a2c 0000 2401 0000 b008 0100 0000 0000  *,..$...........
 000389c0: 0100 0000 2400 0000 3900 0000 0000 0000  ....$...9.......
 000389d0: 0100 0000 4e01 0000 b008 0100 0000 0000  ....N...........
 000389e0: 0100 0000 2e01 0000 e908 0100 0000 0000  ................
-000389f0: 4a2c 0000 2401 0000 e908 0100 0000 0000  J,..$...........
+000389f0: 3c2c 0000 2401 0000 e908 0100 0000 0000  <,..$...........
 00038a00: 0100 0000 2400 0000 6f02 0000 0000 0000  ....$...o.......
 00038a10: 0100 0000 4e01 0000 e908 0100 0000 0000  ....N...........
 00038a20: 0100 0000 2e01 0000 580b 0100 0000 0000  ........X.......
-00038a30: 5a2c 0000 2401 0000 580b 0100 0000 0000  Z,..$...X.......
+00038a30: 4c2c 0000 2401 0000 580b 0100 0000 0000  L,..$...X.......
 00038a40: 0100 0000 2400 0000 9100 0000 0000 0000  ....$...........
 00038a50: 0100 0000 4e01 0000 580b 0100 0000 0000  ....N...X.......
 00038a60: 0100 0000 2e01 0000 e90b 0100 0000 0000  ................
-00038a70: 682c 0000 2401 0000 e90b 0100 0000 0000  h,..$...........
+00038a70: 5a2c 0000 2401 0000 e90b 0100 0000 0000  Z,..$...........
 00038a80: 0100 0000 2400 0000 0c03 0000 0000 0000  ....$...........
 00038a90: 0100 0000 4e01 0000 e90b 0100 0000 0000  ....N...........
 00038aa0: 0100 0000 2e01 0000 f50e 0100 0000 0000  ................
-00038ab0: 7f2c 0000 2401 0000 f50e 0100 0000 0000  .,..$...........
+00038ab0: 712c 0000 2401 0000 f50e 0100 0000 0000  q,..$...........
 00038ac0: 0100 0000 2400 0000 ff03 0000 0000 0000  ....$...........
 00038ad0: 0100 0000 4e01 0000 f50e 0100 0000 0000  ....N...........
 00038ae0: 0100 0000 2e01 0000 f412 0100 0000 0000  ................
-00038af0: 9b2c 0000 2401 0000 f412 0100 0000 0000  .,..$...........
+00038af0: 8d2c 0000 2401 0000 f412 0100 0000 0000  .,..$...........
 00038b00: 0100 0000 2400 0000 4400 0000 0000 0000  ....$...D.......
 00038b10: 0100 0000 4e01 0000 f412 0100 0000 0000  ....N...........
 00038b20: 0100 0000 2e01 0000 3813 0100 0000 0000  ........8.......
-00038b30: a62c 0000 2401 0000 3813 0100 0000 0000  .,..$...8.......
+00038b30: 982c 0000 2401 0000 3813 0100 0000 0000  .,..$...8.......
 00038b40: 0100 0000 2400 0000 5e03 0000 0000 0000  ....$...^.......
 00038b50: 0100 0000 4e01 0000 3813 0100 0000 0000  ....N...8.......
 00038b60: 0100 0000 2e01 0000 9616 0100 0000 0000  ................
-00038b70: bb2c 0000 2401 0000 9616 0100 0000 0000  .,..$...........
+00038b70: ad2c 0000 2401 0000 9616 0100 0000 0000  .,..$...........
 00038b80: 0100 0000 2400 0000 2a01 0000 0000 0000  ....$...*.......
 00038b90: 0100 0000 4e01 0000 9616 0100 0000 0000  ....N...........
 00038ba0: 0100 0000 2e01 0000 c017 0100 0000 0000  ................
-00038bb0: d82c 0000 2401 0000 c017 0100 0000 0000  .,..$...........
+00038bb0: ca2c 0000 2401 0000 c017 0100 0000 0000  .,..$...........
 00038bc0: 0100 0000 2400 0000 9a01 0000 0000 0000  ....$...........
 00038bd0: 0100 0000 4e01 0000 c017 0100 0000 0000  ....N...........
 00038be0: 0100 0000 2e01 0000 5a19 0100 0000 0000  ........Z.......
-00038bf0: ee2c 0000 2401 0000 5a19 0100 0000 0000  .,..$...Z.......
+00038bf0: e02c 0000 2401 0000 5a19 0100 0000 0000  .,..$...Z.......
 00038c00: 0100 0000 2400 0000 c700 0000 0000 0000  ....$...........
 00038c10: 0100 0000 4e01 0000 5a19 0100 0000 0000  ....N...Z.......
 00038c20: 0100 0000 2e01 0000 211a 0100 0000 0000  ........!.......
-00038c30: 052d 0000 2401 0000 211a 0100 0000 0000  .-..$...!.......
+00038c30: f72c 0000 2401 0000 211a 0100 0000 0000  .,..$...!.......
 00038c40: 0100 0000 2400 0000 4201 0000 0000 0000  ....$...B.......
 00038c50: 0100 0000 4e01 0000 211a 0100 0000 0000  ....N...!.......
 00038c60: 0100 0000 2e01 0000 631b 0100 0000 0000  ........c.......
-00038c70: 182d 0000 2401 0000 631b 0100 0000 0000  .-..$...c.......
+00038c70: 0a2d 0000 2401 0000 631b 0100 0000 0000  .-..$...c.......
 00038c80: 0100 0000 2400 0000 9f0e 0000 0000 0000  ....$...........
 00038c90: 0100 0000 4e01 0000 631b 0100 0000 0000  ....N...c.......
 00038ca0: 0100 0000 2e01 0000 022a 0100 0000 0000  .........*......
-00038cb0: 302d 0000 2401 0000 022a 0100 0000 0000  0-..$....*......
+00038cb0: 222d 0000 2401 0000 022a 0100 0000 0000  "-..$....*......
 00038cc0: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 00038cd0: 0100 0000 4e01 0000 022a 0100 0000 0000  ....N....*......
 00038ce0: 0100 0000 2e01 0000 652a 0100 0000 0000  ........e*......
-00038cf0: 452d 0000 2401 0000 652a 0100 0000 0000  E-..$...e*......
+00038cf0: 372d 0000 2401 0000 652a 0100 0000 0000  7-..$...e*......
 00038d00: 0100 0000 2400 0000 f706 0000 0000 0000  ....$...........
 00038d10: 0100 0000 4e01 0000 652a 0100 0000 0000  ....N...e*......
 00038d20: 0100 0000 2e01 0000 5c31 0100 0000 0000  ........\1......
-00038d30: 562d 0000 2401 0000 5c31 0100 0000 0000  V-..$...\1......
+00038d30: 482d 0000 2401 0000 5c31 0100 0000 0000  H-..$...\1......
 00038d40: 0100 0000 2400 0000 6a02 0000 0000 0000  ....$...j.......
 00038d50: 0100 0000 4e01 0000 5c31 0100 0000 0000  ....N...\1......
 00038d60: 0100 0000 2e01 0000 c633 0100 0000 0000  .........3......
-00038d70: 5e2d 0000 2401 0000 c633 0100 0000 0000  ^-..$....3......
+00038d70: 502d 0000 2401 0000 c633 0100 0000 0000  P-..$....3......
 00038d80: 0100 0000 2400 0000 b600 0000 0000 0000  ....$...........
 00038d90: 0100 0000 4e01 0000 c633 0100 0000 0000  ....N....3......
-00038da0: 6f2d 0000 2000 0000 0000 0000 0000 0000  o-.. ...........
-00038db0: 752d 0000 2000 0000 0000 0000 0000 0000  u-.. ...........
-00038dc0: 7f2d 0000 2000 0000 0000 0000 0000 0000  .-.. ...........
+00038da0: 612d 0000 2000 0000 0000 0000 0000 0000  a-.. ...........
+00038db0: 672d 0000 2000 0000 0000 0000 0000 0000  g-.. ...........
+00038dc0: 712d 0000 2000 0000 0000 0000 0000 0000  q-.. ...........
 00038dd0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00038de0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00038df0: 892d 0000 6400 0000 0000 0000 0000 0000  .-..d...........
-00038e00: 912d 0000 6603 0100 8735 3864 0000 0000  .-..f....58d....
+00038de0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00038df0: 7b2d 0000 6400 0000 0000 0000 0000 0000  {-..d...........
+00038e00: 832d 0000 6603 0100 bfb1 3d64 0000 0000  .-..f.....=d....
 00038e10: 0100 0000 2e01 0000 7c34 0100 0000 0000  ........|4......
-00038e20: 242e 0000 2401 0000 7c34 0100 0000 0000  $...$...|4......
+00038e20: 162e 0000 2401 0000 7c34 0100 0000 0000  ....$...|4......
 00038e30: 0100 0000 2400 0000 c808 0000 0000 0000  ....$...........
 00038e40: 0100 0000 4e01 0000 7c34 0100 0000 0000  ....N...|4......
 00038e50: 0100 0000 2e01 0000 443d 0100 0000 0000  ........D=......
-00038e60: 302e 0000 2401 0000 443d 0100 0000 0000  0...$...D=......
+00038e60: 222e 0000 2401 0000 443d 0100 0000 0000  "...$...D=......
 00038e70: 0100 0000 2400 0000 0c00 0000 0000 0000  ....$...........
 00038e80: 0100 0000 4e01 0000 443d 0100 0000 0000  ....N...D=......
 00038e90: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00038ea0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00038eb0: 3b2e 0000 6400 0000 0000 0000 0000 0000  ;...d...........
-00038ec0: 422e 0000 6603 0100 8735 3864 0000 0000  B...f....58d....
+00038ea0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00038eb0: 2d2e 0000 6400 0000 0000 0000 0000 0000  -...d...........
+00038ec0: 342e 0000 6603 0100 bfb1 3d64 0000 0000  4...f.....=d....
 00038ed0: 0100 0000 2e01 0000 503d 0100 0000 0000  ........P=......
-00038ee0: d42e 0000 2401 0000 503d 0100 0000 0000  ....$...P=......
+00038ee0: c62e 0000 2401 0000 503d 0100 0000 0000  ....$...P=......
 00038ef0: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 00038f00: 0100 0000 4e01 0000 503d 0100 0000 0000  ....N...P=......
 00038f10: 0100 0000 2e01 0000 b33d 0100 0000 0000  .........=......
-00038f20: dd2e 0000 2401 0000 b33d 0100 0000 0000  ....$....=......
+00038f20: cf2e 0000 2401 0000 b33d 0100 0000 0000  ....$....=......
 00038f30: 0100 0000 2400 0000 b500 0000 0000 0000  ....$...........
 00038f40: 0100 0000 4e01 0000 b33d 0100 0000 0000  ....N....=......
 00038f50: 0100 0000 2e01 0000 683e 0100 0000 0000  ........h>......
-00038f60: ed2e 0000 2401 0000 683e 0100 0000 0000  ....$...h>......
+00038f60: df2e 0000 2401 0000 683e 0100 0000 0000  ....$...h>......
 00038f70: 0100 0000 2400 0000 1800 0000 0000 0000  ....$...........
 00038f80: 0100 0000 4e01 0000 683e 0100 0000 0000  ....N...h>......
 00038f90: 0100 0000 2e01 0000 803e 0100 0000 0000  .........>......
-00038fa0: fc2e 0000 2401 0000 803e 0100 0000 0000  ....$....>......
+00038fa0: ee2e 0000 2401 0000 803e 0100 0000 0000  ....$....>......
 00038fb0: 0100 0000 2400 0000 de00 0000 0000 0000  ....$...........
 00038fc0: 0100 0000 4e01 0000 803e 0100 0000 0000  ....N....>......
 00038fd0: 0100 0000 2e01 0000 5e3f 0100 0000 0000  ........^?......
-00038fe0: 082f 0000 2401 0000 5e3f 0100 0000 0000  ./..$...^?......
+00038fe0: fa2e 0000 2401 0000 5e3f 0100 0000 0000  ....$...^?......
 00038ff0: 0100 0000 2400 0000 ae00 0000 0000 0000  ....$...........
 00039000: 0100 0000 4e01 0000 5e3f 0100 0000 0000  ....N...^?......
 00039010: 0100 0000 2e01 0000 0c40 0100 0000 0000  .........@......
-00039020: 162f 0000 2401 0000 0c40 0100 0000 0000  ./..$....@......
+00039020: 082f 0000 2401 0000 0c40 0100 0000 0000  ./..$....@......
 00039030: 0100 0000 2400 0000 8700 0000 0000 0000  ....$...........
 00039040: 0100 0000 4e01 0000 0c40 0100 0000 0000  ....N....@......
 00039050: 0100 0000 2e01 0000 9340 0100 0000 0000  .........@......
-00039060: 262f 0000 2401 0000 9340 0100 0000 0000  &/..$....@......
+00039060: 182f 0000 2401 0000 9340 0100 0000 0000  ./..$....@......
 00039070: 0100 0000 2400 0000 3102 0000 0000 0000  ....$...1.......
 00039080: 0100 0000 4e01 0000 9340 0100 0000 0000  ....N....@......
 00039090: 0100 0000 2e01 0000 c442 0100 0000 0000  .........B......
-000390a0: 3b2f 0000 2401 0000 c442 0100 0000 0000  ;/..$....B......
+000390a0: 2d2f 0000 2401 0000 c442 0100 0000 0000  -/..$....B......
 000390b0: 0100 0000 2400 0000 6901 0000 0000 0000  ....$...i.......
 000390c0: 0100 0000 4e01 0000 c442 0100 0000 0000  ....N....B......
 000390d0: 0100 0000 2e01 0000 2d44 0100 0000 0000  ........-D......
-000390e0: 482f 0000 2401 0000 2d44 0100 0000 0000  H/..$...-D......
+000390e0: 3a2f 0000 2401 0000 2d44 0100 0000 0000  :/..$...-D......
 000390f0: 0100 0000 2400 0000 a600 0000 0000 0000  ....$...........
 00039100: 0100 0000 4e01 0000 2d44 0100 0000 0000  ....N...-D......
 00039110: 0100 0000 2e01 0000 d344 0100 0000 0000  .........D......
-00039120: 4f2f 0000 2401 0000 d344 0100 0000 0000  O/..$....D......
+00039120: 412f 0000 2401 0000 d344 0100 0000 0000  A/..$....D......
 00039130: 0100 0000 2400 0000 aa02 0000 0000 0000  ....$...........
 00039140: 0100 0000 4e01 0000 d344 0100 0000 0000  ....N....D......
 00039150: 0100 0000 2e01 0000 7d47 0100 0000 0000  ........}G......
-00039160: 662f 0000 2401 0000 7d47 0100 0000 0000  f/..$...}G......
+00039160: 582f 0000 2401 0000 7d47 0100 0000 0000  X/..$...}G......
 00039170: 0100 0000 2400 0000 0a02 0000 0000 0000  ....$...........
 00039180: 0100 0000 4e01 0000 7d47 0100 0000 0000  ....N...}G......
 00039190: 0100 0000 2e01 0000 8749 0100 0000 0000  .........I......
-000391a0: 7c2f 0000 2401 0000 8749 0100 0000 0000  |/..$....I......
+000391a0: 6e2f 0000 2401 0000 8749 0100 0000 0000  n/..$....I......
 000391b0: 0100 0000 2400 0000 4801 0000 0000 0000  ....$...H.......
 000391c0: 0100 0000 4e01 0000 8749 0100 0000 0000  ....N....I......
 000391d0: 0100 0000 2e01 0000 cf4a 0100 0000 0000  .........J......
-000391e0: 862f 0000 2401 0000 cf4a 0100 0000 0000  ./..$....J......
+000391e0: 782f 0000 2401 0000 cf4a 0100 0000 0000  x/..$....J......
 000391f0: 0100 0000 2400 0000 ad01 0000 0000 0000  ....$...........
 00039200: 0100 0000 4e01 0000 cf4a 0100 0000 0000  ....N....J......
 00039210: 0100 0000 2e01 0000 7c4c 0100 0000 0000  ........|L......
-00039220: 902f 0000 2401 0000 7c4c 0100 0000 0000  ./..$...|L......
+00039220: 822f 0000 2401 0000 7c4c 0100 0000 0000  ./..$...|L......
 00039230: 0100 0000 2400 0000 b400 0000 0000 0000  ....$...........
 00039240: 0100 0000 4e01 0000 7c4c 0100 0000 0000  ....N...|L......
 00039250: 0100 0000 2e01 0000 304d 0100 0000 0000  ........0M......
-00039260: 9a2f 0000 2401 0000 304d 0100 0000 0000  ./..$...0M......
+00039260: 8c2f 0000 2401 0000 304d 0100 0000 0000  ./..$...0M......
 00039270: 0100 0000 2400 0000 b901 0000 0000 0000  ....$...........
 00039280: 0100 0000 4e01 0000 304d 0100 0000 0000  ....N...0M......
 00039290: 0100 0000 2e01 0000 e94e 0100 0000 0000  .........N......
-000392a0: a42f 0000 2401 0000 e94e 0100 0000 0000  ./..$....N......
+000392a0: 962f 0000 2401 0000 e94e 0100 0000 0000  ./..$....N......
 000392b0: 0100 0000 2400 0000 3407 0000 0000 0000  ....$...4.......
 000392c0: 0100 0000 4e01 0000 e94e 0100 0000 0000  ....N....N......
-000392d0: b22f 0000 2000 0000 0000 0000 0000 0000  ./.. ...........
-000392e0: bd2f 0000 2609 0000 00c0 0200 0000 0000  ./..&...........
+000392d0: a42f 0000 2000 0000 0000 0000 0000 0000  ./.. ...........
+000392e0: af2f 0000 2609 0000 00c0 0200 0000 0000  ./..&...........
 000392f0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00039300: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00039310: c32f 0000 6400 0000 0000 0000 0000 0000  ./..d...........
-00039320: cb2f 0000 6603 0100 8835 3864 0000 0000  ./..f....58d....
+00039300: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00039310: b52f 0000 6400 0000 0000 0000 0000 0000  ./..d...........
+00039320: bd2f 0000 6603 0100 bfb1 3d64 0000 0000  ./..f.....=d....
 00039330: 0100 0000 2e01 0000 2056 0100 0000 0000  ........ V......
-00039340: 5e30 0000 2401 0000 2056 0100 0000 0000  ^0..$... V......
+00039340: 5030 0000 2401 0000 2056 0100 0000 0000  P0..$... V......
 00039350: 0100 0000 2400 0000 3700 0000 0000 0000  ....$...7.......
 00039360: 0100 0000 4e01 0000 2056 0100 0000 0000  ....N... V......
 00039370: 0100 0000 2e01 0000 5756 0100 0000 0000  ........WV......
-00039380: 6e30 0000 2401 0000 5756 0100 0000 0000  n0..$...WV......
+00039380: 6030 0000 2401 0000 5756 0100 0000 0000  `0..$...WV......
 00039390: 0100 0000 2400 0000 4500 0000 0000 0000  ....$...E.......
 000393a0: 0100 0000 4e01 0000 5756 0100 0000 0000  ....N...WV......
 000393b0: 0100 0000 2e01 0000 9c56 0100 0000 0000  .........V......
-000393c0: 7c30 0000 2401 0000 9c56 0100 0000 0000  |0..$....V......
+000393c0: 6e30 0000 2401 0000 9c56 0100 0000 0000  n0..$....V......
 000393d0: 0100 0000 2400 0000 eb01 0000 0000 0000  ....$...........
 000393e0: 0100 0000 4e01 0000 9c56 0100 0000 0000  ....N....V......
 000393f0: 0100 0000 2e01 0000 8758 0100 0000 0000  .........X......
-00039400: 8730 0000 2401 0000 8758 0100 0000 0000  .0..$....X......
+00039400: 7930 0000 2401 0000 8758 0100 0000 0000  y0..$....X......
 00039410: 0100 0000 2400 0000 3400 0000 0000 0000  ....$...4.......
 00039420: 0100 0000 4e01 0000 8758 0100 0000 0000  ....N....X......
 00039430: 0100 0000 2e01 0000 bb58 0100 0000 0000  .........X......
-00039440: 9430 0000 2401 0000 bb58 0100 0000 0000  .0..$....X......
+00039440: 8630 0000 2401 0000 bb58 0100 0000 0000  .0..$....X......
 00039450: 0100 0000 2400 0000 1b01 0000 0000 0000  ....$...........
 00039460: 0100 0000 4e01 0000 bb58 0100 0000 0000  ....N....X......
 00039470: 0100 0000 2e01 0000 d659 0100 0000 0000  .........Y......
-00039480: 9f30 0000 2401 0000 d659 0100 0000 0000  .0..$....Y......
+00039480: 9130 0000 2401 0000 d659 0100 0000 0000  .0..$....Y......
 00039490: 0100 0000 2400 0000 3500 0000 0000 0000  ....$...5.......
 000394a0: 0100 0000 4e01 0000 d659 0100 0000 0000  ....N....Y......
 000394b0: 0100 0000 2e01 0000 0b5a 0100 0000 0000  .........Z......
-000394c0: aa30 0000 2401 0000 0b5a 0100 0000 0000  .0..$....Z......
+000394c0: 9c30 0000 2401 0000 0b5a 0100 0000 0000  .0..$....Z......
 000394d0: 0100 0000 2400 0000 1800 0000 0000 0000  ....$...........
 000394e0: 0100 0000 4e01 0000 0b5a 0100 0000 0000  ....N....Z......
 000394f0: 0100 0000 2e01 0000 235a 0100 0000 0000  ........#Z......
-00039500: b730 0000 2401 0000 235a 0100 0000 0000  .0..$...#Z......
+00039500: a930 0000 2401 0000 235a 0100 0000 0000  .0..$...#Z......
 00039510: 0100 0000 2400 0000 ce02 0000 0000 0000  ....$...........
 00039520: 0100 0000 4e01 0000 235a 0100 0000 0000  ....N...#Z......
 00039530: 0100 0000 2e01 0000 f15c 0100 0000 0000  .........\......
-00039540: c130 0000 2401 0000 f15c 0100 0000 0000  .0..$....\......
+00039540: b330 0000 2401 0000 f15c 0100 0000 0000  .0..$....\......
 00039550: 0100 0000 2400 0000 1b00 0000 0000 0000  ....$...........
 00039560: 0100 0000 4e01 0000 f15c 0100 0000 0000  ....N....\......
 00039570: 0100 0000 2e01 0000 0c5d 0100 0000 0000  .........]......
-00039580: cf30 0000 2401 0000 0c5d 0100 0000 0000  .0..$....]......
+00039580: c130 0000 2401 0000 0c5d 0100 0000 0000  .0..$....]......
 00039590: 0100 0000 2400 0000 3700 0000 0000 0000  ....$...7.......
 000395a0: 0100 0000 4e01 0000 0c5d 0100 0000 0000  ....N....]......
 000395b0: 0100 0000 2e01 0000 435d 0100 0000 0000  ........C]......
-000395c0: dd30 0000 2401 0000 435d 0100 0000 0000  .0..$...C]......
+000395c0: cf30 0000 2401 0000 435d 0100 0000 0000  .0..$...C]......
 000395d0: 0100 0000 2400 0000 e900 0000 0000 0000  ....$...........
 000395e0: 0100 0000 4e01 0000 435d 0100 0000 0000  ....N...C]......
 000395f0: 0100 0000 2e01 0000 2c5e 0100 0000 0000  ........,^......
-00039600: ea30 0000 2401 0000 2c5e 0100 0000 0000  .0..$...,^......
+00039600: dc30 0000 2401 0000 2c5e 0100 0000 0000  .0..$...,^......
 00039610: 0100 0000 2400 0000 1e00 0000 0000 0000  ....$...........
 00039620: 0100 0000 4e01 0000 2c5e 0100 0000 0000  ....N...,^......
 00039630: 0100 0000 2e01 0000 4a5e 0100 0000 0000  ........J^......
-00039640: f730 0000 2401 0000 4a5e 0100 0000 0000  .0..$...J^......
+00039640: e930 0000 2401 0000 4a5e 0100 0000 0000  .0..$...J^......
 00039650: 0100 0000 2400 0000 af00 0000 0000 0000  ....$...........
 00039660: 0100 0000 4e01 0000 4a5e 0100 0000 0000  ....N...J^......
 00039670: 0100 0000 2e01 0000 f95e 0100 0000 0000  .........^......
-00039680: 0731 0000 2401 0000 f95e 0100 0000 0000  .1..$....^......
+00039680: f930 0000 2401 0000 f95e 0100 0000 0000  .0..$....^......
 00039690: 0100 0000 2400 0000 a700 0000 0000 0000  ....$...........
 000396a0: 0100 0000 4e01 0000 f95e 0100 0000 0000  ....N....^......
 000396b0: 0100 0000 2e01 0000 a05f 0100 0000 0000  ........._......
-000396c0: 1731 0000 2401 0000 a05f 0100 0000 0000  .1..$...._......
+000396c0: 0931 0000 2401 0000 a05f 0100 0000 0000  .1..$...._......
 000396d0: 0100 0000 2400 0000 5b00 0000 0000 0000  ....$...[.......
 000396e0: 0100 0000 4e01 0000 a05f 0100 0000 0000  ....N...._......
 000396f0: 0100 0000 2e01 0000 fb5f 0100 0000 0000  ........._......
-00039700: 2e31 0000 2401 0000 fb5f 0100 0000 0000  .1..$...._......
+00039700: 2031 0000 2401 0000 fb5f 0100 0000 0000   1..$...._......
 00039710: 0100 0000 2400 0000 ae03 0000 0000 0000  ....$...........
 00039720: 0100 0000 4e01 0000 fb5f 0100 0000 0000  ....N...._......
 00039730: 0100 0000 2e01 0000 a963 0100 0000 0000  .........c......
-00039740: 4331 0000 2401 0000 a963 0100 0000 0000  C1..$....c......
+00039740: 3531 0000 2401 0000 a963 0100 0000 0000  51..$....c......
 00039750: 0100 0000 2400 0000 4803 0000 0000 0000  ....$...H.......
 00039760: 0100 0000 4e01 0000 a963 0100 0000 0000  ....N....c......
 00039770: 0100 0000 2e01 0000 f166 0100 0000 0000  .........f......
-00039780: 4f31 0000 2401 0000 f166 0100 0000 0000  O1..$....f......
+00039780: 4131 0000 2401 0000 f166 0100 0000 0000  A1..$....f......
 00039790: 0100 0000 2400 0000 cf00 0000 0000 0000  ....$...........
 000397a0: 0100 0000 4e01 0000 f166 0100 0000 0000  ....N....f......
 000397b0: 0100 0000 2e01 0000 c067 0100 0000 0000  .........g......
-000397c0: 5f31 0000 2401 0000 c067 0100 0000 0000  _1..$....g......
+000397c0: 5131 0000 2401 0000 c067 0100 0000 0000  Q1..$....g......
 000397d0: 0100 0000 2400 0000 6000 0000 0000 0000  ....$...`.......
 000397e0: 0100 0000 4e01 0000 c067 0100 0000 0000  ....N....g......
 000397f0: 0100 0000 2e01 0000 2068 0100 0000 0000  ........ h......
-00039800: 6c31 0000 2401 0000 2068 0100 0000 0000  l1..$... h......
+00039800: 5e31 0000 2401 0000 2068 0100 0000 0000  ^1..$... h......
 00039810: 0100 0000 2400 0000 6000 0000 0000 0000  ....$...`.......
 00039820: 0100 0000 4e01 0000 2068 0100 0000 0000  ....N... h......
 00039830: 0100 0000 2e01 0000 8068 0100 0000 0000  .........h......
-00039840: 7e31 0000 2401 0000 8068 0100 0000 0000  ~1..$....h......
+00039840: 7031 0000 2401 0000 8068 0100 0000 0000  p1..$....h......
 00039850: 0100 0000 2400 0000 8a00 0000 0000 0000  ....$...........
 00039860: 0100 0000 4e01 0000 8068 0100 0000 0000  ....N....h......
 00039870: 0100 0000 2e01 0000 0a69 0100 0000 0000  .........i......
-00039880: 9331 0000 2401 0000 0a69 0100 0000 0000  .1..$....i......
+00039880: 8531 0000 2401 0000 0a69 0100 0000 0000  .1..$....i......
 00039890: 0100 0000 2400 0000 3f00 0000 0000 0000  ....$...?.......
 000398a0: 0100 0000 4e01 0000 0a69 0100 0000 0000  ....N....i......
 000398b0: 0100 0000 2e01 0000 4969 0100 0000 0000  ........Ii......
-000398c0: a131 0000 2401 0000 4969 0100 0000 0000  .1..$...Ii......
+000398c0: 9331 0000 2401 0000 4969 0100 0000 0000  .1..$...Ii......
 000398d0: 0100 0000 2400 0000 b700 0000 0000 0000  ....$...........
 000398e0: 0100 0000 4e01 0000 4969 0100 0000 0000  ....N...Ii......
 000398f0: 0100 0000 2e01 0000 006a 0100 0000 0000  .........j......
-00039900: ae31 0000 2401 0000 006a 0100 0000 0000  .1..$....j......
+00039900: a031 0000 2401 0000 006a 0100 0000 0000  .1..$....j......
 00039910: 0100 0000 2400 0000 fa00 0000 0000 0000  ....$...........
 00039920: 0100 0000 4e01 0000 006a 0100 0000 0000  ....N....j......
 00039930: 0100 0000 2e01 0000 fa6a 0100 0000 0000  .........j......
-00039940: ba31 0000 2401 0000 fa6a 0100 0000 0000  .1..$....j......
+00039940: ac31 0000 2401 0000 fa6a 0100 0000 0000  .1..$....j......
 00039950: 0100 0000 2400 0000 5100 0000 0000 0000  ....$...Q.......
 00039960: 0100 0000 4e01 0000 fa6a 0100 0000 0000  ....N....j......
 00039970: 0100 0000 2e01 0000 4b6b 0100 0000 0000  ........Kk......
-00039980: c431 0000 2401 0000 4b6b 0100 0000 0000  .1..$...Kk......
+00039980: b631 0000 2401 0000 4b6b 0100 0000 0000  .1..$...Kk......
 00039990: 0100 0000 2400 0000 cb00 0000 0000 0000  ....$...........
 000399a0: 0100 0000 4e01 0000 4b6b 0100 0000 0000  ....N...Kk......
 000399b0: 0100 0000 2e01 0000 166c 0100 0000 0000  .........l......
-000399c0: d831 0000 2401 0000 166c 0100 0000 0000  .1..$....l......
+000399c0: ca31 0000 2401 0000 166c 0100 0000 0000  .1..$....l......
 000399d0: 0100 0000 2400 0000 6b01 0000 0000 0000  ....$...k.......
 000399e0: 0100 0000 4e01 0000 166c 0100 0000 0000  ....N....l......
 000399f0: 0100 0000 2e01 0000 816d 0100 0000 0000  .........m......
-00039a00: e931 0000 2401 0000 816d 0100 0000 0000  .1..$....m......
+00039a00: db31 0000 2401 0000 816d 0100 0000 0000  .1..$....m......
 00039a10: 0100 0000 2400 0000 0605 0000 0000 0000  ....$...........
 00039a20: 0100 0000 4e01 0000 816d 0100 0000 0000  ....N....m......
 00039a30: 0100 0000 2e01 0000 8772 0100 0000 0000  .........r......
-00039a40: f531 0000 2401 0000 8772 0100 0000 0000  .1..$....r......
+00039a40: e731 0000 2401 0000 8772 0100 0000 0000  .1..$....r......
 00039a50: 0100 0000 2400 0000 da01 0000 0000 0000  ....$...........
 00039a60: 0100 0000 4e01 0000 8772 0100 0000 0000  ....N....r......
 00039a70: 0100 0000 2e01 0000 6174 0100 0000 0000  ........at......
-00039a80: 0632 0000 2401 0000 6174 0100 0000 0000  .2..$...at......
+00039a80: f831 0000 2401 0000 6174 0100 0000 0000  .1..$...at......
 00039a90: 0100 0000 2400 0000 0702 0000 0000 0000  ....$...........
 00039aa0: 0100 0000 4e01 0000 6174 0100 0000 0000  ....N...at......
 00039ab0: 0100 0000 2e01 0000 6876 0100 0000 0000  ........hv......
-00039ac0: 1c32 0000 2401 0000 6876 0100 0000 0000  .2..$...hv......
+00039ac0: 0e32 0000 2401 0000 6876 0100 0000 0000  .2..$...hv......
 00039ad0: 0100 0000 2400 0000 7c00 0000 0000 0000  ....$...|.......
 00039ae0: 0100 0000 4e01 0000 6876 0100 0000 0000  ....N...hv......
 00039af0: 0100 0000 2e01 0000 e476 0100 0000 0000  .........v......
-00039b00: 2b32 0000 2401 0000 e476 0100 0000 0000  +2..$....v......
+00039b00: 1d32 0000 2401 0000 e476 0100 0000 0000  .2..$....v......
 00039b10: 0100 0000 2400 0000 1001 0000 0000 0000  ....$...........
 00039b20: 0100 0000 4e01 0000 e476 0100 0000 0000  ....N....v......
 00039b30: 0100 0000 2e01 0000 f477 0100 0000 0000  .........w......
-00039b40: 3c32 0000 2401 0000 f477 0100 0000 0000  <2..$....w......
+00039b40: 2e32 0000 2401 0000 f477 0100 0000 0000  .2..$....w......
 00039b50: 0100 0000 2400 0000 5800 0000 0000 0000  ....$...X.......
 00039b60: 0100 0000 4e01 0000 f477 0100 0000 0000  ....N....w......
 00039b70: 0100 0000 2e01 0000 4c78 0100 0000 0000  ........Lx......
-00039b80: 4732 0000 2401 0000 4c78 0100 0000 0000  G2..$...Lx......
+00039b80: 3932 0000 2401 0000 4c78 0100 0000 0000  92..$...Lx......
 00039b90: 0100 0000 2400 0000 ab07 0000 0000 0000  ....$...........
 00039ba0: 0100 0000 4e01 0000 4c78 0100 0000 0000  ....N...Lx......
 00039bb0: 0100 0000 2e01 0000 f77f 0100 0000 0000  ................
-00039bc0: 5132 0000 2401 0000 f77f 0100 0000 0000  Q2..$...........
+00039bc0: 4332 0000 2401 0000 f77f 0100 0000 0000  C2..$...........
 00039bd0: 0100 0000 2400 0000 bb02 0000 0000 0000  ....$...........
 00039be0: 0100 0000 4e01 0000 f77f 0100 0000 0000  ....N...........
 00039bf0: 0100 0000 2e01 0000 b282 0100 0000 0000  ................
-00039c00: 6132 0000 2401 0000 b282 0100 0000 0000  a2..$...........
+00039c00: 5332 0000 2401 0000 b282 0100 0000 0000  S2..$...........
 00039c10: 0100 0000 2400 0000 8002 0000 0000 0000  ....$...........
 00039c20: 0100 0000 4e01 0000 b282 0100 0000 0000  ....N...........
 00039c30: 0100 0000 2e01 0000 3285 0100 0000 0000  ........2.......
-00039c40: 7432 0000 2401 0000 3285 0100 0000 0000  t2..$...2.......
+00039c40: 6632 0000 2401 0000 3285 0100 0000 0000  f2..$...2.......
 00039c50: 0100 0000 2400 0000 3902 0000 0000 0000  ....$...9.......
 00039c60: 0100 0000 4e01 0000 3285 0100 0000 0000  ....N...2.......
 00039c70: 0100 0000 2e01 0000 6b87 0100 0000 0000  ........k.......
-00039c80: 8632 0000 2401 0000 6b87 0100 0000 0000  .2..$...k.......
+00039c80: 7832 0000 2401 0000 6b87 0100 0000 0000  x2..$...k.......
 00039c90: 0100 0000 2400 0000 1501 0000 0000 0000  ....$...........
 00039ca0: 0100 0000 4e01 0000 6b87 0100 0000 0000  ....N...k.......
 00039cb0: 0100 0000 2e01 0000 8088 0100 0000 0000  ................
-00039cc0: 9932 0000 2401 0000 8088 0100 0000 0000  .2..$...........
+00039cc0: 8b32 0000 2401 0000 8088 0100 0000 0000  .2..$...........
 00039cd0: 0100 0000 2400 0000 9200 0000 0000 0000  ....$...........
 00039ce0: 0100 0000 4e01 0000 8088 0100 0000 0000  ....N...........
 00039cf0: 0100 0000 2e01 0000 1289 0100 0000 0000  ................
-00039d00: ad32 0000 2401 0000 1289 0100 0000 0000  .2..$...........
+00039d00: 9f32 0000 2401 0000 1289 0100 0000 0000  .2..$...........
 00039d10: 0100 0000 2400 0000 5800 0000 0000 0000  ....$...X.......
 00039d20: 0100 0000 4e01 0000 1289 0100 0000 0000  ....N...........
-00039d30: b732 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
-00039d40: c232 0000 2609 0000 a6c1 0200 0000 0000  .2..&...........
-00039d50: ce32 0000 2609 0000 a8c1 0200 0000 0000  .2..&...........
-00039d60: dd32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
-00039d70: ee32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
-00039d80: fb32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
-00039d90: 0833 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
-00039da0: 1233 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
-00039db0: 1e33 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
-00039dc0: 2a33 0000 2000 0000 0000 0000 0000 0000  *3.. ...........
-00039dd0: 3433 0000 2000 0000 0000 0000 0000 0000  43.. ...........
-00039de0: 3e33 0000 260b 0000 d0ce 0200 0000 0000  >3..&...........
-00039df0: 4a33 0000 260b 0000 d0ce 0600 0000 0000  J3..&...........
-00039e00: 5533 0000 260b 0000 d0d0 0600 0000 0000  U3..&...........
-00039e10: 6033 0000 260b 0000 d0d2 0600 0000 0000  `3..&...........
-00039e20: 6c33 0000 260b 0000 e0d2 0600 0000 0000  l3..&...........
-00039e30: 7833 0000 260b 0000 00d3 0600 0000 0000  x3..&...........
-00039e40: 8533 0000 260b 0000 04d3 0600 0000 0000  .3..&...........
+00039d30: a932 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
+00039d40: b432 0000 2609 0000 a6c1 0200 0000 0000  .2..&...........
+00039d50: c032 0000 2609 0000 a8c1 0200 0000 0000  .2..&...........
+00039d60: cf32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
+00039d70: e032 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
+00039d80: ed32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
+00039d90: fa32 0000 2000 0000 0000 0000 0000 0000  .2.. ...........
+00039da0: 0433 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
+00039db0: 1033 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
+00039dc0: 1c33 0000 2000 0000 0000 0000 0000 0000  .3.. ...........
+00039dd0: 2633 0000 2000 0000 0000 0000 0000 0000  &3.. ...........
+00039de0: 3033 0000 260b 0000 d0ce 0200 0000 0000  03..&...........
+00039df0: 3c33 0000 260b 0000 d0ce 0600 0000 0000  <3..&...........
+00039e00: 4733 0000 260b 0000 d0d0 0600 0000 0000  G3..&...........
+00039e10: 5233 0000 260b 0000 d0d2 0600 0000 0000  R3..&...........
+00039e20: 5e33 0000 260b 0000 e0d2 0600 0000 0000  ^3..&...........
+00039e30: 6a33 0000 260b 0000 00d3 0600 0000 0000  j3..&...........
+00039e40: 7733 0000 260b 0000 04d3 0600 0000 0000  w3..&...........
 00039e50: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-00039e60: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-00039e70: 9e33 0000 6400 0000 0000 0000 0000 0000  .3..d...........
-00039e80: a933 0000 6603 0100 8735 3864 0000 0000  .3..f....58d....
+00039e60: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+00039e70: 9033 0000 6400 0000 0000 0000 0000 0000  .3..d...........
+00039e80: 9b33 0000 6603 0100 beb1 3d64 0000 0000  .3..f.....=d....
 00039e90: 0100 0000 2e01 0000 6a89 0100 0000 0000  ........j.......
-00039ea0: 3f34 0000 2401 0000 6a89 0100 0000 0000  ?4..$...j.......
+00039ea0: 3134 0000 2401 0000 6a89 0100 0000 0000  14..$...j.......
 00039eb0: 0100 0000 2400 0000 3602 0000 0000 0000  ....$...6.......
 00039ec0: 0100 0000 4e01 0000 6a89 0100 0000 0000  ....N...j.......
 00039ed0: 0100 0000 2e01 0000 a08b 0100 0000 0000  ................
-00039ee0: 4c34 0000 2401 0000 a08b 0100 0000 0000  L4..$...........
+00039ee0: 3e34 0000 2401 0000 a08b 0100 0000 0000  >4..$...........
 00039ef0: 0100 0000 2400 0000 b700 0000 0000 0000  ....$...........
 00039f00: 0100 0000 4e01 0000 a08b 0100 0000 0000  ....N...........
 00039f10: 0100 0000 2e01 0000 578c 0100 0000 0000  ........W.......
-00039f20: 5a34 0000 2401 0000 578c 0100 0000 0000  Z4..$...W.......
+00039f20: 4c34 0000 2401 0000 578c 0100 0000 0000  L4..$...W.......
 00039f30: 0100 0000 2400 0000 2001 0000 0000 0000  ....$... .......
 00039f40: 0100 0000 4e01 0000 578c 0100 0000 0000  ....N...W.......
 00039f50: 0100 0000 2e01 0000 778d 0100 0000 0000  ........w.......
-00039f60: 6b34 0000 2401 0000 778d 0100 0000 0000  k4..$...w.......
+00039f60: 5d34 0000 2401 0000 778d 0100 0000 0000  ]4..$...w.......
 00039f70: 0100 0000 2400 0000 eb00 0000 0000 0000  ....$...........
 00039f80: 0100 0000 4e01 0000 778d 0100 0000 0000  ....N...w.......
 00039f90: 0100 0000 2e01 0000 628e 0100 0000 0000  ........b.......
-00039fa0: 7834 0000 2401 0000 628e 0100 0000 0000  x4..$...b.......
+00039fa0: 6a34 0000 2401 0000 628e 0100 0000 0000  j4..$...b.......
 00039fb0: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 00039fc0: 0100 0000 4e01 0000 628e 0100 0000 0000  ....N...b.......
 00039fd0: 0100 0000 2e01 0000 a28e 0100 0000 0000  ................
-00039fe0: 8834 0000 2401 0000 a28e 0100 0000 0000  .4..$...........
+00039fe0: 7a34 0000 2401 0000 a28e 0100 0000 0000  z4..$...........
 00039ff0: 0100 0000 2400 0000 6d01 0000 0000 0000  ....$...m.......
 0003a000: 0100 0000 4e01 0000 a28e 0100 0000 0000  ....N...........
 0003a010: 0100 0000 2e01 0000 0f90 0100 0000 0000  ................
-0003a020: 9d34 0000 2401 0000 0f90 0100 0000 0000  .4..$...........
+0003a020: 8f34 0000 2401 0000 0f90 0100 0000 0000  .4..$...........
 0003a030: 0100 0000 2400 0000 7000 0000 0000 0000  ....$...p.......
 0003a040: 0100 0000 4e01 0000 0f90 0100 0000 0000  ....N...........
 0003a050: 0100 0000 2e01 0000 7f90 0100 0000 0000  ................
-0003a060: a834 0000 2401 0000 7f90 0100 0000 0000  .4..$...........
+0003a060: 9a34 0000 2401 0000 7f90 0100 0000 0000  .4..$...........
 0003a070: 0100 0000 2400 0000 5900 0000 0000 0000  ....$...Y.......
 0003a080: 0100 0000 4e01 0000 7f90 0100 0000 0000  ....N...........
 0003a090: 0100 0000 2e01 0000 d890 0100 0000 0000  ................
-0003a0a0: ba34 0000 2401 0000 d890 0100 0000 0000  .4..$...........
+0003a0a0: ac34 0000 2401 0000 d890 0100 0000 0000  .4..$...........
 0003a0b0: 0100 0000 2400 0000 1e01 0000 0000 0000  ....$...........
 0003a0c0: 0100 0000 4e01 0000 d890 0100 0000 0000  ....N...........
 0003a0d0: 0100 0000 2e01 0000 f691 0100 0000 0000  ................
-0003a0e0: cc34 0000 2401 0000 f691 0100 0000 0000  .4..$...........
+0003a0e0: be34 0000 2401 0000 f691 0100 0000 0000  .4..$...........
 0003a0f0: 0100 0000 2400 0000 1300 0000 0000 0000  ....$...........
 0003a100: 0100 0000 4e01 0000 f691 0100 0000 0000  ....N...........
 0003a110: 0100 0000 2e01 0000 0992 0100 0000 0000  ................
-0003a120: dd34 0000 2401 0000 0992 0100 0000 0000  .4..$...........
+0003a120: cf34 0000 2401 0000 0992 0100 0000 0000  .4..$...........
 0003a130: 0100 0000 2400 0000 1a03 0000 0000 0000  ....$...........
 0003a140: 0100 0000 4e01 0000 0992 0100 0000 0000  ....N...........
 0003a150: 0100 0000 2e01 0000 2395 0100 0000 0000  ........#.......
-0003a160: e734 0000 2401 0000 2395 0100 0000 0000  .4..$...#.......
+0003a160: d934 0000 2401 0000 2395 0100 0000 0000  .4..$...#.......
 0003a170: 0100 0000 2400 0000 4200 0000 0000 0000  ....$...B.......
 0003a180: 0100 0000 4e01 0000 2395 0100 0000 0000  ....N...#.......
 0003a190: 0100 0000 2e01 0000 6595 0100 0000 0000  ........e.......
-0003a1a0: 0e35 0000 2401 0000 6595 0100 0000 0000  .5..$...e.......
+0003a1a0: 0035 0000 2401 0000 6595 0100 0000 0000  .5..$...e.......
 0003a1b0: 0100 0000 2400 0000 dd00 0000 0000 0000  ....$...........
 0003a1c0: 0100 0000 4e01 0000 6595 0100 0000 0000  ....N...e.......
 0003a1d0: 0100 0000 2e01 0000 4296 0100 0000 0000  ........B.......
-0003a1e0: 1f35 0000 2401 0000 4296 0100 0000 0000  .5..$...B.......
+0003a1e0: 1135 0000 2401 0000 4296 0100 0000 0000  .5..$...B.......
 0003a1f0: 0100 0000 2400 0000 f100 0000 0000 0000  ....$...........
 0003a200: 0100 0000 4e01 0000 4296 0100 0000 0000  ....N...B.......
 0003a210: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-0003a220: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-0003a230: 3235 0000 6400 0000 0000 0000 0000 0000  25..d...........
-0003a240: 3935 0000 6603 0100 8935 3864 0000 0000  95..f....58d....
+0003a220: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+0003a230: 2435 0000 6400 0000 0000 0000 0000 0000  $5..d...........
+0003a240: 2b35 0000 6603 0100 c0b1 3d64 0000 0000  +5..f.....=d....
 0003a250: 0100 0000 2e01 0000 3497 0100 0000 0000  ........4.......
-0003a260: cb35 0000 2401 0000 3497 0100 0000 0000  .5..$...4.......
+0003a260: bd35 0000 2401 0000 3497 0100 0000 0000  .5..$...4.......
 0003a270: 0100 0000 2400 0000 2300 0000 0000 0000  ....$...#.......
 0003a280: 0100 0000 4e01 0000 3497 0100 0000 0000  ....N...4.......
 0003a290: 0100 0000 2e01 0000 5797 0100 0000 0000  ........W.......
-0003a2a0: e535 0000 2401 0000 5797 0100 0000 0000  .5..$...W.......
+0003a2a0: d735 0000 2401 0000 5797 0100 0000 0000  .5..$...W.......
 0003a2b0: 0100 0000 2400 0000 6000 0000 0000 0000  ....$...`.......
 0003a2c0: 0100 0000 4e01 0000 5797 0100 0000 0000  ....N...W.......
 0003a2d0: 0100 0000 2e01 0000 b797 0100 0000 0000  ................
-0003a2e0: f635 0000 2401 0000 b797 0100 0000 0000  .5..$...........
+0003a2e0: e835 0000 2401 0000 b797 0100 0000 0000  .5..$...........
 0003a2f0: 0100 0000 2400 0000 cf00 0000 0000 0000  ....$...........
 0003a300: 0100 0000 4e01 0000 b797 0100 0000 0000  ....N...........
 0003a310: 0100 0000 2e01 0000 8698 0100 0000 0000  ................
-0003a320: 0c36 0000 2401 0000 8698 0100 0000 0000  .6..$...........
+0003a320: fe35 0000 2401 0000 8698 0100 0000 0000  .5..$...........
 0003a330: 0100 0000 2400 0000 a100 0000 0000 0000  ....$...........
 0003a340: 0100 0000 4e01 0000 8698 0100 0000 0000  ....N...........
 0003a350: 0100 0000 2e01 0000 2799 0100 0000 0000  ........'.......
-0003a360: 1d36 0000 2401 0000 2799 0100 0000 0000  .6..$...'.......
+0003a360: 0f36 0000 2401 0000 2799 0100 0000 0000  .6..$...'.......
 0003a370: 0100 0000 2400 0000 7e00 0000 0000 0000  ....$...~.......
 0003a380: 0100 0000 4e01 0000 2799 0100 0000 0000  ....N...'.......
 0003a390: 0100 0000 2e01 0000 a599 0100 0000 0000  ................
-0003a3a0: 2e36 0000 2401 0000 a599 0100 0000 0000  .6..$...........
+0003a3a0: 2036 0000 2401 0000 a599 0100 0000 0000   6..$...........
 0003a3b0: 0100 0000 2400 0000 b702 0000 0000 0000  ....$...........
 0003a3c0: 0100 0000 4e01 0000 a599 0100 0000 0000  ....N...........
 0003a3d0: 0100 0000 2e01 0000 5c9c 0100 0000 0000  ........\.......
-0003a3e0: 4336 0000 2401 0000 5c9c 0100 0000 0000  C6..$...\.......
+0003a3e0: 3536 0000 2401 0000 5c9c 0100 0000 0000  56..$...\.......
 0003a3f0: 0100 0000 2400 0000 9400 0000 0000 0000  ....$...........
 0003a400: 0100 0000 4e01 0000 5c9c 0100 0000 0000  ....N...\.......
 0003a410: 0100 0000 2e01 0000 f09c 0100 0000 0000  ................
-0003a420: 5636 0000 2401 0000 f09c 0100 0000 0000  V6..$...........
+0003a420: 4836 0000 2401 0000 f09c 0100 0000 0000  H6..$...........
 0003a430: 0100 0000 2400 0000 6000 0000 0000 0000  ....$...`.......
 0003a440: 0100 0000 4e01 0000 f09c 0100 0000 0000  ....N...........
 0003a450: 0100 0000 2e01 0000 509d 0100 0000 0000  ........P.......
-0003a460: 6736 0000 2401 0000 509d 0100 0000 0000  g6..$...P.......
+0003a460: 5936 0000 2401 0000 509d 0100 0000 0000  Y6..$...P.......
 0003a470: 0100 0000 2400 0000 6802 0000 0000 0000  ....$...h.......
 0003a480: 0100 0000 4e01 0000 509d 0100 0000 0000  ....N...P.......
 0003a490: 0100 0000 2e01 0000 b89f 0100 0000 0000  ................
-0003a4a0: 7b36 0000 2401 0000 b89f 0100 0000 0000  {6..$...........
+0003a4a0: 6d36 0000 2401 0000 b89f 0100 0000 0000  m6..$...........
 0003a4b0: 0100 0000 2400 0000 8a02 0000 0000 0000  ....$...........
 0003a4c0: 0100 0000 4e01 0000 b89f 0100 0000 0000  ....N...........
 0003a4d0: 0100 0000 2e01 0000 42a2 0100 0000 0000  ........B.......
-0003a4e0: 8636 0000 2401 0000 42a2 0100 0000 0000  .6..$...B.......
+0003a4e0: 7836 0000 2401 0000 42a2 0100 0000 0000  x6..$...B.......
 0003a4f0: 0100 0000 2400 0000 ad02 0000 0000 0000  ....$...........
 0003a500: 0100 0000 4e01 0000 42a2 0100 0000 0000  ....N...B.......
 0003a510: 0100 0000 2e01 0000 efa4 0100 0000 0000  ................
-0003a520: 9936 0000 2401 0000 efa4 0100 0000 0000  .6..$...........
+0003a520: 8b36 0000 2401 0000 efa4 0100 0000 0000  .6..$...........
 0003a530: 0100 0000 2400 0000 2f02 0000 0000 0000  ....$.../.......
 0003a540: 0100 0000 4e01 0000 efa4 0100 0000 0000  ....N...........
 0003a550: 0100 0000 2e01 0000 1ea7 0100 0000 0000  ................
-0003a560: ae36 0000 2401 0000 1ea7 0100 0000 0000  .6..$...........
+0003a560: a036 0000 2401 0000 1ea7 0100 0000 0000  .6..$...........
 0003a570: 0100 0000 2400 0000 2400 0000 0000 0000  ....$...$.......
 0003a580: 0100 0000 4e01 0000 1ea7 0100 0000 0000  ....N...........
 0003a590: 0100 0000 2e01 0000 42a7 0100 0000 0000  ........B.......
-0003a5a0: c136 0000 2401 0000 42a7 0100 0000 0000  .6..$...B.......
+0003a5a0: b336 0000 2401 0000 42a7 0100 0000 0000  .6..$...B.......
 0003a5b0: 0100 0000 2400 0000 4501 0000 0000 0000  ....$...E.......
 0003a5c0: 0100 0000 4e01 0000 42a7 0100 0000 0000  ....N...B.......
 0003a5d0: 0100 0000 2e01 0000 87a8 0100 0000 0000  ................
-0003a5e0: d836 0000 2401 0000 87a8 0100 0000 0000  .6..$...........
+0003a5e0: ca36 0000 2401 0000 87a8 0100 0000 0000  .6..$...........
 0003a5f0: 0100 0000 2400 0000 f600 0000 0000 0000  ....$...........
 0003a600: 0100 0000 4e01 0000 87a8 0100 0000 0000  ....N...........
 0003a610: 0100 0000 2e01 0000 7da9 0100 0000 0000  ........}.......
-0003a620: eb36 0000 2401 0000 7da9 0100 0000 0000  .6..$...}.......
+0003a620: dd36 0000 2401 0000 7da9 0100 0000 0000  .6..$...}.......
 0003a630: 0100 0000 2400 0000 a801 0000 0000 0000  ....$...........
 0003a640: 0100 0000 4e01 0000 7da9 0100 0000 0000  ....N...}.......
 0003a650: 0100 0000 2e01 0000 25ab 0100 0000 0000  ........%.......
-0003a660: fc36 0000 2401 0000 25ab 0100 0000 0000  .6..$...%.......
+0003a660: ee36 0000 2401 0000 25ab 0100 0000 0000  .6..$...%.......
 0003a670: 0100 0000 2400 0000 7101 0000 0000 0000  ....$...q.......
 0003a680: 0100 0000 4e01 0000 25ab 0100 0000 0000  ....N...%.......
 0003a690: 0100 0000 2e01 0000 96ac 0100 0000 0000  ................
-0003a6a0: 0b37 0000 2401 0000 96ac 0100 0000 0000  .7..$...........
+0003a6a0: fd36 0000 2401 0000 96ac 0100 0000 0000  .6..$...........
 0003a6b0: 0100 0000 2400 0000 5d01 0000 0000 0000  ....$...].......
 0003a6c0: 0100 0000 4e01 0000 96ac 0100 0000 0000  ....N...........
 0003a6d0: 0100 0000 2e01 0000 f3ad 0100 0000 0000  ................
-0003a6e0: 1c37 0000 2401 0000 f3ad 0100 0000 0000  .7..$...........
+0003a6e0: 0e37 0000 2401 0000 f3ad 0100 0000 0000  .7..$...........
 0003a6f0: 0100 0000 2400 0000 a50a 0000 0000 0000  ....$...........
 0003a700: 0100 0000 4e01 0000 f3ad 0100 0000 0000  ....N...........
 0003a710: 0100 0000 2e01 0000 98b8 0100 0000 0000  ................
-0003a720: 3337 0000 2401 0000 98b8 0100 0000 0000  37..$...........
+0003a720: 2537 0000 2401 0000 98b8 0100 0000 0000  %7..$...........
 0003a730: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 0003a740: 0100 0000 4e01 0000 98b8 0100 0000 0000  ....N...........
 0003a750: 0100 0000 2e01 0000 fbb8 0100 0000 0000  ................
-0003a760: 4837 0000 2401 0000 fbb8 0100 0000 0000  H7..$...........
+0003a760: 3a37 0000 2401 0000 fbb8 0100 0000 0000  :7..$...........
 0003a770: 0100 0000 2400 0000 3300 0000 0000 0000  ....$...3.......
 0003a780: 0100 0000 4e01 0000 fbb8 0100 0000 0000  ....N...........
 0003a790: 0100 0000 2e01 0000 2eb9 0100 0000 0000  ................
-0003a7a0: 5e37 0000 2401 0000 2eb9 0100 0000 0000  ^7..$...........
+0003a7a0: 5037 0000 2401 0000 2eb9 0100 0000 0000  P7..$...........
 0003a7b0: 0100 0000 2400 0000 2100 0000 0000 0000  ....$...!.......
 0003a7c0: 0100 0000 4e01 0000 2eb9 0100 0000 0000  ....N...........
 0003a7d0: 0100 0000 2e01 0000 4fb9 0100 0000 0000  ........O.......
-0003a7e0: 6e37 0000 2401 0000 4fb9 0100 0000 0000  n7..$...O.......
+0003a7e0: 6037 0000 2401 0000 4fb9 0100 0000 0000  `7..$...O.......
 0003a7f0: 0100 0000 2400 0000 3300 0000 0000 0000  ....$...3.......
 0003a800: 0100 0000 4e01 0000 4fb9 0100 0000 0000  ....N...O.......
 0003a810: 0100 0000 2e01 0000 82b9 0100 0000 0000  ................
-0003a820: 7e37 0000 2401 0000 82b9 0100 0000 0000  ~7..$...........
+0003a820: 7037 0000 2401 0000 82b9 0100 0000 0000  p7..$...........
 0003a830: 0100 0000 2400 0000 4200 0000 0000 0000  ....$...B.......
 0003a840: 0100 0000 4e01 0000 82b9 0100 0000 0000  ....N...........
 0003a850: 0100 0000 2e01 0000 c4b9 0100 0000 0000  ................
-0003a860: 9037 0000 2401 0000 c4b9 0100 0000 0000  .7..$...........
+0003a860: 8237 0000 2401 0000 c4b9 0100 0000 0000  .7..$...........
 0003a870: 0100 0000 2400 0000 9800 0000 0000 0000  ....$...........
 0003a880: 0100 0000 4e01 0000 c4b9 0100 0000 0000  ....N...........
 0003a890: 0100 0000 2e01 0000 5cba 0100 0000 0000  ........\.......
-0003a8a0: 9f37 0000 2401 0000 5cba 0100 0000 0000  .7..$...\.......
+0003a8a0: 9137 0000 2401 0000 5cba 0100 0000 0000  .7..$...\.......
 0003a8b0: 0100 0000 2400 0000 4e03 0000 0000 0000  ....$...N.......
 0003a8c0: 0100 0000 4e01 0000 5cba 0100 0000 0000  ....N...\.......
 0003a8d0: 0100 0000 2e01 0000 aabd 0100 0000 0000  ................
-0003a8e0: b037 0000 2401 0000 aabd 0100 0000 0000  .7..$...........
+0003a8e0: a237 0000 2401 0000 aabd 0100 0000 0000  .7..$...........
 0003a8f0: 0100 0000 2400 0000 4c05 0000 0000 0000  ....$...L.......
 0003a900: 0100 0000 4e01 0000 aabd 0100 0000 0000  ....N...........
 0003a910: 0100 0000 2e01 0000 f6c2 0100 0000 0000  ................
-0003a920: d537 0000 2401 0000 f6c2 0100 0000 0000  .7..$...........
+0003a920: c737 0000 2401 0000 f6c2 0100 0000 0000  .7..$...........
 0003a930: 0100 0000 2400 0000 1103 0000 0000 0000  ....$...........
 0003a940: 0100 0000 4e01 0000 f6c2 0100 0000 0000  ....N...........
 0003a950: 0100 0000 2e01 0000 07c6 0100 0000 0000  ................
-0003a960: e837 0000 2401 0000 07c6 0100 0000 0000  .7..$...........
+0003a960: da37 0000 2401 0000 07c6 0100 0000 0000  .7..$...........
 0003a970: 0100 0000 2400 0000 5c00 0000 0000 0000  ....$...\.......
 0003a980: 0100 0000 4e01 0000 07c6 0100 0000 0000  ....N...........
 0003a990: 0100 0000 2e01 0000 63c6 0100 0000 0000  ........c.......
-0003a9a0: fa37 0000 2401 0000 63c6 0100 0000 0000  .7..$...c.......
+0003a9a0: ec37 0000 2401 0000 63c6 0100 0000 0000  .7..$...c.......
 0003a9b0: 0100 0000 2400 0000 e800 0000 0000 0000  ....$...........
 0003a9c0: 0100 0000 4e01 0000 63c6 0100 0000 0000  ....N...c.......
 0003a9d0: 0100 0000 2e01 0000 4bc7 0100 0000 0000  ........K.......
-0003a9e0: 1c38 0000 2401 0000 4bc7 0100 0000 0000  .8..$...K.......
+0003a9e0: 0e38 0000 2401 0000 4bc7 0100 0000 0000  .8..$...K.......
 0003a9f0: 0100 0000 2400 0000 4a01 0000 0000 0000  ....$...J.......
 0003aa00: 0100 0000 4e01 0000 4bc7 0100 0000 0000  ....N...K.......
 0003aa10: 0100 0000 2e01 0000 95c8 0100 0000 0000  ................
-0003aa20: 3438 0000 2401 0000 95c8 0100 0000 0000  48..$...........
+0003aa20: 2638 0000 2401 0000 95c8 0100 0000 0000  &8..$...........
 0003aa30: 0100 0000 2400 0000 8a01 0000 0000 0000  ....$...........
 0003aa40: 0100 0000 4e01 0000 95c8 0100 0000 0000  ....N...........
 0003aa50: 0100 0000 2e01 0000 1fca 0100 0000 0000  ................
-0003aa60: 4e38 0000 2401 0000 1fca 0100 0000 0000  N8..$...........
+0003aa60: 4038 0000 2401 0000 1fca 0100 0000 0000  @8..$...........
 0003aa70: 0100 0000 2400 0000 9103 0000 0000 0000  ....$...........
 0003aa80: 0100 0000 4e01 0000 1fca 0100 0000 0000  ....N...........
 0003aa90: 0100 0000 2e01 0000 b0cd 0100 0000 0000  ................
-0003aaa0: 6838 0000 2401 0000 b0cd 0100 0000 0000  h8..$...........
+0003aaa0: 5a38 0000 2401 0000 b0cd 0100 0000 0000  Z8..$...........
 0003aab0: 0100 0000 2400 0000 5100 0000 0000 0000  ....$...Q.......
 0003aac0: 0100 0000 4e01 0000 b0cd 0100 0000 0000  ....N...........
 0003aad0: 0100 0000 2e01 0000 01ce 0100 0000 0000  ................
-0003aae0: 8738 0000 2401 0000 01ce 0100 0000 0000  .8..$...........
+0003aae0: 7938 0000 2401 0000 01ce 0100 0000 0000  y8..$...........
 0003aaf0: 0100 0000 2400 0000 5100 0000 0000 0000  ....$...Q.......
 0003ab00: 0100 0000 4e01 0000 01ce 0100 0000 0000  ....N...........
 0003ab10: 0100 0000 2e01 0000 52ce 0100 0000 0000  ........R.......
-0003ab20: a038 0000 2401 0000 52ce 0100 0000 0000  .8..$...R.......
+0003ab20: 9238 0000 2401 0000 52ce 0100 0000 0000  .8..$...R.......
 0003ab30: 0100 0000 2400 0000 5100 0000 0000 0000  ....$...Q.......
 0003ab40: 0100 0000 4e01 0000 52ce 0100 0000 0000  ....N...R.......
 0003ab50: 0100 0000 2e01 0000 a3ce 0100 0000 0000  ................
-0003ab60: bb38 0000 2401 0000 a3ce 0100 0000 0000  .8..$...........
+0003ab60: ad38 0000 2401 0000 a3ce 0100 0000 0000  .8..$...........
 0003ab70: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003ab80: 0100 0000 4e01 0000 a3ce 0100 0000 0000  ....N...........
 0003ab90: 0100 0000 2e01 0000 adce 0100 0000 0000  ................
-0003aba0: c838 0000 2401 0000 adce 0100 0000 0000  .8..$...........
+0003aba0: ba38 0000 2401 0000 adce 0100 0000 0000  .8..$...........
 0003abb0: 0100 0000 2400 0000 c801 0000 0000 0000  ....$...........
 0003abc0: 0100 0000 4e01 0000 adce 0100 0000 0000  ....N...........
 0003abd0: 0100 0000 2e01 0000 75d0 0100 0000 0000  ........u.......
-0003abe0: de38 0000 2401 0000 75d0 0100 0000 0000  .8..$...u.......
+0003abe0: d038 0000 2401 0000 75d0 0100 0000 0000  .8..$...u.......
 0003abf0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003ac00: 0100 0000 4e01 0000 75d0 0100 0000 0000  ....N...u.......
 0003ac10: 0100 0000 2e01 0000 7fd0 0100 0000 0000  ................
-0003ac20: eb38 0000 2401 0000 7fd0 0100 0000 0000  .8..$...........
+0003ac20: dd38 0000 2401 0000 7fd0 0100 0000 0000  .8..$...........
 0003ac30: 0100 0000 2400 0000 2a02 0000 0000 0000  ....$...*.......
 0003ac40: 0100 0000 4e01 0000 7fd0 0100 0000 0000  ....N...........
 0003ac50: 0100 0000 2e01 0000 a9d2 0100 0000 0000  ................
-0003ac60: 0139 0000 2401 0000 a9d2 0100 0000 0000  .9..$...........
+0003ac60: f338 0000 2401 0000 a9d2 0100 0000 0000  .8..$...........
 0003ac70: 0100 0000 2400 0000 0c00 0000 0000 0000  ....$...........
 0003ac80: 0100 0000 4e01 0000 a9d2 0100 0000 0000  ....N...........
 0003ac90: 0100 0000 2e01 0000 b5d2 0100 0000 0000  ................
-0003aca0: 1839 0000 2401 0000 b5d2 0100 0000 0000  .9..$...........
+0003aca0: 0a39 0000 2401 0000 b5d2 0100 0000 0000  .9..$...........
 0003acb0: 0100 0000 2400 0000 0c00 0000 0000 0000  ....$...........
 0003acc0: 0100 0000 4e01 0000 b5d2 0100 0000 0000  ....N...........
 0003acd0: 0100 0000 2e01 0000 c1d2 0100 0000 0000  ................
-0003ace0: 2f39 0000 2401 0000 c1d2 0100 0000 0000  /9..$...........
+0003ace0: 2139 0000 2401 0000 c1d2 0100 0000 0000  !9..$...........
 0003acf0: 0100 0000 2400 0000 1500 0000 0000 0000  ....$...........
 0003ad00: 0100 0000 4e01 0000 c1d2 0100 0000 0000  ....N...........
 0003ad10: 0100 0000 2e01 0000 d6d2 0100 0000 0000  ................
-0003ad20: 4a39 0000 2401 0000 d6d2 0100 0000 0000  J9..$...........
+0003ad20: 3c39 0000 2401 0000 d6d2 0100 0000 0000  <9..$...........
 0003ad30: 0100 0000 2400 0000 2500 0000 0000 0000  ....$...%.......
 0003ad40: 0100 0000 4e01 0000 d6d2 0100 0000 0000  ....N...........
 0003ad50: 0100 0000 2e01 0000 fbd2 0100 0000 0000  ................
-0003ad60: 6539 0000 2401 0000 fbd2 0100 0000 0000  e9..$...........
+0003ad60: 5739 0000 2401 0000 fbd2 0100 0000 0000  W9..$...........
 0003ad70: 0100 0000 2400 0000 8800 0000 0000 0000  ....$...........
 0003ad80: 0100 0000 4e01 0000 fbd2 0100 0000 0000  ....N...........
 0003ad90: 0100 0000 2e01 0000 83d3 0100 0000 0000  ................
-0003ada0: 7e39 0000 2401 0000 83d3 0100 0000 0000  ~9..$...........
+0003ada0: 7039 0000 2401 0000 83d3 0100 0000 0000  p9..$...........
 0003adb0: 0100 0000 2400 0000 8800 0000 0000 0000  ....$...........
 0003adc0: 0100 0000 4e01 0000 83d3 0100 0000 0000  ....N...........
 0003add0: 0100 0000 2e01 0000 0bd4 0100 0000 0000  ................
-0003ade0: 9d39 0000 2401 0000 0bd4 0100 0000 0000  .9..$...........
+0003ade0: 8f39 0000 2401 0000 0bd4 0100 0000 0000  .9..$...........
 0003adf0: 0100 0000 2400 0000 8100 0000 0000 0000  ....$...........
 0003ae00: 0100 0000 4e01 0000 0bd4 0100 0000 0000  ....N...........
 0003ae10: 0100 0000 2e01 0000 8cd4 0100 0000 0000  ................
-0003ae20: bd39 0000 2401 0000 8cd4 0100 0000 0000  .9..$...........
+0003ae20: af39 0000 2401 0000 8cd4 0100 0000 0000  .9..$...........
 0003ae30: 0100 0000 2400 0000 8800 0000 0000 0000  ....$...........
 0003ae40: 0100 0000 4e01 0000 8cd4 0100 0000 0000  ....N...........
 0003ae50: 0100 0000 2e01 0000 14d5 0100 0000 0000  ................
-0003ae60: e039 0000 2401 0000 14d5 0100 0000 0000  .9..$...........
+0003ae60: d239 0000 2401 0000 14d5 0100 0000 0000  .9..$...........
 0003ae70: 0100 0000 2400 0000 8800 0000 0000 0000  ....$...........
 0003ae80: 0100 0000 4e01 0000 14d5 0100 0000 0000  ....N...........
 0003ae90: 0100 0000 2e01 0000 9cd5 0100 0000 0000  ................
-0003aea0: 033a 0000 2401 0000 9cd5 0100 0000 0000  .:..$...........
+0003aea0: f539 0000 2401 0000 9cd5 0100 0000 0000  .9..$...........
 0003aeb0: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003aec0: 0100 0000 4e01 0000 9cd5 0100 0000 0000  ....N...........
 0003aed0: 0100 0000 2e01 0000 08d6 0100 0000 0000  ................
-0003aee0: 253a 0000 2401 0000 08d6 0100 0000 0000  %:..$...........
+0003aee0: 173a 0000 2401 0000 08d6 0100 0000 0000  .:..$...........
 0003aef0: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003af00: 0100 0000 4e01 0000 08d6 0100 0000 0000  ....N...........
 0003af10: 0100 0000 2e01 0000 74d6 0100 0000 0000  ........t.......
-0003af20: 413a 0000 2401 0000 74d6 0100 0000 0000  A:..$...t.......
+0003af20: 333a 0000 2401 0000 74d6 0100 0000 0000  3:..$...t.......
 0003af30: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003af40: 0100 0000 4e01 0000 74d6 0100 0000 0000  ....N...t.......
 0003af50: 0100 0000 2e01 0000 e0d6 0100 0000 0000  ................
-0003af60: 693a 0000 2401 0000 e0d6 0100 0000 0000  i:..$...........
+0003af60: 5b3a 0000 2401 0000 e0d6 0100 0000 0000  [:..$...........
 0003af70: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003af80: 0100 0000 4e01 0000 e0d6 0100 0000 0000  ....N...........
 0003af90: 0100 0000 2e01 0000 4cd7 0100 0000 0000  ........L.......
-0003afa0: 8d3a 0000 2401 0000 4cd7 0100 0000 0000  .:..$...L.......
+0003afa0: 7f3a 0000 2401 0000 4cd7 0100 0000 0000  .:..$...L.......
 0003afb0: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003afc0: 0100 0000 4e01 0000 4cd7 0100 0000 0000  ....N...L.......
 0003afd0: 0100 0000 2e01 0000 b8d7 0100 0000 0000  ................
-0003afe0: ae3a 0000 2401 0000 b8d7 0100 0000 0000  .:..$...........
+0003afe0: a03a 0000 2401 0000 b8d7 0100 0000 0000  .:..$...........
 0003aff0: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 0003b000: 0100 0000 4e01 0000 b8d7 0100 0000 0000  ....N...........
 0003b010: 0100 0000 2e01 0000 f8d7 0100 0000 0000  ................
-0003b020: c83a 0000 2401 0000 f8d7 0100 0000 0000  .:..$...........
+0003b020: ba3a 0000 2401 0000 f8d7 0100 0000 0000  .:..$...........
 0003b030: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 0003b040: 0100 0000 4e01 0000 f8d7 0100 0000 0000  ....N...........
 0003b050: 0100 0000 2e01 0000 38d8 0100 0000 0000  ........8.......
-0003b060: e43a 0000 2401 0000 38d8 0100 0000 0000  .:..$...8.......
+0003b060: d63a 0000 2401 0000 38d8 0100 0000 0000  .:..$...8.......
 0003b070: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 0003b080: 0100 0000 4e01 0000 38d8 0100 0000 0000  ....N...8.......
 0003b090: 0100 0000 2e01 0000 78d8 0100 0000 0000  ........x.......
-0003b0a0: fc3a 0000 2401 0000 78d8 0100 0000 0000  .:..$...x.......
+0003b0a0: ee3a 0000 2401 0000 78d8 0100 0000 0000  .:..$...x.......
 0003b0b0: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
 0003b0c0: 0100 0000 4e01 0000 78d8 0100 0000 0000  ....N...x.......
 0003b0d0: 0100 0000 2e01 0000 b8d8 0100 0000 0000  ................
-0003b0e0: 163b 0000 2401 0000 b8d8 0100 0000 0000  .;..$...........
+0003b0e0: 083b 0000 2401 0000 b8d8 0100 0000 0000  .;..$...........
 0003b0f0: 0100 0000 2400 0000 1d04 0000 0000 0000  ....$...........
 0003b100: 0100 0000 4e01 0000 b8d8 0100 0000 0000  ....N...........
 0003b110: 0100 0000 2e01 0000 d5dc 0100 0000 0000  ................
-0003b120: 233b 0000 2401 0000 d5dc 0100 0000 0000  #;..$...........
+0003b120: 153b 0000 2401 0000 d5dc 0100 0000 0000  .;..$...........
 0003b130: 0100 0000 2400 0000 1200 0000 0000 0000  ....$...........
 0003b140: 0100 0000 4e01 0000 d5dc 0100 0000 0000  ....N...........
 0003b150: 0100 0000 2e01 0000 e7dc 0100 0000 0000  ................
-0003b160: 343b 0000 2401 0000 e7dc 0100 0000 0000  4;..$...........
+0003b160: 263b 0000 2401 0000 e7dc 0100 0000 0000  &;..$...........
 0003b170: 0100 0000 2400 0000 0f00 0000 0000 0000  ....$...........
 0003b180: 0100 0000 4e01 0000 e7dc 0100 0000 0000  ....N...........
 0003b190: 0100 0000 2e01 0000 f6dc 0100 0000 0000  ................
-0003b1a0: 483b 0000 2401 0000 f6dc 0100 0000 0000  H;..$...........
+0003b1a0: 3a3b 0000 2401 0000 f6dc 0100 0000 0000  :;..$...........
 0003b1b0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b1c0: 0100 0000 4e01 0000 f6dc 0100 0000 0000  ....N...........
 0003b1d0: 0100 0000 2e01 0000 00dd 0100 0000 0000  ................
-0003b1e0: 5b3b 0000 2401 0000 00dd 0100 0000 0000  [;..$...........
+0003b1e0: 4d3b 0000 2401 0000 00dd 0100 0000 0000  M;..$...........
 0003b1f0: 0100 0000 2400 0000 4b01 0000 0000 0000  ....$...K.......
 0003b200: 0100 0000 4e01 0000 00dd 0100 0000 0000  ....N...........
 0003b210: 0100 0000 2e01 0000 4bde 0100 0000 0000  ........K.......
-0003b220: 773b 0000 2401 0000 4bde 0100 0000 0000  w;..$...K.......
+0003b220: 693b 0000 2401 0000 4bde 0100 0000 0000  i;..$...K.......
 0003b230: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b240: 0100 0000 4e01 0000 4bde 0100 0000 0000  ....N...K.......
 0003b250: 0100 0000 2e01 0000 55de 0100 0000 0000  ........U.......
-0003b260: 8d3b 0000 2401 0000 55de 0100 0000 0000  .;..$...U.......
+0003b260: 7f3b 0000 2401 0000 55de 0100 0000 0000  .;..$...U.......
 0003b270: 0100 0000 2400 0000 9801 0000 0000 0000  ....$...........
 0003b280: 0100 0000 4e01 0000 55de 0100 0000 0000  ....N...U.......
 0003b290: 0100 0000 2e01 0000 eddf 0100 0000 0000  ................
-0003b2a0: ac3b 0000 2401 0000 eddf 0100 0000 0000  .;..$...........
+0003b2a0: 9e3b 0000 2401 0000 eddf 0100 0000 0000  .;..$...........
 0003b2b0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b2c0: 0100 0000 4e01 0000 eddf 0100 0000 0000  ....N...........
 0003b2d0: 0100 0000 2e01 0000 f7df 0100 0000 0000  ................
-0003b2e0: be3b 0000 2401 0000 f7df 0100 0000 0000  .;..$...........
+0003b2e0: b03b 0000 2401 0000 f7df 0100 0000 0000  .;..$...........
 0003b2f0: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 0003b300: 0100 0000 4e01 0000 f7df 0100 0000 0000  ....N...........
 0003b310: 0100 0000 2e01 0000 5ae0 0100 0000 0000  ........Z.......
-0003b320: d93b 0000 2401 0000 5ae0 0100 0000 0000  .;..$...Z.......
+0003b320: cb3b 0000 2401 0000 5ae0 0100 0000 0000  .;..$...Z.......
 0003b330: 0100 0000 2400 0000 2e01 0000 0000 0000  ....$...........
 0003b340: 0100 0000 4e01 0000 5ae0 0100 0000 0000  ....N...Z.......
 0003b350: 0100 0000 2e01 0000 88e1 0100 0000 0000  ................
-0003b360: e43b 0000 2401 0000 88e1 0100 0000 0000  .;..$...........
+0003b360: d63b 0000 2401 0000 88e1 0100 0000 0000  .;..$...........
 0003b370: 0100 0000 2400 0000 8700 0000 0000 0000  ....$...........
 0003b380: 0100 0000 4e01 0000 88e1 0100 0000 0000  ....N...........
 0003b390: 0100 0000 2e01 0000 0fe2 0100 0000 0000  ................
-0003b3a0: fa3b 0000 2401 0000 0fe2 0100 0000 0000  .;..$...........
+0003b3a0: ec3b 0000 2401 0000 0fe2 0100 0000 0000  .;..$...........
 0003b3b0: 0100 0000 2400 0000 2900 0000 0000 0000  ....$...).......
 0003b3c0: 0100 0000 4e01 0000 0fe2 0100 0000 0000  ....N...........
 0003b3d0: 0100 0000 2e01 0000 38e2 0100 0000 0000  ........8.......
-0003b3e0: 0d3c 0000 2401 0000 38e2 0100 0000 0000  .<..$...8.......
+0003b3e0: ff3b 0000 2401 0000 38e2 0100 0000 0000  .;..$...8.......
 0003b3f0: 0100 0000 2400 0000 4b00 0000 0000 0000  ....$...K.......
 0003b400: 0100 0000 4e01 0000 38e2 0100 0000 0000  ....N...8.......
 0003b410: 0100 0000 2e01 0000 83e2 0100 0000 0000  ................
-0003b420: 1f3c 0000 2401 0000 83e2 0100 0000 0000  .<..$...........
+0003b420: 113c 0000 2401 0000 83e2 0100 0000 0000  .<..$...........
 0003b430: 0100 0000 2400 0000 6200 0000 0000 0000  ....$...b.......
 0003b440: 0100 0000 4e01 0000 83e2 0100 0000 0000  ....N...........
 0003b450: 0100 0000 2e01 0000 e5e2 0100 0000 0000  ................
-0003b460: 2e3c 0000 2401 0000 e5e2 0100 0000 0000  .<..$...........
+0003b460: 203c 0000 2401 0000 e5e2 0100 0000 0000   <..$...........
 0003b470: 0100 0000 2400 0000 0f01 0000 0000 0000  ....$...........
 0003b480: 0100 0000 4e01 0000 e5e2 0100 0000 0000  ....N...........
 0003b490: 0100 0000 2e01 0000 f4e3 0100 0000 0000  ................
-0003b4a0: 413c 0000 2401 0000 f4e3 0100 0000 0000  A<..$...........
+0003b4a0: 333c 0000 2401 0000 f4e3 0100 0000 0000  3<..$...........
 0003b4b0: 0100 0000 2400 0000 1001 0000 0000 0000  ....$...........
 0003b4c0: 0100 0000 4e01 0000 f4e3 0100 0000 0000  ....N...........
 0003b4d0: 0100 0000 2e01 0000 04e5 0100 0000 0000  ................
-0003b4e0: 543c 0000 2401 0000 04e5 0100 0000 0000  T<..$...........
+0003b4e0: 463c 0000 2401 0000 04e5 0100 0000 0000  F<..$...........
 0003b4f0: 0100 0000 2400 0000 1b02 0000 0000 0000  ....$...........
 0003b500: 0100 0000 4e01 0000 04e5 0100 0000 0000  ....N...........
 0003b510: 0100 0000 2e01 0000 1fe7 0100 0000 0000  ................
-0003b520: 693c 0000 2401 0000 1fe7 0100 0000 0000  i<..$...........
+0003b520: 5b3c 0000 2401 0000 1fe7 0100 0000 0000  [<..$...........
 0003b530: 0100 0000 2400 0000 8400 0000 0000 0000  ....$...........
 0003b540: 0100 0000 4e01 0000 1fe7 0100 0000 0000  ....N...........
 0003b550: 0100 0000 2e01 0000 a3e7 0100 0000 0000  ................
-0003b560: 7a3c 0000 2401 0000 a3e7 0100 0000 0000  z<..$...........
+0003b560: 6c3c 0000 2401 0000 a3e7 0100 0000 0000  l<..$...........
 0003b570: 0100 0000 2400 0000 9200 0000 0000 0000  ....$...........
 0003b580: 0100 0000 4e01 0000 a3e7 0100 0000 0000  ....N...........
 0003b590: 0100 0000 2e01 0000 35e8 0100 0000 0000  ........5.......
-0003b5a0: 933c 0000 2401 0000 35e8 0100 0000 0000  .<..$...5.......
+0003b5a0: 853c 0000 2401 0000 35e8 0100 0000 0000  .<..$...5.......
 0003b5b0: 0100 0000 2400 0000 9100 0000 0000 0000  ....$...........
 0003b5c0: 0100 0000 4e01 0000 35e8 0100 0000 0000  ....N...5.......
 0003b5d0: 0100 0000 2e01 0000 c6e8 0100 0000 0000  ................
-0003b5e0: ad3c 0000 2401 0000 c6e8 0100 0000 0000  .<..$...........
+0003b5e0: 9f3c 0000 2401 0000 c6e8 0100 0000 0000  .<..$...........
 0003b5f0: 0100 0000 2400 0000 1c00 0000 0000 0000  ....$...........
 0003b600: 0100 0000 4e01 0000 c6e8 0100 0000 0000  ....N...........
 0003b610: 0100 0000 2e01 0000 e2e8 0100 0000 0000  ................
-0003b620: c23c 0000 2401 0000 e2e8 0100 0000 0000  .<..$...........
+0003b620: b43c 0000 2401 0000 e2e8 0100 0000 0000  .<..$...........
 0003b630: 0100 0000 2400 0000 9300 0000 0000 0000  ....$...........
 0003b640: 0100 0000 4e01 0000 e2e8 0100 0000 0000  ....N...........
 0003b650: 0100 0000 2e01 0000 75e9 0100 0000 0000  ........u.......
-0003b660: e23c 0000 2401 0000 75e9 0100 0000 0000  .<..$...u.......
+0003b660: d43c 0000 2401 0000 75e9 0100 0000 0000  .<..$...u.......
 0003b670: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b680: 0100 0000 4e01 0000 75e9 0100 0000 0000  ....N...u.......
 0003b690: 0100 0000 2e01 0000 7fe9 0100 0000 0000  ................
-0003b6a0: f93c 0000 2401 0000 7fe9 0100 0000 0000  .<..$...........
+0003b6a0: eb3c 0000 2401 0000 7fe9 0100 0000 0000  .<..$...........
 0003b6b0: 0100 0000 2400 0000 3900 0000 0000 0000  ....$...9.......
 0003b6c0: 0100 0000 4e01 0000 7fe9 0100 0000 0000  ....N...........
 0003b6d0: 0100 0000 2e01 0000 b8e9 0100 0000 0000  ................
-0003b6e0: 153d 0000 2401 0000 b8e9 0100 0000 0000  .=..$...........
+0003b6e0: 073d 0000 2401 0000 b8e9 0100 0000 0000  .=..$...........
 0003b6f0: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 0003b700: 0100 0000 4e01 0000 b8e9 0100 0000 0000  ....N...........
 0003b710: 0100 0000 2e01 0000 1bea 0100 0000 0000  ................
-0003b720: 2f3d 0000 2401 0000 1bea 0100 0000 0000  /=..$...........
+0003b720: 213d 0000 2401 0000 1bea 0100 0000 0000  !=..$...........
 0003b730: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b740: 0100 0000 4e01 0000 1bea 0100 0000 0000  ....N...........
 0003b750: 0100 0000 2e01 0000 25ea 0100 0000 0000  ........%.......
-0003b760: 523d 0000 2401 0000 25ea 0100 0000 0000  R=..$...%.......
+0003b760: 443d 0000 2401 0000 25ea 0100 0000 0000  D=..$...%.......
 0003b770: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003b780: 0100 0000 4e01 0000 25ea 0100 0000 0000  ....N...%.......
 0003b790: 0100 0000 2e01 0000 2fea 0100 0000 0000  ......../.......
-0003b7a0: 6b3d 0000 2401 0000 2fea 0100 0000 0000  k=..$.../.......
+0003b7a0: 5d3d 0000 2401 0000 2fea 0100 0000 0000  ]=..$.../.......
 0003b7b0: 0100 0000 2400 0000 2a00 0000 0000 0000  ....$...*.......
 0003b7c0: 0100 0000 4e01 0000 2fea 0100 0000 0000  ....N.../.......
 0003b7d0: 0100 0000 2e01 0000 59ea 0100 0000 0000  ........Y.......
-0003b7e0: 833d 0000 2401 0000 59ea 0100 0000 0000  .=..$...Y.......
+0003b7e0: 753d 0000 2401 0000 59ea 0100 0000 0000  u=..$...Y.......
 0003b7f0: 0100 0000 2400 0000 a501 0000 0000 0000  ....$...........
 0003b800: 0100 0000 4e01 0000 59ea 0100 0000 0000  ....N...Y.......
 0003b810: 0100 0000 2e01 0000 feeb 0100 0000 0000  ................
-0003b820: a43d 0000 2401 0000 feeb 0100 0000 0000  .=..$...........
+0003b820: 963d 0000 2401 0000 feeb 0100 0000 0000  .=..$...........
 0003b830: 0100 0000 2400 0000 4d00 0000 0000 0000  ....$...M.......
 0003b840: 0100 0000 4e01 0000 feeb 0100 0000 0000  ....N...........
 0003b850: 0100 0000 2e01 0000 4bec 0100 0000 0000  ........K.......
-0003b860: ba3d 0000 2401 0000 4bec 0100 0000 0000  .=..$...K.......
+0003b860: ac3d 0000 2401 0000 4bec 0100 0000 0000  .=..$...K.......
 0003b870: 0100 0000 2400 0000 4900 0000 0000 0000  ....$...I.......
 0003b880: 0100 0000 4e01 0000 4bec 0100 0000 0000  ....N...K.......
 0003b890: 0100 0000 2e01 0000 94ec 0100 0000 0000  ................
-0003b8a0: d93d 0000 2401 0000 94ec 0100 0000 0000  .=..$...........
+0003b8a0: cb3d 0000 2401 0000 94ec 0100 0000 0000  .=..$...........
 0003b8b0: 0100 0000 2400 0000 fd00 0000 0000 0000  ....$...........
 0003b8c0: 0100 0000 4e01 0000 94ec 0100 0000 0000  ....N...........
 0003b8d0: 0100 0000 2e01 0000 91ed 0100 0000 0000  ................
-0003b8e0: ea3d 0000 2401 0000 91ed 0100 0000 0000  .=..$...........
+0003b8e0: dc3d 0000 2401 0000 91ed 0100 0000 0000  .=..$...........
 0003b8f0: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003b900: 0100 0000 4e01 0000 91ed 0100 0000 0000  ....N...........
 0003b910: 0100 0000 2e01 0000 fded 0100 0000 0000  ................
-0003b920: 0c3e 0000 2401 0000 fded 0100 0000 0000  .>..$...........
+0003b920: fe3d 0000 2401 0000 fded 0100 0000 0000  .=..$...........
 0003b930: 0100 0000 2400 0000 2500 0000 0000 0000  ....$...%.......
 0003b940: 0100 0000 4e01 0000 fded 0100 0000 0000  ....N...........
 0003b950: 0100 0000 2e01 0000 22ee 0100 0000 0000  ........".......
-0003b960: 223e 0000 2401 0000 22ee 0100 0000 0000  ">..$...".......
+0003b960: 143e 0000 2401 0000 22ee 0100 0000 0000  .>..$...".......
 0003b970: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
 0003b980: 0100 0000 4e01 0000 22ee 0100 0000 0000  ....N...".......
 0003b990: 0100 0000 2e01 0000 8eee 0100 0000 0000  ................
-0003b9a0: 3b3e 0000 2401 0000 8eee 0100 0000 0000  ;>..$...........
+0003b9a0: 2d3e 0000 2401 0000 8eee 0100 0000 0000  ->..$...........
 0003b9b0: 0100 0000 2400 0000 8603 0000 0000 0000  ....$...........
 0003b9c0: 0100 0000 4e01 0000 8eee 0100 0000 0000  ....N...........
 0003b9d0: 0100 0000 2e01 0000 14f2 0100 0000 0000  ................
-0003b9e0: 4f3e 0000 2401 0000 14f2 0100 0000 0000  O>..$...........
+0003b9e0: 413e 0000 2401 0000 14f2 0100 0000 0000  A>..$...........
 0003b9f0: 0100 0000 2400 0000 8e00 0000 0000 0000  ....$...........
 0003ba00: 0100 0000 4e01 0000 14f2 0100 0000 0000  ....N...........
 0003ba10: 0100 0000 2e01 0000 a2f2 0100 0000 0000  ................
-0003ba20: 653e 0000 2401 0000 a2f2 0100 0000 0000  e>..$...........
+0003ba20: 573e 0000 2401 0000 a2f2 0100 0000 0000  W>..$...........
 0003ba30: 0100 0000 2400 0000 c700 0000 0000 0000  ....$...........
 0003ba40: 0100 0000 4e01 0000 a2f2 0100 0000 0000  ....N...........
 0003ba50: 0100 0000 2e01 0000 69f3 0100 0000 0000  ........i.......
-0003ba60: 7b3e 0000 2401 0000 69f3 0100 0000 0000  {>..$...i.......
+0003ba60: 6d3e 0000 2401 0000 69f3 0100 0000 0000  m>..$...i.......
 0003ba70: 0100 0000 2400 0000 4b00 0000 0000 0000  ....$...K.......
 0003ba80: 0100 0000 4e01 0000 69f3 0100 0000 0000  ....N...i.......
 0003ba90: 0100 0000 2e01 0000 b4f3 0100 0000 0000  ................
-0003baa0: 8c3e 0000 2401 0000 b4f3 0100 0000 0000  .>..$...........
+0003baa0: 7e3e 0000 2401 0000 b4f3 0100 0000 0000  ~>..$...........
 0003bab0: 0100 0000 2400 0000 3405 0000 0000 0000  ....$...4.......
 0003bac0: 0100 0000 4e01 0000 b4f3 0100 0000 0000  ....N...........
 0003bad0: 0100 0000 2e01 0000 e8f8 0100 0000 0000  ................
-0003bae0: a03e 0000 2401 0000 e8f8 0100 0000 0000  .>..$...........
+0003bae0: 923e 0000 2401 0000 e8f8 0100 0000 0000  .>..$...........
 0003baf0: 0100 0000 2400 0000 0d00 0000 0000 0000  ....$...........
 0003bb00: 0100 0000 4e01 0000 e8f8 0100 0000 0000  ....N...........
 0003bb10: 0100 0000 2e01 0000 f5f8 0100 0000 0000  ................
-0003bb20: ac3e 0000 2401 0000 f5f8 0100 0000 0000  .>..$...........
+0003bb20: 9e3e 0000 2401 0000 f5f8 0100 0000 0000  .>..$...........
 0003bb30: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003bb40: 0100 0000 4e01 0000 f5f8 0100 0000 0000  ....N...........
 0003bb50: 0100 0000 2e01 0000 fff8 0100 0000 0000  ................
-0003bb60: b93e 0000 2401 0000 fff8 0100 0000 0000  .>..$...........
+0003bb60: ab3e 0000 2401 0000 fff8 0100 0000 0000  .>..$...........
 0003bb70: 0100 0000 2400 0000 2100 0000 0000 0000  ....$...!.......
 0003bb80: 0100 0000 4e01 0000 fff8 0100 0000 0000  ....N...........
 0003bb90: 0100 0000 2e01 0000 20f9 0100 0000 0000  ........ .......
-0003bba0: cc3e 0000 2401 0000 20f9 0100 0000 0000  .>..$... .......
+0003bba0: be3e 0000 2401 0000 20f9 0100 0000 0000  .>..$... .......
 0003bbb0: 0100 0000 2400 0000 1200 0000 0000 0000  ....$...........
 0003bbc0: 0100 0000 4e01 0000 20f9 0100 0000 0000  ....N... .......
 0003bbd0: 0100 0000 2e01 0000 32f9 0100 0000 0000  ........2.......
-0003bbe0: e03e 0000 2401 0000 32f9 0100 0000 0000  .>..$...2.......
+0003bbe0: d23e 0000 2401 0000 32f9 0100 0000 0000  .>..$...2.......
 0003bbf0: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003bc00: 0100 0000 4e01 0000 32f9 0100 0000 0000  ....N...2.......
 0003bc10: 0100 0000 2e01 0000 3cf9 0100 0000 0000  ........<.......
-0003bc20: f63e 0000 2401 0000 3cf9 0100 0000 0000  .>..$...<.......
+0003bc20: e83e 0000 2401 0000 3cf9 0100 0000 0000  .>..$...<.......
 0003bc30: 0100 0000 2400 0000 4602 0000 0000 0000  ....$...F.......
 0003bc40: 0100 0000 4e01 0000 3cf9 0100 0000 0000  ....N...<.......
 0003bc50: 0100 0000 2e01 0000 82fb 0100 0000 0000  ................
-0003bc60: 093f 0000 2401 0000 82fb 0100 0000 0000  .?..$...........
+0003bc60: fb3e 0000 2401 0000 82fb 0100 0000 0000  .>..$...........
 0003bc70: 0100 0000 2400 0000 5c00 0000 0000 0000  ....$...\.......
 0003bc80: 0100 0000 4e01 0000 82fb 0100 0000 0000  ....N...........
 0003bc90: 0100 0000 2e01 0000 defb 0100 0000 0000  ................
-0003bca0: 163f 0000 2401 0000 defb 0100 0000 0000  .?..$...........
+0003bca0: 083f 0000 2401 0000 defb 0100 0000 0000  .?..$...........
 0003bcb0: 0100 0000 2400 0000 a200 0000 0000 0000  ....$...........
 0003bcc0: 0100 0000 4e01 0000 defb 0100 0000 0000  ....N...........
 0003bcd0: 0100 0000 2e01 0000 80fc 0100 0000 0000  ................
-0003bce0: 273f 0000 2401 0000 80fc 0100 0000 0000  '?..$...........
+0003bce0: 193f 0000 2401 0000 80fc 0100 0000 0000  .?..$...........
 0003bcf0: 0100 0000 2400 0000 9302 0000 0000 0000  ....$...........
 0003bd00: 0100 0000 4e01 0000 80fc 0100 0000 0000  ....N...........
 0003bd10: 0100 0000 2e01 0000 13ff 0100 0000 0000  ................
-0003bd20: 393f 0000 2401 0000 13ff 0100 0000 0000  9?..$...........
+0003bd20: 2b3f 0000 2401 0000 13ff 0100 0000 0000  +?..$...........
 0003bd30: 0100 0000 2400 0000 5700 0000 0000 0000  ....$...W.......
 0003bd40: 0100 0000 4e01 0000 13ff 0100 0000 0000  ....N...........
 0003bd50: 0100 0000 2e01 0000 6aff 0100 0000 0000  ........j.......
-0003bd60: 443f 0000 2401 0000 6aff 0100 0000 0000  D?..$...j.......
+0003bd60: 363f 0000 2401 0000 6aff 0100 0000 0000  6?..$...j.......
 0003bd70: 0100 0000 2400 0000 7c01 0000 0000 0000  ....$...|.......
 0003bd80: 0100 0000 4e01 0000 6aff 0100 0000 0000  ....N...j.......
 0003bd90: 0100 0000 2e01 0000 e600 0200 0000 0000  ................
-0003bda0: 513f 0000 2401 0000 e600 0200 0000 0000  Q?..$...........
+0003bda0: 433f 0000 2401 0000 e600 0200 0000 0000  C?..$...........
 0003bdb0: 0100 0000 2400 0000 6600 0000 0000 0000  ....$...f.......
 0003bdc0: 0100 0000 4e01 0000 e600 0200 0000 0000  ....N...........
 0003bdd0: 0100 0000 2e01 0000 4c01 0200 0000 0000  ........L.......
-0003bde0: 613f 0000 2401 0000 4c01 0200 0000 0000  a?..$...L.......
+0003bde0: 533f 0000 2401 0000 4c01 0200 0000 0000  S?..$...L.......
 0003bdf0: 0100 0000 2400 0000 3a08 0000 0000 0000  ....$...:.......
 0003be00: 0100 0000 4e01 0000 4c01 0200 0000 0000  ....N...L.......
 0003be10: 0100 0000 2e01 0000 8609 0200 0000 0000  ................
-0003be20: 6f3f 0000 2401 0000 8609 0200 0000 0000  o?..$...........
+0003be20: 613f 0000 2401 0000 8609 0200 0000 0000  a?..$...........
 0003be30: 0100 0000 2400 0000 ca02 0000 0000 0000  ....$...........
 0003be40: 0100 0000 4e01 0000 8609 0200 0000 0000  ....N...........
 0003be50: 0100 0000 2e01 0000 500c 0200 0000 0000  ........P.......
-0003be60: 7d3f 0000 2401 0000 500c 0200 0000 0000  }?..$...P.......
+0003be60: 6f3f 0000 2401 0000 500c 0200 0000 0000  o?..$...P.......
 0003be70: 0100 0000 2400 0000 dd02 0000 0000 0000  ....$...........
 0003be80: 0100 0000 4e01 0000 500c 0200 0000 0000  ....N...P.......
 0003be90: 0100 0000 2e01 0000 2d0f 0200 0000 0000  ........-.......
-0003bea0: 8b3f 0000 2401 0000 2d0f 0200 0000 0000  .?..$...-.......
+0003bea0: 7d3f 0000 2401 0000 2d0f 0200 0000 0000  }?..$...-.......
 0003beb0: 0100 0000 2400 0000 a707 0000 0000 0000  ....$...........
 0003bec0: 0100 0000 4e01 0000 2d0f 0200 0000 0000  ....N...-.......
 0003bed0: 0100 0000 2e01 0000 d416 0200 0000 0000  ................
-0003bee0: 9e3f 0000 2401 0000 d416 0200 0000 0000  .?..$...........
+0003bee0: 903f 0000 2401 0000 d416 0200 0000 0000  .?..$...........
 0003bef0: 0100 0000 2400 0000 9a08 0000 0000 0000  ....$...........
 0003bf00: 0100 0000 4e01 0000 d416 0200 0000 0000  ....N...........
 0003bf10: 0100 0000 2e01 0000 6e1f 0200 0000 0000  ........n.......
-0003bf20: ae3f 0000 2401 0000 6e1f 0200 0000 0000  .?..$...n.......
+0003bf20: a03f 0000 2401 0000 6e1f 0200 0000 0000  .?..$...n.......
 0003bf30: 0100 0000 2400 0000 d303 0000 0000 0000  ....$...........
 0003bf40: 0100 0000 4e01 0000 6e1f 0200 0000 0000  ....N...n.......
 0003bf50: 0100 0000 2e01 0000 4123 0200 0000 0000  ........A#......
-0003bf60: bb3f 0000 2401 0000 4123 0200 0000 0000  .?..$...A#......
+0003bf60: ad3f 0000 2401 0000 4123 0200 0000 0000  .?..$...A#......
 0003bf70: 0100 0000 2400 0000 9719 0000 0000 0000  ....$...........
 0003bf80: 0100 0000 4e01 0000 4123 0200 0000 0000  ....N...A#......
 0003bf90: 0100 0000 2e01 0000 d83c 0200 0000 0000  .........<......
-0003bfa0: ca3f 0000 2401 0000 d83c 0200 0000 0000  .?..$....<......
+0003bfa0: bc3f 0000 2401 0000 d83c 0200 0000 0000  .?..$....<......
 0003bfb0: 0100 0000 2400 0000 4600 0000 0000 0000  ....$...F.......
 0003bfc0: 0100 0000 4e01 0000 d83c 0200 0000 0000  ....N....<......
 0003bfd0: 0100 0000 2e01 0000 1e3d 0200 0000 0000  .........=......
-0003bfe0: d83f 0000 2401 0000 1e3d 0200 0000 0000  .?..$....=......
+0003bfe0: ca3f 0000 2401 0000 1e3d 0200 0000 0000  .?..$....=......
 0003bff0: 0100 0000 2400 0000 8c00 0000 0000 0000  ....$...........
 0003c000: 0100 0000 4e01 0000 1e3d 0200 0000 0000  ....N....=......
 0003c010: 0100 0000 2e01 0000 aa3d 0200 0000 0000  .........=......
-0003c020: e93f 0000 2401 0000 aa3d 0200 0000 0000  .?..$....=......
+0003c020: db3f 0000 2401 0000 aa3d 0200 0000 0000  .?..$....=......
 0003c030: 0100 0000 2400 0000 5f00 0000 0000 0000  ....$..._.......
 0003c040: 0100 0000 4e01 0000 aa3d 0200 0000 0000  ....N....=......
 0003c050: 0100 0000 2e01 0000 093e 0200 0000 0000  .........>......
-0003c060: f63f 0000 2401 0000 093e 0200 0000 0000  .?..$....>......
+0003c060: e83f 0000 2401 0000 093e 0200 0000 0000  .?..$....>......
 0003c070: 0100 0000 2400 0000 0600 0000 0000 0000  ....$...........
 0003c080: 0100 0000 4e01 0000 093e 0200 0000 0000  ....N....>......
-0003c090: 0140 0000 2000 0000 0000 0000 0000 0000  .@.. ...........
-0003c0a0: 1b40 0000 2000 0000 0000 0000 0000 0000  .@.. ...........
+0003c090: f33f 0000 2000 0000 0000 0000 0000 0000  .?.. ...........
+0003c0a0: 0d40 0000 2000 0000 0000 0000 0000 0000  .@.. ...........
 0003c0b0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-0003c0c0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-0003c0d0: 2f40 0000 6400 0000 0000 0000 0000 0000  /@..d...........
-0003c0e0: 3740 0000 6603 0100 8835 3864 0000 0000  7@..f....58d....
+0003c0c0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+0003c0d0: 2140 0000 6400 0000 0000 0000 0000 0000  !@..d...........
+0003c0e0: 2940 0000 6603 0100 bfb1 3d64 0000 0000  )@..f.....=d....
 0003c0f0: 0100 0000 2e01 0000 103e 0200 0000 0000  .........>......
-0003c100: ca40 0000 2401 0000 103e 0200 0000 0000  .@..$....>......
+0003c100: bc40 0000 2401 0000 103e 0200 0000 0000  .@..$....>......
 0003c110: 0100 0000 2400 0000 3200 0000 0000 0000  ....$...2.......
 0003c120: 0100 0000 4e01 0000 103e 0200 0000 0000  ....N....>......
 0003c130: 0100 0000 2e01 0000 423e 0200 0000 0000  ........B>......
-0003c140: d740 0000 2401 0000 423e 0200 0000 0000  .@..$...B>......
+0003c140: c940 0000 2401 0000 423e 0200 0000 0000  .@..$...B>......
 0003c150: 0100 0000 2400 0000 2b00 0000 0000 0000  ....$...+.......
 0003c160: 0100 0000 4e01 0000 423e 0200 0000 0000  ....N...B>......
 0003c170: 0100 0000 2e01 0000 6d3e 0200 0000 0000  ........m>......
-0003c180: e540 0000 2401 0000 6d3e 0200 0000 0000  .@..$...m>......
+0003c180: d740 0000 2401 0000 6d3e 0200 0000 0000  .@..$...m>......
 0003c190: 0100 0000 2400 0000 0e00 0000 0000 0000  ....$...........
 0003c1a0: 0100 0000 4e01 0000 6d3e 0200 0000 0000  ....N...m>......
 0003c1b0: 0100 0000 2e01 0000 7b3e 0200 0000 0000  ........{>......
-0003c1c0: f340 0000 2401 0000 7b3e 0200 0000 0000  .@..$...{>......
+0003c1c0: e540 0000 2401 0000 7b3e 0200 0000 0000  .@..$...{>......
 0003c1d0: 0100 0000 2400 0000 0e00 0000 0000 0000  ....$...........
 0003c1e0: 0100 0000 4e01 0000 7b3e 0200 0000 0000  ....N...{>......
 0003c1f0: 0100 0000 2e01 0000 893e 0200 0000 0000  .........>......
-0003c200: 0141 0000 2401 0000 893e 0200 0000 0000  .A..$....>......
+0003c200: f340 0000 2401 0000 893e 0200 0000 0000  .@..$....>......
 0003c210: 0100 0000 2400 0000 1800 0000 0000 0000  ....$...........
 0003c220: 0100 0000 4e01 0000 893e 0200 0000 0000  ....N....>......
 0003c230: 0100 0000 2e01 0000 a13e 0200 0000 0000  .........>......
-0003c240: 0f41 0000 2401 0000 a13e 0200 0000 0000  .A..$....>......
+0003c240: 0141 0000 2401 0000 a13e 0200 0000 0000  .A..$....>......
 0003c250: 0100 0000 2400 0000 3400 0000 0000 0000  ....$...4.......
 0003c260: 0100 0000 4e01 0000 a13e 0200 0000 0000  ....N....>......
 0003c270: 0100 0000 2e01 0000 d53e 0200 0000 0000  .........>......
-0003c280: 1b41 0000 2401 0000 d53e 0200 0000 0000  .A..$....>......
+0003c280: 0d41 0000 2401 0000 d53e 0200 0000 0000  .A..$....>......
 0003c290: 0100 0000 2400 0000 9800 0000 0000 0000  ....$...........
 0003c2a0: 0100 0000 4e01 0000 d53e 0200 0000 0000  ....N....>......
 0003c2b0: 0100 0000 2e01 0000 6d3f 0200 0000 0000  ........m?......
-0003c2c0: 2841 0000 2401 0000 6d3f 0200 0000 0000  (A..$...m?......
+0003c2c0: 1a41 0000 2401 0000 6d3f 0200 0000 0000  .A..$...m?......
 0003c2d0: 0100 0000 2400 0000 4400 0000 0000 0000  ....$...D.......
 0003c2e0: 0100 0000 4e01 0000 6d3f 0200 0000 0000  ....N...m?......
 0003c2f0: 0100 0000 2e01 0000 b13f 0200 0000 0000  .........?......
-0003c300: 3341 0000 2401 0000 b13f 0200 0000 0000  3A..$....?......
+0003c300: 2541 0000 2401 0000 b13f 0200 0000 0000  %A..$....?......
 0003c310: 0100 0000 2400 0000 c900 0000 0000 0000  ....$...........
 0003c320: 0100 0000 4e01 0000 b13f 0200 0000 0000  ....N....?......
 0003c330: 0100 0000 2e01 0000 7a40 0200 0000 0000  ........z@......
-0003c340: 3f41 0000 2401 0000 7a40 0200 0000 0000  ?A..$...z@......
+0003c340: 3141 0000 2401 0000 7a40 0200 0000 0000  1A..$...z@......
 0003c350: 0100 0000 2400 0000 4400 0000 0000 0000  ....$...D.......
 0003c360: 0100 0000 4e01 0000 7a40 0200 0000 0000  ....N...z@......
 0003c370: 0100 0000 2e01 0000 be40 0200 0000 0000  .........@......
-0003c380: 4941 0000 2401 0000 be40 0200 0000 0000  IA..$....@......
+0003c380: 3b41 0000 2401 0000 be40 0200 0000 0000  ;A..$....@......
 0003c390: 0100 0000 2400 0000 7d00 0000 0000 0000  ....$...}.......
 0003c3a0: 0100 0000 4e01 0000 be40 0200 0000 0000  ....N....@......
 0003c3b0: 0100 0000 2e01 0000 3b41 0200 0000 0000  ........;A......
-0003c3c0: 5541 0000 2401 0000 3b41 0200 0000 0000  UA..$...;A......
+0003c3c0: 4741 0000 2401 0000 3b41 0200 0000 0000  GA..$...;A......
 0003c3d0: 0100 0000 2400 0000 ac00 0000 0000 0000  ....$...........
 0003c3e0: 0100 0000 4e01 0000 3b41 0200 0000 0000  ....N...;A......
 0003c3f0: 0100 0000 2e01 0000 e741 0200 0000 0000  .........A......
-0003c400: 6241 0000 2401 0000 e741 0200 0000 0000  bA..$....A......
+0003c400: 5441 0000 2401 0000 e741 0200 0000 0000  TA..$....A......
 0003c410: 0100 0000 2400 0000 5300 0000 0000 0000  ....$...S.......
 0003c420: 0100 0000 4e01 0000 e741 0200 0000 0000  ....N....A......
 0003c430: 0100 0000 2e01 0000 3a42 0200 0000 0000  ........:B......
-0003c440: 6d41 0000 2401 0000 3a42 0200 0000 0000  mA..$...:B......
+0003c440: 5f41 0000 2401 0000 3a42 0200 0000 0000  _A..$...:B......
 0003c450: 0100 0000 2400 0000 5500 0000 0000 0000  ....$...U.......
 0003c460: 0100 0000 4e01 0000 3a42 0200 0000 0000  ....N...:B......
 0003c470: 0100 0000 2e01 0000 8f42 0200 0000 0000  .........B......
-0003c480: 8441 0000 2401 0000 8f42 0200 0000 0000  .A..$....B......
+0003c480: 7641 0000 2401 0000 8f42 0200 0000 0000  vA..$....B......
 0003c490: 0100 0000 2400 0000 4400 0000 0000 0000  ....$...D.......
 0003c4a0: 0100 0000 4e01 0000 8f42 0200 0000 0000  ....N....B......
 0003c4b0: 0100 0000 2e01 0000 d342 0200 0000 0000  .........B......
-0003c4c0: 9941 0000 2401 0000 d342 0200 0000 0000  .A..$....B......
+0003c4c0: 8b41 0000 2401 0000 d342 0200 0000 0000  .A..$....B......
 0003c4d0: 0100 0000 2400 0000 4f01 0000 0000 0000  ....$...O.......
 0003c4e0: 0100 0000 4e01 0000 d342 0200 0000 0000  ....N....B......
 0003c4f0: 0100 0000 2e01 0000 2244 0200 0000 0000  ........"D......
-0003c500: a641 0000 2401 0000 2244 0200 0000 0000  .A..$..."D......
+0003c500: 9841 0000 2401 0000 2244 0200 0000 0000  .A..$..."D......
 0003c510: 0100 0000 2400 0000 6300 0000 0000 0000  ....$...c.......
 0003c520: 0100 0000 4e01 0000 2244 0200 0000 0000  ....N..."D......
 0003c530: 0100 0000 2e01 0000 8544 0200 0000 0000  .........D......
-0003c540: b141 0000 2401 0000 8544 0200 0000 0000  .A..$....D......
+0003c540: a341 0000 2401 0000 8544 0200 0000 0000  .A..$....D......
 0003c550: 0100 0000 2400 0000 0a00 0000 0000 0000  ....$...........
 0003c560: 0100 0000 4e01 0000 8544 0200 0000 0000  ....N....D......
 0003c570: 0100 0000 2e01 0000 8f44 0200 0000 0000  .........D......
-0003c580: c141 0000 2401 0000 8f44 0200 0000 0000  .A..$....D......
+0003c580: b341 0000 2401 0000 8f44 0200 0000 0000  .A..$....D......
 0003c590: 0100 0000 2400 0000 2900 0000 0000 0000  ....$...).......
 0003c5a0: 0100 0000 4e01 0000 8f44 0200 0000 0000  ....N....D......
 0003c5b0: 0100 0000 2e01 0000 b844 0200 0000 0000  .........D......
-0003c5c0: cf41 0000 2401 0000 b844 0200 0000 0000  .A..$....D......
+0003c5c0: c141 0000 2401 0000 b844 0200 0000 0000  .A..$....D......
 0003c5d0: 0100 0000 2400 0000 1000 0000 0000 0000  ....$...........
 0003c5e0: 0100 0000 4e01 0000 b844 0200 0000 0000  ....N....D......
 0003c5f0: 0100 0000 2e01 0000 c844 0200 0000 0000  .........D......
-0003c600: df41 0000 2401 0000 c844 0200 0000 0000  .A..$....D......
+0003c600: d141 0000 2401 0000 c844 0200 0000 0000  .A..$....D......
 0003c610: 0100 0000 2400 0000 3800 0000 0000 0000  ....$...8.......
 0003c620: 0100 0000 4e01 0000 c844 0200 0000 0000  ....N....D......
 0003c630: 0100 0000 2e01 0000 0045 0200 0000 0000  .........E......
-0003c640: ed41 0000 2401 0000 0045 0200 0000 0000  .A..$....E......
+0003c640: df41 0000 2401 0000 0045 0200 0000 0000  .A..$....E......
 0003c650: 0100 0000 2400 0000 3500 0000 0000 0000  ....$...5.......
 0003c660: 0100 0000 4e01 0000 0045 0200 0000 0000  ....N....E......
 0003c670: 0100 0000 2e01 0000 3545 0200 0000 0000  ........5E......
-0003c680: f441 0000 2401 0000 3545 0200 0000 0000  .A..$...5E......
+0003c680: e641 0000 2401 0000 3545 0200 0000 0000  .A..$...5E......
 0003c690: 0100 0000 2400 0000 3302 0000 0000 0000  ....$...3.......
 0003c6a0: 0100 0000 4e01 0000 3545 0200 0000 0000  ....N...5E......
 0003c6b0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
-0003c6c0: 7f22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-0003c6d0: 0242 0000 6400 0000 0000 0000 0000 0000  .B..d...........
-0003c6e0: 0c42 0000 6603 0100 8735 3864 0000 0000  .B..f....58d....
+0003c6c0: 7122 0000 6400 0000 0000 0000 0000 0000  q"..d...........
+0003c6d0: f441 0000 6400 0000 0000 0000 0000 0000  .A..d...........
+0003c6e0: fe41 0000 6603 0100 beb1 3d64 0000 0000  .A..f.....=d....
 0003c6f0: 0100 0000 2e01 0000 6847 0200 0000 0000  ........hG......
-0003c700: a142 0000 2401 0000 6847 0200 0000 0000  .B..$...hG......
+0003c700: 9342 0000 2401 0000 6847 0200 0000 0000  .B..$...hG......
 0003c710: 0100 0000 2400 0000 3000 0000 0000 0000  ....$...0.......
 0003c720: 0100 0000 4e01 0000 6847 0200 0000 0000  ....N...hG......
 0003c730: 0100 0000 2e01 0000 9847 0200 0000 0000  .........G......
-0003c740: af42 0000 2401 0000 9847 0200 0000 0000  .B..$....G......
+0003c740: a142 0000 2401 0000 9847 0200 0000 0000  .B..$....G......
 0003c750: 0100 0000 2400 0000 3600 0000 0000 0000  ....$...6.......
 0003c760: 0100 0000 4e01 0000 9847 0200 0000 0000  ....N....G......
 0003c770: 0100 0000 2e01 0000 ce47 0200 0000 0000  .........G......
-0003c780: c342 0000 2401 0000 ce47 0200 0000 0000  .B..$....G......
+0003c780: b542 0000 2401 0000 ce47 0200 0000 0000  .B..$....G......
 0003c790: 0100 0000 2400 0000 3100 0000 0000 0000  ....$...1.......
 0003c7a0: 0100 0000 4e01 0000 ce47 0200 0000 0000  ....N....G......
 0003c7b0: 0100 0000 2e01 0000 ff47 0200 0000 0000  .........G......
-0003c7c0: ce42 0000 2401 0000 ff47 0200 0000 0000  .B..$....G......
+0003c7c0: c042 0000 2401 0000 ff47 0200 0000 0000  .B..$....G......
 0003c7d0: 0100 0000 2400 0000 2900 0000 0000 0000  ....$...).......
 0003c7e0: 0100 0000 4e01 0000 ff47 0200 0000 0000  ....N....G......
 0003c7f0: 0100 0000 2e01 0000 2848 0200 0000 0000  ........(H......
-0003c800: db42 0000 2401 0000 2848 0200 0000 0000  .B..$...(H......
+0003c800: cd42 0000 2401 0000 2848 0200 0000 0000  .B..$...(H......
 0003c810: 0100 0000 2400 0000 d900 0000 0000 0000  ....$...........
 0003c820: 0100 0000 4e01 0000 2848 0200 0000 0000  ....N...(H......
 0003c830: 0100 0000 2e01 0000 0149 0200 0000 0000  .........I......
-0003c840: ea42 0000 2401 0000 0149 0200 0000 0000  .B..$....I......
+0003c840: dc42 0000 2401 0000 0149 0200 0000 0000  .B..$....I......
 0003c850: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 0003c860: 0100 0000 4e01 0000 0149 0200 0000 0000  ....N....I......
 0003c870: 0100 0000 2e01 0000 2149 0200 0000 0000  ........!I......
-0003c880: f742 0000 2401 0000 2149 0200 0000 0000  .B..$...!I......
+0003c880: e942 0000 2401 0000 2149 0200 0000 0000  .B..$...!I......
 0003c890: 0100 0000 2400 0000 5300 0000 0000 0000  ....$...S.......
 0003c8a0: 0100 0000 4e01 0000 2149 0200 0000 0000  ....N...!I......
 0003c8b0: 0100 0000 2e01 0000 7449 0200 0000 0000  ........tI......
-0003c8c0: 0543 0000 2401 0000 7449 0200 0000 0000  .C..$...tI......
+0003c8c0: f742 0000 2401 0000 7449 0200 0000 0000  .B..$...tI......
 0003c8d0: 0100 0000 2400 0000 1a00 0000 0000 0000  ....$...........
 0003c8e0: 0100 0000 4e01 0000 7449 0200 0000 0000  ....N...tI......
 0003c8f0: 0100 0000 2e01 0000 8e49 0200 0000 0000  .........I......
-0003c900: 2143 0000 2401 0000 8e49 0200 0000 0000  !C..$....I......
+0003c900: 1343 0000 2401 0000 8e49 0200 0000 0000  .C..$....I......
 0003c910: 0100 0000 2400 0000 8000 0000 0000 0000  ....$...........
 0003c920: 0100 0000 4e01 0000 8e49 0200 0000 0000  ....N....I......
 0003c930: 0100 0000 2e01 0000 0e4a 0200 0000 0000  .........J......
-0003c940: 3a43 0000 2401 0000 0e4a 0200 0000 0000  :C..$....J......
+0003c940: 2c43 0000 2401 0000 0e4a 0200 0000 0000  ,C..$....J......
 0003c950: 0100 0000 2400 0000 ad00 0000 0000 0000  ....$...........
 0003c960: 0100 0000 4e01 0000 0e4a 0200 0000 0000  ....N....J......
 0003c970: 0100 0000 2e01 0000 bb4a 0200 0000 0000  .........J......
-0003c980: 4e43 0000 2401 0000 bb4a 0200 0000 0000  NC..$....J......
+0003c980: 4043 0000 2401 0000 bb4a 0200 0000 0000  @C..$....J......
 0003c990: 0100 0000 2400 0000 1600 0000 0000 0000  ....$...........
 0003c9a0: 0100 0000 4e01 0000 bb4a 0200 0000 0000  ....N....J......
 0003c9b0: 0100 0000 2e01 0000 d14a 0200 0000 0000  .........J......
-0003c9c0: 6043 0000 2401 0000 d14a 0200 0000 0000  `C..$....J......
+0003c9c0: 5243 0000 2401 0000 d14a 0200 0000 0000  RC..$....J......
 0003c9d0: 0100 0000 2400 0000 1800 0000 0000 0000  ....$...........
 0003c9e0: 0100 0000 4e01 0000 d14a 0200 0000 0000  ....N....J......
 0003c9f0: 0100 0000 2e01 0000 e94a 0200 0000 0000  .........J......
-0003ca00: 7443 0000 2401 0000 e94a 0200 0000 0000  tC..$....J......
+0003ca00: 6643 0000 2401 0000 e94a 0200 0000 0000  fC..$....J......
 0003ca10: 0100 0000 2400 0000 1000 0000 0000 0000  ....$...........
 0003ca20: 0100 0000 4e01 0000 e94a 0200 0000 0000  ....N....J......
 0003ca30: 0100 0000 2e01 0000 f94a 0200 0000 0000  .........J......
-0003ca40: 8643 0000 2401 0000 f94a 0200 0000 0000  .C..$....J......
+0003ca40: 7843 0000 2401 0000 f94a 0200 0000 0000  xC..$....J......
 0003ca50: 0100 0000 2400 0000 1900 0000 0000 0000  ....$...........
 0003ca60: 0100 0000 4e01 0000 f94a 0200 0000 0000  ....N....J......
 0003ca70: 0100 0000 2e01 0000 124b 0200 0000 0000  .........K......
-0003ca80: 9943 0000 2401 0000 124b 0200 0000 0000  .C..$....K......
+0003ca80: 8b43 0000 2401 0000 124b 0200 0000 0000  .C..$....K......
 0003ca90: 0100 0000 2400 0000 1200 0000 0000 0000  ....$...........
 0003caa0: 0100 0000 4e01 0000 124b 0200 0000 0000  ....N....K......
 0003cab0: 0100 0000 2e01 0000 244b 0200 0000 0000  ........$K......
-0003cac0: a943 0000 2401 0000 244b 0200 0000 0000  .C..$...$K......
+0003cac0: 9b43 0000 2401 0000 244b 0200 0000 0000  .C..$...$K......
 0003cad0: 0100 0000 2400 0000 2600 0000 0000 0000  ....$...&.......
 0003cae0: 0100 0000 4e01 0000 244b 0200 0000 0000  ....N...$K......
 0003caf0: 0100 0000 2e01 0000 4a4b 0200 0000 0000  ........JK......
-0003cb00: b643 0000 2401 0000 4a4b 0200 0000 0000  .C..$...JK......
+0003cb00: a843 0000 2401 0000 4a4b 0200 0000 0000  .C..$...JK......
 0003cb10: 0100 0000 2400 0000 7700 0000 0000 0000  ....$...w.......
 0003cb20: 0100 0000 4e01 0000 4a4b 0200 0000 0000  ....N...JK......
 0003cb30: 0100 0000 2e01 0000 c14b 0200 0000 0000  .........K......
-0003cb40: d243 0000 2401 0000 c14b 0200 0000 0000  .C..$....K......
+0003cb40: c443 0000 2401 0000 c14b 0200 0000 0000  .C..$....K......
 0003cb50: 0100 0000 2400 0000 0d00 0000 0000 0000  ....$...........
 0003cb60: 0100 0000 4e01 0000 c14b 0200 0000 0000  ....N....K......
 0003cb70: 0100 0000 2e01 0000 ce4b 0200 0000 0000  .........K......
-0003cb80: e943 0000 2401 0000 ce4b 0200 0000 0000  .C..$....K......
+0003cb80: db43 0000 2401 0000 ce4b 0200 0000 0000  .C..$....K......
 0003cb90: 0100 0000 2400 0000 1800 0000 0000 0000  ....$...........
 0003cba0: 0100 0000 4e01 0000 ce4b 0200 0000 0000  ....N....K......
 0003cbb0: 0100 0000 2e01 0000 e64b 0200 0000 0000  .........K......
-0003cbc0: 0344 0000 2401 0000 e64b 0200 0000 0000  .D..$....K......
+0003cbc0: f543 0000 2401 0000 e64b 0200 0000 0000  .C..$....K......
 0003cbd0: 0100 0000 2400 0000 0d00 0000 0000 0000  ....$...........
 0003cbe0: 0100 0000 4e01 0000 e64b 0200 0000 0000  ....N....K......
 0003cbf0: 0100 0000 2e01 0000 f34b 0200 0000 0000  .........K......
-0003cc00: 1a44 0000 2401 0000 f34b 0200 0000 0000  .D..$....K......
+0003cc00: 0c44 0000 2401 0000 f34b 0200 0000 0000  .D..$....K......
 0003cc10: 0100 0000 2400 0000 2700 0000 0000 0000  ....$...'.......
 0003cc20: 0100 0000 4e01 0000 f34b 0200 0000 0000  ....N....K......
 0003cc30: 0100 0000 2e01 0000 1a4c 0200 0000 0000  .........L......
-0003cc40: 3244 0000 2401 0000 1a4c 0200 0000 0000  2D..$....L......
+0003cc40: 2444 0000 2401 0000 1a4c 0200 0000 0000  $D..$....L......
 0003cc50: 0100 0000 2400 0000 1300 0000 0000 0000  ....$...........
 0003cc60: 0100 0000 4e01 0000 1a4c 0200 0000 0000  ....N....L......
-0003cc70: 3e44 0000 2609 0000 c0c1 0200 0000 0000  >D..&...........
-0003cc80: 4c44 0000 2609 0000 d0c1 0200 0000 0000  LD..&...........
-0003cc90: 5c44 0000 260b 0000 08d3 0600 0000 0000  \D..&...........
+0003cc70: 3044 0000 2609 0000 c0c1 0200 0000 0000  0D..&...........
+0003cc80: 3e44 0000 2609 0000 d0c1 0200 0000 0000  >D..&...........
+0003cc90: 4e44 0000 260b 0000 08d3 0600 0000 0000  ND..&...........
 0003cca0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0003ccb0: 0200 0000 0f01 0000 39f6 0000 0000 0000  ........9.......
 0003ccc0: 1000 0000 0f01 0000 c442 0100 0000 0000  .........B......
 0003ccd0: 1d00 0000 0f01 0000 b33d 0100 0000 0000  .........=......
 0003cce0: 2d00 0000 0f01 0000 0c40 0100 0000 0000  -........@......
 0003ccf0: 3d00 0000 0f01 0000 9340 0100 0000 0000  =........@......
 0003cd00: 5200 0000 0f01 0000 eba9 0000 0000 0000  R...............
@@ -15930,1382 +15930,1382 @@
 0003e390: 7618 0000 0100 0002 0000 0000 0000 0000  v...............
 0003e3a0: 9518 0000 0100 0002 0000 0000 0000 0000  ................
 0003e3b0: b618 0000 0100 0001 0000 0000 0000 0000  ................
 0003e3c0: be18 0000 0100 0001 0000 0000 0000 0000  ................
 0003e3d0: c618 0000 0100 0001 0000 0000 0000 0000  ................
 0003e3e0: ce18 0000 0100 0001 0000 0000 0000 0000  ................
 0003e3f0: d618 0000 0100 0001 0000 0000 0000 0000  ................
-0003e400: de18 0000 0100 0004 0000 0000 0000 0000  ................
-0003e410: ec18 0000 0100 0001 0000 0000 0000 0000  ................
-0003e420: f218 0000 0100 0001 0000 0000 0000 0000  ................
-0003e430: 0319 0000 0100 0001 0000 0000 0000 0000  ................
-0003e440: 1919 0000 0100 0001 0000 0000 0000 0000  ................
-0003e450: 2c19 0000 0100 0001 0000 0000 0000 0000  ,...............
-0003e460: 4919 0000 0100 0001 0000 0000 0000 0000  I...............
-0003e470: 5919 0000 0100 0001 0000 0000 0000 0000  Y...............
-0003e480: 6f19 0000 0100 0001 0000 0000 0000 0000  o...............
-0003e490: 8219 0000 0100 0001 0000 0000 0000 0000  ................
-0003e4a0: 9719 0000 0100 0001 0000 0000 0000 0000  ................
-0003e4b0: af19 0000 0100 0001 0000 0000 0000 0000  ................
-0003e4c0: c219 0000 0100 0001 0000 0000 0000 0000  ................
-0003e4d0: d219 0000 0100 0001 0000 0000 0000 0000  ................
+0003e400: de18 0000 0100 0001 0000 0000 0000 0000  ................
+0003e410: e418 0000 0100 0001 0000 0000 0000 0000  ................
+0003e420: f518 0000 0100 0001 0000 0000 0000 0000  ................
+0003e430: 0b19 0000 0100 0001 0000 0000 0000 0000  ................
+0003e440: 1e19 0000 0100 0001 0000 0000 0000 0000  ................
+0003e450: 3b19 0000 0100 0001 0000 0000 0000 0000  ;...............
+0003e460: 4b19 0000 0100 0001 0000 0000 0000 0000  K...............
+0003e470: 6119 0000 0100 0001 0000 0000 0000 0000  a...............
+0003e480: 7419 0000 0100 0001 0000 0000 0000 0000  t...............
+0003e490: 8919 0000 0100 0001 0000 0000 0000 0000  ................
+0003e4a0: a119 0000 0100 0001 0000 0000 0000 0000  ................
+0003e4b0: b419 0000 0100 0001 0000 0000 0000 0000  ................
+0003e4c0: c419 0000 0100 0001 0000 0000 0000 0000  ................
+0003e4d0: d919 0000 0100 0001 0000 0000 0000 0000  ................
 0003e4e0: e719 0000 0100 0001 0000 0000 0000 0000  ................
-0003e4f0: f519 0000 0100 0001 0000 0000 0000 0000  ................
-0003e500: 091a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e510: 201a 0000 0100 0001 0000 0000 0000 0000   ...............
-0003e520: 341a 0000 0100 0001 0000 0000 0000 0000  4...............
-0003e530: 481a 0000 0100 0001 0000 0000 0000 0000  H...............
-0003e540: 5f1a 0000 0100 0001 0000 0000 0000 0000  _...............
-0003e550: 751a 0000 0100 0001 0000 0000 0000 0000  u...............
-0003e560: 8d1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e4f0: fb19 0000 0100 0001 0000 0000 0000 0000  ................
+0003e500: 121a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e510: 261a 0000 0100 0001 0000 0000 0000 0000  &...............
+0003e520: 3a1a 0000 0100 0001 0000 0000 0000 0000  :...............
+0003e530: 511a 0000 0100 0001 0000 0000 0000 0000  Q...............
+0003e540: 671a 0000 0100 0001 0000 0000 0000 0000  g...............
+0003e550: 7f1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e560: 9a1a 0000 0100 0001 0000 0000 0000 0000  ................
 0003e570: a81a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e580: b61a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e590: cb1a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5a0: d11a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5b0: d71a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5c0: e81a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5d0: ee1a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5e0: fb1a 0000 0100 0001 0000 0000 0000 0000  ................
-0003e5f0: 011b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e600: 091b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e610: 151b 0000 0100 0001 0000 0000 0000 0000  ................
+0003e580: bd1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e590: c31a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5a0: c91a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5b0: da1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5c0: e01a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5d0: ed1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5e0: f31a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e5f0: fb1a 0000 0100 0001 0000 0000 0000 0000  ................
+0003e600: 071b 0000 0100 0001 0000 0000 0000 0000  ................
+0003e610: 0f1b 0000 0100 0001 0000 0000 0000 0000  ................
 0003e620: 1d1b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e630: 2b1b 0000 0100 0001 0000 0000 0000 0000  +...............
-0003e640: 371b 0000 0100 0001 0000 0000 0000 0000  7...............
-0003e650: 3f1b 0000 0100 0001 0000 0000 0000 0000  ?...............
-0003e660: 471b 0000 0100 0001 0000 0000 0000 0000  G...............
-0003e670: 4f1b 0000 0100 0001 0000 0000 0000 0000  O...............
-0003e680: 591b 0000 0100 0001 0000 0000 0000 0000  Y...............
-0003e690: 611b 0000 0100 0001 0000 0000 0000 0000  a...............
-0003e6a0: 6e1b 0000 0100 0001 0000 0000 0000 0000  n...............
-0003e6b0: 771b 0000 0100 0001 0000 0000 0000 0000  w...............
+0003e630: 291b 0000 0100 0001 0000 0000 0000 0000  )...............
+0003e640: 311b 0000 0100 0001 0000 0000 0000 0000  1...............
+0003e650: 391b 0000 0100 0001 0000 0000 0000 0000  9...............
+0003e660: 411b 0000 0100 0001 0000 0000 0000 0000  A...............
+0003e670: 4b1b 0000 0100 0001 0000 0000 0000 0000  K...............
+0003e680: 531b 0000 0100 0001 0000 0000 0000 0000  S...............
+0003e690: 601b 0000 0100 0001 0000 0000 0000 0000  `...............
+0003e6a0: 691b 0000 0100 0001 0000 0000 0000 0000  i...............
+0003e6b0: 711b 0000 0100 0001 0000 0000 0000 0000  q...............
 0003e6c0: 7f1b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e6d0: 8d1b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e6e0: 931b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e6f0: 9b1b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e700: a61b 0000 0100 0001 0000 0000 0000 0000  ................
-0003e710: b507 0000 b607 0000 b707 0000 b807 0000  ................
-0003e720: b907 0000 ba07 0000 bb07 0000 bc07 0000  ................
-0003e730: bd07 0000 be07 0000 bf07 0000 c007 0000  ................
-0003e740: c107 0000 c207 0000 c307 0000 c407 0000  ................
-0003e750: c507 0000 c607 0000 c707 0000 c807 0000  ................
-0003e760: c907 0000 ca07 0000 cb07 0000 cc07 0000  ................
-0003e770: cd07 0000 ce07 0000 cf07 0000 d007 0000  ................
-0003e780: d107 0000 d207 0000 d307 0000 d607 0000  ................
-0003e790: d707 0000 d807 0000 d907 0000 da07 0000  ................
-0003e7a0: db07 0000 dc07 0000 de07 0000 df07 0000  ................
-0003e7b0: e007 0000 e107 0000 e207 0000 e307 0000  ................
-0003e7c0: e407 0000 e507 0000 e607 0000 e707 0000  ................
-0003e7d0: e807 0000 e907 0000 ea07 0000 eb07 0000  ................
-0003e7e0: ec07 0000 ed07 0000 ee07 0000 ef07 0000  ................
-0003e7f0: f007 0000 f107 0000 f207 0000 f307 0000  ................
-0003e800: f407 0000 f507 0000 fa07 0000 fb07 0000  ................
-0003e810: fc07 0000 fd07 0000 fe07 0000 0008 0000  ................
-0003e820: 0108 0000 0208 0000 0308 0000 0408 0000  ................
-0003e830: 0508 0000 0608 0000 0708 0000 0808 0000  ................
-0003e840: 0908 0000 0a08 0000 0b08 0000 0c08 0000  ................
-0003e850: 0d08 0000 0e08 0000 0f08 0000 1008 0000  ................
-0003e860: 1108 0000 1208 0000 1308 0000 1408 0000  ................
-0003e870: 1508 0000 1608 0000 1708 0000 1808 0000  ................
-0003e880: 1908 0000 1a08 0000 1b08 0000 1c08 0000  ................
-0003e890: 1d08 0000 1e08 0000 1f08 0000 2008 0000  ............ ...
-0003e8a0: 2108 0000 2208 0000 2308 0000 2408 0000  !..."...#...$...
-0003e8b0: 2508 0000 2608 0000 2708 0000 2808 0000  %...&...'...(...
-0003e8c0: 2908 0000 2a08 0000 2b08 0000 2c08 0000  )...*...+...,...
-0003e8d0: 2d08 0000 2e08 0000 2f08 0000 b507 0000  -......./.......
-0003e8e0: b607 0000 b707 0000 b807 0000 b907 0000  ................
-0003e8f0: ba07 0000 bb07 0000 bc07 0000 bd07 0000  ................
-0003e900: be07 0000 bf07 0000 c007 0000 c107 0000  ................
-0003e910: c207 0000 c307 0000 c407 0000 c507 0000  ................
-0003e920: c607 0000 c707 0000 c807 0000 c907 0000  ................
-0003e930: ca07 0000 cb07 0000 cc07 0000 cd07 0000  ................
-0003e940: ce07 0000 cf07 0000 d007 0000 d107 0000  ................
-0003e950: d207 0000 d307 0000 d407 0000 d607 0000  ................
-0003e960: d707 0000 d807 0000 d907 0000 da07 0000  ................
-0003e970: db07 0000 dc07 0000 dd07 0000 de07 0000  ................
-0003e980: df07 0000 e007 0000 e107 0000 e207 0000  ................
-0003e990: e307 0000 e407 0000 e507 0000 e607 0000  ................
-0003e9a0: e707 0000 e807 0000 e907 0000 ea07 0000  ................
-0003e9b0: eb07 0000 ec07 0000 ed07 0000 ee07 0000  ................
-0003e9c0: ef07 0000 f007 0000 f107 0000 f207 0000  ................
-0003e9d0: f307 0000 f407 0000 f507 0000 f607 0000  ................
-0003e9e0: f707 0000 f807 0000 f907 0000 fa07 0000  ................
-0003e9f0: fb07 0000 fc07 0000 fd07 0000 fe07 0000  ................
-0003ea00: 0008 0000 0108 0000 0208 0000 0308 0000  ................
-0003ea10: 0408 0000 0508 0000 0608 0000 0708 0000  ................
-0003ea20: 0808 0000 0908 0000 0a08 0000 0b08 0000  ................
-0003ea30: 0c08 0000 0d08 0000 0e08 0000 0f08 0000  ................
-0003ea40: 1008 0000 1108 0000 1208 0000 1308 0000  ................
-0003ea50: 1408 0000 1508 0000 1608 0000 1708 0000  ................
-0003ea60: 1808 0000 1908 0000 1a08 0000 1b08 0000  ................
-0003ea70: 1c08 0000 1d08 0000 1e08 0000 1f08 0000  ................
-0003ea80: 2008 0000 2108 0000 2208 0000 2308 0000   ...!..."...#...
-0003ea90: 2408 0000 2508 0000 2608 0000 2708 0000  $...%...&...'...
-0003eaa0: 2808 0000 2908 0000 2a08 0000 2b08 0000  (...)...*...+...
-0003eab0: 2c08 0000 2d08 0000 2e08 0000 2f08 0000  ,...-......./...
-0003eac0: 2000 5f42 6c6f 636b 696e 6752 6561 6400   ._BlockingRead.
-0003ead0: 5f43 6865 636b 5753 4175 7468 005f 436f  _CheckWSAuth._Co
-0003eae0: 6d70 7574 6541 7574 6848 4131 005f 436f  mputeAuthHA1._Co
-0003eaf0: 6d70 7574 6541 7574 6848 4132 005f 436f  mputeAuthHA2._Co
-0003eb00: 6d70 7574 6541 7574 6852 6573 706f 6e73  mputeAuthRespons
-0003eb10: 6500 5f46 7573 696f 6e45 7272 6d73 6700  e._FusionErrmsg.
-0003eb20: 5f49 7356 616c 6964 4279 6e46 696c 6500  _IsValidBynFile.
-0003eb30: 5f49 7356 616c 6964 4279 6e48 6561 6400  _IsValidBynHead.
-0003eb40: 5f4d 4435 4164 6444 6174 6100 5f4d 4435  _MD5AddData._MD5
-0003eb50: 4361 6c63 756c 6174 6500 5f4d 4435 496e  Calculate._MD5In
-0003eb60: 6974 6961 6c69 7a65 005f 5365 6e64 4461  itialize._SendDa
-0003eb70: 7461 5061 636b 6574 005f 5365 7269 616c  taPacket._Serial
-0003eb80: 4e75 6d62 6572 5374 7200 5f53 6572 6961  NumberStr._Seria
-0003eb90: 6c52 6566 005f 5661 6c69 6461 7465 4279  lRef._ValidateBy
-0003eba0: 6e43 6f6d 7061 7400 5f57 616b 6555 7041  nCompat._WakeUpA
-0003ebb0: 6c6c 536c 6565 7000 5f59 464f 5045 4e00  llSleep._YFOPEN.
-0003ebc0: 5f59 6374 7844 6576 6963 654c 6973 7456  _YctxDeviceListV
-0003ebd0: 616c 6964 6974 794d 7300 5f59 6374 784e  alidityMs._YctxN
-0003ebe0: 6574 776f 726b 5469 6d65 6f75 7400 5f62  etworkTimeout._b
-0003ebf0: 696e 3273 7472 005f 6368 6563 6b46 6f72  in2str._checkFor
-0003ec00: 5361 6d65 4875 6241 6363 6573 7300 5f64  SameHubAccess._d
-0003ec10: 6267 6c6f 6766 005f 6465 636f 6465 4865  bglogf._decodeHe
-0003ec20: 7800 5f64 6563 6f64 654e 6574 4675 6e63  x._decodeNetFunc
-0003ec30: 5661 6c56 3200 5f64 6563 6f64 6550 7562  ValV2._decodePub
-0003ec40: 5661 6c00 5f64 6574 6563 7465 6449 6661  Val._detectedIfa
-0003ec50: 6365 7300 5f64 6576 4864 6c49 6e66 6f00  ces._devHdlInfo.
-0003ec60: 5f64 6e73 4361 6368 6500 5f64 756d 7059  _dnsCache._dumpY
-0003ec70: 5065 7266 456e 7472 7900 5f66 6374 7800  PerfEntry._fctx.
-0003ec80: 5f66 696e 6444 6576 005f 6669 6e64 4465  _findDev._findDe
-0003ec90: 7646 726f 6d49 4f48 646c 005f 6669 6e64  vFromIOHdl._find
-0003eca0: 4465 7648 646c 4672 6f6d 5374 7200 5f66  DevHdlFromStr._f
-0003ecb0: 6972 6d5f 6465 7600 5f66 6972 6d5f 706b  irm_dev._firm_pk
-0003ecc0: 7400 5f66 7265 6542 6c6b 7300 5f66 7265  t._freeBlks._fre
-0003ecd0: 6544 6576 5964 7849 6e66 6f73 005f 6861  eDevYdxInfos._ha
-0003ece0: 6e64 6c65 4e65 744e 6f74 6966 6963 6174  ndleNetNotificat
-0003ecf0: 696f 6e00 5f69 6e69 7444 6576 5964 7849  ion._initDevYdxI
-0003ed00: 6e66 6f73 005f 6e62 4465 7465 6374 6564  nfos._nbDetected
-0003ed10: 4966 6163 6573 005f 7072 6f67 5f47 6574  Ifaces._prog_Get
-0003ed20: 4350 554e 616d 6500 5f72 6571 7565 7374  CPUName._request
-0003ed30: 5f70 656e 6469 6e67 5f6c 6f67 7300 5f73  _pending_logs._s
-0003ed40: 6861 315f 696e 6974 005f 7546 6c61 7368  ha1_init._uFlash
-0003ed50: 4465 7669 6365 005f 7664 6267 6c6f 6766  Device._vdbglogf
-0003ed60: 005f 7770 416c 6c6f 7755 6e72 6567 6973  ._wpAllowUnregis
-0003ed70: 7465 7245 7800 5f77 7045 6e74 7279 436f  terEx._wpEntryCo
-0003ed80: 756e 7400 5f77 7047 6574 4174 7472 6962  unt._wpGetAttrib
-0003ed90: 7574 6500 5f77 7047 6574 4465 7659 6478  ute._wpGetDevYdx
-0003eda0: 005f 7770 4765 7444 6576 6963 6549 6e66  ._wpGetDeviceInf
-0003edb0: 6f00 5f77 7047 6574 4c6f 6769 6361 6c4e  o._wpGetLogicalN
-0003edc0: 616d 6500 5f77 7047 6574 5365 7269 616c  ame._wpGetSerial
-0003edd0: 005f 7770 4d61 726b 466f 7255 6e72 6567  ._wpMarkForUnreg
-0003ede0: 6973 7465 7200 5f77 7050 7265 7665 6e74  ister._wpPrevent
-0003edf0: 556e 7265 6769 7374 6572 4578 005f 7770  UnregisterEx._wp
-0003ee00: 5265 6769 7374 6572 005f 7770 5365 6172  Register._wpSear
-0003ee10: 6368 005f 7770 5365 6172 6368 4279 4e61  ch._wpSearchByNa
-0003ee20: 6d65 4861 7368 005f 7770 5365 6172 6368  meHash._wpSearch
-0003ee30: 4578 005f 7773 5f63 6c65 616e 7570 005f  Ex._ws_cleanup._
-0003ee40: 7773 5f74 6872 6561 6400 5f79 426c 6b4c  ws_thread._yBlkL
-0003ee50: 6973 744c 656e 6774 6800 5f79 426c 6b4c  istLength._yBlkL
-0003ee60: 6973 7453 6565 6b00 5f79 436c 6f73 6545  istSeek._yCloseE
-0003ee70: 7665 6e74 005f 7943 6f6e 7375 6d65 5761  vent._yConsumeWa
-0003ee80: 6b65 5570 536f 636b 6574 005f 7943 6f6e  keUpSocket._yCon
-0003ee90: 7465 7874 005f 7943 7265 6174 6544 6574  text._yCreateDet
-0003eea0: 6163 6865 6454 6872 6561 644e 616d 6564  achedThreadNamed
-0003eeb0: 005f 7943 7265 6174 6545 7665 6e74 005f  ._yCreateEvent._
-0003eec0: 7943 7265 6174 654d 616e 7561 6c45 7665  yCreateManualEve
-0003eed0: 6e74 005f 7944 656c 6574 6543 7269 7469  nt._yDeleteCriti
-0003eee0: 6361 6c53 6563 7469 6f6e 005f 7944 6967  calSection._yDig
-0003eef0: 6573 7441 7574 686f 7269 7a61 7469 6f6e  estAuthorization
-0003ef00: 005f 7944 7269 6e67 5761 6b65 5570 536f  ._yDringWakeUpSo
-0003ef10: 636b 6574 005f 7944 7570 5365 7400 5f79  cket._yDupSet._y
-0003ef20: 456e 7465 7243 7269 7469 6361 6c53 6563  EnterCriticalSec
-0003ef30: 7469 6f6e 005f 7946 6966 6f43 6c65 616e  tion._yFifoClean
-0003ef40: 7570 005f 7946 6966 6f45 6d70 7479 005f  up._yFifoEmpty._
-0003ef50: 7946 6966 6f45 6d70 7479 4578 005f 7946  yFifoEmptyEx._yF
-0003ef60: 6966 6f45 6e74 6572 4353 005f 7946 6966  ifoEnterCS._yFif
-0003ef70: 6f47 6574 4672 6565 005f 7946 6966 6f47  oGetFree._yFifoG
-0003ef80: 6574 4672 6565 4578 005f 7946 6966 6f47  etFreeEx._yFifoG
-0003ef90: 6574 5573 6564 005f 7946 6966 6f47 6574  etUsed._yFifoGet
-0003efa0: 5573 6564 4578 005f 7946 6966 6f49 6e69  UsedEx._yFifoIni
-0003efb0: 7445 7800 5f79 4669 666f 4c65 6176 6543  tEx._yFifoLeaveC
-0003efc0: 5300 5f79 466f 7263 6546 6966 6f00 5f79  S._yForceFifo._y
-0003efd0: 4672 6565 4d75 7465 7800 5f79 4672 6565  FreeMutex._yFree
-0003efe0: 5761 6b65 5570 536f 636b 6574 005f 7946  WakeUpSocket._yF
-0003eff0: 756e 6374 696f 6e54 696d 6564 5570 6461  unctionTimedUpda
-0003f000: 7465 005f 7946 756e 6374 696f 6e55 7064  te._yFunctionUpd
-0003f010: 6174 6500 5f79 4861 7368 4672 6565 005f  ate._yHashFree._
-0003f020: 7948 6173 6847 6574 4275 6600 5f79 4861  yHashGetBuf._yHa
-0003f030: 7368 4765 7453 7472 005f 7948 6173 6847  shGetStr._yHashG
-0003f040: 6574 5374 724c 656e 005f 7948 6173 6847  etStrLen._yHashG
-0003f050: 6574 5374 7250 7472 005f 7948 6173 6849  etStrPtr._yHashI
-0003f060: 6e69 7400 5f79 4861 7368 4d75 7465 7800  nit._yHashMutex.
-0003f070: 5f79 4861 7368 5075 7442 7566 005f 7948  _yHashPutBuf._yH
-0003f080: 6173 6850 7574 5374 7200 5f79 4861 7368  ashPutStr._yHash
-0003f090: 5465 7374 4275 6600 5f79 4861 7368 5465  TestBuf._yHashTe
-0003f0a0: 7374 5374 7200 5f79 496e 6974 5073 6b00  stStr._yInitPsk.
-0003f0b0: 5f79 496e 6974 5761 6b65 5570 536f 636b  _yInitWakeUpSock
-0003f0c0: 6574 005f 7949 6e69 7469 616c 697a 6543  et._yInitializeC
-0003f0d0: 7269 7469 6361 6c53 6563 7469 6f6e 005f  riticalSection._
-0003f0e0: 7949 7465 7250 736b 005f 794a 736f 6e50  yIterPsk._yJsonP
-0003f0f0: 6172 7365 005f 794a 736f 6e53 6b69 7000  arse._yJsonSkip.
-0003f100: 5f79 4c65 6176 6543 7269 7469 6361 6c53  _yLeaveCriticalS
-0003f110: 6563 7469 6f6e 005f 794e 6574 4875 6247  ection._yNetHubG
-0003f120: 6574 426f 6f74 6c6f 6164 6572 7300 5f79  etBootloaders._y
-0003f130: 4e65 7453 6574 4572 7245 7800 5f79 5061  NetSetErrEx._yPa
-0003f140: 7273 6557 5757 4175 7468 656e 7469 6361  rseWWWAuthentica
-0003f150: 7465 005f 7950 6565 6b43 6f6e 7469 6e75  te._yPeekContinu
-0003f160: 6f75 7346 6966 6f00 5f79 5065 656b 436f  ousFifo._yPeekCo
-0003f170: 6e74 696e 756f 7573 4669 666f 4578 005f  ntinuousFifoEx._
-0003f180: 7950 6565 6b46 6966 6f00 5f79 5065 656b  yPeekFifo._yPeek
-0003f190: 4669 666f 4578 005f 7950 6b74 5175 6575  FifoEx._yPktQueu
-0003f1a0: 6546 7265 6500 5f79 506b 7451 7565 7565  eFree._yPktQueue
-0003f1b0: 496e 6974 005f 7950 6b74 5175 6575 6550  Init._yPktQueueP
-0003f1c0: 6565 6b48 3244 005f 7950 6b74 5175 6575  eekH2D._yPktQueu
-0003f1d0: 6550 6f70 4832 4400 5f79 506b 7451 7565  ePopH2D._yPktQue
-0003f1e0: 7565 5075 7368 4432 4800 5f79 506b 7451  uePushD2H._yPktQ
-0003f1f0: 7565 7565 5075 7368 4832 4400 5f79 506b  ueuePushH2D._yPk
-0003f200: 7451 7565 7565 5365 7445 7272 6f72 005f  tQueueSetError._
-0003f210: 7950 6b74 5175 6575 6557 6169 7441 6e64  yPktQueueWaitAnd
-0003f220: 506f 7044 3248 005f 7950 6f70 4669 666f  PopD2H._yPopFifo
-0003f230: 005f 7950 6f70 4669 666f 4578 005f 7950  ._yPopFifoEx._yP
-0003f240: 726f 6746 7265 6500 5f79 5072 6f67 496e  rogFree._yProgIn
-0003f250: 6974 005f 7950 7573 6846 6966 6f00 5f79  it._yPushFifo._y
-0003f260: 5075 7368 4669 666f 4578 005f 7952 6571  PushFifoEx._yReq
-0003f270: 416c 6c6f 6300 5f79 5265 7143 6c6f 7365  Alloc._yReqClose
-0003f280: 005f 7952 6571 4672 6565 005f 7952 6571  ._yReqFree._yReq
-0003f290: 4765 7400 5f79 5265 7148 6173 5065 6e64  Get._yReqHasPend
-0003f2a0: 696e 6700 5f79 5265 7149 7341 7379 6e63  ing._yReqIsAsync
-0003f2b0: 005f 7952 6571 4973 456f 6600 5f79 5265  ._yReqIsEof._yRe
-0003f2c0: 714d 756c 7469 5365 6c65 6374 005f 7952  qMultiSelect._yR
-0003f2d0: 6571 4f70 656e 005f 7952 6571 5265 6164  eqOpen._yReqRead
-0003f2e0: 005f 7952 6571 5365 6c65 6374 005f 7952  ._yReqSelect._yR
-0003f2f0: 6573 6574 4576 656e 7400 5f79 5265 736f  esetEvent._yReso
-0003f300: 6c76 6544 4e53 005f 7953 4841 3100 5f79  lveDNS._ySHA1._y
-0003f310: 5353 4450 4469 7363 6f76 6572 005f 7953  SSDPDiscover._yS
-0003f320: 5344 5053 7461 7274 005f 7953 5344 5053  SDPStart._ySSDPS
-0003f330: 746f 7000 5f79 5365 656b 4669 666f 005f  top._ySeekFifo._
-0003f340: 7953 6565 6b46 6966 6f45 7800 5f79 5365  ySeekFifoEx._ySe
-0003f350: 7445 7272 005f 7953 6574 4576 656e 7400  tErr._ySetEvent.
-0003f360: 5f79 5374 6172 7457 616b 6555 7053 6f63  _yStartWakeUpSoc
-0003f370: 6b65 7400 5f79 5463 7044 6f77 6e6c 6f61  ket._yTcpDownloa
-0003f380: 6400 5f79 5463 7049 6e69 7400 5f79 5463  d._yTcpInit._yTc
-0003f390: 7053 6875 7464 6f77 6e00 5f79 5468 7265  pShutdown._yThre
-0003f3a0: 6164 4372 6561 7465 4e61 6d65 6400 5f79  adCreateNamed._y
-0003f3b0: 5468 7265 6164 496e 6465 7800 5f79 5468  ThreadIndex._yTh
-0003f3c0: 7265 6164 4973 5275 6e6e 696e 6700 5f79  readIsRunning._y
-0003f3d0: 5468 7265 6164 4b69 6c6c 005f 7954 6872  ThreadKill._yThr
-0003f3e0: 6561 644d 7573 7445 6e64 005f 7954 6872  eadMustEnd._yThr
-0003f3f0: 6561 6452 6571 7565 7374 456e 6400 5f79  eadRequestEnd._y
-0003f400: 5468 7265 6164 5369 676e 616c 456e 6400  ThreadSignalEnd.
-0003f410: 5f79 5468 7265 6164 5369 676e 616c 5374  _yThreadSignalSt
-0003f420: 6172 7400 5f79 5472 7945 6e74 6572 4372  art._yTryEnterCr
-0003f430: 6974 6963 616c 5365 6374 696f 6e00 5f79  iticalSection._y
-0003f440: 5553 4247 6574 426f 6f6c 6f61 6465 7200  USBGetBooloader.
-0003f450: 5f79 5553 4252 656c 6561 7365 416c 6c44  _yUSBReleaseAllD
-0003f460: 6576 6963 6573 005f 7955 5342 5570 6461  evices._yUSBUpda
-0003f470: 7465 4465 7669 6365 4c69 7374 005f 7955  teDeviceList._yU
-0003f480: 7362 436c 6f73 6500 5f79 5573 6245 4f46  sbClose._yUsbEOF
-0003f490: 005f 7955 7362 4672 6565 005f 7955 7362  ._yUsbFree._yUsb
-0003f4a0: 4964 6c65 005f 7955 7362 496e 6974 005f  Idle._yUsbInit._
-0003f4b0: 7955 7362 4f70 656e 005f 7955 7362 4f70  yUsbOpen._yUsbOp
-0003f4c0: 656e 4465 7644 6573 6372 005f 7955 7362  enDevDescr._yUsb
-0003f4d0: 5265 6164 426c 6f63 6b00 5f79 5573 6252  ReadBlock._yUsbR
-0003f4e0: 6561 644e 6f6e 426c 6f63 6b00 5f79 5573  eadNonBlock._yUs
-0003f4f0: 6253 6574 494f 4173 796e 6300 5f79 5573  bSetIOAsync._yUs
-0003f500: 6254 7261 6666 6963 5065 6e64 696e 6700  bTrafficPending.
-0003f510: 5f79 5573 6257 7269 7465 005f 7957 6169  _yUsbWrite._yWai
-0003f520: 7446 6f72 4576 656e 7400 5f79 5770 4c69  tForEvent._yWpLi
-0003f530: 7374 4865 6164 005f 7957 704d 7574 6578  stHead._yWpMutex
-0003f540: 005f 7959 704c 6973 7448 6561 6400 5f79  ._yYpListHead._y
-0003f550: 5970 4d75 7465 7800 5f79 6170 6941 6464  YpMutex._yapiAdd
-0003f560: 5564 6576 5275 6c65 7346 6f72 596f 6374  UdevRulesForYoct
-0003f570: 6f00 5f79 6170 6943 6865 636b 4669 726d  o._yapiCheckFirm
-0003f580: 7761 7265 005f 7961 7069 4368 6563 6b46  ware._yapiCheckF
-0003f590: 6972 6d77 6172 655f 696e 7465 726e 616c  irmware_internal
-0003f5a0: 005f 7961 7069 4368 6563 6b4c 6f67 6963  ._yapiCheckLogic
-0003f5b0: 616c 4e61 6d65 005f 7961 7069 4672 6565  alName._yapiFree
-0003f5c0: 4150 4900 5f79 6170 6946 7265 654d 656d  API._yapiFreeMem
-0003f5d0: 005f 7961 7069 4765 7441 5049 5665 7273  ._yapiGetAPIVers
-0003f5e0: 696f 6e00 5f79 6170 6947 6574 416c 6c44  ion._yapiGetAllD
-0003f5f0: 6576 6963 6573 005f 7961 7069 4765 7441  evices._yapiGetA
-0003f600: 6c6c 4a73 6f6e 4b65 7973 005f 7961 7069  llJsonKeys._yapi
-0003f610: 4765 7442 6f6f 746c 6f61 6465 7273 005f  GetBootloaders._
-0003f620: 7961 7069 4765 7442 6f6f 746c 6f61 6465  yapiGetBootloade
-0003f630: 7273 4465 7673 005f 7961 7069 4765 7443  rsDevs._yapiGetC
-0003f640: 4e6f 6e63 6500 5f79 6170 6947 6574 444c  Nonce._yapiGetDL
-0003f650: 4c50 6174 6800 5f79 6170 6947 6574 4465  LPath._yapiGetDe
-0003f660: 7669 6365 005f 7961 7069 4765 7444 6576  vice._yapiGetDev
-0003f670: 6963 6549 6e66 6f00 5f79 6170 6947 6574  iceInfo._yapiGet
-0003f680: 4465 7669 6365 5061 7468 005f 7961 7069  DevicePath._yapi
-0003f690: 4765 7444 6576 6963 6550 6174 6845 7800  GetDevicePathEx.
-0003f6a0: 5f79 6170 6947 6574 4675 6e63 7469 6f6e  _yapiGetFunction
-0003f6b0: 005f 7961 7069 4765 7446 756e 6374 696f  ._yapiGetFunctio
-0003f6c0: 6e49 6e66 6f00 5f79 6170 6947 6574 4675  nInfo._yapiGetFu
-0003f6d0: 6e63 7469 6f6e 496e 666f 4578 005f 7961  nctionInfoEx._ya
-0003f6e0: 7069 4765 7446 756e 6374 696f 6e73 4279  piGetFunctionsBy
-0003f6f0: 436c 6173 7300 5f79 6170 6947 6574 4675  Class._yapiGetFu
-0003f700: 6e63 7469 6f6e 7342 7944 6576 6963 6500  nctionsByDevice.
-0003f710: 5f79 6170 6947 6574 4d65 6d00 5f79 6170  _yapiGetMem._yap
-0003f720: 6947 6574 4e65 7444 6576 4c69 7374 5661  iGetNetDevListVa
-0003f730: 6c69 6469 7479 005f 7961 7069 4765 744e  lidity._yapiGetN
-0003f740: 6574 776f 726b 5469 6d65 6f75 7400 5f79  etworkTimeout._y
-0003f750: 6170 6947 6574 5375 6264 6576 6963 6573  apiGetSubdevices
-0003f760: 005f 7961 7069 4765 7454 6963 6b43 6f75  ._yapiGetTickCou
-0003f770: 6e74 005f 7961 7069 4854 5450 5265 7175  nt._yapiHTTPRequ
-0003f780: 6573 7400 5f79 6170 6948 5454 5052 6571  est._yapiHTTPReq
-0003f790: 7565 7374 4173 796e 6300 5f79 6170 6948  uestAsync._yapiH
-0003f7a0: 5454 5052 6571 7565 7374 4173 796e 6345  TTPRequestAsyncE
-0003f7b0: 7800 5f79 6170 6948 5454 5052 6571 7565  x._yapiHTTPReque
-0003f7c0: 7374 4173 796e 634f 7574 4f66 4261 6e64  stAsyncOutOfBand
-0003f7d0: 005f 7961 7069 4854 5450 5265 7175 6573  ._yapiHTTPReques
-0003f7e0: 7453 796e 6344 6f6e 6500 5f79 6170 6948  tSyncDone._yapiH
-0003f7f0: 5454 5052 6571 7565 7374 5379 6e63 446f  TTPRequestSyncDo
-0003f800: 6e65 5f69 6e74 6572 6e61 6c00 5f79 6170  ne_internal._yap
-0003f810: 6948 5454 5052 6571 7565 7374 5379 6e63  iHTTPRequestSync
-0003f820: 5374 6172 7400 5f79 6170 6948 5454 5052  Start._yapiHTTPR
-0003f830: 6571 7565 7374 5379 6e63 5374 6172 7445  equestSyncStartE
-0003f840: 7800 5f79 6170 6948 5454 5052 6571 7565  x._yapiHTTPReque
-0003f850: 7374 5379 6e63 5374 6172 7445 785f 696e  stSyncStartEx_in
-0003f860: 7465 726e 616c 005f 7961 7069 4854 5450  ternal._yapiHTTP
-0003f870: 5265 7175 6573 7453 796e 6353 7461 7274  RequestSyncStart
-0003f880: 4f75 744f 6642 616e 6400 5f79 6170 6948  OutOfBand._yapiH
-0003f890: 616e 646c 6545 7665 6e74 7300 5f79 6170  andleEvents._yap
-0003f8a0: 6949 6e69 7441 5049 005f 7961 7069 4973  iInitAPI._yapiIs
-0003f8b0: 4d6f 6475 6c65 5772 6974 6162 6c65 005f  ModuleWritable._
-0003f8c0: 7961 7069 4a73 6f6e 4465 636f 6465 5374  yapiJsonDecodeSt
-0003f8d0: 7269 6e67 005f 7961 7069 4a73 6f6e 4765  ring._yapiJsonGe
-0003f8e0: 7450 6174 6800 5f79 6170 694a 736f 6e47  tPath._yapiJsonG
-0003f8f0: 6574 5061 7468 5f69 6e74 6572 6e61 6c00  etPath_internal.
-0003f900: 5f79 6170 694c 6f63 6b44 6576 6963 6543  _yapiLockDeviceC
-0003f910: 616c 6c42 6163 6b00 5f79 6170 694c 6f63  allBack._yapiLoc
-0003f920: 6b46 756e 6374 696f 6e43 616c 6c42 6163  kFunctionCallBac
-0003f930: 6b00 5f79 6170 6950 7265 7265 6769 7374  k._yapiPreregist
-0003f940: 6572 4875 6200 5f79 6170 6950 756c 6c44  erHub._yapiPullD
-0003f950: 6576 6963 654c 6f67 005f 7961 7069 5075  eviceLog._yapiPu
-0003f960: 6c6c 4465 7669 6365 4c6f 6745 7800 5f79  llDeviceLogEx._y
-0003f970: 6170 6952 6567 6973 7465 7242 6561 636f  apiRegisterBeaco
-0003f980: 6e43 616c 6c62 6163 6b00 5f79 6170 6952  nCallback._yapiR
-0003f990: 6567 6973 7465 7244 6576 6963 6541 7272  egisterDeviceArr
-0003f9a0: 6976 616c 4361 6c6c 6261 636b 005f 7961  ivalCallback._ya
-0003f9b0: 7069 5265 6769 7374 6572 4465 7669 6365  piRegisterDevice
-0003f9c0: 4368 616e 6765 4361 6c6c 6261 636b 005f  ChangeCallback._
-0003f9d0: 7961 7069 5265 6769 7374 6572 4465 7669  yapiRegisterDevi
-0003f9e0: 6365 436f 6e66 6967 4368 616e 6765 4361  ceConfigChangeCa
-0003f9f0: 6c6c 6261 636b 005f 7961 7069 5265 6769  llback._yapiRegi
-0003fa00: 7374 6572 4465 7669 6365 4c6f 6743 616c  sterDeviceLogCal
-0003fa10: 6c62 6163 6b00 5f79 6170 6952 6567 6973  lback._yapiRegis
-0003fa20: 7465 7244 6576 6963 6552 656d 6f76 616c  terDeviceRemoval
-0003fa30: 4361 6c6c 6261 636b 005f 7961 7069 5265  Callback._yapiRe
-0003fa40: 6769 7374 6572 4675 6e63 7469 6f6e 5570  gisterFunctionUp
-0003fa50: 6461 7465 4361 6c6c 6261 636b 005f 7961  dateCallback._ya
-0003fa60: 7069 5265 6769 7374 6572 4875 6200 5f79  piRegisterHub._y
-0003fa70: 6170 6952 6567 6973 7465 7248 7562 4469  apiRegisterHubDi
-0003fa80: 7363 6f76 6572 7943 616c 6c62 6163 6b00  scoveryCallback.
-0003fa90: 5f79 6170 6952 6567 6973 7465 724c 6f67  _yapiRegisterLog
-0003faa0: 4675 6e63 7469 6f6e 005f 7961 7069 5265  Function._yapiRe
-0003fab0: 6769 7374 6572 5261 774e 6f74 6966 6963  gisterRawNotific
-0003fac0: 6174 696f 6e43 6200 5f79 6170 6952 6567  ationCb._yapiReg
-0003fad0: 6973 7465 7252 6177 5265 706f 7274 4362  isterRawReportCb
-0003fae0: 005f 7961 7069 5265 6769 7374 6572 5261  ._yapiRegisterRa
-0003faf0: 7752 6570 6f72 7456 3243 6200 5f79 6170  wReportV2Cb._yap
-0003fb00: 6952 6567 6973 7465 7254 696d 6564 5265  iRegisterTimedRe
-0003fb10: 706f 7274 4361 6c6c 6261 636b 005f 7961  portCallback._ya
-0003fb20: 7069 5265 6769 7374 6572 5761 6b65 5570  piRegisterWakeUp
-0003fb30: 4362 005f 7961 7069 5265 7175 6573 744f  Cb._yapiRequestO
-0003fb40: 7065 6e00 5f79 6170 6953 6574 4e65 7444  pen._yapiSetNetD
-0003fb50: 6576 4c69 7374 5661 6c69 6469 7479 005f  evListValidity._
-0003fb60: 7961 7069 5365 744e 6574 776f 726b 5469  yapiSetNetworkTi
-0003fb70: 6d65 6f75 7400 5f79 6170 6953 6574 5472  meout._yapiSetTr
-0003fb80: 6163 6546 696c 6500 5f79 6170 6953 6c65  aceFile._yapiSle
-0003fb90: 6570 005f 7961 7069 5374 6172 7453 746f  ep._yapiStartSto
-0003fba0: 7044 6576 6963 654c 6f67 4361 6c6c 6261  pDeviceLogCallba
-0003fbb0: 636b 005f 7961 7069 5465 7374 4875 6200  ck._yapiTestHub.
-0003fbc0: 5f79 6170 6954 7269 6767 6572 4875 6244  _yapiTriggerHubD
-0003fbd0: 6973 636f 7665 7279 005f 7961 7069 556e  iscovery._yapiUn
-0003fbe0: 6c6f 636b 4465 7669 6365 4361 6c6c 4261  lockDeviceCallBa
-0003fbf0: 636b 005f 7961 7069 556e 6c6f 636b 4675  ck._yapiUnlockFu
-0003fc00: 6e63 7469 6f6e 4361 6c6c 4261 636b 005f  nctionCallBack._
-0003fc10: 7961 7069 556e 7265 6769 7374 6572 4875  yapiUnregisterHu
-0003fc20: 6200 5f79 6170 6955 7064 6174 6544 6576  b._yapiUpdateDev
-0003fc30: 6963 654c 6973 7400 5f79 6170 6955 7064  iceList._yapiUpd
-0003fc40: 6174 6546 6972 6d77 6172 6500 5f79 6170  ateFirmware._yap
-0003fc50: 6955 7064 6174 6546 6972 6d77 6172 6545  iUpdateFirmwareE
-0003fc60: 7800 5f79 6170 6955 7064 6174 6546 6972  x._yapiUpdateFir
-0003fc70: 6d77 6172 655f 696e 7465 726e 616c 005f  mware_internal._
-0003fc80: 796d 656d 6669 6e64 005f 7970 4669 6e64  ymemfind._ypFind
-0003fc90: 426f 6f74 6c6f 6164 6572 7300 5f79 7047  Bootloaders._ypG
-0003fca0: 6574 4174 7472 6962 7574 6573 005f 7970  etAttributes._yp
-0003fcb0: 4765 7441 7474 7269 6275 7465 7342 7959  GetAttributesByY
-0003fcc0: 6478 005f 7970 4765 7442 6f6f 746c 6f61  dx._ypGetBootloa
-0003fcd0: 6465 7252 6570 6c79 005f 7970 4765 7443  derReply._ypGetC
-0003fce0: 6174 6567 6f72 7900 5f79 7047 6574 4675  ategory._ypGetFu
-0003fcf0: 6e63 7469 6f6e 496e 666f 005f 7970 4765  nctionInfo._ypGe
-0003fd00: 7446 756e 6374 696f 6e73 005f 7970 4765  tFunctions._ypGe
-0003fd10: 7446 756e 6374 696f 6e73 4578 005f 7970  tFunctionsEx._yp
-0003fd20: 4765 7454 7970 6500 5f79 7049 7353 656e  GetType._ypIsSen
-0003fd30: 6442 6f6f 746c 6f61 6465 7242 7573 7900  dBootloaderBusy.
-0003fd40: 5f79 7052 6567 6973 7465 7200 5f79 7052  _ypRegister._ypR
-0003fd50: 6567 6973 7465 7242 7959 6478 005f 7970  egisterByYdx._yp
-0003fd60: 5365 6172 6368 005f 7970 5365 6e64 426f  Search._ypSendBo
-0003fd70: 6f74 6c6f 6164 6572 436d 6400 5f79 7055  otloaderCmd._ypU
-0003fd80: 7064 6174 6554 4350 005f 7970 5570 6461  pdateTCP._ypUpda
-0003fd90: 7465 5964 7800 5f79 7370 7269 6e74 665f  teYdx._ysprintf_
-0003fda0: 7300 5f79 7374 7263 6174 5f73 005f 7973  s._ystrcat_s._ys
-0003fdb0: 7472 6370 795f 7300 5f79 7374 7264 7570  trcpy_s._ystrdup
-0003fdc0: 5f73 005f 7973 7472 6e63 6174 5f73 005f  _s._ystrncat_s._
-0003fdd0: 7973 7472 6e63 7079 5f73 005f 7973 7472  ystrncpy_s._ystr
-0003fde0: 6e64 7570 5f73 005f 7974 7261 6365 6669  ndup_s._ytracefi
-0003fdf0: 6c65 005f 7976 7370 7269 6e74 665f 7300  le._yvsprintf_s.
-0003fe00: 5f79 7770 4765 7444 6576 6963 6548 7562  _ywpGetDeviceHub
-0003fe10: 005f 7977 7047 6574 4465 7669 6365 5572  ._ywpGetDeviceUr
-0003fe20: 6c00 5f79 7770 5361 6665 5265 6769 7374  l._ywpSafeRegist
-0003fe30: 6572 005f 7977 7053 6166 6555 6e72 6567  er._ywpSafeUnreg
-0003fe40: 6973 7465 7200 5f79 7770 5361 6665 5570  ister._ywpSafeUp
-0003fe50: 6461 7465 005f 7978 746f 6100 5f79 7979  date._yxtoa._yyy
-0003fe60: 4f53 6864 6c43 6f6d 7061 7265 005f 7979  OShdlCompare._yy
-0003fe70: 7950 6163 6b65 7453 6875 7464 6f77 6e00  yPacketShutdown.
-0003fe80: 5f79 7979 5365 6e64 5061 636b 6574 005f  _yyySendPacket._
-0003fe90: 7979 7953 6574 7570 005f 7979 7953 6967  yyySetup._yyySig
-0003fea0: 6e61 6c4f 7574 506b 7400 5f79 7979 5553  nalOutPkt._yyyUS
-0003feb0: 4247 6574 496e 7465 7266 6163 6573 005f  BGetInterfaces._
-0003fec0: 7979 7955 5342 5f69 6e69 7400 5f79 7979  yyyUSB_init._yyy
-0003fed0: 5553 425f 7374 6f70 005f 4346 4469 6374  USB_stop._CFDict
-0003fee0: 696f 6e61 7279 4372 6561 7465 4d75 7461  ionaryCreateMuta
-0003fef0: 626c 6500 5f43 4644 6963 7469 6f6e 6172  ble._CFDictionar
-0003ff00: 7953 6574 5661 6c75 6500 5f43 4647 6574  ySetValue._CFGet
-0003ff10: 5479 7065 4944 005f 4346 4e75 6d62 6572  TypeID._CFNumber
-0003ff20: 4372 6561 7465 005f 4346 4e75 6d62 6572  Create._CFNumber
-0003ff30: 4765 7454 7970 6549 4400 5f43 464e 756d  GetTypeID._CFNum
-0003ff40: 6265 7247 6574 5661 6c75 6500 5f43 4652  berGetValue._CFR
-0003ff50: 656c 6561 7365 005f 4346 5275 6e4c 6f6f  elease._CFRunLoo
-0003ff60: 7047 6574 4375 7272 656e 7400 5f43 4652  pGetCurrent._CFR
-0003ff70: 756e 4c6f 6f70 5275 6e49 6e4d 6f64 6500  unLoopRunInMode.
-0003ff80: 5f43 4652 756e 4c6f 6f70 5374 6f70 005f  _CFRunLoopStop._
-0003ff90: 4346 5365 7447 6574 436f 756e 7400 5f43  CFSetGetCount._C
-0003ffa0: 4653 6574 4765 7456 616c 7565 7300 5f43  FSetGetValues._C
-0003ffb0: 4653 7472 696e 6743 7265 6174 6557 6974  FStringCreateWit
-0003ffc0: 6843 5374 7269 6e67 005f 4346 5374 7269  hCString._CFStri
-0003ffd0: 6e67 4765 7443 5374 7269 6e67 005f 4346  ngGetCString._CF
-0003ffe0: 5374 7269 6e67 4765 7443 5374 7269 6e67  StringGetCString
-0003fff0: 5074 7200 5f43 4653 7472 696e 6747 6574  Ptr._CFStringGet
-00040000: 4c65 6e67 7468 005f 4346 5374 7269 6e67  Length._CFString
-00040010: 4765 7453 7973 7465 6d45 6e63 6f64 696e  GetSystemEncodin
-00040020: 6700 5f43 4653 7472 696e 6747 6574 5479  g._CFStringGetTy
-00040030: 7065 4944 005f 494f 4849 4444 6576 6963  peID._IOHIDDevic
-00040040: 6543 6c6f 7365 005f 494f 4849 4444 6576  eClose._IOHIDDev
-00040050: 6963 6547 6574 5072 6f70 6572 7479 005f  iceGetProperty._
-00040060: 494f 4849 4444 6576 6963 654f 7065 6e00  IOHIDDeviceOpen.
-00040070: 5f49 4f48 4944 4465 7669 6365 5265 6769  _IOHIDDeviceRegi
-00040080: 7374 6572 496e 7075 7452 6570 6f72 7443  sterInputReportC
-00040090: 616c 6c62 6163 6b00 5f49 4f48 4944 4465  allback._IOHIDDe
-000400a0: 7669 6365 5363 6865 6475 6c65 5769 7468  viceScheduleWith
-000400b0: 5275 6e4c 6f6f 7000 5f49 4f48 4944 4465  RunLoop._IOHIDDe
-000400c0: 7669 6365 5365 7452 6570 6f72 7400 5f49  viceSetReport._I
-000400d0: 4f48 4944 4d61 6e61 6765 7243 6c6f 7365  OHIDManagerClose
-000400e0: 005f 494f 4849 444d 616e 6167 6572 436f  ._IOHIDManagerCo
-000400f0: 7079 4465 7669 6365 7300 5f49 4f48 4944  pyDevices._IOHID
-00040100: 4d61 6e61 6765 7243 7265 6174 6500 5f49  ManagerCreate._I
-00040110: 4f48 4944 4d61 6e61 6765 7247 6574 5479  OHIDManagerGetTy
-00040120: 7065 4944 005f 494f 4849 444d 616e 6167  peID._IOHIDManag
-00040130: 6572 4f70 656e 005f 494f 4849 444d 616e  erOpen._IOHIDMan
-00040140: 6167 6572 5363 6865 6475 6c65 5769 7468  agerScheduleWith
-00040150: 5275 6e4c 6f6f 7000 5f49 4f48 4944 4d61  RunLoop._IOHIDMa
-00040160: 6e61 6765 7253 6574 4465 7669 6365 4d61  nagerSetDeviceMa
-00040170: 7463 6869 6e67 005f 5f44 6566 6175 6c74  tching.__Default
-00040180: 5275 6e65 4c6f 6361 6c65 005f 5f5f 4346  RuneLocale.___CF
-00040190: 436f 6e73 7461 6e74 5374 7269 6e67 436c  ConstantStringCl
-000401a0: 6173 7352 6566 6572 656e 6365 005f 5f5f  assReference.___
-000401b0: 5f63 686b 7374 6b5f 6461 7277 696e 005f  _chkstk_darwin._
-000401c0: 5f5f 627a 6572 6f00 5f5f 5f64 6172 7769  __bzero.___darwi
-000401d0: 6e5f 6368 6563 6b5f 6664 5f73 6574 5f6f  n_check_fd_set_o
-000401e0: 7665 7266 6c6f 7700 5f5f 5f65 7272 6f72  verflow.___error
-000401f0: 005f 5f5f 6d65 6d63 7079 5f63 686b 005f  .___memcpy_chk._
-00040200: 5f5f 7370 7269 6e74 665f 6368 6b00 5f5f  __sprintf_chk.__
-00040210: 5f73 7461 636b 5f63 686b 5f66 6169 6c00  _stack_chk_fail.
-00040220: 5f5f 5f73 7461 636b 5f63 686b 5f67 7561  ___stack_chk_gua
-00040230: 7264 005f 6174 6f66 005f 6174 6f69 005f  rd._atof._atoi._
-00040240: 6269 6e64 005f 6361 6c6c 6f63 005f 636c  bind._calloc._cl
-00040250: 6f73 6500 5f63 6c6f 7365 6469 7200 5f63  ose._closedir._c
-00040260: 6f6e 6e65 6374 005f 6663 6c6f 7365 005f  onnect._fclose._
-00040270: 6663 6e74 6c00 5f66 6f70 656e 005f 6670  fcntl._fopen._fp
-00040280: 7269 6e74 6600 5f66 7265 6164 005f 6672  rintf._fread._fr
-00040290: 6565 005f 6672 6565 6164 6472 696e 666f  ee._freeaddrinfo
-000402a0: 005f 6673 6565 6b00 5f66 7465 6c6c 005f  ._fseek._ftell._
-000402b0: 6677 7269 7465 005f 6765 7461 6464 7269  fwrite._getaddri
-000402c0: 6e66 6f00 5f67 6574 6966 6164 6472 7300  nfo._getifaddrs.
-000402d0: 5f67 6574 7069 6400 5f67 6574 736f 636b  _getpid._getsock
-000402e0: 6e61 6d65 005f 6765 7473 6f63 6b6f 7074  name._getsockopt
-000402f0: 005f 6765 7474 696d 656f 6664 6179 005f  ._gettimeofday._
-00040300: 696e 6574 5f61 6464 7200 5f6b 4346 416c  inet_addr._kCFAl
-00040310: 6c6f 6361 746f 7244 6566 6175 6c74 005f  locatorDefault._
-00040320: 6b43 4652 756e 4c6f 6f70 4465 6661 756c  kCFRunLoopDefaul
-00040330: 744d 6f64 6500 5f6b 4346 5479 7065 4469  tMode._kCFTypeDi
-00040340: 6374 696f 6e61 7279 4b65 7943 616c 6c42  ctionaryKeyCallB
-00040350: 6163 6b73 005f 6b43 4654 7970 6544 6963  acks._kCFTypeDic
-00040360: 7469 6f6e 6172 7956 616c 7565 4361 6c6c  tionaryValueCall
-00040370: 4261 636b 7300 5f6d 616c 6c6f 6300 5f6d  Backs._malloc._m
-00040380: 656d 636d 7000 5f6d 656d 6370 7900 5f6d  emcmp._memcpy._m
-00040390: 656d 7365 7400 5f6d 6b66 6966 6f00 5f6f  emset._mkfifo._o
-000403a0: 626a 635f 6d73 6753 656e 6400 5f6f 7065  bjc_msgSend._ope
-000403b0: 6e00 5f6f 7065 6e64 6972 2449 4e4f 4445  n._opendir$INODE
-000403c0: 3634 005f 7074 6872 6561 645f 6174 7472  64._pthread_attr
-000403d0: 5f64 6573 7472 6f79 005f 7074 6872 6561  _destroy._pthrea
-000403e0: 645f 6174 7472 5f69 6e69 7400 5f70 7468  d_attr_init._pth
-000403f0: 7265 6164 5f61 7474 725f 7365 7464 6574  read_attr_setdet
-00040400: 6163 6873 7461 7465 005f 7074 6872 6561  achstate._pthrea
-00040410: 645f 6361 6e63 656c 005f 7074 6872 6561  d_cancel._pthrea
-00040420: 645f 636f 6e64 5f64 6573 7472 6f79 005f  d_cond_destroy._
-00040430: 7074 6872 6561 645f 636f 6e64 5f69 6e69  pthread_cond_ini
-00040440: 7400 5f70 7468 7265 6164 5f63 6f6e 645f  t._pthread_cond_
-00040450: 7369 676e 616c 005f 7074 6872 6561 645f  signal._pthread_
-00040460: 636f 6e64 5f74 696d 6564 7761 6974 005f  cond_timedwait._
-00040470: 7074 6872 6561 645f 636f 6e64 5f77 6169  pthread_cond_wai
-00040480: 7400 5f70 7468 7265 6164 5f63 7265 6174  t._pthread_creat
-00040490: 6500 5f70 7468 7265 6164 5f67 6574 7370  e._pthread_getsp
-000404a0: 6563 6966 6963 005f 7074 6872 6561 645f  ecific._pthread_
-000404b0: 6a6f 696e 005f 7074 6872 6561 645f 6b65  join._pthread_ke
-000404c0: 795f 6372 6561 7465 005f 7074 6872 6561  y_create._pthrea
-000404d0: 645f 6d75 7465 785f 6465 7374 726f 7900  d_mutex_destroy.
-000404e0: 5f70 7468 7265 6164 5f6d 7574 6578 5f69  _pthread_mutex_i
-000404f0: 6e69 7400 5f70 7468 7265 6164 5f6d 7574  nit._pthread_mut
-00040500: 6578 5f6c 6f63 6b00 5f70 7468 7265 6164  ex_lock._pthread
-00040510: 5f6d 7574 6578 5f74 7279 6c6f 636b 005f  _mutex_trylock._
-00040520: 7074 6872 6561 645f 6d75 7465 785f 756e  pthread_mutex_un
-00040530: 6c6f 636b 005f 7074 6872 6561 645f 6d75  lock._pthread_mu
-00040540: 7465 7861 7474 725f 696e 6974 005f 7074  texattr_init._pt
-00040550: 6872 6561 645f 6d75 7465 7861 7474 725f  hread_mutexattr_
-00040560: 7365 7474 7970 6500 5f70 7468 7265 6164  settype._pthread
-00040570: 5f6f 6e63 6500 5f70 7468 7265 6164 5f73  _once._pthread_s
-00040580: 6574 7370 6563 6966 6963 005f 7261 6e64  etspecific._rand
-00040590: 005f 7265 6164 005f 7265 6164 6469 7224  ._read._readdir$
-000405a0: 494e 4f44 4536 3400 5f72 6563 7600 5f73  INODE64._recv._s
-000405b0: 656c 6563 7424 3130 3530 005f 7365 6e64  elect$1050._send
-000405c0: 005f 7365 6e64 746f 005f 7365 7473 6f63  ._sendto._setsoc
-000405d0: 6b6f 7074 005f 736f 636b 6574 005f 7374  kopt._socket._st
-000405e0: 6174 2449 4e4f 4445 3634 005f 7374 7263  at$INODE64._strc
-000405f0: 6173 6563 6d70 005f 7374 7263 6872 005f  asecmp._strchr._
-00040600: 7374 7263 6d70 005f 7374 7263 7079 005f  strcmp._strcpy._
-00040610: 7374 7265 7272 6f72 005f 7374 726c 656e  strerror._strlen
-00040620: 005f 7374 726e 6361 7365 636d 7000 5f73  ._strncasecmp._s
-00040630: 7472 6e63 6d70 005f 7374 7273 7472 005f  trncmp._strstr._
-00040640: 7379 7363 746c 6279 6e61 6d65 005f 7469  sysctlbyname._ti
-00040650: 6d65 005f 7573 6c65 6570 005f 7673 6e70  me._usleep._vsnp
-00040660: 7269 6e74 6600 5f77 7269 7465 005f 7954  rintf._write._yT
-00040670: 6370 4f70 656e 005f 7954 6370 5772 6974  cpOpen._yTcpWrit
-00040680: 6500 5f79 5463 7052 6561 6400 5f79 4854  e._yTcpRead._yHT
-00040690: 5450 4f70 656e 5265 7145 7800 5f79 4854  TPOpenReqEx._yHT
-000406a0: 5450 4d75 6c74 6953 656c 6563 7452 6571  TPMultiSelectReq
-000406b0: 005f 7954 6370 4368 6563 6b52 6571 5469  ._yTcpCheckReqTi
-000406c0: 6d65 6f75 7400 5f79 4854 5450 436c 6f73  meout._yHTTPClos
-000406d0: 6552 6571 4578 005f 7957 5343 6c6f 7365  eReqEx._yWSClose
-000406e0: 5265 7100 5f79 5753 5265 6d6f 7665 5265  Req._yWSRemoveRe
-000406f0: 7100 5f63 6c6f 7365 416c 6c52 6571 005f  q._closeAllReq._
-00040700: 7953 5344 505f 7468 7265 6164 005f 7265  ySSDP_thread._re
-00040710: 736f 6c76 6544 4e53 4361 6368 6500 5f42  solveDNSCache._B
-00040720: 6173 6536 3445 6e63 6f64 6500 5f77 735f  ase64Encode._ws_
-00040730: 6170 7065 6e64 5443 5044 6174 6100 5f77  appendTCPData._w
-00040740: 735f 7365 6e64 4672 616d 6500 5f79 5353  s_sendFrame._ySS
-00040750: 4450 5f70 6172 7365 5353 5044 4d65 7373  DP_parseSSPDMess
-00040760: 6167 6500 5f79 7055 7064 6174 6555 5342  age._ypUpdateUSB
-00040770: 005f 7950 6b74 5175 6575 6550 7573 6845  ._yPktQueuePushE
-00040780: 7800 5f79 506b 7451 7565 7565 506f 7000  x._yPktQueuePop.
-00040790: 5f65 6e75 5570 6461 7465 4453 7461 7475  _enuUpdateDStatu
-000407a0: 7300 5f79 4469 7370 6174 6368 5265 6365  s._yDispatchRece
-000407b0: 6976 6500 5f79 5374 7265 616d 5472 616e  ive._yStreamTran
-000407c0: 736d 6974 005f 7953 7472 6561 6d46 6c75  smit._yStreamFlu
-000407d0: 7368 005f 6465 7652 6570 6f72 7445 7272  sh._devReportErr
-000407e0: 6f72 005f 6465 7653 746f 7049 4f00 5f64  or._devStopIO._d
-000407f0: 6576 5061 7573 6549 4f00 5f64 6576 4368  evPauseIO._devCh
-00040800: 6563 6b49 4f00 5f64 6576 5374 6172 7445  eckIO._devStartE
-00040810: 6e75 6d00 5f53 7461 7274 4465 7669 6365  num._StartDevice
-00040820: 005f 7953 7472 6561 6d53 6875 7464 6f77  ._yStreamShutdow
-00040830: 6e00 5f79 7957 6169 744f 6e6c 7943 6f6e  n._yyWaitOnlyCon
-00040840: 6650 6b74 005f 7953 7472 6561 6d52 6563  fPkt._yStreamRec
-00040850: 6569 7665 6400 5f79 4469 7370 6174 6368  eived._yDispatch
-00040860: 4e6f 7469 6365 005f 7950 726f 674c 6f67  Notice._yProgLog
-00040870: 5072 6f67 7265 7373 005f 7547 6574 4465  Progress._uGetDe
-00040880: 7669 6365 496e 666f 005f 7947 6574 4669  viceInfo._yGetFi
-00040890: 726d 7761 7265 005f 6973 5765 6250 6174  rmware._isWebPat
-000408a0: 6800 5f79 6170 6943 6865 636b 4669 726d  h._yapiCheckFirm
-000408b0: 7761 7265 5f72 005f 7953 7461 7274 4669  ware_r._yStartFi
-000408c0: 726d 7761 7265 5570 6461 7465 005f 7961  rmwareUpdate._ya
-000408d0: 7069 4368 6563 6b46 6972 6d77 6172 6546  piCheckFirmwareF
-000408e0: 696c 6500 5f79 4c6f 6164 4669 726d 7761  ile._yLoadFirmwa
-000408f0: 7265 4669 6c65 005f 7946 6972 6d77 6172  reFile._yFirmwar
-00040900: 6555 7064 6174 655f 7468 7265 6164 005f  eUpdate_thread._
-00040910: 6f73 5072 6f67 4c6f 6750 726f 6772 6573  osProgLogProgres
-00040920: 7345 7800 5f73 656e 6448 7562 466c 6173  sEx._sendHubFlas
-00040930: 6843 6d64 005f 7570 6c6f 6164 005f 6368  hCmd._upload._ch
-00040940: 6563 6b48 5454 5048 6561 6465 7200 5f69  eckHTTPHeader._i
-00040950: 6e69 7473 6861 7700 5f69 7465 7273 6861  nitshaw._itersha
-00040960: 7700 5f4d 4435 5472 616e 7366 6f72 6d00  w._MD5Transform.
-00040970: 5f79 426c 6b41 6c6c 6f63 005f 7948 6173  _yBlkAlloc._yHas
-00040980: 6850 7574 005f 7942 6c6b 4672 6565 005f  hPut._yBlkFree._
-00040990: 6576 656e 745f 7468 7265 6164 005f 7365  event_thread._se
-000409a0: 7475 7048 4944 4d61 6e61 6765 7200 5f73  tupHIDManager._s
-000409b0: 746f 7048 4944 4d61 6e61 6765 7200 5f67  topHIDManager._g
-000409c0: 6574 4465 7652 6566 005f 6765 745f 696e  etDevRef._get_in
-000409d0: 745f 7072 6f70 6572 7479 005f 6765 745f  t_property._get_
-000409e0: 7478 745f 7072 6f70 6572 7479 005f 4861  txt_property._Ha
-000409f0: 6e64 6c65 5f49 4f48 4944 4465 7669 6365  ndle_IOHIDDevice
-00040a00: 494f 4849 4452 6570 6f72 7443 616c 6c62  IOHIDReportCallb
-00040a10: 6163 6b00 5f79 6170 6952 6571 7565 7374  ack._yapiRequest
-00040a20: 4f70 656e 5553 4200 5f6c 6f67 5265 7375  OpenUSB._logResu
-00040a30: 6c74 005f 7961 7069 5265 7175 6573 744f  lt._yapiRequestO
-00040a40: 7065 6e57 5300 5f79 6170 6952 6571 7565  penWS._yapiReque
-00040a50: 7374 4f70 656e 4854 5450 005f 756e 7265  stOpenHTTP._unre
-00040a60: 6769 7374 6572 4e65 7444 6576 6963 6500  gisterNetDevice.
-00040a70: 5f75 6e70 6163 6b48 5454 5052 6571 7565  _unpackHTTPReque
-00040a80: 7374 005f 7961 7069 5265 7175 6573 7443  st._yapiRequestC
-00040a90: 6c6f 7365 005f 7961 7069 4a73 6f6e 5661  lose._yapiJsonVa
-00040aa0: 6c75 6550 6172 7365 5374 7275 6374 005f  lueParseStruct._
-00040ab0: 7961 7069 496e 6974 4150 495f 696e 7465  yapiInitAPI_inte
-00040ac0: 726e 616c 005f 7961 7069 4672 6565 4150  rnal._yapiFreeAP
-00040ad0: 495f 696e 7465 726e 616c 005f 7961 7069  I_internal._yapi
-00040ae0: 556e 7265 6769 7374 6572 4875 625f 696e  UnregisterHub_in
-00040af0: 7465 726e 616c 005f 7961 7069 5570 6461  ternal._yapiUpda
-00040b00: 7465 4465 7669 6365 4c69 7374 5f69 6e74  teDeviceList_int
-00040b10: 6572 6e61 6c00 5f79 6170 6948 616e 646c  ernal._yapiHandl
-00040b20: 6545 7665 6e74 735f 696e 7465 726e 616c  eEvents_internal
-00040b30: 005f 7961 7069 4765 7446 756e 6374 696f  ._yapiGetFunctio
-00040b40: 6e49 6e66 6f45 785f 696e 7465 726e 616c  nInfoEx_internal
-00040b50: 005f 7961 7069 4854 5450 5265 7175 6573  ._yapiHTTPReques
-00040b60: 7441 7379 6e63 4578 5f69 6e74 6572 6e61  tAsyncEx_interna
-00040b70: 6c00 5f64 656c 6574 6541 6c6c 4353 005f  l._deleteAllCS._
-00040b80: 7373 6470 456e 7472 7955 7064 6174 6500  ssdpEntryUpdate.
-00040b90: 5f75 6e72 6567 6973 7465 724e 6574 4875  _unregisterNetHu
-00040ba0: 6200 5f69 7353 616d 6548 7562 005f 7961  b._isSameHub._ya
-00040bb0: 7069 4672 6565 4875 6200 5f79 4672 6565  piFreeHub._yFree
-00040bc0: 5061 7273 6564 5552 4c00 5f79 6170 6941  ParsedURL._yapiA
-00040bd0: 6c6c 6f63 4875 6200 5f70 696e 6755 524c  llocHub._pingURL
-00040be0: 4f6e 6875 6200 5f79 5061 7273 6548 7562  Onhub._yParseHub
-00040bf0: 5552 4c00 5f79 6170 6952 6567 6973 7465  URL._yapiRegiste
-00040c00: 7248 7562 4578 005f 7968 656c 7065 725f  rHubEx._yhelper_
-00040c10: 7468 7265 6164 005f 794e 6574 4875 6245  thread._yNetHubE
-00040c20: 6e75 6d00 5f79 4e65 7448 7562 456e 756d  num._yNetHubEnum
-00040c30: 4578 005f 6469 7361 626c 655f 6a7a 6f6e  Ex._disable_jzon
-00040c40: 005f 7061 7273 654e 6574 5770 456e 7472  ._parseNetWpEntr
-00040c50: 7900 5f79 7055 7064 6174 654e 6574 005f  y._ypUpdateNet._
-00040c60: 6173 796e 6344 726f 7000 5f79 4372 6561  asyncDrop._yCrea
-00040c70: 7465 4465 7461 6368 6564 5468 7265 6164  teDetachedThread
-00040c80: 4578 005f 696e 6974 5473 644b 6579 005f  Ex._initTsdKey._
-00040c90: 6461 796f 6673 005f 7770 616b 005f 6e65  dayofs._wpak._ne
-00040ca0: 7874 4361 7459 6478 005f 6e65 7874 4861  xtCatYdx._nextHa
-00040cb0: 7368 456e 7472 7900 5f79 496e 6974 4b65  shEntry._yInitKe
-00040cc0: 794f 6e63 6500 5f79 4e65 7874 5468 7265  yOnce._yNextThre
-00040cd0: 6164 4964 7800 5f79 4861 7368 5461 626c  adIdx._yHashTabl
-00040ce0: 6500 5f64 6576 5964 7850 7472 005f 6675  e._devYdxPtr._fu
-00040cf0: 6e59 6478 5074 7200 5f6e 6578 7444 6576  nYdxPtr._nextDev
-00040d00: 5964 7800 5f75 7365 6444 6576 5964 7800  Ydx._usedDevYdx.
-00040d10: 5f77 704c 6f63 6b43 6f75 6e74 005f 7770  _wpLockCount._wp
-00040d20: 536f 6d65 7468 696e 6755 6e72 6567 6973  SomethingUnregis
-00040d30: 7465 7265 6400 5f79 5473 644b 6579 002f  tered._yTsdKey./
-00040d40: 5573 6572 732f 796f 6374 6f2f 746d 705f  Users/yocto/tmp_
-00040d50: 6275 696c 642f 796f 6374 6f70 726f 642f  build/yoctoprod/
-00040d60: 796f 6374 6f6c 6962 2f76 312e 302f 5075  yoctolib/v1.0/Pu
-00040d70: 626c 6963 2f63 7070 2f53 6f75 7263 6573  blic/cpp/Sources
-00040d80: 2f79 6170 692f 0079 6d65 6d6f 7279 2e63  /yapi/.ymemory.c
-00040d90: 002f 5573 6572 732f 796f 6374 6f2f 746d  ./Users/yocto/tm
-00040da0: 705f 6275 696c 642f 796f 6374 6f70 726f  p_build/yoctopro
-00040db0: 642f 796f 6374 6f6c 6962 2f76 312e 302f  d/yoctolib/v1.0/
-00040dc0: 5075 626c 6963 2f63 7070 2f42 696e 6172  Public/cpp/Binar
-00040dd0: 6965 732f 7863 6f64 655f 6173 2f79 6170  ies/xcode_as/yap
-00040de0: 692f 6275 696c 642f 7961 7069 2e62 7569  i/build/yapi.bui
-00040df0: 6c64 2f52 656c 6561 7365 2f79 6170 692e  ld/Release/yapi.
-00040e00: 6275 696c 642f 4f62 6a65 6374 732d 6e6f  build/Objects-no
-00040e10: 726d 616c 2f78 3836 5f36 342f 796d 656d  rmal/x86_64/ymem
-00040e20: 6f72 792e 6f00 5f79 7374 7263 7079 5f73  ory.o._ystrcpy_s
-00040e30: 005f 7973 7472 6e63 7079 5f73 005f 7973  ._ystrncpy_s._ys
-00040e40: 7472 6475 705f 7300 5f79 7374 726e 6475  trdup_s._ystrndu
-00040e50: 705f 7300 5f79 7374 7263 6174 5f73 005f  p_s._ystrcat_s._
-00040e60: 7973 7472 6e63 6174 5f73 005f 7973 7072  ystrncat_s._yspr
-00040e70: 696e 7466 5f73 005f 7976 7370 7269 6e74  intf_s._yvsprint
-00040e80: 665f 7300 5f79 6d65 6d66 696e 6400 7974  f_s._ymemfind.yt
-00040e90: 6370 2e63 002f 5573 6572 732f 796f 6374  cp.c./Users/yoct
-00040ea0: 6f2f 746d 705f 6275 696c 642f 796f 6374  o/tmp_build/yoct
-00040eb0: 6f70 726f 642f 796f 6374 6f6c 6962 2f76  oprod/yoctolib/v
-00040ec0: 312e 302f 5075 626c 6963 2f63 7070 2f42  1.0/Public/cpp/B
-00040ed0: 696e 6172 6965 732f 7863 6f64 655f 6173  inaries/xcode_as
-00040ee0: 2f79 6170 692f 6275 696c 642f 7961 7069  /yapi/build/yapi
-00040ef0: 2e62 7569 6c64 2f52 656c 6561 7365 2f79  .build/Release/y
-00040f00: 6170 692e 6275 696c 642f 4f62 6a65 6374  api.build/Object
-00040f10: 732d 6e6f 726d 616c 2f78 3836 5f36 342f  s-normal/x86_64/
-00040f20: 7974 6370 2e6f 005f 7944 7570 5365 7400  ytcp.o._yDupSet.
-00040f30: 5f79 4e65 7453 6574 4572 7245 7800 5f79  _yNetSetErrEx._y
-00040f40: 496e 6974 5761 6b65 5570 536f 636b 6574  InitWakeUpSocket
-00040f50: 005f 7953 7461 7274 5761 6b65 5570 536f  ._yStartWakeUpSo
-00040f60: 636b 6574 005f 7944 7269 6e67 5761 6b65  cket._yDringWake
-00040f70: 5570 536f 636b 6574 005f 7943 6f6e 7375  UpSocket._yConsu
-00040f80: 6d65 5761 6b65 5570 536f 636b 6574 005f  meWakeUpSocket._
-00040f90: 7946 7265 6557 616b 6555 7053 6f63 6b65  yFreeWakeUpSocke
-00040fa0: 7400 5f79 5265 736f 6c76 6544 4e53 005f  t._yResolveDNS._
-00040fb0: 7954 6370 496e 6974 005f 7954 6370 5368  yTcpInit._yTcpSh
-00040fc0: 7574 646f 776e 005f 6465 636f 6465 4865  utdown._decodeHe
-00040fd0: 7800 5f79 5463 7044 6f77 6e6c 6f61 6400  x._yTcpDownload.
-00040fe0: 5f79 5463 704f 7065 6e00 5f79 5463 7057  _yTcpOpen._yTcpW
-00040ff0: 7269 7465 005f 7954 6370 5265 6164 005f  rite._yTcpRead._
-00041000: 7952 6571 416c 6c6f 6300 5f79 5265 714f  yReqAlloc._yReqO
-00041010: 7065 6e00 5f79 4854 5450 4f70 656e 5265  pen._yHTTPOpenRe
-00041020: 7145 7800 5f79 5265 7153 656c 6563 7400  qEx._yReqSelect.
-00041030: 5f79 4854 5450 4d75 6c74 6953 656c 6563  _yHTTPMultiSelec
-00041040: 7452 6571 005f 7952 6571 4d75 6c74 6953  tReq._yReqMultiS
-00041050: 656c 6563 7400 5f79 5265 7149 7345 6f66  elect._yReqIsEof
-00041060: 005f 7954 6370 4368 6563 6b52 6571 5469  ._yTcpCheckReqTi
-00041070: 6d65 6f75 7400 5f79 5265 7147 6574 005f  meout._yReqGet._
-00041080: 7952 6571 5265 6164 005f 7952 6571 436c  yReqRead._yReqCl
-00041090: 6f73 6500 5f79 4854 5450 436c 6f73 6552  ose._yHTTPCloseR
-000410a0: 6571 4578 005f 7957 5343 6c6f 7365 5265  eqEx._yWSCloseRe
-000410b0: 7100 5f79 5753 5265 6d6f 7665 5265 7100  q._yWSRemoveReq.
-000410c0: 5f79 5265 7149 7341 7379 6e63 005f 7952  _yReqIsAsync._yR
-000410d0: 6571 4672 6565 005f 7952 6571 4861 7350  eqFree._yReqHasP
-000410e0: 656e 6469 6e67 005f 7773 5f63 6c65 616e  ending._ws_clean
-000410f0: 7570 005f 7773 5f74 6872 6561 6400 5f63  up._ws_thread._c
-00041100: 6c6f 7365 416c 6c52 6571 005f 7953 5344  loseAllReq._ySSD
-00041110: 5044 6973 636f 7665 7200 5f79 5353 4450  PDiscover._ySSDP
-00041120: 5374 6172 7400 5f79 5353 4450 5f74 6872  Start._ySSDP_thr
-00041130: 6561 6400 5f79 5353 4450 5374 6f70 005f  ead._ySSDPStop._
-00041140: 7265 736f 6c76 6544 4e53 4361 6368 6500  resolveDNSCache.
-00041150: 5f42 6173 6536 3445 6e63 6f64 6500 5f77  _Base64Encode._w
-00041160: 735f 6170 7065 6e64 5443 5044 6174 6100  s_appendTCPData.
-00041170: 5f77 735f 7365 6e64 4672 616d 6500 5f79  _ws_sendFrame._y
-00041180: 5353 4450 5f70 6172 7365 5353 5044 4d65  SSDP_parseSSPDMe
-00041190: 7373 6167 6500 5f64 6e73 4361 6368 6500  ssage._dnsCache.
-000411a0: 5f6e 6244 6574 6563 7465 6449 6661 6365  _nbDetectedIface
-000411b0: 7300 5f64 6574 6563 7465 6449 6661 6365  s._detectedIface
-000411c0: 7300 7973 7472 6561 6d2e 6300 2f55 7365  s.ystream.c./Use
-000411d0: 7273 2f79 6f63 746f 2f74 6d70 5f62 7569  rs/yocto/tmp_bui
-000411e0: 6c64 2f79 6f63 746f 7072 6f64 2f79 6f63  ld/yoctoprod/yoc
-000411f0: 746f 6c69 622f 7631 2e30 2f50 7562 6c69  tolib/v1.0/Publi
-00041200: 632f 6370 702f 4269 6e61 7269 6573 2f78  c/cpp/Binaries/x
-00041210: 636f 6465 5f61 732f 7961 7069 2f62 7569  code_as/yapi/bui
-00041220: 6c64 2f79 6170 692e 6275 696c 642f 5265  ld/yapi.build/Re
-00041230: 6c65 6173 652f 7961 7069 2e62 7569 6c64  lease/yapi.build
-00041240: 2f4f 626a 6563 7473 2d6e 6f72 6d61 6c2f  /Objects-normal/
-00041250: 7838 365f 3634 2f79 7374 7265 616d 2e6f  x86_64/ystream.o
-00041260: 005f 7953 6574 4572 7200 5f46 7573 696f  ._ySetErr._Fusio
-00041270: 6e45 7272 6d73 6700 5f59 464f 5045 4e00  nErrmsg._YFOPEN.
-00041280: 5f76 6462 676c 6f67 6600 5f64 6267 6c6f  _vdbglogf._dbglo
-00041290: 6766 005f 7970 5570 6461 7465 5443 5000  gf._ypUpdateTCP.
-000412a0: 5f79 7055 7064 6174 6555 5342 005f 7970  _ypUpdateUSB._yp
-000412b0: 5570 6461 7465 5964 7800 5f79 506b 7451  UpdateYdx._yPktQ
-000412c0: 7565 7565 496e 6974 005f 7950 6b74 5175  ueueInit._yPktQu
-000412d0: 6575 6546 7265 6500 5f79 506b 7451 7565  eueFree._yPktQue
-000412e0: 7565 5365 7445 7272 6f72 005f 7950 6b74  ueSetError._yPkt
-000412f0: 5175 6575 6550 7573 6844 3248 005f 7950  QueuePushD2H._yP
-00041300: 6b74 5175 6575 6550 7573 6845 7800 5f79  ktQueuePushEx._y
-00041310: 506b 7451 7565 7565 5761 6974 416e 6450  PktQueueWaitAndP
-00041320: 6f70 4432 4800 5f79 506b 7451 7565 7565  opD2H._yPktQueue
-00041330: 506f 7000 5f79 506b 7451 7565 7565 5075  Pop._yPktQueuePu
-00041340: 7368 4832 4400 5f79 506b 7451 7565 7565  shH2D._yPktQueue
-00041350: 5065 656b 4832 4400 5f79 506b 7451 7565  PeekH2D._yPktQue
-00041360: 7565 506f 7048 3244 005f 7979 7953 656e  uePopH2D._yyySen
-00041370: 6450 6163 6b65 7400 5f79 5553 4252 656c  dPacket._yUSBRel
-00041380: 6561 7365 416c 6c44 6576 6963 6573 005f  easeAllDevices._
-00041390: 656e 7555 7064 6174 6544 5374 6174 7573  enuUpdateDStatus
-000413a0: 005f 7955 5342 5570 6461 7465 4465 7669  ._yUSBUpdateDevi
-000413b0: 6365 4c69 7374 005f 6669 6e64 4465 7600  ceList._findDev.
-000413c0: 5f66 696e 6444 6576 4864 6c46 726f 6d53  _findDevHdlFromS
-000413d0: 7472 005f 6669 6e64 4465 7646 726f 6d49  tr._findDevFromI
-000413e0: 4f48 646c 005f 6465 7648 646c 496e 666f  OHdl._devHdlInfo
-000413f0: 005f 6475 6d70 5950 6572 6645 6e74 7279  ._dumpYPerfEntry
-00041400: 005f 7955 7362 496e 6974 005f 7955 7362  ._yUsbInit._yUsb
-00041410: 4672 6565 005f 7955 7362 4964 6c65 005f  Free._yUsbIdle._
-00041420: 7944 6973 7061 7463 6852 6563 6569 7665  yDispatchReceive
-00041430: 005f 7953 7472 6561 6d54 7261 6e73 6d69  ._yStreamTransmi
-00041440: 7400 5f79 5374 7265 616d 466c 7573 6800  t._yStreamFlush.
-00041450: 5f64 6576 5265 706f 7274 4572 726f 7200  _devReportError.
-00041460: 5f64 6576 5374 6f70 494f 005f 6465 7650  _devStopIO._devP
-00041470: 6175 7365 494f 005f 7955 7362 5472 6166  auseIO._yUsbTraf
-00041480: 6669 6350 656e 6469 6e67 005f 7955 7362  ficPending._yUsb
-00041490: 4f70 656e 4465 7644 6573 6372 005f 7955  OpenDevDescr._yU
-000414a0: 7362 4f70 656e 005f 7955 7362 5365 7449  sbOpen._yUsbSetI
-000414b0: 4f41 7379 6e63 005f 6465 7643 6865 636b  OAsync._devCheck
-000414c0: 494f 005f 7955 7362 5772 6974 6500 5f79  IO._yUsbWrite._y
-000414d0: 5573 6252 6561 644e 6f6e 426c 6f63 6b00  UsbReadNonBlock.
-000414e0: 5f79 5573 6252 6561 6442 6c6f 636b 005f  _yUsbReadBlock._
-000414f0: 7955 7362 454f 4600 5f79 5573 6243 6c6f  yUsbEOF._yUsbClo
-00041500: 7365 005f 6465 7653 7461 7274 456e 756d  se._devStartEnum
-00041510: 005f 5374 6172 7444 6576 6963 6500 5f79  ._StartDevice._y
-00041520: 5374 7265 616d 5368 7574 646f 776e 005f  StreamShutdown._
-00041530: 7979 5761 6974 4f6e 6c79 436f 6e66 506b  yyWaitOnlyConfPk
-00041540: 7400 5f79 5374 7265 616d 5265 6365 6976  t._yStreamReceiv
-00041550: 6564 005f 7944 6973 7061 7463 684e 6f74  ed._yDispatchNot
-00041560: 6963 6500 5f64 6179 6f66 7300 5f79 436f  ice._dayofs._yCo
-00041570: 6e74 6578 7400 5f79 7472 6163 6566 696c  ntext._ytracefil
-00041580: 6500 7970 726f 672e 6300 2f55 7365 7273  e.yprog.c./Users
-00041590: 2f79 6f63 746f 2f74 6d70 5f62 7569 6c64  /yocto/tmp_build
-000415a0: 2f79 6f63 746f 7072 6f64 2f79 6f63 746f  /yoctoprod/yocto
-000415b0: 6c69 622f 7631 2e30 2f50 7562 6c69 632f  lib/v1.0/Public/
-000415c0: 6370 702f 4269 6e61 7269 6573 2f78 636f  cpp/Binaries/xco
-000415d0: 6465 5f61 732f 7961 7069 2f62 7569 6c64  de_as/yapi/build
-000415e0: 2f79 6170 692e 6275 696c 642f 5265 6c65  /yapi.build/Rele
-000415f0: 6173 652f 7961 7069 2e62 7569 6c64 2f4f  ase/yapi.build/O
-00041600: 626a 6563 7473 2d6e 6f72 6d61 6c2f 7838  bjects-normal/x8
-00041610: 365f 3634 2f79 7072 6f67 2e6f 005f 7950  6_64/yprog.o._yP
-00041620: 726f 6749 6e69 7400 5f79 5072 6f67 4672  rogInit._yProgFr
-00041630: 6565 005f 7072 6f67 5f47 6574 4350 554e  ee._prog_GetCPUN
-00041640: 616d 6500 5f49 7356 616c 6964 4279 6e48  ame._IsValidBynH
-00041650: 6561 6400 5f56 616c 6964 6174 6542 796e  ead._ValidateByn
-00041660: 436f 6d70 6174 005f 4973 5661 6c69 6442  Compat._IsValidB
-00041670: 796e 4669 6c65 005f 7970 4973 5365 6e64  ynFile._ypIsSend
-00041680: 426f 6f74 6c6f 6164 6572 4275 7379 005f  BootloaderBusy._
-00041690: 7970 5365 6e64 426f 6f74 6c6f 6164 6572  ypSendBootloader
-000416a0: 436d 6400 5f79 7047 6574 426f 6f74 6c6f  Cmd._ypGetBootlo
-000416b0: 6164 6572 5265 706c 7900 5f42 6c6f 636b  aderReply._Block
-000416c0: 696e 6752 6561 6400 5f53 656e 6444 6174  ingRead._SendDat
-000416d0: 6150 6163 6b65 7400 5f79 5553 4247 6574  aPacket._yUSBGet
-000416e0: 426f 6f6c 6f61 6465 7200 5f75 466c 6173  Booloader._uFlas
-000416f0: 6844 6576 6963 6500 5f79 5072 6f67 4c6f  hDevice._yProgLo
-00041700: 6750 726f 6772 6573 7300 5f75 4765 7444  gProgress._uGetD
-00041710: 6576 6963 6549 6e66 6f00 5f79 4765 7446  eviceInfo._yGetF
-00041720: 6972 6d77 6172 6500 5f79 4e65 7448 7562  irmware._yNetHub
-00041730: 4765 7442 6f6f 746c 6f61 6465 7273 005f  GetBootloaders._
-00041740: 7961 7069 4368 6563 6b46 6972 6d77 6172  yapiCheckFirmwar
-00041750: 655f 696e 7465 726e 616c 005f 6973 5765  e_internal._isWe
-00041760: 6250 6174 6800 5f79 6170 6943 6865 636b  bPath._yapiCheck
-00041770: 4669 726d 7761 7265 5f72 005f 7961 7069  Firmware_r._yapi
-00041780: 5570 6461 7465 4669 726d 7761 7265 5f69  UpdateFirmware_i
-00041790: 6e74 6572 6e61 6c00 5f79 5374 6172 7446  nternal._yStartF
-000417a0: 6972 6d77 6172 6555 7064 6174 6500 5f79  irmwareUpdate._y
-000417b0: 6170 6943 6865 636b 4669 726d 7761 7265  apiCheckFirmware
-000417c0: 4669 6c65 005f 794c 6f61 6446 6972 6d77  File._yLoadFirmw
-000417d0: 6172 6546 696c 6500 5f79 4669 726d 7761  areFile._yFirmwa
-000417e0: 7265 5570 6461 7465 5f74 6872 6561 6400  reUpdate_thread.
-000417f0: 5f6f 7350 726f 674c 6f67 5072 6f67 7265  _osProgLogProgre
-00041800: 7373 4578 005f 7365 6e64 4875 6246 6c61  ssEx._sendHubFla
-00041810: 7368 436d 6400 5f75 706c 6f61 6400 5f63  shCmd._upload._c
-00041820: 6865 636b 4854 5450 4865 6164 6572 005f  heckHTTPHeader._
-00041830: 6663 7478 005f 6669 726d 5f64 6576 005f  fctx._firm_dev._
-00041840: 6669 726d 5f70 6b74 0079 6a73 6f6e 2e63  firm_pkt.yjson.c
-00041850: 002f 5573 6572 732f 796f 6374 6f2f 746d  ./Users/yocto/tm
-00041860: 705f 6275 696c 642f 796f 6374 6f70 726f  p_build/yoctopro
-00041870: 642f 796f 6374 6f6c 6962 2f76 312e 302f  d/yoctolib/v1.0/
-00041880: 5075 626c 6963 2f63 7070 2f42 696e 6172  Public/cpp/Binar
-00041890: 6965 732f 7863 6f64 655f 6173 2f79 6170  ies/xcode_as/yap
-000418a0: 692f 6275 696c 642f 7961 7069 2e62 7569  i/build/yapi.bui
-000418b0: 6c64 2f52 656c 6561 7365 2f79 6170 692e  ld/Release/yapi.
-000418c0: 6275 696c 642f 4f62 6a65 6374 732d 6e6f  build/Objects-no
-000418d0: 726d 616c 2f78 3836 5f36 342f 796a 736f  rmal/x86_64/yjso
-000418e0: 6e2e 6f00 5f79 4a73 6f6e 5061 7273 6500  n.o._yJsonParse.
-000418f0: 5f79 4a73 6f6e 536b 6970 0079 6b65 792e  _yJsonSkip.ykey.
-00041900: 6300 2f55 7365 7273 2f79 6f63 746f 2f74  c./Users/yocto/t
-00041910: 6d70 5f62 7569 6c64 2f79 6f63 746f 7072  mp_build/yoctopr
-00041920: 6f64 2f79 6f63 746f 6c69 622f 7631 2e30  od/yoctolib/v1.0
-00041930: 2f50 7562 6c69 632f 6370 702f 4269 6e61  /Public/cpp/Bina
-00041940: 7269 6573 2f78 636f 6465 5f61 732f 7961  ries/xcode_as/ya
-00041950: 7069 2f62 7569 6c64 2f79 6170 692e 6275  pi/build/yapi.bu
-00041960: 696c 642f 5265 6c65 6173 652f 7961 7069  ild/Release/yapi
-00041970: 2e62 7569 6c64 2f4f 626a 6563 7473 2d6e  .build/Objects-n
-00041980: 6f72 6d61 6c2f 7838 365f 3634 2f79 6b65  ormal/x86_64/yke
-00041990: 792e 6f00 5f62 696e 3273 7472 005f 436f  y.o._bin2str._Co
-000419a0: 6d70 7574 6541 7574 6848 4131 005f 4d44  mputeAuthHA1._MD
-000419b0: 3549 6e69 7469 616c 697a 6500 5f4d 4435  5Initialize._MD5
-000419c0: 4164 6444 6174 6100 5f4d 4435 4361 6c63  AddData._MD5Calc
-000419d0: 756c 6174 6500 5f43 6f6d 7075 7465 4175  ulate._ComputeAu
-000419e0: 7468 4841 3200 5f43 6f6d 7075 7465 4175  thHA2._ComputeAu
-000419f0: 7468 5265 7370 6f6e 7365 005f 4368 6563  thResponse._Chec
-00041a00: 6b57 5341 7574 6800 5f79 5348 4131 005f  kWSAuth._ySHA1._
-00041a10: 7950 6172 7365 5757 5741 7574 6865 6e74  yParseWWWAuthent
-00041a20: 6963 6174 6500 5f79 4469 6765 7374 4175  icate._yDigestAu
-00041a30: 7468 6f72 697a 6174 696f 6e00 5f69 6e69  thorization._ini
-00041a40: 7473 6861 7700 5f69 7465 7273 6861 7700  tshaw._itershaw.
-00041a50: 5f79 496e 6974 5073 6b00 5f79 4974 6572  _yInitPsk._yIter
-00041a60: 5073 6b00 5f4d 4435 5472 616e 7366 6f72  Psk._MD5Transfor
-00041a70: 6d00 5f73 6861 315f 696e 6974 005f 7770  m._sha1_init._wp
-00041a80: 616b 0079 6861 7368 2e63 002f 5573 6572  ak.yhash.c./User
-00041a90: 732f 796f 6374 6f2f 746d 705f 6275 696c  s/yocto/tmp_buil
-00041aa0: 642f 796f 6374 6f70 726f 642f 796f 6374  d/yoctoprod/yoct
-00041ab0: 6f6c 6962 2f76 312e 302f 5075 626c 6963  olib/v1.0/Public
-00041ac0: 2f63 7070 2f42 696e 6172 6965 732f 7863  /cpp/Binaries/xc
-00041ad0: 6f64 655f 6173 2f79 6170 692f 6275 696c  ode_as/yapi/buil
-00041ae0: 642f 7961 7069 2e62 7569 6c64 2f52 656c  d/yapi.build/Rel
-00041af0: 6561 7365 2f79 6170 692e 6275 696c 642f  ease/yapi.build/
-00041b00: 4f62 6a65 6374 732d 6e6f 726d 616c 2f78  Objects-normal/x
-00041b10: 3836 5f36 342f 7968 6173 682e 6f00 5f79  86_64/yhash.o._y
-00041b20: 426c 6b4c 6973 744c 656e 6774 6800 5f79  BlkListLength._y
-00041b30: 426c 6b4c 6973 7453 6565 6b00 5f79 4861  BlkListSeek._yHa
-00041b40: 7368 496e 6974 005f 7948 6173 6850 7574  shInit._yHashPut
-00041b50: 5374 7200 5f79 426c 6b41 6c6c 6f63 005f  Str._yBlkAlloc._
-00041b60: 7948 6173 6846 7265 6500 5f79 4861 7368  yHashFree._yHash
-00041b70: 5075 7442 7566 005f 7948 6173 6850 7574  PutBuf._yHashPut
-00041b80: 005f 7948 6173 6854 6573 7442 7566 005f  ._yHashTestBuf._
-00041b90: 7948 6173 6854 6573 7453 7472 005f 7948  yHashTestStr._yH
-00041ba0: 6173 6847 6574 4275 6600 5f79 4861 7368  ashGetBuf._yHash
-00041bb0: 4765 7453 7472 005f 7948 6173 6847 6574  GetStr._yHashGet
-00041bc0: 5374 724c 656e 005f 7948 6173 6847 6574  StrLen._yHashGet
-00041bd0: 5374 7250 7472 005f 7770 5072 6576 656e  StrPtr._wpPreven
-00041be0: 7455 6e72 6567 6973 7465 7245 7800 5f77  tUnregisterEx._w
-00041bf0: 7041 6c6c 6f77 556e 7265 6769 7374 6572  pAllowUnregister
-00041c00: 4578 005f 7770 5265 6769 7374 6572 005f  Ex._wpRegister._
-00041c10: 7770 4765 7441 7474 7269 6275 7465 005f  wpGetAttribute._
-00041c20: 7770 4765 7453 6572 6961 6c00 5f77 7047  wpGetSerial._wpG
-00041c30: 6574 4c6f 6769 6361 6c4e 616d 6500 5f77  etLogicalName._w
-00041c40: 704d 6172 6b46 6f72 556e 7265 6769 7374  pMarkForUnregist
-00041c50: 6572 005f 7770 456e 7472 7943 6f75 6e74  er._wpEntryCount
-00041c60: 005f 7770 4765 7444 6576 5964 7800 5f77  ._wpGetDevYdx._w
-00041c70: 7053 6561 7263 6845 7800 5f77 7053 6561  pSearchEx._wpSea
-00041c80: 7263 6800 5f77 7053 6561 7263 6842 794e  rch._wpSearchByN
-00041c90: 616d 6548 6173 6800 5f77 7047 6574 4465  ameHash._wpGetDe
-00041ca0: 7669 6365 496e 666f 005f 7970 5265 6769  viceInfo._ypRegi
-00041cb0: 7374 6572 005f 7970 5265 6769 7374 6572  ster._ypRegister
-00041cc0: 4279 5964 7800 5f79 7047 6574 4174 7472  ByYdx._ypGetAttr
-00041cd0: 6962 7574 6573 4279 5964 7800 5f79 7047  ibutesByYdx._ypG
-00041ce0: 6574 4361 7465 676f 7279 005f 7970 4765  etCategory._ypGe
-00041cf0: 7441 7474 7269 6275 7465 7300 5f79 7047  tAttributes._ypG
-00041d00: 6574 5479 7065 005f 7970 5365 6172 6368  etType._ypSearch
-00041d10: 005f 7970 4765 7446 756e 6374 696f 6e73  ._ypGetFunctions
-00041d20: 005f 7970 4765 7446 756e 6374 696f 6e49  ._ypGetFunctionI
-00041d30: 6e66 6f00 5f79 7047 6574 4675 6e63 7469  nfo._ypGetFuncti
-00041d40: 6f6e 7345 7800 5f79 7046 696e 6442 6f6f  onsEx._ypFindBoo
-00041d50: 746c 6f61 6465 7273 005f 6465 636f 6465  tloaders._decode
-00041d60: 4e65 7446 756e 6356 616c 5632 005f 7942  NetFuncValV2._yB
-00041d70: 6c6b 4672 6565 005f 5365 7269 616c 5265  lkFree._SerialRe
-00041d80: 6600 5f6e 6578 7443 6174 5964 7800 5f6e  f._nextCatYdx._n
-00041d90: 6578 7448 6173 6845 6e74 7279 005f 5365  extHashEntry._Se
-00041da0: 7269 616c 4e75 6d62 6572 5374 7200 5f79  rialNumberStr._y
-00041db0: 5770 4c69 7374 4865 6164 005f 7959 704c  WpListHead._yYpL
-00041dc0: 6973 7448 6561 6400 5f66 7265 6542 6c6b  istHead._freeBlk
-00041dd0: 7300 5f79 4861 7368 4d75 7465 7800 5f79  s._yHashMutex._y
-00041de0: 4672 6565 4d75 7465 7800 5f79 5770 4d75  FreeMutex._yWpMu
-00041df0: 7465 7800 5f79 5970 4d75 7465 7800 5f79  tex._yYpMutex._y
-00041e00: 4861 7368 5461 626c 6500 5f64 6576 5964  HashTable._devYd
-00041e10: 7850 7472 005f 6675 6e59 6478 5074 7200  xPtr._funYdxPtr.
-00041e20: 5f6e 6578 7444 6576 5964 7800 5f75 7365  _nextDevYdx._use
-00041e30: 6444 6576 5964 7800 5f77 704c 6f63 6b43  dDevYdx._wpLockC
-00041e40: 6f75 6e74 005f 7770 536f 6d65 7468 696e  ount._wpSomethin
-00041e50: 6755 6e72 6567 6973 7465 7265 6400 7970  gUnregistered.yp
-00041e60: 6b74 5f6f 7378 2e63 002f 5573 6572 732f  kt_osx.c./Users/
-00041e70: 796f 6374 6f2f 746d 705f 6275 696c 642f  yocto/tmp_build/
-00041e80: 796f 6374 6f70 726f 642f 796f 6374 6f6c  yoctoprod/yoctol
-00041e90: 6962 2f76 312e 302f 5075 626c 6963 2f63  ib/v1.0/Public/c
-00041ea0: 7070 2f42 696e 6172 6965 732f 7863 6f64  pp/Binaries/xcod
-00041eb0: 655f 6173 2f79 6170 692f 6275 696c 642f  e_as/yapi/build/
-00041ec0: 7961 7069 2e62 7569 6c64 2f52 656c 6561  yapi.build/Relea
-00041ed0: 7365 2f79 6170 692e 6275 696c 642f 4f62  se/yapi.build/Ob
-00041ee0: 6a65 6374 732d 6e6f 726d 616c 2f78 3836  jects-normal/x86
-00041ef0: 5f36 342f 7970 6b74 5f6f 7378 2e6f 005f  _64/ypkt_osx.o._
-00041f00: 7979 7955 5342 5f69 6e69 7400 5f65 7665  yyyUSB_init._eve
-00041f10: 6e74 5f74 6872 6561 6400 5f73 6574 7570  nt_thread._setup
-00041f20: 4849 444d 616e 6167 6572 005f 7979 7955  HIDManager._yyyU
-00041f30: 5342 5f73 746f 7000 5f73 746f 7048 4944  SB_stop._stopHID
-00041f40: 4d61 6e61 6765 7200 5f79 7979 5553 4247  Manager._yyyUSBG
-00041f50: 6574 496e 7465 7266 6163 6573 005f 6765  etInterfaces._ge
-00041f60: 7444 6576 5265 6600 5f67 6574 5f69 6e74  tDevRef._get_int
-00041f70: 5f70 726f 7065 7274 7900 5f67 6574 5f74  _property._get_t
-00041f80: 7874 5f70 726f 7065 7274 7900 5f79 7979  xt_property._yyy
-00041f90: 4f53 6864 6c43 6f6d 7061 7265 005f 7979  OShdlCompare._yy
-00041fa0: 7953 6574 7570 005f 4861 6e64 6c65 5f49  ySetup._Handle_I
-00041fb0: 4f48 4944 4465 7669 6365 494f 4849 4452  OHIDDeviceIOHIDR
-00041fc0: 6570 6f72 7443 616c 6c62 6163 6b00 5f79  eportCallback._y
-00041fd0: 7979 5369 676e 616c 4f75 7450 6b74 005f  yySignalOutPkt._
-00041fe0: 7979 7950 6163 6b65 7453 6875 7464 6f77  yyyPacketShutdow
-00041ff0: 6e00 7961 7069 2e63 002f 5573 6572 732f  n.yapi.c./Users/
-00042000: 796f 6374 6f2f 746d 705f 6275 696c 642f  yocto/tmp_build/
-00042010: 796f 6374 6f70 726f 642f 796f 6374 6f6c  yoctoprod/yoctol
-00042020: 6962 2f76 312e 302f 5075 626c 6963 2f63  ib/v1.0/Public/c
-00042030: 7070 2f42 696e 6172 6965 732f 7863 6f64  pp/Binaries/xcod
-00042040: 655f 6173 2f79 6170 692f 6275 696c 642f  e_as/yapi/build/
-00042050: 7961 7069 2e62 7569 6c64 2f52 656c 6561  yapi.build/Relea
-00042060: 7365 2f79 6170 692e 6275 696c 642f 4f62  se/yapi.build/Ob
-00042070: 6a65 6374 732d 6e6f 726d 616c 2f78 3836  jects-normal/x86
-00042080: 5f36 342f 7961 7069 2e6f 005f 7961 7069  _64/yapi.o._yapi
-00042090: 4164 6455 6465 7652 756c 6573 466f 7259  AddUdevRulesForY
-000420a0: 6f63 746f 005f 7946 756e 6374 696f 6e55  octo._yFunctionU
-000420b0: 7064 6174 6500 5f79 4675 6e63 7469 6f6e  pdate._yFunction
-000420c0: 5469 6d65 6455 7064 6174 6500 5f69 6e69  TimedUpdate._ini
-000420d0: 7444 6576 5964 7849 6e66 6f73 005f 6672  tDevYdxInfos._fr
-000420e0: 6565 4465 7659 6478 496e 666f 7300 5f79  eeDevYdxInfos._y
-000420f0: 6170 6950 756c 6c44 6576 6963 654c 6f67  apiPullDeviceLog
-00042100: 4578 005f 7961 7069 4765 7444 6576 6963  Ex._yapiGetDevic
-00042110: 6550 6174 6800 5f79 7770 4765 7444 6576  ePath._ywpGetDev
-00042120: 6963 6548 7562 005f 7961 7069 5265 7175  iceHub._yapiRequ
-00042130: 6573 744f 7065 6e55 5342 005f 6c6f 6752  estOpenUSB._logR
-00042140: 6573 756c 7400 5f79 6170 6952 6571 7565  esult._yapiReque
-00042150: 7374 4f70 656e 5753 005f 7961 7069 5265  stOpenWS._yapiRe
-00042160: 7175 6573 744f 7065 6e48 5454 5000 5f79  questOpenHTTP._y
-00042170: 6170 6950 756c 6c44 6576 6963 654c 6f67  apiPullDeviceLog
-00042180: 005f 6368 6563 6b46 6f72 5361 6d65 4875  ._checkForSameHu
-00042190: 6241 6363 6573 7300 5f79 7770 5361 6665  bAccess._ywpSafe
-000421a0: 556e 7265 6769 7374 6572 005f 7977 7053  Unregister._ywpS
-000421b0: 6166 6552 6567 6973 7465 7200 5f79 7770  afeRegister._ywp
-000421c0: 5361 6665 5570 6461 7465 005f 7977 7047  SafeUpdate._ywpG
-000421d0: 6574 4465 7669 6365 5572 6c00 5f68 616e  etDeviceUrl._han
-000421e0: 646c 654e 6574 4e6f 7469 6669 6361 7469  dleNetNotificati
-000421f0: 6f6e 005f 756e 7265 6769 7374 6572 4e65  on._unregisterNe
-00042200: 7444 6576 6963 6500 5f72 6571 7565 7374  tDevice._request
-00042210: 5f70 656e 6469 6e67 5f6c 6f67 7300 5f79  _pending_logs._y
-00042220: 6170 6947 6574 444c 4c50 6174 6800 5f57  apiGetDLLPath._W
-00042230: 616b 6555 7041 6c6c 536c 6565 7000 5f79  akeUpAllSleep._y
-00042240: 6170 6947 6574 5469 636b 436f 756e 7400  apiGetTickCount.
-00042250: 5f79 6170 6947 6574 434e 6f6e 6365 005f  _yapiGetCNonce._
-00042260: 7961 7069 5265 7175 6573 744f 7065 6e00  yapiRequestOpen.
-00042270: 5f79 6170 6948 5454 5052 6571 7565 7374  _yapiHTTPRequest
-00042280: 5379 6e63 5374 6172 7445 785f 696e 7465  SyncStartEx_inte
-00042290: 726e 616c 005f 756e 7061 636b 4854 5450  rnal._unpackHTTP
-000422a0: 5265 7175 6573 7400 5f79 6170 6952 6571  Request._yapiReq
-000422b0: 7565 7374 436c 6f73 6500 5f79 6170 6948  uestClose._yapiH
-000422c0: 5454 5052 6571 7565 7374 5379 6e63 446f  TTPRequestSyncDo
-000422d0: 6e65 5f69 6e74 6572 6e61 6c00 5f79 6170  ne_internal._yap
-000422e0: 6947 6574 426f 6f74 6c6f 6164 6572 7344  iGetBootloadersD
-000422f0: 6576 7300 5f79 6170 694a 736f 6e47 6574  evs._yapiJsonGet
-00042300: 5061 7468 5f69 6e74 6572 6e61 6c00 5f79  Path_internal._y
-00042310: 6170 694a 736f 6e56 616c 7565 5061 7273  apiJsonValuePars
-00042320: 6553 7472 7563 7400 5f79 6170 6952 6567  eStruct._yapiReg
-00042330: 6973 7465 7252 6177 4e6f 7469 6669 6361  isterRawNotifica
-00042340: 7469 6f6e 4362 005f 7961 7069 5265 6769  tionCb._yapiRegi
-00042350: 7374 6572 5261 7752 6570 6f72 7443 6200  sterRawReportCb.
-00042360: 5f79 6170 6952 6567 6973 7465 7252 6177  _yapiRegisterRaw
-00042370: 5265 706f 7274 5632 4362 005f 7961 7069  ReportV2Cb._yapi
-00042380: 496e 6974 4150 4900 5f79 6170 6949 6e69  InitAPI._yapiIni
-00042390: 7441 5049 5f69 6e74 6572 6e61 6c00 5f79  tAPI_internal._y
-000423a0: 6170 6946 7265 6541 5049 005f 7961 7069  apiFreeAPI._yapi
-000423b0: 4672 6565 4150 495f 696e 7465 726e 616c  FreeAPI_internal
-000423c0: 005f 7961 7069 5365 744e 6574 776f 726b  ._yapiSetNetwork
-000423d0: 5469 6d65 6f75 7400 5f79 6170 6947 6574  Timeout._yapiGet
-000423e0: 4e65 7477 6f72 6b54 696d 656f 7574 005f  NetworkTimeout._
-000423f0: 7961 7069 5365 744e 6574 4465 764c 6973  yapiSetNetDevLis
-00042400: 7456 616c 6964 6974 7900 5f79 6170 6947  tValidity._yapiG
-00042410: 6574 4e65 7444 6576 4c69 7374 5661 6c69  etNetDevListVali
-00042420: 6469 7479 005f 7961 7069 5265 6769 7374  dity._yapiRegist
-00042430: 6572 4c6f 6746 756e 6374 696f 6e00 5f79  erLogFunction._y
-00042440: 6170 6952 6567 6973 7465 7244 6576 6963  apiRegisterDevic
-00042450: 654c 6f67 4361 6c6c 6261 636b 005f 7961  eLogCallback._ya
-00042460: 7069 5374 6172 7453 746f 7044 6576 6963  piStartStopDevic
-00042470: 654c 6f67 4361 6c6c 6261 636b 005f 7961  eLogCallback._ya
-00042480: 7069 5265 6769 7374 6572 4465 7669 6365  piRegisterDevice
-00042490: 4172 7269 7661 6c43 616c 6c62 6163 6b00  ArrivalCallback.
-000424a0: 5f79 6170 6952 6567 6973 7465 7244 6576  _yapiRegisterDev
-000424b0: 6963 6552 656d 6f76 616c 4361 6c6c 6261  iceRemovalCallba
-000424c0: 636b 005f 7961 7069 5265 6769 7374 6572  ck._yapiRegister
-000424d0: 4465 7669 6365 4368 616e 6765 4361 6c6c  DeviceChangeCall
-000424e0: 6261 636b 005f 7961 7069 5265 6769 7374  back._yapiRegist
-000424f0: 6572 4265 6163 6f6e 4361 6c6c 6261 636b  erBeaconCallback
-00042500: 005f 7961 7069 5265 6769 7374 6572 4465  ._yapiRegisterDe
-00042510: 7669 6365 436f 6e66 6967 4368 616e 6765  viceConfigChange
-00042520: 4361 6c6c 6261 636b 005f 7961 7069 5265  Callback._yapiRe
-00042530: 6769 7374 6572 4675 6e63 7469 6f6e 5570  gisterFunctionUp
-00042540: 6461 7465 4361 6c6c 6261 636b 005f 7961  dateCallback._ya
-00042550: 7069 5265 6769 7374 6572 5469 6d65 6452  piRegisterTimedR
-00042560: 6570 6f72 7443 616c 6c62 6163 6b00 5f79  eportCallback._y
-00042570: 6170 694c 6f63 6b46 756e 6374 696f 6e43  apiLockFunctionC
-00042580: 616c 6c42 6163 6b00 5f79 6170 6955 6e6c  allBack._yapiUnl
-00042590: 6f63 6b46 756e 6374 696f 6e43 616c 6c42  ockFunctionCallB
-000425a0: 6163 6b00 5f79 6170 694c 6f63 6b44 6576  ack._yapiLockDev
-000425b0: 6963 6543 616c 6c42 6163 6b00 5f79 6170  iceCallBack._yap
-000425c0: 6955 6e6c 6f63 6b44 6576 6963 6543 616c  iUnlockDeviceCal
-000425d0: 6c42 6163 6b00 5f79 6170 6954 6573 7448  lBack._yapiTestH
-000425e0: 7562 005f 7961 7069 5265 6769 7374 6572  ub._yapiRegister
-000425f0: 4875 6200 5f79 6170 6950 7265 7265 6769  Hub._yapiPreregi
-00042600: 7374 6572 4875 6200 5f79 6170 6955 6e72  sterHub._yapiUnr
-00042610: 6567 6973 7465 7248 7562 005f 7961 7069  egisterHub._yapi
-00042620: 556e 7265 6769 7374 6572 4875 625f 696e  UnregisterHub_in
-00042630: 7465 726e 616c 005f 7961 7069 5570 6461  ternal._yapiUpda
-00042640: 7465 4465 7669 6365 4c69 7374 005f 7961  teDeviceList._ya
-00042650: 7069 5570 6461 7465 4465 7669 6365 4c69  piUpdateDeviceLi
-00042660: 7374 5f69 6e74 6572 6e61 6c00 5f79 6170  st_internal._yap
-00042670: 6948 616e 646c 6545 7665 6e74 7300 5f79  iHandleEvents._y
-00042680: 6170 6948 616e 646c 6545 7665 6e74 735f  apiHandleEvents_
-00042690: 696e 7465 726e 616c 005f 7961 7069 536c  internal._yapiSl
-000426a0: 6565 7000 5f79 6170 6943 6865 636b 4c6f  eep._yapiCheckLo
-000426b0: 6769 6361 6c4e 616d 6500 5f79 6170 6947  gicalName._yapiG
-000426c0: 6574 4150 4956 6572 7369 6f6e 005f 7961  etAPIVersion._ya
-000426d0: 7069 5365 7454 7261 6365 4669 6c65 005f  piSetTraceFile._
-000426e0: 7961 7069 4765 7444 6576 6963 6500 5f79  yapiGetDevice._y
-000426f0: 6170 6947 6574 416c 6c44 6576 6963 6573  apiGetAllDevices
-00042700: 005f 7961 7069 4765 7444 6576 6963 6549  ._yapiGetDeviceI
-00042710: 6e66 6f00 5f79 6170 6947 6574 4465 7669  nfo._yapiGetDevi
-00042720: 6365 5061 7468 4578 005f 7961 7069 4765  cePathEx._yapiGe
-00042730: 7446 756e 6374 696f 6e00 5f79 6170 6947  tFunction._yapiG
-00042740: 6574 4675 6e63 7469 6f6e 7342 7943 6c61  etFunctionsByCla
-00042750: 7373 005f 7961 7069 4765 7446 756e 6374  ss._yapiGetFunct
-00042760: 696f 6e73 4279 4465 7669 6365 005f 7961  ionsByDevice._ya
-00042770: 7069 4765 7446 756e 6374 696f 6e49 6e66  piGetFunctionInf
-00042780: 6f00 5f79 6170 6947 6574 4675 6e63 7469  o._yapiGetFuncti
-00042790: 6f6e 496e 666f 4578 5f69 6e74 6572 6e61  onInfoEx_interna
-000427a0: 6c00 5f79 6170 6947 6574 4675 6e63 7469  l._yapiGetFuncti
-000427b0: 6f6e 496e 666f 4578 005f 7961 7069 4854  onInfoEx._yapiHT
-000427c0: 5450 5265 7175 6573 7453 796e 6353 7461  TPRequestSyncSta
-000427d0: 7274 4578 005f 7961 7069 4854 5450 5265  rtEx._yapiHTTPRe
-000427e0: 7175 6573 7453 796e 6353 7461 7274 005f  questSyncStart._
-000427f0: 7961 7069 4854 5450 5265 7175 6573 7453  yapiHTTPRequestS
-00042800: 796e 6353 7461 7274 4f75 744f 6642 616e  yncStartOutOfBan
-00042810: 6400 5f79 6170 6948 5454 5052 6571 7565  d._yapiHTTPReque
-00042820: 7374 5379 6e63 446f 6e65 005f 7961 7069  stSyncDone._yapi
-00042830: 4854 5450 5265 7175 6573 7441 7379 6e63  HTTPRequestAsync
-00042840: 4578 005f 7961 7069 4854 5450 5265 7175  Ex._yapiHTTPRequ
-00042850: 6573 7441 7379 6e63 4578 5f69 6e74 6572  estAsyncEx_inter
-00042860: 6e61 6c00 5f79 6170 6948 5454 5052 6571  nal._yapiHTTPReq
-00042870: 7565 7374 4173 796e 6300 5f79 6170 6948  uestAsync._yapiH
-00042880: 5454 5052 6571 7565 7374 4173 796e 634f  TTPRequestAsyncO
-00042890: 7574 4f66 4261 6e64 005f 7961 7069 4854  utOfBand._yapiHT
-000428a0: 5450 5265 7175 6573 7400 5f79 6170 6952  TPRequest._yapiR
-000428b0: 6567 6973 7465 7248 7562 4469 7363 6f76  egisterHubDiscov
-000428c0: 6572 7943 616c 6c62 6163 6b00 5f79 6170  eryCallback._yap
-000428d0: 6952 6567 6973 7465 7257 616b 6555 7043  iRegisterWakeUpC
-000428e0: 6200 5f79 6170 6954 7269 6767 6572 4875  b._yapiTriggerHu
-000428f0: 6244 6973 636f 7665 7279 005f 7961 7069  bDiscovery._yapi
-00042900: 4765 7442 6f6f 746c 6f61 6465 7273 005f  GetBootloaders._
-00042910: 7961 7069 4973 4d6f 6475 6c65 5772 6974  yapiIsModuleWrit
-00042920: 6162 6c65 005f 7961 7069 4a73 6f6e 4465  able._yapiJsonDe
-00042930: 636f 6465 5374 7269 6e67 005f 7961 7069  codeString._yapi
-00042940: 4a73 6f6e 4765 7450 6174 6800 5f79 6170  JsonGetPath._yap
-00042950: 6947 6574 416c 6c4a 736f 6e4b 6579 7300  iGetAllJsonKeys.
-00042960: 5f79 6170 6947 6574 4d65 6d00 5f79 6170  _yapiGetMem._yap
-00042970: 6946 7265 654d 656d 005f 7961 7069 4368  iFreeMem._yapiCh
-00042980: 6563 6b46 6972 6d77 6172 6500 5f79 6170  eckFirmware._yap
-00042990: 6955 7064 6174 6546 6972 6d77 6172 6500  iUpdateFirmware.
-000429a0: 5f79 6170 6955 7064 6174 6546 6972 6d77  _yapiUpdateFirmw
-000429b0: 6172 6545 7800 5f79 6170 6947 6574 5375  areEx._yapiGetSu
-000429c0: 6264 6576 6963 6573 005f 6465 6c65 7465  bdevices._delete
-000429d0: 416c 6c43 5300 5f73 7364 7045 6e74 7279  AllCS._ssdpEntry
-000429e0: 5570 6461 7465 005f 756e 7265 6769 7374  Update._unregist
-000429f0: 6572 4e65 7448 7562 005f 6973 5361 6d65  erNetHub._isSame
-00042a00: 4875 6200 5f79 6170 6946 7265 6548 7562  Hub._yapiFreeHub
-00042a10: 005f 7946 7265 6550 6172 7365 6455 524c  ._yFreeParsedURL
-00042a20: 005f 7961 7069 416c 6c6f 6348 7562 005f  ._yapiAllocHub._
-00042a30: 7069 6e67 5552 4c4f 6e68 7562 005f 7950  pingURLOnhub._yP
-00042a40: 6172 7365 4875 6255 524c 005f 7961 7069  arseHubURL._yapi
-00042a50: 5265 6769 7374 6572 4875 6245 7800 5f79  RegisterHubEx._y
-00042a60: 6865 6c70 6572 5f74 6872 6561 6400 5f79  helper_thread._y
-00042a70: 4e65 7448 7562 456e 756d 005f 794e 6574  NetHubEnum._yNet
-00042a80: 4875 6245 6e75 6d45 7800 5f64 6973 6162  HubEnumEx._disab
-00042a90: 6c65 5f6a 7a6f 6e00 5f70 6172 7365 4e65  le_jzon._parseNe
-00042aa0: 7457 7045 6e74 7279 005f 7970 5570 6461  tWpEntry._ypUpda
-00042ab0: 7465 4e65 7400 5f61 7379 6e63 4472 6f70  teNet._asyncDrop
-00042ac0: 005f 5963 7478 4465 7669 6365 4c69 7374  ._YctxDeviceList
-00042ad0: 5661 6c69 6469 7479 4d73 005f 5963 7478  ValidityMs._Yctx
-00042ae0: 4e65 7477 6f72 6b54 696d 656f 7574 0079  NetworkTimeout.y
-00042af0: 6669 666f 2e63 002f 5573 6572 732f 796f  fifo.c./Users/yo
-00042b00: 6374 6f2f 746d 705f 6275 696c 642f 796f  cto/tmp_build/yo
-00042b10: 6374 6f70 726f 642f 796f 6374 6f6c 6962  ctoprod/yoctolib
-00042b20: 2f76 312e 302f 5075 626c 6963 2f63 7070  /v1.0/Public/cpp
-00042b30: 2f42 696e 6172 6965 732f 7863 6f64 655f  /Binaries/xcode_
-00042b40: 6173 2f79 6170 692f 6275 696c 642f 7961  as/yapi/build/ya
-00042b50: 7069 2e62 7569 6c64 2f52 656c 6561 7365  pi.build/Release
-00042b60: 2f79 6170 692e 6275 696c 642f 4f62 6a65  /yapi.build/Obje
-00042b70: 6374 732d 6e6f 726d 616c 2f78 3836 5f36  cts-normal/x86_6
-00042b80: 342f 7966 6966 6f2e 6f00 5f79 4669 666f  4/yfifo.o._yFifo
-00042b90: 496e 6974 4578 005f 7946 6966 6f43 6c65  InitEx._yFifoCle
-00042ba0: 616e 7570 005f 7946 6966 6f45 6e74 6572  anup._yFifoEnter
-00042bb0: 4353 005f 7946 6966 6f4c 6561 7665 4353  CS._yFifoLeaveCS
-00042bc0: 005f 7946 6966 6f45 6d70 7479 4578 005f  ._yFifoEmptyEx._
-00042bd0: 7946 6966 6f45 6d70 7479 005f 7950 7573  yFifoEmpty._yPus
-00042be0: 6846 6966 6f45 7800 5f79 5075 7368 4669  hFifoEx._yPushFi
-00042bf0: 666f 005f 7950 6f70 4669 666f 4578 005f  fo._yPopFifoEx._
-00042c00: 7950 6f70 4669 666f 005f 7946 6f72 6365  yPopFifo._yForce
-00042c10: 4669 666f 005f 7950 6565 6b46 6966 6f45  Fifo._yPeekFifoE
-00042c20: 7800 5f79 5065 656b 4669 666f 005f 7950  x._yPeekFifo._yP
-00042c30: 6565 6b43 6f6e 7469 6e75 6f75 7346 6966  eekContinuousFif
-00042c40: 6f45 7800 5f79 5065 656b 436f 6e74 696e  oEx._yPeekContin
-00042c50: 756f 7573 4669 666f 005f 7953 6565 6b46  uousFifo._ySeekF
-00042c60: 6966 6f45 7800 5f79 5365 656b 4669 666f  ifoEx._ySeekFifo
-00042c70: 005f 7946 6966 6f47 6574 5573 6564 4578  ._yFifoGetUsedEx
-00042c80: 005f 7946 6966 6f47 6574 5573 6564 005f  ._yFifoGetUsed._
-00042c90: 7946 6966 6f47 6574 4672 6565 4578 005f  yFifoGetFreeEx._
-00042ca0: 7946 6966 6f47 6574 4672 6565 005f 7978  yFifoGetFree._yx
-00042cb0: 746f 6100 5f64 6563 6f64 6550 7562 5661  toa._decodePubVa
-00042cc0: 6c00 7974 6872 6561 642e 6300 2f55 7365  l.ythread.c./Use
-00042cd0: 7273 2f79 6f63 746f 2f74 6d70 5f62 7569  rs/yocto/tmp_bui
-00042ce0: 6c64 2f79 6f63 746f 7072 6f64 2f79 6f63  ld/yoctoprod/yoc
-00042cf0: 746f 6c69 622f 7631 2e30 2f50 7562 6c69  tolib/v1.0/Publi
-00042d00: 632f 6370 702f 4269 6e61 7269 6573 2f78  c/cpp/Binaries/x
-00042d10: 636f 6465 5f61 732f 7961 7069 2f62 7569  code_as/yapi/bui
-00042d20: 6c64 2f79 6170 692e 6275 696c 642f 5265  ld/yapi.build/Re
-00042d30: 6c65 6173 652f 7961 7069 2e62 7569 6c64  lease/yapi.build
-00042d40: 2f4f 626a 6563 7473 2d6e 6f72 6d61 6c2f  /Objects-normal/
-00042d50: 7838 365f 3634 2f79 7468 7265 6164 2e6f  x86_64/ythread.o
-00042d60: 005f 7943 7265 6174 6545 7665 6e74 005f  ._yCreateEvent._
-00042d70: 7943 7265 6174 654d 616e 7561 6c45 7665  yCreateManualEve
-00042d80: 6e74 005f 7953 6574 4576 656e 7400 5f79  nt._ySetEvent._y
-00042d90: 5265 7365 7445 7665 6e74 005f 7957 6169  ResetEvent._yWai
-00042da0: 7446 6f72 4576 656e 7400 5f79 436c 6f73  tForEvent._yClos
-00042db0: 6545 7665 6e74 005f 7954 6872 6561 6449  eEvent._yThreadI
-00042dc0: 6e64 6578 005f 7943 7265 6174 6544 6574  ndex._yCreateDet
-00042dd0: 6163 6865 6454 6872 6561 644e 616d 6564  achedThreadNamed
-00042de0: 005f 7943 7265 6174 6544 6574 6163 6865  ._yCreateDetache
-00042df0: 6454 6872 6561 6445 7800 5f79 5468 7265  dThreadEx._yThre
-00042e00: 6164 4372 6561 7465 4e61 6d65 6400 5f79  adCreateNamed._y
-00042e10: 5468 7265 6164 4973 5275 6e6e 696e 6700  ThreadIsRunning.
-00042e20: 5f79 5468 7265 6164 5369 676e 616c 5374  _yThreadSignalSt
-00042e30: 6172 7400 5f79 5468 7265 6164 5369 676e  art._yThreadSign
-00042e40: 616c 456e 6400 5f79 5468 7265 6164 5265  alEnd._yThreadRe
-00042e50: 7175 6573 7445 6e64 005f 7954 6872 6561  questEnd._yThrea
-00042e60: 644d 7573 7445 6e64 005f 7954 6872 6561  dMustEnd._yThrea
-00042e70: 644b 696c 6c00 5f79 496e 6974 6961 6c69  dKill._yInitiali
-00042e80: 7a65 4372 6974 6963 616c 5365 6374 696f  zeCriticalSectio
-00042e90: 6e00 5f79 456e 7465 7243 7269 7469 6361  n._yEnterCritica
-00042ea0: 6c53 6563 7469 6f6e 005f 7954 7279 456e  lSection._yTryEn
-00042eb0: 7465 7243 7269 7469 6361 6c53 6563 7469  terCriticalSecti
-00042ec0: 6f6e 005f 794c 6561 7665 4372 6974 6963  on._yLeaveCritic
-00042ed0: 616c 5365 6374 696f 6e00 5f79 4465 6c65  alSection._yDele
-00042ee0: 7465 4372 6974 6963 616c 5365 6374 696f  teCriticalSectio
-00042ef0: 6e00 5f69 6e69 7454 7364 4b65 7900 5f79  n._initTsdKey._y
-00042f00: 496e 6974 4b65 794f 6e63 6500 5f79 4e65  InitKeyOnce._yNe
-00042f10: 7874 5468 7265 6164 4964 7800 5f79 5473  xtThreadIdx._yTs
-00042f20: 644b 6579 0000 0000 0000 0000 0000 0000  dKey............
-00042f30: fade 0cc0 0000 0a4d 0000 0004 0000 0000  .......M........
-00042f40: 0000 002c 0000 0002 0000 0935 0000 0005  ...,.......5....
-00042f50: 0000 0941 0001 0000 0000 0a45 fade 0c02  ...A.......E....
-00042f60: 0000 0909 0002 0400 0000 0002 0000 0129  ...............)
-00042f70: 0000 0058 0000 0005 0000 003f 0003 ef30  ...X.......?...0
-00042f80: 2002 000c 0000 0000 0000 0000 0000 0000   ...............
-00042f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00042fa0: 0000 0000 0000 0000 0002 8000 0000 0000  ................
-00042fb0: 0000 0000 6c69 6279 6170 692d 3535 3535  ....libyapi-5555
-00042fc0: 3439 3434 6166 3366 3566 3961 3031 3365  4944af3f5f9a013e
-00042fd0: 3363 3566 6263 6534 3336 3762 3634 3262  3c5fbce4367b642b
-00042fe0: 3230 3335 00c6 dc9c 8e50 8ccb 383c 8c74  2035.....P..8<.t
-00042ff0: 84e8 3d73 a81a c271 ac0d c9ba 1ea2 efca  ..=s...q........
-00043000: 12de fda0 c600 0000 0000 0000 0000 0000  ................
+0003e6d0: 851b 0000 0100 0001 0000 0000 0000 0000  ................
+0003e6e0: 8d1b 0000 0100 0001 0000 0000 0000 0000  ................
+0003e6f0: 981b 0000 0100 0001 0000 0000 0000 0000  ................
+0003e700: b507 0000 b607 0000 b707 0000 b807 0000  ................
+0003e710: b907 0000 ba07 0000 bb07 0000 bc07 0000  ................
+0003e720: bd07 0000 be07 0000 bf07 0000 c007 0000  ................
+0003e730: c107 0000 c207 0000 c307 0000 c407 0000  ................
+0003e740: c507 0000 c607 0000 c707 0000 c807 0000  ................
+0003e750: c907 0000 ca07 0000 cb07 0000 cc07 0000  ................
+0003e760: cd07 0000 ce07 0000 cf07 0000 d007 0000  ................
+0003e770: d107 0000 d207 0000 d307 0000 d607 0000  ................
+0003e780: d707 0000 d807 0000 d907 0000 da07 0000  ................
+0003e790: db07 0000 dc07 0000 de07 0000 df07 0000  ................
+0003e7a0: e007 0000 e107 0000 e207 0000 e307 0000  ................
+0003e7b0: e407 0000 e507 0000 e607 0000 e707 0000  ................
+0003e7c0: e807 0000 e907 0000 ea07 0000 eb07 0000  ................
+0003e7d0: ec07 0000 ed07 0000 ee07 0000 ef07 0000  ................
+0003e7e0: f007 0000 f107 0000 f207 0000 f307 0000  ................
+0003e7f0: f407 0000 f507 0000 fa07 0000 fb07 0000  ................
+0003e800: fc07 0000 fd07 0000 fe07 0000 ff07 0000  ................
+0003e810: 0008 0000 0108 0000 0208 0000 0308 0000  ................
+0003e820: 0408 0000 0508 0000 0608 0000 0708 0000  ................
+0003e830: 0808 0000 0908 0000 0a08 0000 0b08 0000  ................
+0003e840: 0c08 0000 0d08 0000 0e08 0000 0f08 0000  ................
+0003e850: 1008 0000 1108 0000 1208 0000 1308 0000  ................
+0003e860: 1408 0000 1508 0000 1608 0000 1708 0000  ................
+0003e870: 1808 0000 1908 0000 1a08 0000 1b08 0000  ................
+0003e880: 1c08 0000 1d08 0000 1e08 0000 1f08 0000  ................
+0003e890: 2008 0000 2108 0000 2208 0000 2308 0000   ...!..."...#...
+0003e8a0: 2408 0000 2508 0000 2608 0000 2708 0000  $...%...&...'...
+0003e8b0: 2808 0000 2908 0000 2a08 0000 2b08 0000  (...)...*...+...
+0003e8c0: 2c08 0000 2d08 0000 2e08 0000 b507 0000  ,...-...........
+0003e8d0: b607 0000 b707 0000 b807 0000 b907 0000  ................
+0003e8e0: ba07 0000 bb07 0000 bc07 0000 bd07 0000  ................
+0003e8f0: be07 0000 bf07 0000 c007 0000 c107 0000  ................
+0003e900: c207 0000 c307 0000 c407 0000 c507 0000  ................
+0003e910: c607 0000 c707 0000 c807 0000 c907 0000  ................
+0003e920: ca07 0000 cb07 0000 cc07 0000 cd07 0000  ................
+0003e930: ce07 0000 cf07 0000 d007 0000 d107 0000  ................
+0003e940: d207 0000 d307 0000 d407 0000 d607 0000  ................
+0003e950: d707 0000 d807 0000 d907 0000 da07 0000  ................
+0003e960: db07 0000 dc07 0000 dd07 0000 de07 0000  ................
+0003e970: df07 0000 e007 0000 e107 0000 e207 0000  ................
+0003e980: e307 0000 e407 0000 e507 0000 e607 0000  ................
+0003e990: e707 0000 e807 0000 e907 0000 ea07 0000  ................
+0003e9a0: eb07 0000 ec07 0000 ed07 0000 ee07 0000  ................
+0003e9b0: ef07 0000 f007 0000 f107 0000 f207 0000  ................
+0003e9c0: f307 0000 f407 0000 f507 0000 f607 0000  ................
+0003e9d0: f707 0000 f807 0000 f907 0000 fa07 0000  ................
+0003e9e0: fb07 0000 fc07 0000 fd07 0000 fe07 0000  ................
+0003e9f0: ff07 0000 0008 0000 0108 0000 0208 0000  ................
+0003ea00: 0308 0000 0408 0000 0508 0000 0608 0000  ................
+0003ea10: 0708 0000 0808 0000 0908 0000 0a08 0000  ................
+0003ea20: 0b08 0000 0c08 0000 0d08 0000 0e08 0000  ................
+0003ea30: 0f08 0000 1008 0000 1108 0000 1208 0000  ................
+0003ea40: 1308 0000 1408 0000 1508 0000 1608 0000  ................
+0003ea50: 1708 0000 1808 0000 1908 0000 1a08 0000  ................
+0003ea60: 1b08 0000 1c08 0000 1d08 0000 1e08 0000  ................
+0003ea70: 1f08 0000 2008 0000 2108 0000 2208 0000  .... ...!..."...
+0003ea80: 2308 0000 2408 0000 2508 0000 2608 0000  #...$...%...&...
+0003ea90: 2708 0000 2808 0000 2908 0000 2a08 0000  '...(...)...*...
+0003eaa0: 2b08 0000 2c08 0000 2d08 0000 2e08 0000  +...,...-.......
+0003eab0: 2000 5f42 6c6f 636b 696e 6752 6561 6400   ._BlockingRead.
+0003eac0: 5f43 6865 636b 5753 4175 7468 005f 436f  _CheckWSAuth._Co
+0003ead0: 6d70 7574 6541 7574 6848 4131 005f 436f  mputeAuthHA1._Co
+0003eae0: 6d70 7574 6541 7574 6848 4132 005f 436f  mputeAuthHA2._Co
+0003eaf0: 6d70 7574 6541 7574 6852 6573 706f 6e73  mputeAuthRespons
+0003eb00: 6500 5f46 7573 696f 6e45 7272 6d73 6700  e._FusionErrmsg.
+0003eb10: 5f49 7356 616c 6964 4279 6e46 696c 6500  _IsValidBynFile.
+0003eb20: 5f49 7356 616c 6964 4279 6e48 6561 6400  _IsValidBynHead.
+0003eb30: 5f4d 4435 4164 6444 6174 6100 5f4d 4435  _MD5AddData._MD5
+0003eb40: 4361 6c63 756c 6174 6500 5f4d 4435 496e  Calculate._MD5In
+0003eb50: 6974 6961 6c69 7a65 005f 5365 6e64 4461  itialize._SendDa
+0003eb60: 7461 5061 636b 6574 005f 5365 7269 616c  taPacket._Serial
+0003eb70: 4e75 6d62 6572 5374 7200 5f53 6572 6961  NumberStr._Seria
+0003eb80: 6c52 6566 005f 5661 6c69 6461 7465 4279  lRef._ValidateBy
+0003eb90: 6e43 6f6d 7061 7400 5f57 616b 6555 7041  nCompat._WakeUpA
+0003eba0: 6c6c 536c 6565 7000 5f59 464f 5045 4e00  llSleep._YFOPEN.
+0003ebb0: 5f59 6374 7844 6576 6963 654c 6973 7456  _YctxDeviceListV
+0003ebc0: 616c 6964 6974 794d 7300 5f59 6374 784e  alidityMs._YctxN
+0003ebd0: 6574 776f 726b 5469 6d65 6f75 7400 5f62  etworkTimeout._b
+0003ebe0: 696e 3273 7472 005f 6368 6563 6b46 6f72  in2str._checkFor
+0003ebf0: 5361 6d65 4875 6241 6363 6573 7300 5f64  SameHubAccess._d
+0003ec00: 6267 6c6f 6766 005f 6465 636f 6465 4865  bglogf._decodeHe
+0003ec10: 7800 5f64 6563 6f64 654e 6574 4675 6e63  x._decodeNetFunc
+0003ec20: 5661 6c56 3200 5f64 6563 6f64 6550 7562  ValV2._decodePub
+0003ec30: 5661 6c00 5f64 6574 6563 7465 6449 6661  Val._detectedIfa
+0003ec40: 6365 7300 5f64 6576 4864 6c49 6e66 6f00  ces._devHdlInfo.
+0003ec50: 5f64 6e73 4361 6368 6500 5f64 756d 7059  _dnsCache._dumpY
+0003ec60: 5065 7266 456e 7472 7900 5f66 6374 7800  PerfEntry._fctx.
+0003ec70: 5f66 696e 6444 6576 005f 6669 6e64 4465  _findDev._findDe
+0003ec80: 7646 726f 6d49 4f48 646c 005f 6669 6e64  vFromIOHdl._find
+0003ec90: 4465 7648 646c 4672 6f6d 5374 7200 5f66  DevHdlFromStr._f
+0003eca0: 6972 6d5f 6465 7600 5f66 6972 6d5f 706b  irm_dev._firm_pk
+0003ecb0: 7400 5f66 7265 6542 6c6b 7300 5f66 7265  t._freeBlks._fre
+0003ecc0: 6544 6576 5964 7849 6e66 6f73 005f 6861  eDevYdxInfos._ha
+0003ecd0: 6e64 6c65 4e65 744e 6f74 6966 6963 6174  ndleNetNotificat
+0003ece0: 696f 6e00 5f69 6e69 7444 6576 5964 7849  ion._initDevYdxI
+0003ecf0: 6e66 6f73 005f 6e62 4465 7465 6374 6564  nfos._nbDetected
+0003ed00: 4966 6163 6573 005f 7072 6f67 5f47 6574  Ifaces._prog_Get
+0003ed10: 4350 554e 616d 6500 5f72 6571 7565 7374  CPUName._request
+0003ed20: 5f70 656e 6469 6e67 5f6c 6f67 7300 5f73  _pending_logs._s
+0003ed30: 6861 315f 696e 6974 005f 7546 6c61 7368  ha1_init._uFlash
+0003ed40: 4465 7669 6365 005f 7664 6267 6c6f 6766  Device._vdbglogf
+0003ed50: 005f 7770 416c 6c6f 7755 6e72 6567 6973  ._wpAllowUnregis
+0003ed60: 7465 7245 7800 5f77 7045 6e74 7279 436f  terEx._wpEntryCo
+0003ed70: 756e 7400 5f77 7047 6574 4174 7472 6962  unt._wpGetAttrib
+0003ed80: 7574 6500 5f77 7047 6574 4465 7659 6478  ute._wpGetDevYdx
+0003ed90: 005f 7770 4765 7444 6576 6963 6549 6e66  ._wpGetDeviceInf
+0003eda0: 6f00 5f77 7047 6574 4c6f 6769 6361 6c4e  o._wpGetLogicalN
+0003edb0: 616d 6500 5f77 7047 6574 5365 7269 616c  ame._wpGetSerial
+0003edc0: 005f 7770 4d61 726b 466f 7255 6e72 6567  ._wpMarkForUnreg
+0003edd0: 6973 7465 7200 5f77 7050 7265 7665 6e74  ister._wpPrevent
+0003ede0: 556e 7265 6769 7374 6572 4578 005f 7770  UnregisterEx._wp
+0003edf0: 5265 6769 7374 6572 005f 7770 5365 6172  Register._wpSear
+0003ee00: 6368 005f 7770 5365 6172 6368 4279 4e61  ch._wpSearchByNa
+0003ee10: 6d65 4861 7368 005f 7770 5365 6172 6368  meHash._wpSearch
+0003ee20: 4578 005f 7773 5f63 6c65 616e 7570 005f  Ex._ws_cleanup._
+0003ee30: 7773 5f74 6872 6561 6400 5f79 426c 6b4c  ws_thread._yBlkL
+0003ee40: 6973 744c 656e 6774 6800 5f79 426c 6b4c  istLength._yBlkL
+0003ee50: 6973 7453 6565 6b00 5f79 436c 6f73 6545  istSeek._yCloseE
+0003ee60: 7665 6e74 005f 7943 6f6e 7375 6d65 5761  vent._yConsumeWa
+0003ee70: 6b65 5570 536f 636b 6574 005f 7943 6f6e  keUpSocket._yCon
+0003ee80: 7465 7874 005f 7943 7265 6174 6544 6574  text._yCreateDet
+0003ee90: 6163 6865 6454 6872 6561 644e 616d 6564  achedThreadNamed
+0003eea0: 005f 7943 7265 6174 6545 7665 6e74 005f  ._yCreateEvent._
+0003eeb0: 7943 7265 6174 654d 616e 7561 6c45 7665  yCreateManualEve
+0003eec0: 6e74 005f 7944 656c 6574 6543 7269 7469  nt._yDeleteCriti
+0003eed0: 6361 6c53 6563 7469 6f6e 005f 7944 6967  calSection._yDig
+0003eee0: 6573 7441 7574 686f 7269 7a61 7469 6f6e  estAuthorization
+0003eef0: 005f 7944 7269 6e67 5761 6b65 5570 536f  ._yDringWakeUpSo
+0003ef00: 636b 6574 005f 7944 7570 5365 7400 5f79  cket._yDupSet._y
+0003ef10: 456e 7465 7243 7269 7469 6361 6c53 6563  EnterCriticalSec
+0003ef20: 7469 6f6e 005f 7946 6966 6f43 6c65 616e  tion._yFifoClean
+0003ef30: 7570 005f 7946 6966 6f45 6d70 7479 005f  up._yFifoEmpty._
+0003ef40: 7946 6966 6f45 6d70 7479 4578 005f 7946  yFifoEmptyEx._yF
+0003ef50: 6966 6f45 6e74 6572 4353 005f 7946 6966  ifoEnterCS._yFif
+0003ef60: 6f47 6574 4672 6565 005f 7946 6966 6f47  oGetFree._yFifoG
+0003ef70: 6574 4672 6565 4578 005f 7946 6966 6f47  etFreeEx._yFifoG
+0003ef80: 6574 5573 6564 005f 7946 6966 6f47 6574  etUsed._yFifoGet
+0003ef90: 5573 6564 4578 005f 7946 6966 6f49 6e69  UsedEx._yFifoIni
+0003efa0: 7445 7800 5f79 4669 666f 4c65 6176 6543  tEx._yFifoLeaveC
+0003efb0: 5300 5f79 466f 7263 6546 6966 6f00 5f79  S._yForceFifo._y
+0003efc0: 4672 6565 4d75 7465 7800 5f79 4672 6565  FreeMutex._yFree
+0003efd0: 5761 6b65 5570 536f 636b 6574 005f 7946  WakeUpSocket._yF
+0003efe0: 756e 6374 696f 6e54 696d 6564 5570 6461  unctionTimedUpda
+0003eff0: 7465 005f 7946 756e 6374 696f 6e55 7064  te._yFunctionUpd
+0003f000: 6174 6500 5f79 4861 7368 4672 6565 005f  ate._yHashFree._
+0003f010: 7948 6173 6847 6574 4275 6600 5f79 4861  yHashGetBuf._yHa
+0003f020: 7368 4765 7453 7472 005f 7948 6173 6847  shGetStr._yHashG
+0003f030: 6574 5374 724c 656e 005f 7948 6173 6847  etStrLen._yHashG
+0003f040: 6574 5374 7250 7472 005f 7948 6173 6849  etStrPtr._yHashI
+0003f050: 6e69 7400 5f79 4861 7368 4d75 7465 7800  nit._yHashMutex.
+0003f060: 5f79 4861 7368 5075 7442 7566 005f 7948  _yHashPutBuf._yH
+0003f070: 6173 6850 7574 5374 7200 5f79 4861 7368  ashPutStr._yHash
+0003f080: 5465 7374 4275 6600 5f79 4861 7368 5465  TestBuf._yHashTe
+0003f090: 7374 5374 7200 5f79 496e 6974 5073 6b00  stStr._yInitPsk.
+0003f0a0: 5f79 496e 6974 5761 6b65 5570 536f 636b  _yInitWakeUpSock
+0003f0b0: 6574 005f 7949 6e69 7469 616c 697a 6543  et._yInitializeC
+0003f0c0: 7269 7469 6361 6c53 6563 7469 6f6e 005f  riticalSection._
+0003f0d0: 7949 7465 7250 736b 005f 794a 736f 6e50  yIterPsk._yJsonP
+0003f0e0: 6172 7365 005f 794a 736f 6e53 6b69 7000  arse._yJsonSkip.
+0003f0f0: 5f79 4c65 6176 6543 7269 7469 6361 6c53  _yLeaveCriticalS
+0003f100: 6563 7469 6f6e 005f 794e 6574 4875 6247  ection._yNetHubG
+0003f110: 6574 426f 6f74 6c6f 6164 6572 7300 5f79  etBootloaders._y
+0003f120: 4e65 7453 6574 4572 7245 7800 5f79 5061  NetSetErrEx._yPa
+0003f130: 7273 6557 5757 4175 7468 656e 7469 6361  rseWWWAuthentica
+0003f140: 7465 005f 7950 6565 6b43 6f6e 7469 6e75  te._yPeekContinu
+0003f150: 6f75 7346 6966 6f00 5f79 5065 656b 436f  ousFifo._yPeekCo
+0003f160: 6e74 696e 756f 7573 4669 666f 4578 005f  ntinuousFifoEx._
+0003f170: 7950 6565 6b46 6966 6f00 5f79 5065 656b  yPeekFifo._yPeek
+0003f180: 4669 666f 4578 005f 7950 6b74 5175 6575  FifoEx._yPktQueu
+0003f190: 6546 7265 6500 5f79 506b 7451 7565 7565  eFree._yPktQueue
+0003f1a0: 496e 6974 005f 7950 6b74 5175 6575 6550  Init._yPktQueueP
+0003f1b0: 6565 6b48 3244 005f 7950 6b74 5175 6575  eekH2D._yPktQueu
+0003f1c0: 6550 6f70 4832 4400 5f79 506b 7451 7565  ePopH2D._yPktQue
+0003f1d0: 7565 5075 7368 4432 4800 5f79 506b 7451  uePushD2H._yPktQ
+0003f1e0: 7565 7565 5075 7368 4832 4400 5f79 506b  ueuePushH2D._yPk
+0003f1f0: 7451 7565 7565 5365 7445 7272 6f72 005f  tQueueSetError._
+0003f200: 7950 6b74 5175 6575 6557 6169 7441 6e64  yPktQueueWaitAnd
+0003f210: 506f 7044 3248 005f 7950 6f70 4669 666f  PopD2H._yPopFifo
+0003f220: 005f 7950 6f70 4669 666f 4578 005f 7950  ._yPopFifoEx._yP
+0003f230: 726f 6746 7265 6500 5f79 5072 6f67 496e  rogFree._yProgIn
+0003f240: 6974 005f 7950 7573 6846 6966 6f00 5f79  it._yPushFifo._y
+0003f250: 5075 7368 4669 666f 4578 005f 7952 6571  PushFifoEx._yReq
+0003f260: 416c 6c6f 6300 5f79 5265 7143 6c6f 7365  Alloc._yReqClose
+0003f270: 005f 7952 6571 4672 6565 005f 7952 6571  ._yReqFree._yReq
+0003f280: 4765 7400 5f79 5265 7148 6173 5065 6e64  Get._yReqHasPend
+0003f290: 696e 6700 5f79 5265 7149 7341 7379 6e63  ing._yReqIsAsync
+0003f2a0: 005f 7952 6571 4973 456f 6600 5f79 5265  ._yReqIsEof._yRe
+0003f2b0: 714d 756c 7469 5365 6c65 6374 005f 7952  qMultiSelect._yR
+0003f2c0: 6571 4f70 656e 005f 7952 6571 5265 6164  eqOpen._yReqRead
+0003f2d0: 005f 7952 6571 5365 6c65 6374 005f 7952  ._yReqSelect._yR
+0003f2e0: 6573 6574 4576 656e 7400 5f79 5265 736f  esetEvent._yReso
+0003f2f0: 6c76 6544 4e53 005f 7953 4841 3100 5f79  lveDNS._ySHA1._y
+0003f300: 5353 4450 4469 7363 6f76 6572 005f 7953  SSDPDiscover._yS
+0003f310: 5344 5053 7461 7274 005f 7953 5344 5053  SDPStart._ySSDPS
+0003f320: 746f 7000 5f79 5365 656b 4669 666f 005f  top._ySeekFifo._
+0003f330: 7953 6565 6b46 6966 6f45 7800 5f79 5365  ySeekFifoEx._ySe
+0003f340: 7445 7272 005f 7953 6574 4576 656e 7400  tErr._ySetEvent.
+0003f350: 5f79 5374 6172 7457 616b 6555 7053 6f63  _yStartWakeUpSoc
+0003f360: 6b65 7400 5f79 5463 7044 6f77 6e6c 6f61  ket._yTcpDownloa
+0003f370: 6400 5f79 5463 7049 6e69 7400 5f79 5463  d._yTcpInit._yTc
+0003f380: 7053 6875 7464 6f77 6e00 5f79 5468 7265  pShutdown._yThre
+0003f390: 6164 4372 6561 7465 4e61 6d65 6400 5f79  adCreateNamed._y
+0003f3a0: 5468 7265 6164 496e 6465 7800 5f79 5468  ThreadIndex._yTh
+0003f3b0: 7265 6164 4973 5275 6e6e 696e 6700 5f79  readIsRunning._y
+0003f3c0: 5468 7265 6164 4b69 6c6c 005f 7954 6872  ThreadKill._yThr
+0003f3d0: 6561 644d 7573 7445 6e64 005f 7954 6872  eadMustEnd._yThr
+0003f3e0: 6561 6452 6571 7565 7374 456e 6400 5f79  eadRequestEnd._y
+0003f3f0: 5468 7265 6164 5369 676e 616c 456e 6400  ThreadSignalEnd.
+0003f400: 5f79 5468 7265 6164 5369 676e 616c 5374  _yThreadSignalSt
+0003f410: 6172 7400 5f79 5472 7945 6e74 6572 4372  art._yTryEnterCr
+0003f420: 6974 6963 616c 5365 6374 696f 6e00 5f79  iticalSection._y
+0003f430: 5553 4247 6574 426f 6f6c 6f61 6465 7200  USBGetBooloader.
+0003f440: 5f79 5553 4252 656c 6561 7365 416c 6c44  _yUSBReleaseAllD
+0003f450: 6576 6963 6573 005f 7955 5342 5570 6461  evices._yUSBUpda
+0003f460: 7465 4465 7669 6365 4c69 7374 005f 7955  teDeviceList._yU
+0003f470: 7362 436c 6f73 6500 5f79 5573 6245 4f46  sbClose._yUsbEOF
+0003f480: 005f 7955 7362 4672 6565 005f 7955 7362  ._yUsbFree._yUsb
+0003f490: 4964 6c65 005f 7955 7362 496e 6974 005f  Idle._yUsbInit._
+0003f4a0: 7955 7362 4f70 656e 005f 7955 7362 4f70  yUsbOpen._yUsbOp
+0003f4b0: 656e 4465 7644 6573 6372 005f 7955 7362  enDevDescr._yUsb
+0003f4c0: 5265 6164 426c 6f63 6b00 5f79 5573 6252  ReadBlock._yUsbR
+0003f4d0: 6561 644e 6f6e 426c 6f63 6b00 5f79 5573  eadNonBlock._yUs
+0003f4e0: 6253 6574 494f 4173 796e 6300 5f79 5573  bSetIOAsync._yUs
+0003f4f0: 6254 7261 6666 6963 5065 6e64 696e 6700  bTrafficPending.
+0003f500: 5f79 5573 6257 7269 7465 005f 7957 6169  _yUsbWrite._yWai
+0003f510: 7446 6f72 4576 656e 7400 5f79 5770 4c69  tForEvent._yWpLi
+0003f520: 7374 4865 6164 005f 7957 704d 7574 6578  stHead._yWpMutex
+0003f530: 005f 7959 704c 6973 7448 6561 6400 5f79  ._yYpListHead._y
+0003f540: 5970 4d75 7465 7800 5f79 6170 6941 6464  YpMutex._yapiAdd
+0003f550: 5564 6576 5275 6c65 7346 6f72 596f 6374  UdevRulesForYoct
+0003f560: 6f00 5f79 6170 6943 6865 636b 4669 726d  o._yapiCheckFirm
+0003f570: 7761 7265 005f 7961 7069 4368 6563 6b46  ware._yapiCheckF
+0003f580: 6972 6d77 6172 655f 696e 7465 726e 616c  irmware_internal
+0003f590: 005f 7961 7069 4368 6563 6b4c 6f67 6963  ._yapiCheckLogic
+0003f5a0: 616c 4e61 6d65 005f 7961 7069 4672 6565  alName._yapiFree
+0003f5b0: 4150 4900 5f79 6170 6946 7265 654d 656d  API._yapiFreeMem
+0003f5c0: 005f 7961 7069 4765 7441 5049 5665 7273  ._yapiGetAPIVers
+0003f5d0: 696f 6e00 5f79 6170 6947 6574 416c 6c44  ion._yapiGetAllD
+0003f5e0: 6576 6963 6573 005f 7961 7069 4765 7441  evices._yapiGetA
+0003f5f0: 6c6c 4a73 6f6e 4b65 7973 005f 7961 7069  llJsonKeys._yapi
+0003f600: 4765 7442 6f6f 746c 6f61 6465 7273 005f  GetBootloaders._
+0003f610: 7961 7069 4765 7442 6f6f 746c 6f61 6465  yapiGetBootloade
+0003f620: 7273 4465 7673 005f 7961 7069 4765 7443  rsDevs._yapiGetC
+0003f630: 4e6f 6e63 6500 5f79 6170 6947 6574 444c  Nonce._yapiGetDL
+0003f640: 4c50 6174 6800 5f79 6170 6947 6574 4465  LPath._yapiGetDe
+0003f650: 7669 6365 005f 7961 7069 4765 7444 6576  vice._yapiGetDev
+0003f660: 6963 6549 6e66 6f00 5f79 6170 6947 6574  iceInfo._yapiGet
+0003f670: 4465 7669 6365 5061 7468 005f 7961 7069  DevicePath._yapi
+0003f680: 4765 7444 6576 6963 6550 6174 6845 7800  GetDevicePathEx.
+0003f690: 5f79 6170 6947 6574 4675 6e63 7469 6f6e  _yapiGetFunction
+0003f6a0: 005f 7961 7069 4765 7446 756e 6374 696f  ._yapiGetFunctio
+0003f6b0: 6e49 6e66 6f00 5f79 6170 6947 6574 4675  nInfo._yapiGetFu
+0003f6c0: 6e63 7469 6f6e 496e 666f 4578 005f 7961  nctionInfoEx._ya
+0003f6d0: 7069 4765 7446 756e 6374 696f 6e73 4279  piGetFunctionsBy
+0003f6e0: 436c 6173 7300 5f79 6170 6947 6574 4675  Class._yapiGetFu
+0003f6f0: 6e63 7469 6f6e 7342 7944 6576 6963 6500  nctionsByDevice.
+0003f700: 5f79 6170 6947 6574 4d65 6d00 5f79 6170  _yapiGetMem._yap
+0003f710: 6947 6574 4e65 7444 6576 4c69 7374 5661  iGetNetDevListVa
+0003f720: 6c69 6469 7479 005f 7961 7069 4765 744e  lidity._yapiGetN
+0003f730: 6574 776f 726b 5469 6d65 6f75 7400 5f79  etworkTimeout._y
+0003f740: 6170 6947 6574 5375 6264 6576 6963 6573  apiGetSubdevices
+0003f750: 005f 7961 7069 4765 7454 6963 6b43 6f75  ._yapiGetTickCou
+0003f760: 6e74 005f 7961 7069 4854 5450 5265 7175  nt._yapiHTTPRequ
+0003f770: 6573 7400 5f79 6170 6948 5454 5052 6571  est._yapiHTTPReq
+0003f780: 7565 7374 4173 796e 6300 5f79 6170 6948  uestAsync._yapiH
+0003f790: 5454 5052 6571 7565 7374 4173 796e 6345  TTPRequestAsyncE
+0003f7a0: 7800 5f79 6170 6948 5454 5052 6571 7565  x._yapiHTTPReque
+0003f7b0: 7374 4173 796e 634f 7574 4f66 4261 6e64  stAsyncOutOfBand
+0003f7c0: 005f 7961 7069 4854 5450 5265 7175 6573  ._yapiHTTPReques
+0003f7d0: 7453 796e 6344 6f6e 6500 5f79 6170 6948  tSyncDone._yapiH
+0003f7e0: 5454 5052 6571 7565 7374 5379 6e63 446f  TTPRequestSyncDo
+0003f7f0: 6e65 5f69 6e74 6572 6e61 6c00 5f79 6170  ne_internal._yap
+0003f800: 6948 5454 5052 6571 7565 7374 5379 6e63  iHTTPRequestSync
+0003f810: 5374 6172 7400 5f79 6170 6948 5454 5052  Start._yapiHTTPR
+0003f820: 6571 7565 7374 5379 6e63 5374 6172 7445  equestSyncStartE
+0003f830: 7800 5f79 6170 6948 5454 5052 6571 7565  x._yapiHTTPReque
+0003f840: 7374 5379 6e63 5374 6172 7445 785f 696e  stSyncStartEx_in
+0003f850: 7465 726e 616c 005f 7961 7069 4854 5450  ternal._yapiHTTP
+0003f860: 5265 7175 6573 7453 796e 6353 7461 7274  RequestSyncStart
+0003f870: 4f75 744f 6642 616e 6400 5f79 6170 6948  OutOfBand._yapiH
+0003f880: 616e 646c 6545 7665 6e74 7300 5f79 6170  andleEvents._yap
+0003f890: 6949 6e69 7441 5049 005f 7961 7069 4973  iInitAPI._yapiIs
+0003f8a0: 4d6f 6475 6c65 5772 6974 6162 6c65 005f  ModuleWritable._
+0003f8b0: 7961 7069 4a73 6f6e 4465 636f 6465 5374  yapiJsonDecodeSt
+0003f8c0: 7269 6e67 005f 7961 7069 4a73 6f6e 4765  ring._yapiJsonGe
+0003f8d0: 7450 6174 6800 5f79 6170 694a 736f 6e47  tPath._yapiJsonG
+0003f8e0: 6574 5061 7468 5f69 6e74 6572 6e61 6c00  etPath_internal.
+0003f8f0: 5f79 6170 694c 6f63 6b44 6576 6963 6543  _yapiLockDeviceC
+0003f900: 616c 6c42 6163 6b00 5f79 6170 694c 6f63  allBack._yapiLoc
+0003f910: 6b46 756e 6374 696f 6e43 616c 6c42 6163  kFunctionCallBac
+0003f920: 6b00 5f79 6170 6950 7265 7265 6769 7374  k._yapiPreregist
+0003f930: 6572 4875 6200 5f79 6170 6950 756c 6c44  erHub._yapiPullD
+0003f940: 6576 6963 654c 6f67 005f 7961 7069 5075  eviceLog._yapiPu
+0003f950: 6c6c 4465 7669 6365 4c6f 6745 7800 5f79  llDeviceLogEx._y
+0003f960: 6170 6952 6567 6973 7465 7242 6561 636f  apiRegisterBeaco
+0003f970: 6e43 616c 6c62 6163 6b00 5f79 6170 6952  nCallback._yapiR
+0003f980: 6567 6973 7465 7244 6576 6963 6541 7272  egisterDeviceArr
+0003f990: 6976 616c 4361 6c6c 6261 636b 005f 7961  ivalCallback._ya
+0003f9a0: 7069 5265 6769 7374 6572 4465 7669 6365  piRegisterDevice
+0003f9b0: 4368 616e 6765 4361 6c6c 6261 636b 005f  ChangeCallback._
+0003f9c0: 7961 7069 5265 6769 7374 6572 4465 7669  yapiRegisterDevi
+0003f9d0: 6365 436f 6e66 6967 4368 616e 6765 4361  ceConfigChangeCa
+0003f9e0: 6c6c 6261 636b 005f 7961 7069 5265 6769  llback._yapiRegi
+0003f9f0: 7374 6572 4465 7669 6365 4c6f 6743 616c  sterDeviceLogCal
+0003fa00: 6c62 6163 6b00 5f79 6170 6952 6567 6973  lback._yapiRegis
+0003fa10: 7465 7244 6576 6963 6552 656d 6f76 616c  terDeviceRemoval
+0003fa20: 4361 6c6c 6261 636b 005f 7961 7069 5265  Callback._yapiRe
+0003fa30: 6769 7374 6572 4675 6e63 7469 6f6e 5570  gisterFunctionUp
+0003fa40: 6461 7465 4361 6c6c 6261 636b 005f 7961  dateCallback._ya
+0003fa50: 7069 5265 6769 7374 6572 4875 6200 5f79  piRegisterHub._y
+0003fa60: 6170 6952 6567 6973 7465 7248 7562 4469  apiRegisterHubDi
+0003fa70: 7363 6f76 6572 7943 616c 6c62 6163 6b00  scoveryCallback.
+0003fa80: 5f79 6170 6952 6567 6973 7465 724c 6f67  _yapiRegisterLog
+0003fa90: 4675 6e63 7469 6f6e 005f 7961 7069 5265  Function._yapiRe
+0003faa0: 6769 7374 6572 5261 774e 6f74 6966 6963  gisterRawNotific
+0003fab0: 6174 696f 6e43 6200 5f79 6170 6952 6567  ationCb._yapiReg
+0003fac0: 6973 7465 7252 6177 5265 706f 7274 4362  isterRawReportCb
+0003fad0: 005f 7961 7069 5265 6769 7374 6572 5261  ._yapiRegisterRa
+0003fae0: 7752 6570 6f72 7456 3243 6200 5f79 6170  wReportV2Cb._yap
+0003faf0: 6952 6567 6973 7465 7254 696d 6564 5265  iRegisterTimedRe
+0003fb00: 706f 7274 4361 6c6c 6261 636b 005f 7961  portCallback._ya
+0003fb10: 7069 5265 6769 7374 6572 5761 6b65 5570  piRegisterWakeUp
+0003fb20: 4362 005f 7961 7069 5265 7175 6573 744f  Cb._yapiRequestO
+0003fb30: 7065 6e00 5f79 6170 6953 6574 4e65 7444  pen._yapiSetNetD
+0003fb40: 6576 4c69 7374 5661 6c69 6469 7479 005f  evListValidity._
+0003fb50: 7961 7069 5365 744e 6574 776f 726b 5469  yapiSetNetworkTi
+0003fb60: 6d65 6f75 7400 5f79 6170 6953 6574 5472  meout._yapiSetTr
+0003fb70: 6163 6546 696c 6500 5f79 6170 6953 6c65  aceFile._yapiSle
+0003fb80: 6570 005f 7961 7069 5374 6172 7453 746f  ep._yapiStartSto
+0003fb90: 7044 6576 6963 654c 6f67 4361 6c6c 6261  pDeviceLogCallba
+0003fba0: 636b 005f 7961 7069 5465 7374 4875 6200  ck._yapiTestHub.
+0003fbb0: 5f79 6170 6954 7269 6767 6572 4875 6244  _yapiTriggerHubD
+0003fbc0: 6973 636f 7665 7279 005f 7961 7069 556e  iscovery._yapiUn
+0003fbd0: 6c6f 636b 4465 7669 6365 4361 6c6c 4261  lockDeviceCallBa
+0003fbe0: 636b 005f 7961 7069 556e 6c6f 636b 4675  ck._yapiUnlockFu
+0003fbf0: 6e63 7469 6f6e 4361 6c6c 4261 636b 005f  nctionCallBack._
+0003fc00: 7961 7069 556e 7265 6769 7374 6572 4875  yapiUnregisterHu
+0003fc10: 6200 5f79 6170 6955 7064 6174 6544 6576  b._yapiUpdateDev
+0003fc20: 6963 654c 6973 7400 5f79 6170 6955 7064  iceList._yapiUpd
+0003fc30: 6174 6546 6972 6d77 6172 6500 5f79 6170  ateFirmware._yap
+0003fc40: 6955 7064 6174 6546 6972 6d77 6172 6545  iUpdateFirmwareE
+0003fc50: 7800 5f79 6170 6955 7064 6174 6546 6972  x._yapiUpdateFir
+0003fc60: 6d77 6172 655f 696e 7465 726e 616c 005f  mware_internal._
+0003fc70: 796d 656d 6669 6e64 005f 7970 4669 6e64  ymemfind._ypFind
+0003fc80: 426f 6f74 6c6f 6164 6572 7300 5f79 7047  Bootloaders._ypG
+0003fc90: 6574 4174 7472 6962 7574 6573 005f 7970  etAttributes._yp
+0003fca0: 4765 7441 7474 7269 6275 7465 7342 7959  GetAttributesByY
+0003fcb0: 6478 005f 7970 4765 7442 6f6f 746c 6f61  dx._ypGetBootloa
+0003fcc0: 6465 7252 6570 6c79 005f 7970 4765 7443  derReply._ypGetC
+0003fcd0: 6174 6567 6f72 7900 5f79 7047 6574 4675  ategory._ypGetFu
+0003fce0: 6e63 7469 6f6e 496e 666f 005f 7970 4765  nctionInfo._ypGe
+0003fcf0: 7446 756e 6374 696f 6e73 005f 7970 4765  tFunctions._ypGe
+0003fd00: 7446 756e 6374 696f 6e73 4578 005f 7970  tFunctionsEx._yp
+0003fd10: 4765 7454 7970 6500 5f79 7049 7353 656e  GetType._ypIsSen
+0003fd20: 6442 6f6f 746c 6f61 6465 7242 7573 7900  dBootloaderBusy.
+0003fd30: 5f79 7052 6567 6973 7465 7200 5f79 7052  _ypRegister._ypR
+0003fd40: 6567 6973 7465 7242 7959 6478 005f 7970  egisterByYdx._yp
+0003fd50: 5365 6172 6368 005f 7970 5365 6e64 426f  Search._ypSendBo
+0003fd60: 6f74 6c6f 6164 6572 436d 6400 5f79 7055  otloaderCmd._ypU
+0003fd70: 7064 6174 6554 4350 005f 7970 5570 6461  pdateTCP._ypUpda
+0003fd80: 7465 5964 7800 5f79 7370 7269 6e74 665f  teYdx._ysprintf_
+0003fd90: 7300 5f79 7374 7263 6174 5f73 005f 7973  s._ystrcat_s._ys
+0003fda0: 7472 6370 795f 7300 5f79 7374 7264 7570  trcpy_s._ystrdup
+0003fdb0: 5f73 005f 7973 7472 6e63 6174 5f73 005f  _s._ystrncat_s._
+0003fdc0: 7973 7472 6e63 7079 5f73 005f 7973 7472  ystrncpy_s._ystr
+0003fdd0: 6e64 7570 5f73 005f 7974 7261 6365 6669  ndup_s._ytracefi
+0003fde0: 6c65 005f 7976 7370 7269 6e74 665f 7300  le._yvsprintf_s.
+0003fdf0: 5f79 7770 4765 7444 6576 6963 6548 7562  _ywpGetDeviceHub
+0003fe00: 005f 7977 7047 6574 4465 7669 6365 5572  ._ywpGetDeviceUr
+0003fe10: 6c00 5f79 7770 5361 6665 5265 6769 7374  l._ywpSafeRegist
+0003fe20: 6572 005f 7977 7053 6166 6555 6e72 6567  er._ywpSafeUnreg
+0003fe30: 6973 7465 7200 5f79 7770 5361 6665 5570  ister._ywpSafeUp
+0003fe40: 6461 7465 005f 7978 746f 6100 5f79 7979  date._yxtoa._yyy
+0003fe50: 4f53 6864 6c43 6f6d 7061 7265 005f 7979  OShdlCompare._yy
+0003fe60: 7950 6163 6b65 7453 6875 7464 6f77 6e00  yPacketShutdown.
+0003fe70: 5f79 7979 5365 6e64 5061 636b 6574 005f  _yyySendPacket._
+0003fe80: 7979 7953 6574 7570 005f 7979 7953 6967  yyySetup._yyySig
+0003fe90: 6e61 6c4f 7574 506b 7400 5f79 7979 5553  nalOutPkt._yyyUS
+0003fea0: 4247 6574 496e 7465 7266 6163 6573 005f  BGetInterfaces._
+0003feb0: 7979 7955 5342 5f69 6e69 7400 5f79 7979  yyyUSB_init._yyy
+0003fec0: 5553 425f 7374 6f70 005f 4346 4469 6374  USB_stop._CFDict
+0003fed0: 696f 6e61 7279 4372 6561 7465 4d75 7461  ionaryCreateMuta
+0003fee0: 626c 6500 5f43 4644 6963 7469 6f6e 6172  ble._CFDictionar
+0003fef0: 7953 6574 5661 6c75 6500 5f43 4647 6574  ySetValue._CFGet
+0003ff00: 5479 7065 4944 005f 4346 4e75 6d62 6572  TypeID._CFNumber
+0003ff10: 4372 6561 7465 005f 4346 4e75 6d62 6572  Create._CFNumber
+0003ff20: 4765 7454 7970 6549 4400 5f43 464e 756d  GetTypeID._CFNum
+0003ff30: 6265 7247 6574 5661 6c75 6500 5f43 4652  berGetValue._CFR
+0003ff40: 656c 6561 7365 005f 4346 5275 6e4c 6f6f  elease._CFRunLoo
+0003ff50: 7047 6574 4375 7272 656e 7400 5f43 4652  pGetCurrent._CFR
+0003ff60: 756e 4c6f 6f70 5275 6e49 6e4d 6f64 6500  unLoopRunInMode.
+0003ff70: 5f43 4652 756e 4c6f 6f70 5374 6f70 005f  _CFRunLoopStop._
+0003ff80: 4346 5365 7447 6574 436f 756e 7400 5f43  CFSetGetCount._C
+0003ff90: 4653 6574 4765 7456 616c 7565 7300 5f43  FSetGetValues._C
+0003ffa0: 4653 7472 696e 6743 7265 6174 6557 6974  FStringCreateWit
+0003ffb0: 6843 5374 7269 6e67 005f 4346 5374 7269  hCString._CFStri
+0003ffc0: 6e67 4765 7443 5374 7269 6e67 005f 4346  ngGetCString._CF
+0003ffd0: 5374 7269 6e67 4765 7443 5374 7269 6e67  StringGetCString
+0003ffe0: 5074 7200 5f43 4653 7472 696e 6747 6574  Ptr._CFStringGet
+0003fff0: 4c65 6e67 7468 005f 4346 5374 7269 6e67  Length._CFString
+00040000: 4765 7453 7973 7465 6d45 6e63 6f64 696e  GetSystemEncodin
+00040010: 6700 5f43 4653 7472 696e 6747 6574 5479  g._CFStringGetTy
+00040020: 7065 4944 005f 494f 4849 4444 6576 6963  peID._IOHIDDevic
+00040030: 6543 6c6f 7365 005f 494f 4849 4444 6576  eClose._IOHIDDev
+00040040: 6963 6547 6574 5072 6f70 6572 7479 005f  iceGetProperty._
+00040050: 494f 4849 4444 6576 6963 654f 7065 6e00  IOHIDDeviceOpen.
+00040060: 5f49 4f48 4944 4465 7669 6365 5265 6769  _IOHIDDeviceRegi
+00040070: 7374 6572 496e 7075 7452 6570 6f72 7443  sterInputReportC
+00040080: 616c 6c62 6163 6b00 5f49 4f48 4944 4465  allback._IOHIDDe
+00040090: 7669 6365 5363 6865 6475 6c65 5769 7468  viceScheduleWith
+000400a0: 5275 6e4c 6f6f 7000 5f49 4f48 4944 4465  RunLoop._IOHIDDe
+000400b0: 7669 6365 5365 7452 6570 6f72 7400 5f49  viceSetReport._I
+000400c0: 4f48 4944 4d61 6e61 6765 7243 6c6f 7365  OHIDManagerClose
+000400d0: 005f 494f 4849 444d 616e 6167 6572 436f  ._IOHIDManagerCo
+000400e0: 7079 4465 7669 6365 7300 5f49 4f48 4944  pyDevices._IOHID
+000400f0: 4d61 6e61 6765 7243 7265 6174 6500 5f49  ManagerCreate._I
+00040100: 4f48 4944 4d61 6e61 6765 7247 6574 5479  OHIDManagerGetTy
+00040110: 7065 4944 005f 494f 4849 444d 616e 6167  peID._IOHIDManag
+00040120: 6572 4f70 656e 005f 494f 4849 444d 616e  erOpen._IOHIDMan
+00040130: 6167 6572 5363 6865 6475 6c65 5769 7468  agerScheduleWith
+00040140: 5275 6e4c 6f6f 7000 5f49 4f48 4944 4d61  RunLoop._IOHIDMa
+00040150: 6e61 6765 7253 6574 4465 7669 6365 4d61  nagerSetDeviceMa
+00040160: 7463 6869 6e67 005f 5f44 6566 6175 6c74  tching.__Default
+00040170: 5275 6e65 4c6f 6361 6c65 005f 5f5f 4346  RuneLocale.___CF
+00040180: 436f 6e73 7461 6e74 5374 7269 6e67 436c  ConstantStringCl
+00040190: 6173 7352 6566 6572 656e 6365 005f 5f5f  assReference.___
+000401a0: 5f63 686b 7374 6b5f 6461 7277 696e 005f  _chkstk_darwin._
+000401b0: 5f5f 627a 6572 6f00 5f5f 5f64 6172 7769  __bzero.___darwi
+000401c0: 6e5f 6368 6563 6b5f 6664 5f73 6574 5f6f  n_check_fd_set_o
+000401d0: 7665 7266 6c6f 7700 5f5f 5f65 7272 6f72  verflow.___error
+000401e0: 005f 5f5f 6d65 6d63 7079 5f63 686b 005f  .___memcpy_chk._
+000401f0: 5f5f 7370 7269 6e74 665f 6368 6b00 5f5f  __sprintf_chk.__
+00040200: 5f73 7461 636b 5f63 686b 5f66 6169 6c00  _stack_chk_fail.
+00040210: 5f5f 5f73 7461 636b 5f63 686b 5f67 7561  ___stack_chk_gua
+00040220: 7264 005f 6174 6f66 005f 6174 6f69 005f  rd._atof._atoi._
+00040230: 6269 6e64 005f 6361 6c6c 6f63 005f 636c  bind._calloc._cl
+00040240: 6f73 6500 5f63 6c6f 7365 6469 7200 5f63  ose._closedir._c
+00040250: 6f6e 6e65 6374 005f 6663 6c6f 7365 005f  onnect._fclose._
+00040260: 6663 6e74 6c00 5f66 6f70 656e 005f 6670  fcntl._fopen._fp
+00040270: 7269 6e74 6600 5f66 7265 6164 005f 6672  rintf._fread._fr
+00040280: 6565 005f 6672 6565 6164 6472 696e 666f  ee._freeaddrinfo
+00040290: 005f 6673 6565 6b00 5f66 7465 6c6c 005f  ._fseek._ftell._
+000402a0: 6677 7269 7465 005f 6765 7461 6464 7269  fwrite._getaddri
+000402b0: 6e66 6f00 5f67 6574 6966 6164 6472 7300  nfo._getifaddrs.
+000402c0: 5f67 6574 7069 6400 5f67 6574 736f 636b  _getpid._getsock
+000402d0: 6e61 6d65 005f 6765 7473 6f63 6b6f 7074  name._getsockopt
+000402e0: 005f 6765 7474 696d 656f 6664 6179 005f  ._gettimeofday._
+000402f0: 696e 6574 5f61 6464 7200 5f6b 4346 416c  inet_addr._kCFAl
+00040300: 6c6f 6361 746f 7244 6566 6175 6c74 005f  locatorDefault._
+00040310: 6b43 4652 756e 4c6f 6f70 4465 6661 756c  kCFRunLoopDefaul
+00040320: 744d 6f64 6500 5f6b 4346 5479 7065 4469  tMode._kCFTypeDi
+00040330: 6374 696f 6e61 7279 4b65 7943 616c 6c42  ctionaryKeyCallB
+00040340: 6163 6b73 005f 6b43 4654 7970 6544 6963  acks._kCFTypeDic
+00040350: 7469 6f6e 6172 7956 616c 7565 4361 6c6c  tionaryValueCall
+00040360: 4261 636b 7300 5f6d 616c 6c6f 6300 5f6d  Backs._malloc._m
+00040370: 656d 636d 7000 5f6d 656d 6370 7900 5f6d  emcmp._memcpy._m
+00040380: 656d 7365 7400 5f6d 6b66 6966 6f00 5f6f  emset._mkfifo._o
+00040390: 7065 6e00 5f6f 7065 6e64 6972 2449 4e4f  pen._opendir$INO
+000403a0: 4445 3634 005f 7074 6872 6561 645f 6174  DE64._pthread_at
+000403b0: 7472 5f64 6573 7472 6f79 005f 7074 6872  tr_destroy._pthr
+000403c0: 6561 645f 6174 7472 5f69 6e69 7400 5f70  ead_attr_init._p
+000403d0: 7468 7265 6164 5f61 7474 725f 7365 7464  thread_attr_setd
+000403e0: 6574 6163 6873 7461 7465 005f 7074 6872  etachstate._pthr
+000403f0: 6561 645f 6361 6e63 656c 005f 7074 6872  ead_cancel._pthr
+00040400: 6561 645f 636f 6e64 5f64 6573 7472 6f79  ead_cond_destroy
+00040410: 005f 7074 6872 6561 645f 636f 6e64 5f69  ._pthread_cond_i
+00040420: 6e69 7400 5f70 7468 7265 6164 5f63 6f6e  nit._pthread_con
+00040430: 645f 7369 676e 616c 005f 7074 6872 6561  d_signal._pthrea
+00040440: 645f 636f 6e64 5f74 696d 6564 7761 6974  d_cond_timedwait
+00040450: 005f 7074 6872 6561 645f 636f 6e64 5f77  ._pthread_cond_w
+00040460: 6169 7400 5f70 7468 7265 6164 5f63 7265  ait._pthread_cre
+00040470: 6174 6500 5f70 7468 7265 6164 5f67 6574  ate._pthread_get
+00040480: 7370 6563 6966 6963 005f 7074 6872 6561  specific._pthrea
+00040490: 645f 6a6f 696e 005f 7074 6872 6561 645f  d_join._pthread_
+000404a0: 6b65 795f 6372 6561 7465 005f 7074 6872  key_create._pthr
+000404b0: 6561 645f 6d75 7465 785f 6465 7374 726f  ead_mutex_destro
+000404c0: 7900 5f70 7468 7265 6164 5f6d 7574 6578  y._pthread_mutex
+000404d0: 5f69 6e69 7400 5f70 7468 7265 6164 5f6d  _init._pthread_m
+000404e0: 7574 6578 5f6c 6f63 6b00 5f70 7468 7265  utex_lock._pthre
+000404f0: 6164 5f6d 7574 6578 5f74 7279 6c6f 636b  ad_mutex_trylock
+00040500: 005f 7074 6872 6561 645f 6d75 7465 785f  ._pthread_mutex_
+00040510: 756e 6c6f 636b 005f 7074 6872 6561 645f  unlock._pthread_
+00040520: 6d75 7465 7861 7474 725f 696e 6974 005f  mutexattr_init._
+00040530: 7074 6872 6561 645f 6d75 7465 7861 7474  pthread_mutexatt
+00040540: 725f 7365 7474 7970 6500 5f70 7468 7265  r_settype._pthre
+00040550: 6164 5f6f 6e63 6500 5f70 7468 7265 6164  ad_once._pthread
+00040560: 5f73 6574 7370 6563 6966 6963 005f 7261  _setspecific._ra
+00040570: 6e64 005f 7265 6164 005f 7265 6164 6469  nd._read._readdi
+00040580: 7224 494e 4f44 4536 3400 5f72 6563 7600  r$INODE64._recv.
+00040590: 5f73 656c 6563 7424 3130 3530 005f 7365  _select$1050._se
+000405a0: 6e64 005f 7365 6e64 746f 005f 7365 7473  nd._sendto._sets
+000405b0: 6f63 6b6f 7074 005f 736f 636b 6574 005f  ockopt._socket._
+000405c0: 7374 6174 2449 4e4f 4445 3634 005f 7374  stat$INODE64._st
+000405d0: 7263 6173 6563 6d70 005f 7374 7263 6872  rcasecmp._strchr
+000405e0: 005f 7374 7263 6d70 005f 7374 7263 7079  ._strcmp._strcpy
+000405f0: 005f 7374 7265 7272 6f72 005f 7374 726c  ._strerror._strl
+00040600: 656e 005f 7374 726e 6361 7365 636d 7000  en._strncasecmp.
+00040610: 5f73 7472 6e63 6d70 005f 7374 7273 7472  _strncmp._strstr
+00040620: 005f 7379 7363 746c 6279 6e61 6d65 005f  ._sysctlbyname._
+00040630: 7469 6d65 005f 7573 6c65 6570 005f 7673  time._usleep._vs
+00040640: 6e70 7269 6e74 6600 5f77 7269 7465 005f  nprintf._write._
+00040650: 7954 6370 4f70 656e 005f 7954 6370 5772  yTcpOpen._yTcpWr
+00040660: 6974 6500 5f79 5463 7052 6561 6400 5f79  ite._yTcpRead._y
+00040670: 4854 5450 4f70 656e 5265 7145 7800 5f79  HTTPOpenReqEx._y
+00040680: 4854 5450 4d75 6c74 6953 656c 6563 7452  HTTPMultiSelectR
+00040690: 6571 005f 7954 6370 4368 6563 6b52 6571  eq._yTcpCheckReq
+000406a0: 5469 6d65 6f75 7400 5f79 4854 5450 436c  Timeout._yHTTPCl
+000406b0: 6f73 6552 6571 4578 005f 7957 5343 6c6f  oseReqEx._yWSClo
+000406c0: 7365 5265 7100 5f79 5753 5265 6d6f 7665  seReq._yWSRemove
+000406d0: 5265 7100 5f63 6c6f 7365 416c 6c52 6571  Req._closeAllReq
+000406e0: 005f 7953 5344 505f 7468 7265 6164 005f  ._ySSDP_thread._
+000406f0: 7265 736f 6c76 6544 4e53 4361 6368 6500  resolveDNSCache.
+00040700: 5f42 6173 6536 3445 6e63 6f64 6500 5f77  _Base64Encode._w
+00040710: 735f 6170 7065 6e64 5443 5044 6174 6100  s_appendTCPData.
+00040720: 5f77 735f 7365 6e64 4672 616d 6500 5f79  _ws_sendFrame._y
+00040730: 5353 4450 5f70 6172 7365 5353 5044 4d65  SSDP_parseSSPDMe
+00040740: 7373 6167 6500 5f79 7055 7064 6174 6555  ssage._ypUpdateU
+00040750: 5342 005f 7950 6b74 5175 6575 6550 7573  SB._yPktQueuePus
+00040760: 6845 7800 5f79 506b 7451 7565 7565 506f  hEx._yPktQueuePo
+00040770: 7000 5f65 6e75 5570 6461 7465 4453 7461  p._enuUpdateDSta
+00040780: 7475 7300 5f79 4469 7370 6174 6368 5265  tus._yDispatchRe
+00040790: 6365 6976 6500 5f79 5374 7265 616d 5472  ceive._yStreamTr
+000407a0: 616e 736d 6974 005f 7953 7472 6561 6d46  ansmit._yStreamF
+000407b0: 6c75 7368 005f 6465 7652 6570 6f72 7445  lush._devReportE
+000407c0: 7272 6f72 005f 6465 7653 746f 7049 4f00  rror._devStopIO.
+000407d0: 5f64 6576 5061 7573 6549 4f00 5f64 6576  _devPauseIO._dev
+000407e0: 4368 6563 6b49 4f00 5f64 6576 5374 6172  CheckIO._devStar
+000407f0: 7445 6e75 6d00 5f53 7461 7274 4465 7669  tEnum._StartDevi
+00040800: 6365 005f 7953 7472 6561 6d53 6875 7464  ce._yStreamShutd
+00040810: 6f77 6e00 5f79 7957 6169 744f 6e6c 7943  own._yyWaitOnlyC
+00040820: 6f6e 6650 6b74 005f 7953 7472 6561 6d52  onfPkt._yStreamR
+00040830: 6563 6569 7665 6400 5f79 4469 7370 6174  eceived._yDispat
+00040840: 6368 4e6f 7469 6365 005f 7950 726f 674c  chNotice._yProgL
+00040850: 6f67 5072 6f67 7265 7373 005f 7547 6574  ogProgress._uGet
+00040860: 4465 7669 6365 496e 666f 005f 7947 6574  DeviceInfo._yGet
+00040870: 4669 726d 7761 7265 005f 6973 5765 6250  Firmware._isWebP
+00040880: 6174 6800 5f79 6170 6943 6865 636b 4669  ath._yapiCheckFi
+00040890: 726d 7761 7265 5f72 005f 7953 7461 7274  rmware_r._yStart
+000408a0: 4669 726d 7761 7265 5570 6461 7465 005f  FirmwareUpdate._
+000408b0: 7961 7069 4368 6563 6b46 6972 6d77 6172  yapiCheckFirmwar
+000408c0: 6546 696c 6500 5f79 4c6f 6164 4669 726d  eFile._yLoadFirm
+000408d0: 7761 7265 4669 6c65 005f 7946 6972 6d77  wareFile._yFirmw
+000408e0: 6172 6555 7064 6174 655f 7468 7265 6164  areUpdate_thread
+000408f0: 005f 6f73 5072 6f67 4c6f 6750 726f 6772  ._osProgLogProgr
+00040900: 6573 7345 7800 5f73 656e 6448 7562 466c  essEx._sendHubFl
+00040910: 6173 6843 6d64 005f 7570 6c6f 6164 005f  ashCmd._upload._
+00040920: 6368 6563 6b48 5454 5048 6561 6465 7200  checkHTTPHeader.
+00040930: 5f69 6e69 7473 6861 7700 5f69 7465 7273  _initshaw._iters
+00040940: 6861 7700 5f4d 4435 5472 616e 7366 6f72  haw._MD5Transfor
+00040950: 6d00 5f79 426c 6b41 6c6c 6f63 005f 7948  m._yBlkAlloc._yH
+00040960: 6173 6850 7574 005f 7942 6c6b 4672 6565  ashPut._yBlkFree
+00040970: 005f 6576 656e 745f 7468 7265 6164 005f  ._event_thread._
+00040980: 7365 7475 7048 4944 4d61 6e61 6765 7200  setupHIDManager.
+00040990: 5f73 746f 7048 4944 4d61 6e61 6765 7200  _stopHIDManager.
+000409a0: 5f67 6574 4465 7652 6566 005f 6765 745f  _getDevRef._get_
+000409b0: 696e 745f 7072 6f70 6572 7479 005f 6765  int_property._ge
+000409c0: 745f 7478 745f 7072 6f70 6572 7479 005f  t_txt_property._
+000409d0: 4861 6e64 6c65 5f49 4f48 4944 4465 7669  Handle_IOHIDDevi
+000409e0: 6365 494f 4849 4452 6570 6f72 7443 616c  ceIOHIDReportCal
+000409f0: 6c62 6163 6b00 5f79 6170 6952 6571 7565  lback._yapiReque
+00040a00: 7374 4f70 656e 5553 4200 5f6c 6f67 5265  stOpenUSB._logRe
+00040a10: 7375 6c74 005f 7961 7069 5265 7175 6573  sult._yapiReques
+00040a20: 744f 7065 6e57 5300 5f79 6170 6952 6571  tOpenWS._yapiReq
+00040a30: 7565 7374 4f70 656e 4854 5450 005f 756e  uestOpenHTTP._un
+00040a40: 7265 6769 7374 6572 4e65 7444 6576 6963  registerNetDevic
+00040a50: 6500 5f75 6e70 6163 6b48 5454 5052 6571  e._unpackHTTPReq
+00040a60: 7565 7374 005f 7961 7069 5265 7175 6573  uest._yapiReques
+00040a70: 7443 6c6f 7365 005f 7961 7069 4a73 6f6e  tClose._yapiJson
+00040a80: 5661 6c75 6550 6172 7365 5374 7275 6374  ValueParseStruct
+00040a90: 005f 7961 7069 496e 6974 4150 495f 696e  ._yapiInitAPI_in
+00040aa0: 7465 726e 616c 005f 7961 7069 4672 6565  ternal._yapiFree
+00040ab0: 4150 495f 696e 7465 726e 616c 005f 7961  API_internal._ya
+00040ac0: 7069 556e 7265 6769 7374 6572 4875 625f  piUnregisterHub_
+00040ad0: 696e 7465 726e 616c 005f 7961 7069 5570  internal._yapiUp
+00040ae0: 6461 7465 4465 7669 6365 4c69 7374 5f69  dateDeviceList_i
+00040af0: 6e74 6572 6e61 6c00 5f79 6170 6948 616e  nternal._yapiHan
+00040b00: 646c 6545 7665 6e74 735f 696e 7465 726e  dleEvents_intern
+00040b10: 616c 005f 7961 7069 4765 7446 756e 6374  al._yapiGetFunct
+00040b20: 696f 6e49 6e66 6f45 785f 696e 7465 726e  ionInfoEx_intern
+00040b30: 616c 005f 7961 7069 4854 5450 5265 7175  al._yapiHTTPRequ
+00040b40: 6573 7441 7379 6e63 4578 5f69 6e74 6572  estAsyncEx_inter
+00040b50: 6e61 6c00 5f64 656c 6574 6541 6c6c 4353  nal._deleteAllCS
+00040b60: 005f 7373 6470 456e 7472 7955 7064 6174  ._ssdpEntryUpdat
+00040b70: 6500 5f75 6e72 6567 6973 7465 724e 6574  e._unregisterNet
+00040b80: 4875 6200 5f69 7353 616d 6548 7562 005f  Hub._isSameHub._
+00040b90: 7961 7069 4672 6565 4875 6200 5f79 4672  yapiFreeHub._yFr
+00040ba0: 6565 5061 7273 6564 5552 4c00 5f79 6170  eeParsedURL._yap
+00040bb0: 6941 6c6c 6f63 4875 6200 5f70 696e 6755  iAllocHub._pingU
+00040bc0: 524c 4f6e 6875 6200 5f79 5061 7273 6548  RLOnhub._yParseH
+00040bd0: 7562 5552 4c00 5f79 6170 6952 6567 6973  ubURL._yapiRegis
+00040be0: 7465 7248 7562 4578 005f 7968 656c 7065  terHubEx._yhelpe
+00040bf0: 725f 7468 7265 6164 005f 794e 6574 4875  r_thread._yNetHu
+00040c00: 6245 6e75 6d00 5f79 4e65 7448 7562 456e  bEnum._yNetHubEn
+00040c10: 756d 4578 005f 6469 7361 626c 655f 6a7a  umEx._disable_jz
+00040c20: 6f6e 005f 7061 7273 654e 6574 5770 456e  on._parseNetWpEn
+00040c30: 7472 7900 5f79 7055 7064 6174 654e 6574  try._ypUpdateNet
+00040c40: 005f 6173 796e 6344 726f 7000 5f79 4372  ._asyncDrop._yCr
+00040c50: 6561 7465 4465 7461 6368 6564 5468 7265  eateDetachedThre
+00040c60: 6164 4578 005f 696e 6974 5473 644b 6579  adEx._initTsdKey
+00040c70: 005f 6461 796f 6673 005f 7770 616b 005f  ._dayofs._wpak._
+00040c80: 6e65 7874 4361 7459 6478 005f 6e65 7874  nextCatYdx._next
+00040c90: 4861 7368 456e 7472 7900 5f79 496e 6974  HashEntry._yInit
+00040ca0: 4b65 794f 6e63 6500 5f79 4e65 7874 5468  KeyOnce._yNextTh
+00040cb0: 7265 6164 4964 7800 5f79 4861 7368 5461  readIdx._yHashTa
+00040cc0: 626c 6500 5f64 6576 5964 7850 7472 005f  ble._devYdxPtr._
+00040cd0: 6675 6e59 6478 5074 7200 5f6e 6578 7444  funYdxPtr._nextD
+00040ce0: 6576 5964 7800 5f75 7365 6444 6576 5964  evYdx._usedDevYd
+00040cf0: 7800 5f77 704c 6f63 6b43 6f75 6e74 005f  x._wpLockCount._
+00040d00: 7770 536f 6d65 7468 696e 6755 6e72 6567  wpSomethingUnreg
+00040d10: 6973 7465 7265 6400 5f79 5473 644b 6579  istered._yTsdKey
+00040d20: 002f 5573 6572 732f 796f 6374 6f2f 746d  ./Users/yocto/tm
+00040d30: 705f 6275 696c 642f 796f 6374 6f70 726f  p_build/yoctopro
+00040d40: 642f 796f 6374 6f6c 6962 2f76 312e 302f  d/yoctolib/v1.0/
+00040d50: 5075 626c 6963 2f63 7070 2f53 6f75 7263  Public/cpp/Sourc
+00040d60: 6573 2f79 6170 692f 0079 6d65 6d6f 7279  es/yapi/.ymemory
+00040d70: 2e63 002f 5573 6572 732f 796f 6374 6f2f  .c./Users/yocto/
+00040d80: 746d 705f 6275 696c 642f 796f 6374 6f70  tmp_build/yoctop
+00040d90: 726f 642f 796f 6374 6f6c 6962 2f76 312e  rod/yoctolib/v1.
+00040da0: 302f 5075 626c 6963 2f63 7070 2f42 696e  0/Public/cpp/Bin
+00040db0: 6172 6965 732f 7863 6f64 655f 6173 2f79  aries/xcode_as/y
+00040dc0: 6170 692f 6275 696c 642f 7961 7069 2e62  api/build/yapi.b
+00040dd0: 7569 6c64 2f52 656c 6561 7365 2f79 6170  uild/Release/yap
+00040de0: 692e 6275 696c 642f 4f62 6a65 6374 732d  i.build/Objects-
+00040df0: 6e6f 726d 616c 2f78 3836 5f36 342f 796d  normal/x86_64/ym
+00040e00: 656d 6f72 792e 6f00 5f79 7374 7263 7079  emory.o._ystrcpy
+00040e10: 5f73 005f 7973 7472 6e63 7079 5f73 005f  _s._ystrncpy_s._
+00040e20: 7973 7472 6475 705f 7300 5f79 7374 726e  ystrdup_s._ystrn
+00040e30: 6475 705f 7300 5f79 7374 7263 6174 5f73  dup_s._ystrcat_s
+00040e40: 005f 7973 7472 6e63 6174 5f73 005f 7973  ._ystrncat_s._ys
+00040e50: 7072 696e 7466 5f73 005f 7976 7370 7269  printf_s._yvspri
+00040e60: 6e74 665f 7300 5f79 6d65 6d66 696e 6400  ntf_s._ymemfind.
+00040e70: 7974 6370 2e63 002f 5573 6572 732f 796f  ytcp.c./Users/yo
+00040e80: 6374 6f2f 746d 705f 6275 696c 642f 796f  cto/tmp_build/yo
+00040e90: 6374 6f70 726f 642f 796f 6374 6f6c 6962  ctoprod/yoctolib
+00040ea0: 2f76 312e 302f 5075 626c 6963 2f63 7070  /v1.0/Public/cpp
+00040eb0: 2f42 696e 6172 6965 732f 7863 6f64 655f  /Binaries/xcode_
+00040ec0: 6173 2f79 6170 692f 6275 696c 642f 7961  as/yapi/build/ya
+00040ed0: 7069 2e62 7569 6c64 2f52 656c 6561 7365  pi.build/Release
+00040ee0: 2f79 6170 692e 6275 696c 642f 4f62 6a65  /yapi.build/Obje
+00040ef0: 6374 732d 6e6f 726d 616c 2f78 3836 5f36  cts-normal/x86_6
+00040f00: 342f 7974 6370 2e6f 005f 7944 7570 5365  4/ytcp.o._yDupSe
+00040f10: 7400 5f79 4e65 7453 6574 4572 7245 7800  t._yNetSetErrEx.
+00040f20: 5f79 496e 6974 5761 6b65 5570 536f 636b  _yInitWakeUpSock
+00040f30: 6574 005f 7953 7461 7274 5761 6b65 5570  et._yStartWakeUp
+00040f40: 536f 636b 6574 005f 7944 7269 6e67 5761  Socket._yDringWa
+00040f50: 6b65 5570 536f 636b 6574 005f 7943 6f6e  keUpSocket._yCon
+00040f60: 7375 6d65 5761 6b65 5570 536f 636b 6574  sumeWakeUpSocket
+00040f70: 005f 7946 7265 6557 616b 6555 7053 6f63  ._yFreeWakeUpSoc
+00040f80: 6b65 7400 5f79 5265 736f 6c76 6544 4e53  ket._yResolveDNS
+00040f90: 005f 7954 6370 496e 6974 005f 7954 6370  ._yTcpInit._yTcp
+00040fa0: 5368 7574 646f 776e 005f 6465 636f 6465  Shutdown._decode
+00040fb0: 4865 7800 5f79 5463 7044 6f77 6e6c 6f61  Hex._yTcpDownloa
+00040fc0: 6400 5f79 5463 704f 7065 6e00 5f79 5463  d._yTcpOpen._yTc
+00040fd0: 7057 7269 7465 005f 7954 6370 5265 6164  pWrite._yTcpRead
+00040fe0: 005f 7952 6571 416c 6c6f 6300 5f79 5265  ._yReqAlloc._yRe
+00040ff0: 714f 7065 6e00 5f79 4854 5450 4f70 656e  qOpen._yHTTPOpen
+00041000: 5265 7145 7800 5f79 5265 7153 656c 6563  ReqEx._yReqSelec
+00041010: 7400 5f79 4854 5450 4d75 6c74 6953 656c  t._yHTTPMultiSel
+00041020: 6563 7452 6571 005f 7952 6571 4d75 6c74  ectReq._yReqMult
+00041030: 6953 656c 6563 7400 5f79 5265 7149 7345  iSelect._yReqIsE
+00041040: 6f66 005f 7954 6370 4368 6563 6b52 6571  of._yTcpCheckReq
+00041050: 5469 6d65 6f75 7400 5f79 5265 7147 6574  Timeout._yReqGet
+00041060: 005f 7952 6571 5265 6164 005f 7952 6571  ._yReqRead._yReq
+00041070: 436c 6f73 6500 5f79 4854 5450 436c 6f73  Close._yHTTPClos
+00041080: 6552 6571 4578 005f 7957 5343 6c6f 7365  eReqEx._yWSClose
+00041090: 5265 7100 5f79 5753 5265 6d6f 7665 5265  Req._yWSRemoveRe
+000410a0: 7100 5f79 5265 7149 7341 7379 6e63 005f  q._yReqIsAsync._
+000410b0: 7952 6571 4672 6565 005f 7952 6571 4861  yReqFree._yReqHa
+000410c0: 7350 656e 6469 6e67 005f 7773 5f63 6c65  sPending._ws_cle
+000410d0: 616e 7570 005f 7773 5f74 6872 6561 6400  anup._ws_thread.
+000410e0: 5f63 6c6f 7365 416c 6c52 6571 005f 7953  _closeAllReq._yS
+000410f0: 5344 5044 6973 636f 7665 7200 5f79 5353  SDPDiscover._ySS
+00041100: 4450 5374 6172 7400 5f79 5353 4450 5f74  DPStart._ySSDP_t
+00041110: 6872 6561 6400 5f79 5353 4450 5374 6f70  hread._ySSDPStop
+00041120: 005f 7265 736f 6c76 6544 4e53 4361 6368  ._resolveDNSCach
+00041130: 6500 5f42 6173 6536 3445 6e63 6f64 6500  e._Base64Encode.
+00041140: 5f77 735f 6170 7065 6e64 5443 5044 6174  _ws_appendTCPDat
+00041150: 6100 5f77 735f 7365 6e64 4672 616d 6500  a._ws_sendFrame.
+00041160: 5f79 5353 4450 5f70 6172 7365 5353 5044  _ySSDP_parseSSPD
+00041170: 4d65 7373 6167 6500 5f64 6e73 4361 6368  Message._dnsCach
+00041180: 6500 5f6e 6244 6574 6563 7465 6449 6661  e._nbDetectedIfa
+00041190: 6365 7300 5f64 6574 6563 7465 6449 6661  ces._detectedIfa
+000411a0: 6365 7300 7973 7472 6561 6d2e 6300 2f55  ces.ystream.c./U
+000411b0: 7365 7273 2f79 6f63 746f 2f74 6d70 5f62  sers/yocto/tmp_b
+000411c0: 7569 6c64 2f79 6f63 746f 7072 6f64 2f79  uild/yoctoprod/y
+000411d0: 6f63 746f 6c69 622f 7631 2e30 2f50 7562  octolib/v1.0/Pub
+000411e0: 6c69 632f 6370 702f 4269 6e61 7269 6573  lic/cpp/Binaries
+000411f0: 2f78 636f 6465 5f61 732f 7961 7069 2f62  /xcode_as/yapi/b
+00041200: 7569 6c64 2f79 6170 692e 6275 696c 642f  uild/yapi.build/
+00041210: 5265 6c65 6173 652f 7961 7069 2e62 7569  Release/yapi.bui
+00041220: 6c64 2f4f 626a 6563 7473 2d6e 6f72 6d61  ld/Objects-norma
+00041230: 6c2f 7838 365f 3634 2f79 7374 7265 616d  l/x86_64/ystream
+00041240: 2e6f 005f 7953 6574 4572 7200 5f46 7573  .o._ySetErr._Fus
+00041250: 696f 6e45 7272 6d73 6700 5f59 464f 5045  ionErrmsg._YFOPE
+00041260: 4e00 5f76 6462 676c 6f67 6600 5f64 6267  N._vdbglogf._dbg
+00041270: 6c6f 6766 005f 7970 5570 6461 7465 5443  logf._ypUpdateTC
+00041280: 5000 5f79 7055 7064 6174 6555 5342 005f  P._ypUpdateUSB._
+00041290: 7970 5570 6461 7465 5964 7800 5f79 506b  ypUpdateYdx._yPk
+000412a0: 7451 7565 7565 496e 6974 005f 7950 6b74  tQueueInit._yPkt
+000412b0: 5175 6575 6546 7265 6500 5f79 506b 7451  QueueFree._yPktQ
+000412c0: 7565 7565 5365 7445 7272 6f72 005f 7950  ueueSetError._yP
+000412d0: 6b74 5175 6575 6550 7573 6844 3248 005f  ktQueuePushD2H._
+000412e0: 7950 6b74 5175 6575 6550 7573 6845 7800  yPktQueuePushEx.
+000412f0: 5f79 506b 7451 7565 7565 5761 6974 416e  _yPktQueueWaitAn
+00041300: 6450 6f70 4432 4800 5f79 506b 7451 7565  dPopD2H._yPktQue
+00041310: 7565 506f 7000 5f79 506b 7451 7565 7565  uePop._yPktQueue
+00041320: 5075 7368 4832 4400 5f79 506b 7451 7565  PushH2D._yPktQue
+00041330: 7565 5065 656b 4832 4400 5f79 506b 7451  uePeekH2D._yPktQ
+00041340: 7565 7565 506f 7048 3244 005f 7979 7953  ueuePopH2D._yyyS
+00041350: 656e 6450 6163 6b65 7400 5f79 5553 4252  endPacket._yUSBR
+00041360: 656c 6561 7365 416c 6c44 6576 6963 6573  eleaseAllDevices
+00041370: 005f 656e 7555 7064 6174 6544 5374 6174  ._enuUpdateDStat
+00041380: 7573 005f 7955 5342 5570 6461 7465 4465  us._yUSBUpdateDe
+00041390: 7669 6365 4c69 7374 005f 6669 6e64 4465  viceList._findDe
+000413a0: 7600 5f66 696e 6444 6576 4864 6c46 726f  v._findDevHdlFro
+000413b0: 6d53 7472 005f 6669 6e64 4465 7646 726f  mStr._findDevFro
+000413c0: 6d49 4f48 646c 005f 6465 7648 646c 496e  mIOHdl._devHdlIn
+000413d0: 666f 005f 6475 6d70 5950 6572 6645 6e74  fo._dumpYPerfEnt
+000413e0: 7279 005f 7955 7362 496e 6974 005f 7955  ry._yUsbInit._yU
+000413f0: 7362 4672 6565 005f 7955 7362 4964 6c65  sbFree._yUsbIdle
+00041400: 005f 7944 6973 7061 7463 6852 6563 6569  ._yDispatchRecei
+00041410: 7665 005f 7953 7472 6561 6d54 7261 6e73  ve._yStreamTrans
+00041420: 6d69 7400 5f79 5374 7265 616d 466c 7573  mit._yStreamFlus
+00041430: 6800 5f64 6576 5265 706f 7274 4572 726f  h._devReportErro
+00041440: 7200 5f64 6576 5374 6f70 494f 005f 6465  r._devStopIO._de
+00041450: 7650 6175 7365 494f 005f 7955 7362 5472  vPauseIO._yUsbTr
+00041460: 6166 6669 6350 656e 6469 6e67 005f 7955  afficPending._yU
+00041470: 7362 4f70 656e 4465 7644 6573 6372 005f  sbOpenDevDescr._
+00041480: 7955 7362 4f70 656e 005f 7955 7362 5365  yUsbOpen._yUsbSe
+00041490: 7449 4f41 7379 6e63 005f 6465 7643 6865  tIOAsync._devChe
+000414a0: 636b 494f 005f 7955 7362 5772 6974 6500  ckIO._yUsbWrite.
+000414b0: 5f79 5573 6252 6561 644e 6f6e 426c 6f63  _yUsbReadNonBloc
+000414c0: 6b00 5f79 5573 6252 6561 6442 6c6f 636b  k._yUsbReadBlock
+000414d0: 005f 7955 7362 454f 4600 5f79 5573 6243  ._yUsbEOF._yUsbC
+000414e0: 6c6f 7365 005f 6465 7653 7461 7274 456e  lose._devStartEn
+000414f0: 756d 005f 5374 6172 7444 6576 6963 6500  um._StartDevice.
+00041500: 5f79 5374 7265 616d 5368 7574 646f 776e  _yStreamShutdown
+00041510: 005f 7979 5761 6974 4f6e 6c79 436f 6e66  ._yyWaitOnlyConf
+00041520: 506b 7400 5f79 5374 7265 616d 5265 6365  Pkt._yStreamRece
+00041530: 6976 6564 005f 7944 6973 7061 7463 684e  ived._yDispatchN
+00041540: 6f74 6963 6500 5f64 6179 6f66 7300 5f79  otice._dayofs._y
+00041550: 436f 6e74 6578 7400 5f79 7472 6163 6566  Context._ytracef
+00041560: 696c 6500 7970 726f 672e 6300 2f55 7365  ile.yprog.c./Use
+00041570: 7273 2f79 6f63 746f 2f74 6d70 5f62 7569  rs/yocto/tmp_bui
+00041580: 6c64 2f79 6f63 746f 7072 6f64 2f79 6f63  ld/yoctoprod/yoc
+00041590: 746f 6c69 622f 7631 2e30 2f50 7562 6c69  tolib/v1.0/Publi
+000415a0: 632f 6370 702f 4269 6e61 7269 6573 2f78  c/cpp/Binaries/x
+000415b0: 636f 6465 5f61 732f 7961 7069 2f62 7569  code_as/yapi/bui
+000415c0: 6c64 2f79 6170 692e 6275 696c 642f 5265  ld/yapi.build/Re
+000415d0: 6c65 6173 652f 7961 7069 2e62 7569 6c64  lease/yapi.build
+000415e0: 2f4f 626a 6563 7473 2d6e 6f72 6d61 6c2f  /Objects-normal/
+000415f0: 7838 365f 3634 2f79 7072 6f67 2e6f 005f  x86_64/yprog.o._
+00041600: 7950 726f 6749 6e69 7400 5f79 5072 6f67  yProgInit._yProg
+00041610: 4672 6565 005f 7072 6f67 5f47 6574 4350  Free._prog_GetCP
+00041620: 554e 616d 6500 5f49 7356 616c 6964 4279  UName._IsValidBy
+00041630: 6e48 6561 6400 5f56 616c 6964 6174 6542  nHead._ValidateB
+00041640: 796e 436f 6d70 6174 005f 4973 5661 6c69  ynCompat._IsVali
+00041650: 6442 796e 4669 6c65 005f 7970 4973 5365  dBynFile._ypIsSe
+00041660: 6e64 426f 6f74 6c6f 6164 6572 4275 7379  ndBootloaderBusy
+00041670: 005f 7970 5365 6e64 426f 6f74 6c6f 6164  ._ypSendBootload
+00041680: 6572 436d 6400 5f79 7047 6574 426f 6f74  erCmd._ypGetBoot
+00041690: 6c6f 6164 6572 5265 706c 7900 5f42 6c6f  loaderReply._Blo
+000416a0: 636b 696e 6752 6561 6400 5f53 656e 6444  ckingRead._SendD
+000416b0: 6174 6150 6163 6b65 7400 5f79 5553 4247  ataPacket._yUSBG
+000416c0: 6574 426f 6f6c 6f61 6465 7200 5f75 466c  etBooloader._uFl
+000416d0: 6173 6844 6576 6963 6500 5f79 5072 6f67  ashDevice._yProg
+000416e0: 4c6f 6750 726f 6772 6573 7300 5f75 4765  LogProgress._uGe
+000416f0: 7444 6576 6963 6549 6e66 6f00 5f79 4765  tDeviceInfo._yGe
+00041700: 7446 6972 6d77 6172 6500 5f79 4e65 7448  tFirmware._yNetH
+00041710: 7562 4765 7442 6f6f 746c 6f61 6465 7273  ubGetBootloaders
+00041720: 005f 7961 7069 4368 6563 6b46 6972 6d77  ._yapiCheckFirmw
+00041730: 6172 655f 696e 7465 726e 616c 005f 6973  are_internal._is
+00041740: 5765 6250 6174 6800 5f79 6170 6943 6865  WebPath._yapiChe
+00041750: 636b 4669 726d 7761 7265 5f72 005f 7961  ckFirmware_r._ya
+00041760: 7069 5570 6461 7465 4669 726d 7761 7265  piUpdateFirmware
+00041770: 5f69 6e74 6572 6e61 6c00 5f79 5374 6172  _internal._yStar
+00041780: 7446 6972 6d77 6172 6555 7064 6174 6500  tFirmwareUpdate.
+00041790: 5f79 6170 6943 6865 636b 4669 726d 7761  _yapiCheckFirmwa
+000417a0: 7265 4669 6c65 005f 794c 6f61 6446 6972  reFile._yLoadFir
+000417b0: 6d77 6172 6546 696c 6500 5f79 4669 726d  mwareFile._yFirm
+000417c0: 7761 7265 5570 6461 7465 5f74 6872 6561  wareUpdate_threa
+000417d0: 6400 5f6f 7350 726f 674c 6f67 5072 6f67  d._osProgLogProg
+000417e0: 7265 7373 4578 005f 7365 6e64 4875 6246  ressEx._sendHubF
+000417f0: 6c61 7368 436d 6400 5f75 706c 6f61 6400  lashCmd._upload.
+00041800: 5f63 6865 636b 4854 5450 4865 6164 6572  _checkHTTPHeader
+00041810: 005f 6663 7478 005f 6669 726d 5f64 6576  ._fctx._firm_dev
+00041820: 005f 6669 726d 5f70 6b74 0079 6a73 6f6e  ._firm_pkt.yjson
+00041830: 2e63 002f 5573 6572 732f 796f 6374 6f2f  .c./Users/yocto/
+00041840: 746d 705f 6275 696c 642f 796f 6374 6f70  tmp_build/yoctop
+00041850: 726f 642f 796f 6374 6f6c 6962 2f76 312e  rod/yoctolib/v1.
+00041860: 302f 5075 626c 6963 2f63 7070 2f42 696e  0/Public/cpp/Bin
+00041870: 6172 6965 732f 7863 6f64 655f 6173 2f79  aries/xcode_as/y
+00041880: 6170 692f 6275 696c 642f 7961 7069 2e62  api/build/yapi.b
+00041890: 7569 6c64 2f52 656c 6561 7365 2f79 6170  uild/Release/yap
+000418a0: 692e 6275 696c 642f 4f62 6a65 6374 732d  i.build/Objects-
+000418b0: 6e6f 726d 616c 2f78 3836 5f36 342f 796a  normal/x86_64/yj
+000418c0: 736f 6e2e 6f00 5f79 4a73 6f6e 5061 7273  son.o._yJsonPars
+000418d0: 6500 5f79 4a73 6f6e 536b 6970 0079 6b65  e._yJsonSkip.yke
+000418e0: 792e 6300 2f55 7365 7273 2f79 6f63 746f  y.c./Users/yocto
+000418f0: 2f74 6d70 5f62 7569 6c64 2f79 6f63 746f  /tmp_build/yocto
+00041900: 7072 6f64 2f79 6f63 746f 6c69 622f 7631  prod/yoctolib/v1
+00041910: 2e30 2f50 7562 6c69 632f 6370 702f 4269  .0/Public/cpp/Bi
+00041920: 6e61 7269 6573 2f78 636f 6465 5f61 732f  naries/xcode_as/
+00041930: 7961 7069 2f62 7569 6c64 2f79 6170 692e  yapi/build/yapi.
+00041940: 6275 696c 642f 5265 6c65 6173 652f 7961  build/Release/ya
+00041950: 7069 2e62 7569 6c64 2f4f 626a 6563 7473  pi.build/Objects
+00041960: 2d6e 6f72 6d61 6c2f 7838 365f 3634 2f79  -normal/x86_64/y
+00041970: 6b65 792e 6f00 5f62 696e 3273 7472 005f  key.o._bin2str._
+00041980: 436f 6d70 7574 6541 7574 6848 4131 005f  ComputeAuthHA1._
+00041990: 4d44 3549 6e69 7469 616c 697a 6500 5f4d  MD5Initialize._M
+000419a0: 4435 4164 6444 6174 6100 5f4d 4435 4361  D5AddData._MD5Ca
+000419b0: 6c63 756c 6174 6500 5f43 6f6d 7075 7465  lculate._Compute
+000419c0: 4175 7468 4841 3200 5f43 6f6d 7075 7465  AuthHA2._Compute
+000419d0: 4175 7468 5265 7370 6f6e 7365 005f 4368  AuthResponse._Ch
+000419e0: 6563 6b57 5341 7574 6800 5f79 5348 4131  eckWSAuth._ySHA1
+000419f0: 005f 7950 6172 7365 5757 5741 7574 6865  ._yParseWWWAuthe
+00041a00: 6e74 6963 6174 6500 5f79 4469 6765 7374  nticate._yDigest
+00041a10: 4175 7468 6f72 697a 6174 696f 6e00 5f69  Authorization._i
+00041a20: 6e69 7473 6861 7700 5f69 7465 7273 6861  nitshaw._itersha
+00041a30: 7700 5f79 496e 6974 5073 6b00 5f79 4974  w._yInitPsk._yIt
+00041a40: 6572 5073 6b00 5f4d 4435 5472 616e 7366  erPsk._MD5Transf
+00041a50: 6f72 6d00 5f73 6861 315f 696e 6974 005f  orm._sha1_init._
+00041a60: 7770 616b 0079 6861 7368 2e63 002f 5573  wpak.yhash.c./Us
+00041a70: 6572 732f 796f 6374 6f2f 746d 705f 6275  ers/yocto/tmp_bu
+00041a80: 696c 642f 796f 6374 6f70 726f 642f 796f  ild/yoctoprod/yo
+00041a90: 6374 6f6c 6962 2f76 312e 302f 5075 626c  ctolib/v1.0/Publ
+00041aa0: 6963 2f63 7070 2f42 696e 6172 6965 732f  ic/cpp/Binaries/
+00041ab0: 7863 6f64 655f 6173 2f79 6170 692f 6275  xcode_as/yapi/bu
+00041ac0: 696c 642f 7961 7069 2e62 7569 6c64 2f52  ild/yapi.build/R
+00041ad0: 656c 6561 7365 2f79 6170 692e 6275 696c  elease/yapi.buil
+00041ae0: 642f 4f62 6a65 6374 732d 6e6f 726d 616c  d/Objects-normal
+00041af0: 2f78 3836 5f36 342f 7968 6173 682e 6f00  /x86_64/yhash.o.
+00041b00: 5f79 426c 6b4c 6973 744c 656e 6774 6800  _yBlkListLength.
+00041b10: 5f79 426c 6b4c 6973 7453 6565 6b00 5f79  _yBlkListSeek._y
+00041b20: 4861 7368 496e 6974 005f 7948 6173 6850  HashInit._yHashP
+00041b30: 7574 5374 7200 5f79 426c 6b41 6c6c 6f63  utStr._yBlkAlloc
+00041b40: 005f 7948 6173 6846 7265 6500 5f79 4861  ._yHashFree._yHa
+00041b50: 7368 5075 7442 7566 005f 7948 6173 6850  shPutBuf._yHashP
+00041b60: 7574 005f 7948 6173 6854 6573 7442 7566  ut._yHashTestBuf
+00041b70: 005f 7948 6173 6854 6573 7453 7472 005f  ._yHashTestStr._
+00041b80: 7948 6173 6847 6574 4275 6600 5f79 4861  yHashGetBuf._yHa
+00041b90: 7368 4765 7453 7472 005f 7948 6173 6847  shGetStr._yHashG
+00041ba0: 6574 5374 724c 656e 005f 7948 6173 6847  etStrLen._yHashG
+00041bb0: 6574 5374 7250 7472 005f 7770 5072 6576  etStrPtr._wpPrev
+00041bc0: 656e 7455 6e72 6567 6973 7465 7245 7800  entUnregisterEx.
+00041bd0: 5f77 7041 6c6c 6f77 556e 7265 6769 7374  _wpAllowUnregist
+00041be0: 6572 4578 005f 7770 5265 6769 7374 6572  erEx._wpRegister
+00041bf0: 005f 7770 4765 7441 7474 7269 6275 7465  ._wpGetAttribute
+00041c00: 005f 7770 4765 7453 6572 6961 6c00 5f77  ._wpGetSerial._w
+00041c10: 7047 6574 4c6f 6769 6361 6c4e 616d 6500  pGetLogicalName.
+00041c20: 5f77 704d 6172 6b46 6f72 556e 7265 6769  _wpMarkForUnregi
+00041c30: 7374 6572 005f 7770 456e 7472 7943 6f75  ster._wpEntryCou
+00041c40: 6e74 005f 7770 4765 7444 6576 5964 7800  nt._wpGetDevYdx.
+00041c50: 5f77 7053 6561 7263 6845 7800 5f77 7053  _wpSearchEx._wpS
+00041c60: 6561 7263 6800 5f77 7053 6561 7263 6842  earch._wpSearchB
+00041c70: 794e 616d 6548 6173 6800 5f77 7047 6574  yNameHash._wpGet
+00041c80: 4465 7669 6365 496e 666f 005f 7970 5265  DeviceInfo._ypRe
+00041c90: 6769 7374 6572 005f 7970 5265 6769 7374  gister._ypRegist
+00041ca0: 6572 4279 5964 7800 5f79 7047 6574 4174  erByYdx._ypGetAt
+00041cb0: 7472 6962 7574 6573 4279 5964 7800 5f79  tributesByYdx._y
+00041cc0: 7047 6574 4361 7465 676f 7279 005f 7970  pGetCategory._yp
+00041cd0: 4765 7441 7474 7269 6275 7465 7300 5f79  GetAttributes._y
+00041ce0: 7047 6574 5479 7065 005f 7970 5365 6172  pGetType._ypSear
+00041cf0: 6368 005f 7970 4765 7446 756e 6374 696f  ch._ypGetFunctio
+00041d00: 6e73 005f 7970 4765 7446 756e 6374 696f  ns._ypGetFunctio
+00041d10: 6e49 6e66 6f00 5f79 7047 6574 4675 6e63  nInfo._ypGetFunc
+00041d20: 7469 6f6e 7345 7800 5f79 7046 696e 6442  tionsEx._ypFindB
+00041d30: 6f6f 746c 6f61 6465 7273 005f 6465 636f  ootloaders._deco
+00041d40: 6465 4e65 7446 756e 6356 616c 5632 005f  deNetFuncValV2._
+00041d50: 7942 6c6b 4672 6565 005f 5365 7269 616c  yBlkFree._Serial
+00041d60: 5265 6600 5f6e 6578 7443 6174 5964 7800  Ref._nextCatYdx.
+00041d70: 5f6e 6578 7448 6173 6845 6e74 7279 005f  _nextHashEntry._
+00041d80: 5365 7269 616c 4e75 6d62 6572 5374 7200  SerialNumberStr.
+00041d90: 5f79 5770 4c69 7374 4865 6164 005f 7959  _yWpListHead._yY
+00041da0: 704c 6973 7448 6561 6400 5f66 7265 6542  pListHead._freeB
+00041db0: 6c6b 7300 5f79 4861 7368 4d75 7465 7800  lks._yHashMutex.
+00041dc0: 5f79 4672 6565 4d75 7465 7800 5f79 5770  _yFreeMutex._yWp
+00041dd0: 4d75 7465 7800 5f79 5970 4d75 7465 7800  Mutex._yYpMutex.
+00041de0: 5f79 4861 7368 5461 626c 6500 5f64 6576  _yHashTable._dev
+00041df0: 5964 7850 7472 005f 6675 6e59 6478 5074  YdxPtr._funYdxPt
+00041e00: 7200 5f6e 6578 7444 6576 5964 7800 5f75  r._nextDevYdx._u
+00041e10: 7365 6444 6576 5964 7800 5f77 704c 6f63  sedDevYdx._wpLoc
+00041e20: 6b43 6f75 6e74 005f 7770 536f 6d65 7468  kCount._wpSometh
+00041e30: 696e 6755 6e72 6567 6973 7465 7265 6400  ingUnregistered.
+00041e40: 7970 6b74 5f6f 7378 2e63 002f 5573 6572  ypkt_osx.c./User
+00041e50: 732f 796f 6374 6f2f 746d 705f 6275 696c  s/yocto/tmp_buil
+00041e60: 642f 796f 6374 6f70 726f 642f 796f 6374  d/yoctoprod/yoct
+00041e70: 6f6c 6962 2f76 312e 302f 5075 626c 6963  olib/v1.0/Public
+00041e80: 2f63 7070 2f42 696e 6172 6965 732f 7863  /cpp/Binaries/xc
+00041e90: 6f64 655f 6173 2f79 6170 692f 6275 696c  ode_as/yapi/buil
+00041ea0: 642f 7961 7069 2e62 7569 6c64 2f52 656c  d/yapi.build/Rel
+00041eb0: 6561 7365 2f79 6170 692e 6275 696c 642f  ease/yapi.build/
+00041ec0: 4f62 6a65 6374 732d 6e6f 726d 616c 2f78  Objects-normal/x
+00041ed0: 3836 5f36 342f 7970 6b74 5f6f 7378 2e6f  86_64/ypkt_osx.o
+00041ee0: 005f 7979 7955 5342 5f69 6e69 7400 5f65  ._yyyUSB_init._e
+00041ef0: 7665 6e74 5f74 6872 6561 6400 5f73 6574  vent_thread._set
+00041f00: 7570 4849 444d 616e 6167 6572 005f 7979  upHIDManager._yy
+00041f10: 7955 5342 5f73 746f 7000 5f73 746f 7048  yUSB_stop._stopH
+00041f20: 4944 4d61 6e61 6765 7200 5f79 7979 5553  IDManager._yyyUS
+00041f30: 4247 6574 496e 7465 7266 6163 6573 005f  BGetInterfaces._
+00041f40: 6765 7444 6576 5265 6600 5f67 6574 5f69  getDevRef._get_i
+00041f50: 6e74 5f70 726f 7065 7274 7900 5f67 6574  nt_property._get
+00041f60: 5f74 7874 5f70 726f 7065 7274 7900 5f79  _txt_property._y
+00041f70: 7979 4f53 6864 6c43 6f6d 7061 7265 005f  yyOShdlCompare._
+00041f80: 7979 7953 6574 7570 005f 4861 6e64 6c65  yyySetup._Handle
+00041f90: 5f49 4f48 4944 4465 7669 6365 494f 4849  _IOHIDDeviceIOHI
+00041fa0: 4452 6570 6f72 7443 616c 6c62 6163 6b00  DReportCallback.
+00041fb0: 5f79 7979 5369 676e 616c 4f75 7450 6b74  _yyySignalOutPkt
+00041fc0: 005f 7979 7950 6163 6b65 7453 6875 7464  ._yyyPacketShutd
+00041fd0: 6f77 6e00 7961 7069 2e63 002f 5573 6572  own.yapi.c./User
+00041fe0: 732f 796f 6374 6f2f 746d 705f 6275 696c  s/yocto/tmp_buil
+00041ff0: 642f 796f 6374 6f70 726f 642f 796f 6374  d/yoctoprod/yoct
+00042000: 6f6c 6962 2f76 312e 302f 5075 626c 6963  olib/v1.0/Public
+00042010: 2f63 7070 2f42 696e 6172 6965 732f 7863  /cpp/Binaries/xc
+00042020: 6f64 655f 6173 2f79 6170 692f 6275 696c  ode_as/yapi/buil
+00042030: 642f 7961 7069 2e62 7569 6c64 2f52 656c  d/yapi.build/Rel
+00042040: 6561 7365 2f79 6170 692e 6275 696c 642f  ease/yapi.build/
+00042050: 4f62 6a65 6374 732d 6e6f 726d 616c 2f78  Objects-normal/x
+00042060: 3836 5f36 342f 7961 7069 2e6f 005f 7961  86_64/yapi.o._ya
+00042070: 7069 4164 6455 6465 7652 756c 6573 466f  piAddUdevRulesFo
+00042080: 7259 6f63 746f 005f 7946 756e 6374 696f  rYocto._yFunctio
+00042090: 6e55 7064 6174 6500 5f79 4675 6e63 7469  nUpdate._yFuncti
+000420a0: 6f6e 5469 6d65 6455 7064 6174 6500 5f69  onTimedUpdate._i
+000420b0: 6e69 7444 6576 5964 7849 6e66 6f73 005f  nitDevYdxInfos._
+000420c0: 6672 6565 4465 7659 6478 496e 666f 7300  freeDevYdxInfos.
+000420d0: 5f79 6170 6950 756c 6c44 6576 6963 654c  _yapiPullDeviceL
+000420e0: 6f67 4578 005f 7961 7069 4765 7444 6576  ogEx._yapiGetDev
+000420f0: 6963 6550 6174 6800 5f79 7770 4765 7444  icePath._ywpGetD
+00042100: 6576 6963 6548 7562 005f 7961 7069 5265  eviceHub._yapiRe
+00042110: 7175 6573 744f 7065 6e55 5342 005f 6c6f  questOpenUSB._lo
+00042120: 6752 6573 756c 7400 5f79 6170 6952 6571  gResult._yapiReq
+00042130: 7565 7374 4f70 656e 5753 005f 7961 7069  uestOpenWS._yapi
+00042140: 5265 7175 6573 744f 7065 6e48 5454 5000  RequestOpenHTTP.
+00042150: 5f79 6170 6950 756c 6c44 6576 6963 654c  _yapiPullDeviceL
+00042160: 6f67 005f 6368 6563 6b46 6f72 5361 6d65  og._checkForSame
+00042170: 4875 6241 6363 6573 7300 5f79 7770 5361  HubAccess._ywpSa
+00042180: 6665 556e 7265 6769 7374 6572 005f 7977  feUnregister._yw
+00042190: 7053 6166 6552 6567 6973 7465 7200 5f79  pSafeRegister._y
+000421a0: 7770 5361 6665 5570 6461 7465 005f 7977  wpSafeUpdate._yw
+000421b0: 7047 6574 4465 7669 6365 5572 6c00 5f68  pGetDeviceUrl._h
+000421c0: 616e 646c 654e 6574 4e6f 7469 6669 6361  andleNetNotifica
+000421d0: 7469 6f6e 005f 756e 7265 6769 7374 6572  tion._unregister
+000421e0: 4e65 7444 6576 6963 6500 5f72 6571 7565  NetDevice._reque
+000421f0: 7374 5f70 656e 6469 6e67 5f6c 6f67 7300  st_pending_logs.
+00042200: 5f79 6170 6947 6574 444c 4c50 6174 6800  _yapiGetDLLPath.
+00042210: 5f57 616b 6555 7041 6c6c 536c 6565 7000  _WakeUpAllSleep.
+00042220: 5f79 6170 6947 6574 5469 636b 436f 756e  _yapiGetTickCoun
+00042230: 7400 5f79 6170 6947 6574 434e 6f6e 6365  t._yapiGetCNonce
+00042240: 005f 7961 7069 5265 7175 6573 744f 7065  ._yapiRequestOpe
+00042250: 6e00 5f79 6170 6948 5454 5052 6571 7565  n._yapiHTTPReque
+00042260: 7374 5379 6e63 5374 6172 7445 785f 696e  stSyncStartEx_in
+00042270: 7465 726e 616c 005f 756e 7061 636b 4854  ternal._unpackHT
+00042280: 5450 5265 7175 6573 7400 5f79 6170 6952  TPRequest._yapiR
+00042290: 6571 7565 7374 436c 6f73 6500 5f79 6170  equestClose._yap
+000422a0: 6948 5454 5052 6571 7565 7374 5379 6e63  iHTTPRequestSync
+000422b0: 446f 6e65 5f69 6e74 6572 6e61 6c00 5f79  Done_internal._y
+000422c0: 6170 6947 6574 426f 6f74 6c6f 6164 6572  apiGetBootloader
+000422d0: 7344 6576 7300 5f79 6170 694a 736f 6e47  sDevs._yapiJsonG
+000422e0: 6574 5061 7468 5f69 6e74 6572 6e61 6c00  etPath_internal.
+000422f0: 5f79 6170 694a 736f 6e56 616c 7565 5061  _yapiJsonValuePa
+00042300: 7273 6553 7472 7563 7400 5f79 6170 6952  rseStruct._yapiR
+00042310: 6567 6973 7465 7252 6177 4e6f 7469 6669  egisterRawNotifi
+00042320: 6361 7469 6f6e 4362 005f 7961 7069 5265  cationCb._yapiRe
+00042330: 6769 7374 6572 5261 7752 6570 6f72 7443  gisterRawReportC
+00042340: 6200 5f79 6170 6952 6567 6973 7465 7252  b._yapiRegisterR
+00042350: 6177 5265 706f 7274 5632 4362 005f 7961  awReportV2Cb._ya
+00042360: 7069 496e 6974 4150 4900 5f79 6170 6949  piInitAPI._yapiI
+00042370: 6e69 7441 5049 5f69 6e74 6572 6e61 6c00  nitAPI_internal.
+00042380: 5f79 6170 6946 7265 6541 5049 005f 7961  _yapiFreeAPI._ya
+00042390: 7069 4672 6565 4150 495f 696e 7465 726e  piFreeAPI_intern
+000423a0: 616c 005f 7961 7069 5365 744e 6574 776f  al._yapiSetNetwo
+000423b0: 726b 5469 6d65 6f75 7400 5f79 6170 6947  rkTimeout._yapiG
+000423c0: 6574 4e65 7477 6f72 6b54 696d 656f 7574  etNetworkTimeout
+000423d0: 005f 7961 7069 5365 744e 6574 4465 764c  ._yapiSetNetDevL
+000423e0: 6973 7456 616c 6964 6974 7900 5f79 6170  istValidity._yap
+000423f0: 6947 6574 4e65 7444 6576 4c69 7374 5661  iGetNetDevListVa
+00042400: 6c69 6469 7479 005f 7961 7069 5265 6769  lidity._yapiRegi
+00042410: 7374 6572 4c6f 6746 756e 6374 696f 6e00  sterLogFunction.
+00042420: 5f79 6170 6952 6567 6973 7465 7244 6576  _yapiRegisterDev
+00042430: 6963 654c 6f67 4361 6c6c 6261 636b 005f  iceLogCallback._
+00042440: 7961 7069 5374 6172 7453 746f 7044 6576  yapiStartStopDev
+00042450: 6963 654c 6f67 4361 6c6c 6261 636b 005f  iceLogCallback._
+00042460: 7961 7069 5265 6769 7374 6572 4465 7669  yapiRegisterDevi
+00042470: 6365 4172 7269 7661 6c43 616c 6c62 6163  ceArrivalCallbac
+00042480: 6b00 5f79 6170 6952 6567 6973 7465 7244  k._yapiRegisterD
+00042490: 6576 6963 6552 656d 6f76 616c 4361 6c6c  eviceRemovalCall
+000424a0: 6261 636b 005f 7961 7069 5265 6769 7374  back._yapiRegist
+000424b0: 6572 4465 7669 6365 4368 616e 6765 4361  erDeviceChangeCa
+000424c0: 6c6c 6261 636b 005f 7961 7069 5265 6769  llback._yapiRegi
+000424d0: 7374 6572 4265 6163 6f6e 4361 6c6c 6261  sterBeaconCallba
+000424e0: 636b 005f 7961 7069 5265 6769 7374 6572  ck._yapiRegister
+000424f0: 4465 7669 6365 436f 6e66 6967 4368 616e  DeviceConfigChan
+00042500: 6765 4361 6c6c 6261 636b 005f 7961 7069  geCallback._yapi
+00042510: 5265 6769 7374 6572 4675 6e63 7469 6f6e  RegisterFunction
+00042520: 5570 6461 7465 4361 6c6c 6261 636b 005f  UpdateCallback._
+00042530: 7961 7069 5265 6769 7374 6572 5469 6d65  yapiRegisterTime
+00042540: 6452 6570 6f72 7443 616c 6c62 6163 6b00  dReportCallback.
+00042550: 5f79 6170 694c 6f63 6b46 756e 6374 696f  _yapiLockFunctio
+00042560: 6e43 616c 6c42 6163 6b00 5f79 6170 6955  nCallBack._yapiU
+00042570: 6e6c 6f63 6b46 756e 6374 696f 6e43 616c  nlockFunctionCal
+00042580: 6c42 6163 6b00 5f79 6170 694c 6f63 6b44  lBack._yapiLockD
+00042590: 6576 6963 6543 616c 6c42 6163 6b00 5f79  eviceCallBack._y
+000425a0: 6170 6955 6e6c 6f63 6b44 6576 6963 6543  apiUnlockDeviceC
+000425b0: 616c 6c42 6163 6b00 5f79 6170 6954 6573  allBack._yapiTes
+000425c0: 7448 7562 005f 7961 7069 5265 6769 7374  tHub._yapiRegist
+000425d0: 6572 4875 6200 5f79 6170 6950 7265 7265  erHub._yapiPrere
+000425e0: 6769 7374 6572 4875 6200 5f79 6170 6955  gisterHub._yapiU
+000425f0: 6e72 6567 6973 7465 7248 7562 005f 7961  nregisterHub._ya
+00042600: 7069 556e 7265 6769 7374 6572 4875 625f  piUnregisterHub_
+00042610: 696e 7465 726e 616c 005f 7961 7069 5570  internal._yapiUp
+00042620: 6461 7465 4465 7669 6365 4c69 7374 005f  dateDeviceList._
+00042630: 7961 7069 5570 6461 7465 4465 7669 6365  yapiUpdateDevice
+00042640: 4c69 7374 5f69 6e74 6572 6e61 6c00 5f79  List_internal._y
+00042650: 6170 6948 616e 646c 6545 7665 6e74 7300  apiHandleEvents.
+00042660: 5f79 6170 6948 616e 646c 6545 7665 6e74  _yapiHandleEvent
+00042670: 735f 696e 7465 726e 616c 005f 7961 7069  s_internal._yapi
+00042680: 536c 6565 7000 5f79 6170 6943 6865 636b  Sleep._yapiCheck
+00042690: 4c6f 6769 6361 6c4e 616d 6500 5f79 6170  LogicalName._yap
+000426a0: 6947 6574 4150 4956 6572 7369 6f6e 005f  iGetAPIVersion._
+000426b0: 7961 7069 5365 7454 7261 6365 4669 6c65  yapiSetTraceFile
+000426c0: 005f 7961 7069 4765 7444 6576 6963 6500  ._yapiGetDevice.
+000426d0: 5f79 6170 6947 6574 416c 6c44 6576 6963  _yapiGetAllDevic
+000426e0: 6573 005f 7961 7069 4765 7444 6576 6963  es._yapiGetDevic
+000426f0: 6549 6e66 6f00 5f79 6170 6947 6574 4465  eInfo._yapiGetDe
+00042700: 7669 6365 5061 7468 4578 005f 7961 7069  vicePathEx._yapi
+00042710: 4765 7446 756e 6374 696f 6e00 5f79 6170  GetFunction._yap
+00042720: 6947 6574 4675 6e63 7469 6f6e 7342 7943  iGetFunctionsByC
+00042730: 6c61 7373 005f 7961 7069 4765 7446 756e  lass._yapiGetFun
+00042740: 6374 696f 6e73 4279 4465 7669 6365 005f  ctionsByDevice._
+00042750: 7961 7069 4765 7446 756e 6374 696f 6e49  yapiGetFunctionI
+00042760: 6e66 6f00 5f79 6170 6947 6574 4675 6e63  nfo._yapiGetFunc
+00042770: 7469 6f6e 496e 666f 4578 5f69 6e74 6572  tionInfoEx_inter
+00042780: 6e61 6c00 5f79 6170 6947 6574 4675 6e63  nal._yapiGetFunc
+00042790: 7469 6f6e 496e 666f 4578 005f 7961 7069  tionInfoEx._yapi
+000427a0: 4854 5450 5265 7175 6573 7453 796e 6353  HTTPRequestSyncS
+000427b0: 7461 7274 4578 005f 7961 7069 4854 5450  tartEx._yapiHTTP
+000427c0: 5265 7175 6573 7453 796e 6353 7461 7274  RequestSyncStart
+000427d0: 005f 7961 7069 4854 5450 5265 7175 6573  ._yapiHTTPReques
+000427e0: 7453 796e 6353 7461 7274 4f75 744f 6642  tSyncStartOutOfB
+000427f0: 616e 6400 5f79 6170 6948 5454 5052 6571  and._yapiHTTPReq
+00042800: 7565 7374 5379 6e63 446f 6e65 005f 7961  uestSyncDone._ya
+00042810: 7069 4854 5450 5265 7175 6573 7441 7379  piHTTPRequestAsy
+00042820: 6e63 4578 005f 7961 7069 4854 5450 5265  ncEx._yapiHTTPRe
+00042830: 7175 6573 7441 7379 6e63 4578 5f69 6e74  questAsyncEx_int
+00042840: 6572 6e61 6c00 5f79 6170 6948 5454 5052  ernal._yapiHTTPR
+00042850: 6571 7565 7374 4173 796e 6300 5f79 6170  equestAsync._yap
+00042860: 6948 5454 5052 6571 7565 7374 4173 796e  iHTTPRequestAsyn
+00042870: 634f 7574 4f66 4261 6e64 005f 7961 7069  cOutOfBand._yapi
+00042880: 4854 5450 5265 7175 6573 7400 5f79 6170  HTTPRequest._yap
+00042890: 6952 6567 6973 7465 7248 7562 4469 7363  iRegisterHubDisc
+000428a0: 6f76 6572 7943 616c 6c62 6163 6b00 5f79  overyCallback._y
+000428b0: 6170 6952 6567 6973 7465 7257 616b 6555  apiRegisterWakeU
+000428c0: 7043 6200 5f79 6170 6954 7269 6767 6572  pCb._yapiTrigger
+000428d0: 4875 6244 6973 636f 7665 7279 005f 7961  HubDiscovery._ya
+000428e0: 7069 4765 7442 6f6f 746c 6f61 6465 7273  piGetBootloaders
+000428f0: 005f 7961 7069 4973 4d6f 6475 6c65 5772  ._yapiIsModuleWr
+00042900: 6974 6162 6c65 005f 7961 7069 4a73 6f6e  itable._yapiJson
+00042910: 4465 636f 6465 5374 7269 6e67 005f 7961  DecodeString._ya
+00042920: 7069 4a73 6f6e 4765 7450 6174 6800 5f79  piJsonGetPath._y
+00042930: 6170 6947 6574 416c 6c4a 736f 6e4b 6579  apiGetAllJsonKey
+00042940: 7300 5f79 6170 6947 6574 4d65 6d00 5f79  s._yapiGetMem._y
+00042950: 6170 6946 7265 654d 656d 005f 7961 7069  apiFreeMem._yapi
+00042960: 4368 6563 6b46 6972 6d77 6172 6500 5f79  CheckFirmware._y
+00042970: 6170 6955 7064 6174 6546 6972 6d77 6172  apiUpdateFirmwar
+00042980: 6500 5f79 6170 6955 7064 6174 6546 6972  e._yapiUpdateFir
+00042990: 6d77 6172 6545 7800 5f79 6170 6947 6574  mwareEx._yapiGet
+000429a0: 5375 6264 6576 6963 6573 005f 6465 6c65  Subdevices._dele
+000429b0: 7465 416c 6c43 5300 5f73 7364 7045 6e74  teAllCS._ssdpEnt
+000429c0: 7279 5570 6461 7465 005f 756e 7265 6769  ryUpdate._unregi
+000429d0: 7374 6572 4e65 7448 7562 005f 6973 5361  sterNetHub._isSa
+000429e0: 6d65 4875 6200 5f79 6170 6946 7265 6548  meHub._yapiFreeH
+000429f0: 7562 005f 7946 7265 6550 6172 7365 6455  ub._yFreeParsedU
+00042a00: 524c 005f 7961 7069 416c 6c6f 6348 7562  RL._yapiAllocHub
+00042a10: 005f 7069 6e67 5552 4c4f 6e68 7562 005f  ._pingURLOnhub._
+00042a20: 7950 6172 7365 4875 6255 524c 005f 7961  yParseHubURL._ya
+00042a30: 7069 5265 6769 7374 6572 4875 6245 7800  piRegisterHubEx.
+00042a40: 5f79 6865 6c70 6572 5f74 6872 6561 6400  _yhelper_thread.
+00042a50: 5f79 4e65 7448 7562 456e 756d 005f 794e  _yNetHubEnum._yN
+00042a60: 6574 4875 6245 6e75 6d45 7800 5f64 6973  etHubEnumEx._dis
+00042a70: 6162 6c65 5f6a 7a6f 6e00 5f70 6172 7365  able_jzon._parse
+00042a80: 4e65 7457 7045 6e74 7279 005f 7970 5570  NetWpEntry._ypUp
+00042a90: 6461 7465 4e65 7400 5f61 7379 6e63 4472  dateNet._asyncDr
+00042aa0: 6f70 005f 5963 7478 4465 7669 6365 4c69  op._YctxDeviceLi
+00042ab0: 7374 5661 6c69 6469 7479 4d73 005f 5963  stValidityMs._Yc
+00042ac0: 7478 4e65 7477 6f72 6b54 696d 656f 7574  txNetworkTimeout
+00042ad0: 0079 6669 666f 2e63 002f 5573 6572 732f  .yfifo.c./Users/
+00042ae0: 796f 6374 6f2f 746d 705f 6275 696c 642f  yocto/tmp_build/
+00042af0: 796f 6374 6f70 726f 642f 796f 6374 6f6c  yoctoprod/yoctol
+00042b00: 6962 2f76 312e 302f 5075 626c 6963 2f63  ib/v1.0/Public/c
+00042b10: 7070 2f42 696e 6172 6965 732f 7863 6f64  pp/Binaries/xcod
+00042b20: 655f 6173 2f79 6170 692f 6275 696c 642f  e_as/yapi/build/
+00042b30: 7961 7069 2e62 7569 6c64 2f52 656c 6561  yapi.build/Relea
+00042b40: 7365 2f79 6170 692e 6275 696c 642f 4f62  se/yapi.build/Ob
+00042b50: 6a65 6374 732d 6e6f 726d 616c 2f78 3836  jects-normal/x86
+00042b60: 5f36 342f 7966 6966 6f2e 6f00 5f79 4669  _64/yfifo.o._yFi
+00042b70: 666f 496e 6974 4578 005f 7946 6966 6f43  foInitEx._yFifoC
+00042b80: 6c65 616e 7570 005f 7946 6966 6f45 6e74  leanup._yFifoEnt
+00042b90: 6572 4353 005f 7946 6966 6f4c 6561 7665  erCS._yFifoLeave
+00042ba0: 4353 005f 7946 6966 6f45 6d70 7479 4578  CS._yFifoEmptyEx
+00042bb0: 005f 7946 6966 6f45 6d70 7479 005f 7950  ._yFifoEmpty._yP
+00042bc0: 7573 6846 6966 6f45 7800 5f79 5075 7368  ushFifoEx._yPush
+00042bd0: 4669 666f 005f 7950 6f70 4669 666f 4578  Fifo._yPopFifoEx
+00042be0: 005f 7950 6f70 4669 666f 005f 7946 6f72  ._yPopFifo._yFor
+00042bf0: 6365 4669 666f 005f 7950 6565 6b46 6966  ceFifo._yPeekFif
+00042c00: 6f45 7800 5f79 5065 656b 4669 666f 005f  oEx._yPeekFifo._
+00042c10: 7950 6565 6b43 6f6e 7469 6e75 6f75 7346  yPeekContinuousF
+00042c20: 6966 6f45 7800 5f79 5065 656b 436f 6e74  ifoEx._yPeekCont
+00042c30: 696e 756f 7573 4669 666f 005f 7953 6565  inuousFifo._ySee
+00042c40: 6b46 6966 6f45 7800 5f79 5365 656b 4669  kFifoEx._ySeekFi
+00042c50: 666f 005f 7946 6966 6f47 6574 5573 6564  fo._yFifoGetUsed
+00042c60: 4578 005f 7946 6966 6f47 6574 5573 6564  Ex._yFifoGetUsed
+00042c70: 005f 7946 6966 6f47 6574 4672 6565 4578  ._yFifoGetFreeEx
+00042c80: 005f 7946 6966 6f47 6574 4672 6565 005f  ._yFifoGetFree._
+00042c90: 7978 746f 6100 5f64 6563 6f64 6550 7562  yxtoa._decodePub
+00042ca0: 5661 6c00 7974 6872 6561 642e 6300 2f55  Val.ythread.c./U
+00042cb0: 7365 7273 2f79 6f63 746f 2f74 6d70 5f62  sers/yocto/tmp_b
+00042cc0: 7569 6c64 2f79 6f63 746f 7072 6f64 2f79  uild/yoctoprod/y
+00042cd0: 6f63 746f 6c69 622f 7631 2e30 2f50 7562  octolib/v1.0/Pub
+00042ce0: 6c69 632f 6370 702f 4269 6e61 7269 6573  lic/cpp/Binaries
+00042cf0: 2f78 636f 6465 5f61 732f 7961 7069 2f62  /xcode_as/yapi/b
+00042d00: 7569 6c64 2f79 6170 692e 6275 696c 642f  uild/yapi.build/
+00042d10: 5265 6c65 6173 652f 7961 7069 2e62 7569  Release/yapi.bui
+00042d20: 6c64 2f4f 626a 6563 7473 2d6e 6f72 6d61  ld/Objects-norma
+00042d30: 6c2f 7838 365f 3634 2f79 7468 7265 6164  l/x86_64/ythread
+00042d40: 2e6f 005f 7943 7265 6174 6545 7665 6e74  .o._yCreateEvent
+00042d50: 005f 7943 7265 6174 654d 616e 7561 6c45  ._yCreateManualE
+00042d60: 7665 6e74 005f 7953 6574 4576 656e 7400  vent._ySetEvent.
+00042d70: 5f79 5265 7365 7445 7665 6e74 005f 7957  _yResetEvent._yW
+00042d80: 6169 7446 6f72 4576 656e 7400 5f79 436c  aitForEvent._yCl
+00042d90: 6f73 6545 7665 6e74 005f 7954 6872 6561  oseEvent._yThrea
+00042da0: 6449 6e64 6578 005f 7943 7265 6174 6544  dIndex._yCreateD
+00042db0: 6574 6163 6865 6454 6872 6561 644e 616d  etachedThreadNam
+00042dc0: 6564 005f 7943 7265 6174 6544 6574 6163  ed._yCreateDetac
+00042dd0: 6865 6454 6872 6561 6445 7800 5f79 5468  hedThreadEx._yTh
+00042de0: 7265 6164 4372 6561 7465 4e61 6d65 6400  readCreateNamed.
+00042df0: 5f79 5468 7265 6164 4973 5275 6e6e 696e  _yThreadIsRunnin
+00042e00: 6700 5f79 5468 7265 6164 5369 676e 616c  g._yThreadSignal
+00042e10: 5374 6172 7400 5f79 5468 7265 6164 5369  Start._yThreadSi
+00042e20: 676e 616c 456e 6400 5f79 5468 7265 6164  gnalEnd._yThread
+00042e30: 5265 7175 6573 7445 6e64 005f 7954 6872  RequestEnd._yThr
+00042e40: 6561 644d 7573 7445 6e64 005f 7954 6872  eadMustEnd._yThr
+00042e50: 6561 644b 696c 6c00 5f79 496e 6974 6961  eadKill._yInitia
+00042e60: 6c69 7a65 4372 6974 6963 616c 5365 6374  lizeCriticalSect
+00042e70: 696f 6e00 5f79 456e 7465 7243 7269 7469  ion._yEnterCriti
+00042e80: 6361 6c53 6563 7469 6f6e 005f 7954 7279  calSection._yTry
+00042e90: 456e 7465 7243 7269 7469 6361 6c53 6563  EnterCriticalSec
+00042ea0: 7469 6f6e 005f 794c 6561 7665 4372 6974  tion._yLeaveCrit
+00042eb0: 6963 616c 5365 6374 696f 6e00 5f79 4465  icalSection._yDe
+00042ec0: 6c65 7465 4372 6974 6963 616c 5365 6374  leteCriticalSect
+00042ed0: 696f 6e00 5f69 6e69 7454 7364 4b65 7900  ion._initTsdKey.
+00042ee0: 5f79 496e 6974 4b65 794f 6e63 6500 5f79  _yInitKeyOnce._y
+00042ef0: 4e65 7874 5468 7265 6164 4964 7800 5f79  NextThreadIdx._y
+00042f00: 5473 644b 6579 0000 0000 0000 0000 0000  TsdKey..........
+00042f10: fade 0cc0 0000 0a4d 0000 0004 0000 0000  .......M........
+00042f20: 0000 002c 0000 0002 0000 0935 0000 0005  ...,.......5....
+00042f30: 0000 0941 0001 0000 0000 0a45 fade 0c02  ...A.......E....
+00042f40: 0000 0909 0002 0400 0000 0002 0000 0129  ...............)
+00042f50: 0000 0058 0000 0005 0000 003f 0003 ef10  ...X.......?....
+00042f60: 2002 000c 0000 0000 0000 0000 0000 0000   ...............
+00042f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00042f80: 0000 0000 0000 0000 0002 8000 0000 0000  ................
+00042f90: 0000 0000 6c69 6279 6170 692d 3535 3535  ....libyapi-5555
+00042fa0: 3439 3434 3565 3765 3239 3533 6231 3861  49445e7e2953b18a
+00042fb0: 3334 3037 6262 3063 6236 3966 3537 3636  3407bb0cb69f5766
+00042fc0: 6637 6637 00c6 dc9c 8e50 8ccb 383c 8c74  f7f7.....P..8<.t
+00042fd0: 84e8 3d73 a81a c271 ac0d c9ba 1ea2 efca  ..=s...q........
+00042fe0: 12de fda0 c600 0000 0000 0000 0000 0000  ................
+00042ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00043000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00043010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00043020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00043030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00043040: 0000 0000 0098 7920 904e ab65 0e75 788c  ......y .N.e.ux.
-00043050: 054a a0b0 524e 6a80 bfc7 1aa3 2df8 d237  .J..RNj.....-..7
-00043060: a617 43f9 8600 0000 0000 0000 0000 0000  ..C.............
-00043070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00043080: 0000 0000 005a 470d 2c4a 5d6b 61e2 90b5  .....ZG.,J]ka...
-00043090: 1c50 3f6e a509 c9d2 cd68 601e 109e 9d24  .P?n.....h`....$
-000430a0: 3e8e 483f dcad 7fac b258 6fc6 e966 c004  >.H?.....Xo..f..
+00043020: 0000 0000 0098 7920 904e ab65 0e75 788c  ......y .N.e.ux.
+00043030: 054a a0b0 524e 6a80 bfc7 1aa3 2df8 d237  .J..RNj.....-..7
+00043040: a617 43f9 8600 0000 0000 0000 0000 0000  ..C.............
+00043050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00043060: 0000 0000 003d e7ed 704e fd57 06f3 c797  .....=..pN.W....
+00043070: 7e1e bdee 8a19 0bd8 8fa9 d9d8 6f71 fa0b  ~...........oq..
+00043080: 08bd 2949 9ead 7fac b258 6fc6 e966 c004  ..)I.....Xo..f..
+00043090: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
+000430a0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 000430b0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-000430c0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
-000430d0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-000430e0: 8b48 892c a76a 6027 f5a0 7aff 8b4b 1993  .H.,.j`'..z..K..
-000430f0: d5b1 004d 44f9 2f94 0fc4 8096 19d5 840e  ...MD./.........
-00043100: 72cf 375f 4dff 33bb cd66 60a1 0309 20b8  r.7_M.3..f`... .
-00043110: 1d7d 0b90 0e6b 1676 42bb 9d02 221a 79ca  .}...k.vB...".y.
-00043120: 5cb9 98ed 4220 11f3 f439 3eee c4de 7e7d  \...B ...9>...~}
-00043130: 2a07 7828 9df8 da5c 70ce 587d e3a4 374c  *.x(...\p.X}..7L
-00043140: ea0e e08a 9867 52e9 1310 4c41 f5b8 bf6d  .....gR...LA...m
-00043150: f004 9492 0c50 4ae6 a496 0b38 7575 6f7a  .....PJ....8uuoz
-00043160: d935 a62e 2ca4 ad3f 116e c7d2 ead1 23f6  .5..,..?.n....#.
-00043170: e64a 380c 24bd 772f ad11 8e5f 8b6c 1408  .J8.$.w/..._.l..
-00043180: daf9 4f0b 385b 5686 a5b7 f6df 56b5 5075  ..O.8[V.....V.Pu
-00043190: bba1 2229 10fa ee57 af79 7479 849f 6ff8  ..")...W.yty..o.
-000431a0: c96f 752f e6db 3a44 0b5e bc26 0742 f230  .ou/..:D.^.&.B.0
-000431b0: 2c85 b371 acd8 e30d 922a df6e 52eb 11cb  ,..q.....*.nR...
-000431c0: fa95 ed74 f93c e226 2d61 e1e8 7d47 25ac  ...t.<.&-a..}G%.
-000431d0: 6d55 b3b8 d542 38bd d924 c865 d053 b695  mU...B8..$.e.S..
-000431e0: e352 5694 9e41 2aa2 0b52 6f13 5851 e8dd  .RV..A*..Ro.XQ..
-000431f0: cc70 f425 997a 3b25 acf1 18b9 d887 51d4  .p.%.z;%......Q.
-00043200: 1b4c d7cb 18b1 e4ad d5ef 3d4e c60f 9b6d  .L........=N...m
-00043210: 6c6a 4201 df67 ef1d f2a6 9a0e 30ba f5b1  ljB..g......0...
-00043220: dbaa f131 ebab 5427 edaf c567 bbd3 41e7  ...1..T'...g..A.
-00043230: a540 369f fc91 2db5 43f2 661c 6e8a 498b  .@6...-.C.f.n.I.
-00043240: 1485 610e e570 c993 1048 4115 8521 90ea  ..a..p...HA..!..
-00043250: 6218 38ad c0e0 de77 53bc e931 5a8e ce1d  b.8....wS..1Z...
-00043260: 0abb 36ec ce1f ef5d 6e11 43b1 2349 6299  ..6....]n.C.#Ib.
-00043270: 7dc3 18ed be55 c3c8 985e bb7b d3a6 a138  }....U...^.{...8
-00043280: 0adc 3c17 270e cfd1 f349 1162 e9b4 ab60  ..<.'....I.b...`
-00043290: b8e0 8024 ac09 7d05 7577 4cd9 bd06 07c6  ...$..}.uwL.....
-000432a0: cd6e 497a 68f6 9a79 7d05 2c65 68cd 5da3  .nIzh..y}.,eh.].
-000432b0: 77c0 8712 e2a5 c29f c108 5038 a9dc 1aa2  w.........P8....
-000432c0: bde5 bf5c 3df8 dc87 ae2d 393d d796 7ff0  ...\=....-9=....
-000432d0: a83d bfa4 3319 3e9f 3f55 441a 5a3d 15f7  .=..3.>.?UD.Z=..
-000432e0: b836 d71f 56d7 ed6e c555 8080 090c ea19  .6..V..n.U......
-000432f0: 6aac ea75 5473 2c93 e31d f7d2 fe3b 5e4c  j..uTs,......;^L
-00043300: 965f 4cdd 26bf 0894 a87c 5f62 7576 d970  ._L.&....|_buv.p
-00043310: e775 b8a0 62fc 9177 901a a8f2 5082 8083  .u..b..w....P...
-00043320: 9649 71c0 4fe7 04aa 7f11 5a93 61a7 6e0e  .Iq.O.....Z.a.n.
-00043330: e3cf 78ea 18c2 bfed 828d 218a 27cb 47fa  ..x.......!.'.G.
-00043340: 2b14 5e7b 6cb3 8226 cb56 6c6f a927 ba3b  +.^{l..&.Vlo.'.;
-00043350: 170e 3215 a67d 0328 6413 1b42 0e0e 0f9c  ..2..}.(d..B....
-00043360: b009 5905 3e42 0e02 2e6f 90c0 f692 6d30  ..Y.>B...o....m0
-00043370: 3451 a78b e70e 12cc 916c 23ea 1f19 3374  4Q.......l#...3t
-00043380: 890a ea36 cbac cb2f b992 0107 36b6 bde8  ...6.../....6...
-00043390: 8f82 108b 5fff 698f 5847 1fba 485f a6aa  ...._.i.XG..H_..
-000433a0: c4dd 41e9 244c 7431 85e8 0b5e 46bc a606  ..A.$Lt1...^F...
-000433b0: 6574 46b2 03ab 931a c5da 3f60 0b45 a828  etF.......?`.E.(
-000433c0: 6e4c 896a 4e22 acc5 b9ec dba9 d759 c574  nL.jN".......Y.t
-000433d0: 927c aacb 2278 9fd6 6da7 b2ff 342c 0d49  .|.."x..m...4,.I
-000433e0: 216e 6076 da1c e5f1 8da1 45f9 21c4 29e3  !n`v......E.!.).
-000433f0: dfe3 73c9 3be4 5c23 1a9d 6e30 ba31 51a2  ..s.;.\#..n0.1Q.
-00043400: 11ef b362 564b 0da8 9318 6248 accf 87ae  ...bVK....bH....
-00043410: 9042 3312 998b 56c6 f5bf 6c7d 255c f430  .B3...V...l}%\.0
-00043420: 4ea6 056d efc2 fbe0 7602 48b2 0852 c916  N..m....v.H..R..
-00043430: cf15 3afb 7afe c936 094a 8cde b4d0 4ea6  ..:.z..6.J....N.
-00043440: 86a6 5529 deb2 843c a183 e8c2 18a1 6f4f  ..U)...<......oO
-00043450: 2280 bc1a 6380 f88e 5e7a 7b36 b272 b76f  "...c...^z{6.r.o
-00043460: 776a a14c 846a 5cce 652c 3088 3565 5f46  wj.L.j\.e,0.5e_F
-00043470: 529b b99a 2836 c25c 0f8f 3a3e b0c7 734a  R...(6.\..:>..sJ
-00043480: 13ee 90ef f67d 87bd 1db0 7327 30ca 9774  .....}....s'0..t
-00043490: 4b4b 7db0 2bad 5ce4 f532 7764 0258 fa68  KK}.+.\..2wd.X.h
-000434a0: 9605 6e71 8f97 35b0 6a32 99cc 8e69 a8db  ..nq..5.j2...i..
-000434b0: 07d7 e21d 4423 1084 ed09 1343 03fa 3906  ....D#.....C..9.
-000434c0: dae3 188f dd93 9bca 4fee d0ba dc4b baff  ........O....K..
-000434d0: dfc5 0355 3cc4 4812 342f 6320 3287 d002  ...U<.H.4/c 2...
-000434e0: 157a 5618 0c7a c750 059a a4a1 e52e 01ce  .zV..z.P........
-000434f0: d634 1a51 6a8a df48 a497 bb78 aa54 6e23  .4.Qj..H...x.Tn#
-00043500: 3bfc b7f4 ea63 700d 98ed 564e b1db 1440  ;....cp...VN...@
-00043510: 2d25 8537 5029 38f6 5c1e b8ac 7ab5 a1b1  -%.7P)8.\...z...
-00043520: 0d62 ec73 6638 138c 6619 c896 d588 32d5  .b.sf8..f.....2.
-00043530: 454a 8d97 072c d39d b19c 35a7 54c5 aee0  EJ...,....5.T...
-00043540: 1612 7722 0a8d 5e03 8d5c b085 2f2d dbc8  ..w"..^..\../-..
-00043550: 798e d41a 8e5f 60f4 99ab e0d1 565e 3e1c  y...._`.....V^>.
-00043560: 5b08 b8ae 745f 119c acad 7232 4af0 3050  [...t_....r2J.0P
-00043570: 139c faa4 ada2 61e8 8272 10d8 ba2a b034  ......a..r...*.4
-00043580: d5d1 ef88 704a 4f23 3e65 4236 6482 4bae  ....pJO#>eB6d.K.
-00043590: 5fcc fc1f 726a b30c 8e60 d238 973b bb6a  _...rj...`.8.;.j
-000435a0: 9071 05f8 8bad 7fac b258 6fc6 e966 c004  .q.......Xo..f..
+000430c0: 8b48 892c a76a 6027 f5a0 7aff 8b4b 1993  .H.,.j`'..z..K..
+000430d0: d5b1 004d 44f9 2f94 0fc4 8096 19d5 840e  ...MD./.........
+000430e0: 72cf 375f 4dff 33bb cd66 60a1 0309 20b8  r.7_M.3..f`... .
+000430f0: 1d7d 0b90 0e6b 1676 42bb 9d02 221a 79ca  .}...k.vB...".y.
+00043100: 5cb9 98ed 4220 11f3 f439 3eee c4de 7e7d  \...B ...9>...~}
+00043110: 2a07 7828 9df8 da5c 70ce 587d e3a4 374c  *.x(...\p.X}..7L
+00043120: ea0e e08a 9867 52e9 1310 4c41 f5b8 bf6d  .....gR...LA...m
+00043130: f004 9492 0c50 4ae6 a496 0b38 7575 6f7a  .....PJ....8uuoz
+00043140: d935 a62e 2ca4 ad3f 116e c7d2 ead1 23f6  .5..,..?.n....#.
+00043150: e64a 380c 24bd 772f ad11 8e5f 8b6c 1408  .J8.$.w/..._.l..
+00043160: daf9 4f0b 385b 5686 a5b7 f6df 56b5 5075  ..O.8[V.....V.Pu
+00043170: bba1 2229 10fa ee57 af79 7479 849f 6ff8  ..")...W.yty..o.
+00043180: c96f 752f e6db 3a44 0b5e bc26 0742 f230  .ou/..:D.^.&.B.0
+00043190: 2c85 b371 acd8 e30d 922a df6e 52eb 11cb  ,..q.....*.nR...
+000431a0: fa95 ed74 f93c e226 2d61 e1e8 7d47 25ac  ...t.<.&-a..}G%.
+000431b0: 6d55 b3b8 d542 38bd d924 c865 d053 b695  mU...B8..$.e.S..
+000431c0: e352 5694 9e41 2aa2 0b52 6f13 5851 e8dd  .RV..A*..Ro.XQ..
+000431d0: cc70 f425 997a 3b25 acf1 18b9 d887 51d4  .p.%.z;%......Q.
+000431e0: 1b4c d7cb 18b1 e4ad d5ef 3d4e c60f 9b6d  .L........=N...m
+000431f0: 6c6a 4201 df67 ef1d f2a6 9a0e 30ba f5b1  ljB..g......0...
+00043200: dbaa f131 ebab 5427 edaf c567 bbd3 41e7  ...1..T'...g..A.
+00043210: a540 369f fc91 2db5 43f2 661c 6e8a 498b  .@6...-.C.f.n.I.
+00043220: 1485 610e e570 c993 1048 4115 8521 90ea  ..a..p...HA..!..
+00043230: 6218 38ad c0e0 de77 53bc e931 5a8e ce1d  b.8....wS..1Z...
+00043240: 0abb 36ec ce5f 8794 356a 6957 6de9 1102  ..6.._..5jiWm...
+00043250: b6fc f2eb bd75 e058 7410 6860 df55 9ef2  .....u.Xt.h`.U..
+00043260: 32a0 4eb6 4f0e cfd1 f349 1162 e9b4 ab60  2.N.O....I.b...`
+00043270: b8e0 8024 ac09 7d05 7577 4cd9 bd06 07c6  ...$..}.uwL.....
+00043280: cd6e 497a 68f6 9a79 7d05 2c65 68cd 5da3  .nIzh..y}.,eh.].
+00043290: 77c0 8712 e2a5 c29f c108 5038 a9dc 1aa2  w.........P8....
+000432a0: bde5 bf5c 3df8 dc87 ae2d 393d d796 7ff0  ...\=....-9=....
+000432b0: a83d bfa4 3319 3e9f 3f55 441a 5a3d 15f7  .=..3.>.?UD.Z=..
+000432c0: b836 d71f 56d7 ed6e c555 8080 090c ea19  .6..V..n.U......
+000432d0: 6aac ea75 5473 2c93 e31d f7d2 fe3b 5e4c  j..uTs,......;^L
+000432e0: 965f 4cdd 26bf 0894 a87c 5f62 7576 d970  ._L.&....|_buv.p
+000432f0: e775 b8a0 62fc 9177 901a a8f2 5082 8083  .u..b..w....P...
+00043300: 9649 71c0 4fe7 04aa 7f11 5a93 61a7 6e0e  .Iq.O.....Z.a.n.
+00043310: e3cf 78ea 18c2 bfed 828d 218a 27cb 47fa  ..x.......!.'.G.
+00043320: 2b14 5e7b 6cb3 8226 cb56 6c6f a927 ba3b  +.^{l..&.Vlo.'.;
+00043330: 170e 3215 a67d 0328 6413 1b42 0e0e 0f9c  ..2..}.(d..B....
+00043340: b009 5905 3e42 0e02 2e6f 90c0 f692 6d30  ..Y.>B...o....m0
+00043350: 3451 a78b e70e 12cc 916c 23ea 1f19 3374  4Q.......l#...3t
+00043360: 890a ea36 cbac cb2f b992 0107 36b6 bde8  ...6.../....6...
+00043370: 8f82 108b 5fff 698f 5847 1fba 485f a6aa  ...._.i.XG..H_..
+00043380: c4dd 41e9 244c 7431 85e8 0b5e 46bc a606  ..A.$Lt1...^F...
+00043390: 6574 46b2 03ab 931a c5da 3f60 0b45 a828  etF.......?`.E.(
+000433a0: 6e4c 896a 4e22 acc5 b9ec dba9 d759 c574  nL.jN".......Y.t
+000433b0: 927c aacb 2278 9fd6 6da7 b2ff 342c 0d49  .|.."x..m...4,.I
+000433c0: 216e 6076 da1c e5f1 8da1 45f9 21c4 29e3  !n`v......E.!.).
+000433d0: dfe3 73c9 3be4 5c23 1a9d 6e30 ba31 51a2  ..s.;.\#..n0.1Q.
+000433e0: 11ef b362 564b 0da8 9318 6248 accf 87ae  ...bVK....bH....
+000433f0: 9042 3312 998b 56c6 f5bf 6c7d 255c f430  .B3...V...l}%\.0
+00043400: 4ea6 056d efc2 fbe0 7602 48b2 0852 c916  N..m....v.H..R..
+00043410: cf15 3afb 7afe c936 094a 8cde b4d0 4ea6  ..:.z..6.J....N.
+00043420: 86a6 5529 deb2 843c a183 e8c2 18a1 6f4f  ..U)...<......oO
+00043430: 2280 bc1a 6380 f88e 5e7a 7b36 b272 b76f  "...c...^z{6.r.o
+00043440: 776a a14c 846a 5cce 652c 3088 3565 5f46  wj.L.j\.e,0.5e_F
+00043450: 529b b99a 2836 c25c 0f8f 3a3e b0c7 734a  R...(6.\..:>..sJ
+00043460: 13ee 90ef f67d 87bd 1db0 7327 30ca 9774  .....}....s'0..t
+00043470: 4b4b 7db0 2bad 5ce4 f532 7764 0258 fa68  KK}.+.\..2wd.X.h
+00043480: 9605 6e71 8f97 35b0 6a32 99cc 8e69 a8db  ..nq..5.j2...i..
+00043490: 07d7 e21d 4423 1084 ed09 1343 03fa 3906  ....D#.....C..9.
+000434a0: dae3 188f dd93 9bca 4fee d0ba dc4b baff  ........O....K..
+000434b0: dfc5 0355 3cc4 4812 342f 6320 3287 d002  ...U<.H.4/c 2...
+000434c0: 157a 5618 0c7a c750 059a a4a1 e52e 01ce  .zV..z.P........
+000434d0: d634 1a51 6a8a df48 a497 bb78 aa54 6e23  .4.Qj..H...x.Tn#
+000434e0: 3bfc b7f4 ea63 700d 98ed 564e b1db 1440  ;....cp...VN...@
+000434f0: 2d25 8537 5029 38f6 5c1e b8ac 7ab5 a1b1  -%.7P)8.\...z...
+00043500: 0d62 ec73 6638 138c 6619 c896 d588 32d5  .b.sf8..f.....2.
+00043510: 454a 8d97 072c d39d b19c 35a7 54c5 aee0  EJ...,....5.T...
+00043520: 1612 7722 0a8d 5e03 8d5c b085 2f2d dbc8  ..w"..^..\../-..
+00043530: 798e d41a 8e5f 60f4 99ab e0d1 565e 3e1c  y...._`.....V^>.
+00043540: 5b08 b8ae 74be 34b0 2d3a 027c 98b1 704d  [...t.4.-:.|..pM
+00043550: 2fc8 002d efe3 8f6f fb3f 8c2e dc42 6a4f  /..-...o.?...BjO
+00043560: b1ae d575 194a 4f23 3e65 4236 6482 4bae  ...u.JO#>eB6d.K.
+00043570: 5fcc fc1f 726a b30c 8e60 d238 973b bb6a  _...rj...`.8.;.j
+00043580: 9071 05f8 8bad 7fac b258 6fc6 e966 c004  .q.......Xo..f..
+00043590: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
+000435a0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 000435b0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 000435c0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 000435d0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-000435e0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
-000435f0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-00043600: 8b48 892c a720 8a09 3c68 c9ec a624 913d  .H.,. ..<h...$.=
-00043610: a1b1 c053 d6a1 4715 8f94 2cf5 e5b6 9dd0  ...S..G...,.....
-00043620: 6071 a3a3 e7ad 7fac b258 6fc6 e966 c004  `q.......Xo..f..
+000435e0: 8b48 892c a720 8a09 3c68 c9ec a624 913d  .H.,. ..<h...$.=
+000435f0: a1b1 c053 d6a1 4715 8f94 2cf5 e5b6 9dd0  ...S..G...,.....
+00043600: 6071 a3a3 e7ad 7fac b258 6fc6 e966 c004  `q.......Xo..f..
+00043610: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
+00043620: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00043630: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00043640: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00043650: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-00043660: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
-00043670: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
-00043680: 8b48 892c a768 0fed f017 e3c5 e5eb bac6  .H.,.h..........
-00043690: 1cfc d714 7ddb 5b1a eb97 caba dc97 c871  ....}.[........q
-000436a0: 7a19 bdf8 8bc1 649e cd3b 34cb 1aef 5e2a  z.....d..;4...^*
-000436b0: a9e7 cb16 5abd 6094 ef37 8d40 89a2 7dcf  ....Z.`..7.@..}.
-000436c0: 4284 8a2d 78e7 6b8d 989e 951a f0e6 08d9  B..-x.k.........
-000436d0: 3bb4 82f0 437f 5c8f 4645 0e7a 89b8 1de5  ;...C.\.FE.z....
-000436e0: a918 79c4 371a 0ab6 23f4 fe42 dc34 cd47  ..y.7...#..B.4.G
-000436f0: ee97 edaf e34f 7e82 7917 7a9c dae4 cfa6  .....O~.y.z.....
-00043700: 1358 005e e748 5699 a975 7441 ba23 82bb  .X.^.HV..utA.#..
-00043710: 2f78 6827 96d5 3891 bbc0 d11b fa70 4a45  /xh'..8......pJE
-00043720: 5528 5c68 56cb 7264 8fcb 1ab5 33f0 fd91  U(\hV.rd....3...
-00043730: 2215 5f4f 4670 620b 6407 60df bb94 84c5  "._OFpb.d.`.....
-00043740: 93be 278d 9af9 364c 297f fb19 8bf5 e65c  ..'...6L)......\
-00043750: e0fb c092 0740 1fc6 240a 32de 478d 1f45  .....@..$.2.G..E
-00043760: 9655 ed95 a33d 33a8 2615 7968 aca4 fcf6  .U...=3.&.yh....
-00043770: 1b57 e452 429f 202d 1cb9 3772 edab fdeb  .W.RB. -..7r....
-00043780: 3fee 80e6 65da 7ab8 639b 6984 cbc2 18e9  ?...e.z.c.i.....
-00043790: fa87 0cf0 ba2d b902 6980 8700 10e3 d51a  .....-..i.......
-000437a0: e352 80f3 2348 1bc6 f638 b620 233c 6b45  .R..#H...8. #<kE
-000437b0: 3c3a fcef 8d2c 4eae 05da 6b34 6b81 9ade  <:...,N...k4k...
-000437c0: 8210 a71a adf1 9091 f427 6aa3 f477 3999  .........'j..w9.
-000437d0: 2cbf 07a0 074b 8b23 71ca 4f41 0dfd 6fc8  ,....K.#q.OA..o.
-000437e0: bb76 e290 f803 8c7e 424f 6f8e 66bf 4979  .v.....~BOo.f.Iy
-000437f0: fcaf 6081 8979 f821 81ef c907 c8fc 71bf  ..`..y.!......q.
-00043800: 2bb1 d465 b670 a5f0 5238 2094 bb50 9fbb  +..e.p..R8 ..P..
-00043810: c861 e2af 75fe e2bf df6c 7b20 60d7 7d20  .a..u....l{ `.} 
-00043820: c808 b8f6 6f26 1a0b 9751 0135 a8c2 2ff7  ....o&...Q.5../.
-00043830: c51f 5665 d81e cffa c05b 3a61 9a00 ab7d  ..Ve.....[:a...}
-00043840: 0802 ae7c ccab afb5 7e3d fcb4 0d6a f69f  ...|....~=...j..
-00043850: e68a ff21 0e7b b79a 01da 552e 2296 a808  ...!.{....U."...
-00043860: cea1 3ad2 c5fa de0c 0100 0000 0c00 0000  ..:.............
-00043870: 00fa de71 7100 0001 043c 3f78 6d6c 2076  ...qq....<?xml v
-00043880: 6572 7369 6f6e 3d22 312e 3022 2065 6e63  ersion="1.0" enc
-00043890: 6f64 696e 673d 2255 5446 2d38 223f 3e0a  oding="UTF-8"?>.
-000438a0: 3c21 444f 4354 5950 4520 706c 6973 7420  <!DOCTYPE plist 
-000438b0: 5055 424c 4943 2022 2d2f 2f41 7070 6c65  PUBLIC "-//Apple
-000438c0: 2f2f 4454 4420 504c 4953 5420 312e 302f  //DTD PLIST 1.0/
-000438d0: 2f45 4e22 2022 6874 7470 3a2f 2f77 7777  /EN" "http://www
-000438e0: 2e61 7070 6c65 2e63 6f6d 2f44 5444 732f  .apple.com/DTDs/
-000438f0: 5072 6f70 6572 7479 4c69 7374 2d31 2e30  PropertyList-1.0
-00043900: 2e64 7464 223e 0a3c 706c 6973 7420 7665  .dtd">.<plist ve
-00043910: 7273 696f 6e3d 2231 2e30 223e 0a3c 6469  rsion="1.0">.<di
-00043920: 6374 3e0a 093c 6b65 793e 636f 6d2e 6170  ct>..<key>com.ap
-00043930: 706c 652e 6170 706c 6963 6174 696f 6e2d  ple.application-
-00043940: 6964 656e 7469 6669 6572 3c2f 6b65 793e  identifier</key>
-00043950: 0a09 3c73 7472 696e 673e 3c2f 7374 7269  ..<string></stri
-00043960: 6e67 3e0a 3c2f 6469 6374 3e0a 3c2f 706c  ng>.</dict>.</pl
-00043970: 6973 743e 0afa de0b 0100 0000 0800 0000  ist>............
+00043660: 8b48 892c a768 0fed f017 e3c5 e5eb bac6  .H.,.h..........
+00043670: 1cfc d714 7ddb 5b1a eb97 caba dc97 c871  ....}.[........q
+00043680: 7a19 bdf8 8bc1 649e cd3b 34cb 1aef 5e2a  z.....d..;4...^*
+00043690: a9e7 cb16 5abd 6094 ef37 8d40 89a2 7dcf  ....Z.`..7.@..}.
+000436a0: 4284 8a2d 789c 24c8 4010 7801 bacd 95de  B..-x.$.@.x.....
+000436b0: 1da7 09c9 0ec8 e26c 086d 40b8 8804 f8d0  .......l.m@.....
+000436c0: 70d6 627f 3810 a813 a117 35ca c456 cd4a  p.b.8.....5..V.J
+000436d0: eb43 5319 a979 c2d6 fd52 2ca0 1a08 8cd0  .CS..y...R,.....
+000436e0: 95bb fe13 6cc6 89fb 7a89 9bd5 6a5b 2f19  ....l...z...j[/.
+000436f0: a2d9 efde 2501 5b47 bf74 5b9e 808e 89fe  ....%.[G.t[.....
+00043700: ecdc 0ca0 ca3a 917d f16c 33ba 34bf 7456  .....:.}.l3.4.tV
+00043710: 0044 053c e4f4 171b 0dc7 b980 3815 f671  .D.<........8..q
+00043720: 3bdd 261d 7154 d16f dfee 7cd8 1af8 ae48  ;.&.qT.o..|....H
+00043730: c196 2296 6af7 7b98 bc56 347f 9cb3 b8b9  ..".j.{..V4.....
+00043740: 7ebe 9dc5 1e32 59b3 7485 c991 d1a9 05d6  ~....2Y.t.......
+00043750: 2034 8f24 7b3c 90d3 129d ff29 d41c f905   4.${<.....)....
+00043760: 2bc3 0af1 07e4 44f6 e650 768b b0e2 e743  +.....D..Pv....C
+00043770: 9885 bded bbea 2827 8ca8 7446 7e01 1ba8  ......('..tF~...
+00043780: c952 bb18 d048 1bc6 f638 b620 233c 6b45  .R...H...8. #<kE
+00043790: 3c3a fcef 8d2c 4eae 05da 6b34 6b81 9ade  <:...,N...k4k...
+000437a0: 8210 a71a ad91 585d 759c b2cc 10b2 0fa2  ......X]u.......
+000437b0: 0632 7400 abad 73b9 5b45 363f 081e 4b90  .2t...s.[E6?..K.
+000437c0: 6b1a d2ac b656 d7b9 5f17 8782 fbfb 140f  k....V.._.......
+000437d0: 0ee8 530e e42e 10af b3c3 3f77 7b53 b512  ..S.......?w{S..
+000437e0: 4d5e 6cad 8998 01c0 a831 f452 320b 04ec  M^l......1.R2...
+000437f0: 5ff3 09b7 8ea9 b6ae 5058 60dc d0d0 2e80  _.......PX`.....
+00043800: 994e fc16 f7df c457 422c a455 75d5 f217  .N.....WB,.Uu...
+00043810: 33f8 c490 70c8 31ef a56c e6a6 c4ba fe8f  3...p.1..l......
+00043820: dff4 bf31 e810 9c9b 128a e0ee f3b4 fae7  ...1............
+00043830: 8e4e 0338 49fd c91c 6688 387a 3e3b 4cd9  .N.8I...f.8z>;L.
+00043840: cb01 49ec 5ffa de0c 0100 0000 0c00 0000  ..I._...........
+00043850: 00fa de71 7100 0001 043c 3f78 6d6c 2076  ...qq....<?xml v
+00043860: 6572 7369 6f6e 3d22 312e 3022 2065 6e63  ersion="1.0" enc
+00043870: 6f64 696e 673d 2255 5446 2d38 223f 3e0a  oding="UTF-8"?>.
+00043880: 3c21 444f 4354 5950 4520 706c 6973 7420  <!DOCTYPE plist 
+00043890: 5055 424c 4943 2022 2d2f 2f41 7070 6c65  PUBLIC "-//Apple
+000438a0: 2f2f 4454 4420 504c 4953 5420 312e 302f  //DTD PLIST 1.0/
+000438b0: 2f45 4e22 2022 6874 7470 3a2f 2f77 7777  /EN" "http://www
+000438c0: 2e61 7070 6c65 2e63 6f6d 2f44 5444 732f  .apple.com/DTDs/
+000438d0: 5072 6f70 6572 7479 4c69 7374 2d31 2e30  PropertyList-1.0
+000438e0: 2e64 7464 223e 0a3c 706c 6973 7420 7665  .dtd">.<plist ve
+000438f0: 7273 696f 6e3d 2231 2e30 223e 0a3c 6469  rsion="1.0">.<di
+00043900: 6374 3e0a 093c 6b65 793e 636f 6d2e 6170  ct>..<key>com.ap
+00043910: 706c 652e 6170 706c 6963 6174 696f 6e2d  ple.application-
+00043920: 6964 656e 7469 6669 6572 3c2f 6b65 793e  identifier</key>
+00043930: 0a09 3c73 7472 696e 673e 3c2f 7374 7269  ..<string></stri
+00043940: 6e67 3e0a 3c2f 6469 6374 3e0a 3c2f 706c  ng>.</dict>.</pl
+00043950: 6973 743e 0afa de0b 0100 0000 0800 0000  ist>............
+00043960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00043970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00043980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00043990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000439a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000439b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000439c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000439d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000439e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -18513,16 +18513,16 @@
 00048500: a009 0300 9017 0000 0200 0000 1800 0000  ................
 00048510: 8023 0300 2f08 0000 20aa 0300 3044 0000  .#../... ...0D..
 00048520: 0b00 0000 5000 0000 0000 0000 8a06 0000  ....P...........
 00048530: 8a06 0000 2b01 0000 b507 0000 7a00 0000  ....+.......z...
 00048540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00048550: 0000 0000 0000 0000 70a6 0300 eb00 0000  ........p.......
 00048560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00048570: 1b00 0000 1800 0000 7028 c13b f4f3 335b  ........p(.;..3[
-00048580: 80cf 92d6 52b5 e4ec 3200 0000 2000 0000  ....R...2... ...
+00048570: 1b00 0000 1800 0000 d89f 72ff 4b5d 31fe  ..........r.K]1.
+00048580: 9af9 4a87 978e 1130 3200 0000 2000 0000  ..J....02... ...
 00048590: 0100 0000 0001 0c00 0001 0d00 0100 0000  ................
 000485a0: 0300 0000 0001 3403 2a00 0000 1000 0000  ......4.*.......
 000485b0: 0000 0000 0000 0000 0c00 0000 3800 0000  ............8...
 000485c0: 1800 0000 0200 0000 0000 2705 0000 0100  ..........'.....
 000485d0: 2f75 7372 2f6c 6962 2f6c 6962 5379 7374  /usr/lib/libSyst
 000485e0: 656d 2e42 2e64 796c 6962 0000 0000 0000  em.B.dylib......
 000485f0: 0c00 0000 6800 0000 1800 0000 0200 0000  ....h...........
@@ -22251,19 +22251,19 @@
 00056ea0: 0800 0014 029e 0b30 1f20 03d5 6393 0b70  .......0. ..c..p
 00056eb0: 1f20 03d5 2000 8012 e103 13aa 2421 8052  . .. .......$!.R
 00056ec0: fd7b 43a9 f44f 42a9 f657 41a9 f85f c4a8  .{C..OB..WA.._..
 00056ed0: 55ee ff17 8866 40b9 e903 152a 29a1 01d1  U....f@....*)...
 00056ee0: 3f01 08eb e009 0054 8294 0b70 1f20 03d5  ?......T...p. ..
 00056ef0: 4391 0b70 1f20 03d5 2000 8012 e103 13aa  C..p. .. .......
 00056f00: 641b 8052 efff ff17 1604 0037 a802 4039  d..R.......7..@9
-00056f10: c803 0034 e003 15aa b956 0094 c862 9a52  ...4.....V...b.R
+00056f10: c803 0034 e003 15aa b956 0094 e866 9a52  ...4.....V...f.R
 00056f20: 1f00 086b 2b03 0054 4295 0b50 1f20 03d5  ...k+..TB..P. ..
 00056f30: 438f 0b70 1f20 03d5 8000 8012 e103 13aa  C..p. ..........
 00056f40: 641f 8052 dfff ff17 7603 0037 e802 4039  d..R....v..7..@9
-00056f50: 2803 0034 e003 17aa a956 0094 c862 9a52  (..4.....V...b.R
+00056f50: 2803 0034 e003 17aa a956 0094 e866 9a52  (..4.....V...f.R
 00056f60: 1f00 086b 8b02 0054 4293 0b50 1f20 03d5  ...k...TB..P. ..
 00056f70: 438d 0b70 1f20 03d5 8000 8012 e103 13aa  C..p. ..........
 00056f80: e41c 8052 cfff ff17 881a 4239 1f45 0071  ...R......B9.E.q
 00056f90: 8302 0054 6294 0b70 1f20 03d5 e38b 0b70  ...Tb..p. .....p
 00056fa0: 1f20 03d5 2000 8012 e103 13aa 0420 8052  . .. ........ .R
 00056fb0: c4ff ff17 887a 40b9 1f45 0071 8302 0054  .....z@..E.q...T
 00056fc0: e28c 0b70 1f20 03d5 838a 0b70 1f20 03d5  ...p. .....p. ..
@@ -28529,17 +28529,17 @@
 0006f700: 6265 6163 6f6e 0069 6e64 6578 0062 6173  beacon.index.bas
 0006f710: 6554 7970 6500 6861 7264 7761 7265 4964  eType.hardwareId
 0006f720: 0061 6476 6572 7469 7365 6456 616c 7565  .advertisedValue
 0006f730: 0044 6973 6162 6c65 204a 5a4f 4e20 656e  .Disable JZON en
 0006f740: 636f 6469 6e67 2066 6f72 2068 7562 2025  coding for hub %
 0006f750: 0a00 456e 756d 6572 6174 696f 6e20 6661  ..Enumeration fa
 0006f760: 696c 6564 2066 6f72 2025 733a 2564 2028  iled for %s:%d (
-0006f770: 2573 2900 312e 3130 2e35 3430 3337 0041  %s).1.10.54037.A
-0006f780: 7072 2031 3320 3230 3233 2031 393a 3032  pr 13 2023 19:02
-0006f790: 3a30 3100 596f 6374 6f70 7563 6500 2573  :01.Yoctopuce.%s
+0006f770: 2573 2900 312e 3130 2e35 3430 3730 0041  %s).1.10.54070.A
+0006f780: 7072 2031 3720 3230 3233 2032 323a 3533  pr 17 2023 22:53
+0006f790: 3a32 3000 596f 6374 6f70 7563 6500 2573  :20.Yoctopuce.%s
 0006f7a0: 3a2f 2f25 733a 2564 2573 2573 004e 6f20  ://%s:%d%s%s.No 
 0006f7b0: 6675 6e63 7469 6f6e 206f 6620 7468 6174  function of that
 0006f7c0: 2063 6c61 7373 0041 5379 6e63 2072 6571   class.ASync req
 0006f7d0: 7565 7374 2066 6f72 2025 7320 6661 696c  uest for %s fail
 0006f7e0: 6564 2e20 5265 7472 7969 6e67 2061 6674  ed. Retrying aft
 0006f7f0: 6572 2079 6170 6955 7064 6174 6544 6576  er yapiUpdateDev
 0006f800: 6963 654c 6973 740a 0079 6170 6955 7064  iceList..yapiUpd
@@ -31392,15 +31392,15 @@
 0007a9f0: 1622 0000 0e0b 0000 b2d2 0600 0000 0000  ."..............
 0007aa00: 2222 0000 0e0b 0000 d4d2 0600 0000 0000  ""..............
 0007aa10: 2f22 0000 0e0b 0000 d8d2 0600 0000 0000  /"..............
 0007aa20: 4822 0000 0e0b 0000 e0d2 0600 0000 0000  H"..............
 0007aa30: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007aa40: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007aa50: 9922 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-0007aa60: a322 0000 6600 0100 8835 3864 0000 0000  ."..f....58d....
+0007aa60: a322 0000 6600 0100 bfb1 3d64 0000 0000  ."..f.....=d....
 0007aa70: 0100 0000 2e01 0000 0843 0000 0000 0000  .........C......
 0007aa80: 3723 0000 2401 0000 0843 0000 0000 0000  7#..$....C......
 0007aa90: 0100 0000 2400 0000 0800 0000 0000 0000  ....$...........
 0007aaa0: 0100 0000 4e01 0000 0843 0000 0000 0000  ....N....C......
 0007aab0: 0100 0000 2e01 0000 1043 0000 0000 0000  .........C......
 0007aac0: 4223 0000 2401 0000 1043 0000 0000 0000  B#..$....C......
 0007aad0: 0100 0000 2400 0000 1401 0000 0000 0000  ....$...........
@@ -31432,15 +31432,15 @@
 0007ac70: 0100 0000 2e01 0000 3846 0000 0000 0000  ........8F......
 0007ac80: 9523 0000 2401 0000 3846 0000 0000 0000  .#..$...8F......
 0007ac90: 0100 0000 2400 0000 9000 0000 0000 0000  ....$...........
 0007aca0: 0100 0000 4e01 0000 3846 0000 0000 0000  ....N...8F......
 0007acb0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007acc0: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007acd0: 9f23 0000 6400 0000 0000 0000 0000 0000  .#..d...........
-0007ace0: a623 0000 6600 0100 8835 3864 0000 0000  .#..f....58d....
+0007ace0: a623 0000 6600 0100 c0b1 3d64 0000 0000  .#..f.....=d....
 0007acf0: 0100 0000 2e01 0000 c846 0000 0000 0000  .........F......
 0007ad00: 3724 0000 2401 0000 c846 0000 0000 0000  7$..$....F......
 0007ad10: 0100 0000 2400 0000 7400 0000 0000 0000  ....$...t.......
 0007ad20: 0100 0000 4e01 0000 c846 0000 0000 0000  ....N....F......
 0007ad30: 0100 0000 2e01 0000 3c47 0000 0000 0000  ........<G......
 0007ad40: 4024 0000 2401 0000 3c47 0000 0000 0000  @$..$...<G......
 0007ad50: 0100 0000 2400 0000 6c00 0000 0000 0000  ....$...l.......
@@ -31615,15 +31615,15 @@
 0007b7e0: 0100 0000 4e01 0000 88a2 0000 0000 0000  ....N...........
 0007b7f0: a626 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
 0007b800: b026 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
 0007b810: c226 0000 2000 0000 0000 0000 0000 0000  .&.. ...........
 0007b820: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007b830: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007b840: d226 0000 6400 0000 0000 0000 0000 0000  .&..d...........
-0007b850: dc26 0000 6600 0100 8835 3864 0000 0000  .&..f....58d....
+0007b850: dc26 0000 6600 0100 bfb1 3d64 0000 0000  .&..f.....=d....
 0007b860: 0100 0000 2e01 0000 24a8 0000 0000 0000  ........$.......
 0007b870: 7027 0000 2401 0000 24a8 0000 0000 0000  p'..$...$.......
 0007b880: 0100 0000 2400 0000 8400 0000 0000 0000  ....$...........
 0007b890: 0100 0000 4e01 0000 24a8 0000 0000 0000  ....N...$.......
 0007b8a0: 0100 0000 2e01 0000 a8a8 0000 0000 0000  ................
 0007b8b0: 7927 0000 2401 0000 a8a8 0000 0000 0000  y'..$...........
 0007b8c0: 0100 0000 2400 0000 7800 0000 0000 0000  ....$...x.......
@@ -31830,15 +31830,15 @@
 0007c550: 0100 0000 4e01 0000 4ce6 0000 0000 0000  ....N...L.......
 0007c560: 732a 0000 2604 0000 e878 0200 0000 0000  s*..&....x......
 0007c570: 7b2a 0000 2000 0000 0000 0000 0000 0000  {*.. ...........
 0007c580: 852a 0000 2000 0000 0000 0000 0000 0000  .*.. ...........
 0007c590: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007c5a0: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007c5b0: 912a 0000 6400 0000 0000 0000 0000 0000  .*..d...........
-0007c5c0: 992a 0000 6600 0100 8835 3864 0000 0000  .*..f....58d....
+0007c5c0: 992a 0000 6600 0100 bfb1 3d64 0000 0000  .*..f.....=d....
 0007c5d0: 0100 0000 2e01 0000 c4ea 0000 0000 0000  ................
 0007c5e0: 2b2b 0000 2401 0000 c4ea 0000 0000 0000  ++..$...........
 0007c5f0: 0100 0000 2400 0000 9800 0000 0000 0000  ....$...........
 0007c600: 0100 0000 4e01 0000 c4ea 0000 0000 0000  ....N...........
 0007c610: 0100 0000 2e01 0000 5ceb 0000 0000 0000  ........\.......
 0007c620: 362b 0000 2401 0000 5ceb 0000 0000 0000  6+..$...\.......
 0007c630: 0100 0000 2400 0000 0c01 0000 0000 0000  ....$...........
@@ -31953,27 +31953,27 @@
 0007cd00: 0100 0000 4e01 0000 382d 0100 0000 0000  ....N...8-......
 0007cd10: 3d2d 0000 2000 0000 0000 0000 0000 0000  =-.. ...........
 0007cd20: 432d 0000 2000 0000 0000 0000 0000 0000  C-.. ...........
 0007cd30: 4d2d 0000 2000 0000 0000 0000 0000 0000  M-.. ...........
 0007cd40: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007cd50: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007cd60: 572d 0000 6400 0000 0000 0000 0000 0000  W-..d...........
-0007cd70: 5f2d 0000 6600 0100 8835 3864 0000 0000  _-..f....58d....
+0007cd70: 5f2d 0000 6600 0100 c0b1 3d64 0000 0000  _-..f.....=d....
 0007cd80: 0100 0000 2e01 0000 082e 0100 0000 0000  ................
 0007cd90: f12d 0000 2401 0000 082e 0100 0000 0000  .-..$...........
 0007cda0: 0100 0000 2400 0000 b008 0000 0000 0000  ....$...........
 0007cdb0: 0100 0000 4e01 0000 082e 0100 0000 0000  ....N...........
 0007cdc0: 0100 0000 2e01 0000 b836 0100 0000 0000  .........6......
 0007cdd0: fd2d 0000 2401 0000 b836 0100 0000 0000  .-..$....6......
 0007cde0: 0100 0000 2400 0000 1000 0000 0000 0000  ....$...........
 0007cdf0: 0100 0000 4e01 0000 b836 0100 0000 0000  ....N....6......
 0007ce00: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007ce10: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007ce20: 082e 0000 6400 0000 0000 0000 0000 0000  ....d...........
-0007ce30: 0f2e 0000 6600 0100 8935 3864 0000 0000  ....f....58d....
+0007ce30: 0f2e 0000 6600 0100 c0b1 3d64 0000 0000  ....f.....=d....
 0007ce40: 0100 0000 2e01 0000 c836 0100 0000 0000  .........6......
 0007ce50: a02e 0000 2401 0000 c836 0100 0000 0000  ....$....6......
 0007ce60: 0100 0000 2400 0000 6400 0000 0000 0000  ....$...d.......
 0007ce70: 0100 0000 4e01 0000 c836 0100 0000 0000  ....N....6......
 0007ce80: 0100 0000 2e01 0000 2c37 0100 0000 0000  ........,7......
 0007ce90: a92e 0000 2401 0000 2c37 0100 0000 0000  ....$...,7......
 0007cea0: 0100 0000 2400 0000 c400 0000 0000 0000  ....$...........
@@ -32035,15 +32035,15 @@
 0007d220: 0100 0000 2400 0000 e409 0000 0000 0000  ....$...........
 0007d230: 0100 0000 4e01 0000 9c49 0100 0000 0000  ....N....I......
 0007d240: 7e2f 0000 2000 0000 0000 0000 0000 0000  ~/.. ...........
 0007d250: 892f 0000 2609 0000 00c0 0200 0000 0000  ./..&...........
 0007d260: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007d270: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007d280: 8f2f 0000 6400 0000 0000 0000 0000 0000  ./..d...........
-0007d290: 972f 0000 6600 0100 8935 3864 0000 0000  ./..f....58d....
+0007d290: 972f 0000 6600 0100 c0b1 3d64 0000 0000  ./..f.....=d....
 0007d2a0: 0100 0000 2e01 0000 8053 0100 0000 0000  .........S......
 0007d2b0: 2930 0000 2401 0000 8053 0100 0000 0000  )0..$....S......
 0007d2c0: 0100 0000 2400 0000 3400 0000 0000 0000  ....$...4.......
 0007d2d0: 0100 0000 4e01 0000 8053 0100 0000 0000  ....N....S......
 0007d2e0: 0100 0000 2e01 0000 b453 0100 0000 0000  .........S......
 0007d2f0: 3930 0000 2401 0000 b453 0100 0000 0000  90..$....S......
 0007d300: 0100 0000 2400 0000 3c00 0000 0000 0000  ....$...<.......
@@ -32217,15 +32217,15 @@
 0007dd80: 2b33 0000 260b 0000 b0d2 0600 0000 0000  +3..&...........
 0007dd90: 3733 0000 260b 0000 b2d2 0600 0000 0000  73..&...........
 0007dda0: 4333 0000 260b 0000 d4d2 0600 0000 0000  C3..&...........
 0007ddb0: 5033 0000 260b 0000 d8d2 0600 0000 0000  P3..&...........
 0007ddc0: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007ddd0: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007dde0: 6933 0000 6400 0000 0000 0000 0000 0000  i3..d...........
-0007ddf0: 7433 0000 6600 0100 8835 3864 0000 0000  t3..f....58d....
+0007ddf0: 7433 0000 6600 0100 bfb1 3d64 0000 0000  t3..f.....=d....
 0007de00: 0100 0000 2e01 0000 0c87 0100 0000 0000  ................
 0007de10: 0934 0000 2401 0000 0c87 0100 0000 0000  .4..$...........
 0007de20: 0100 0000 2400 0000 2c02 0000 0000 0000  ....$...,.......
 0007de30: 0100 0000 4e01 0000 0c87 0100 0000 0000  ....N...........
 0007de40: 0100 0000 2e01 0000 3889 0100 0000 0000  ........8.......
 0007de50: 1634 0000 2401 0000 3889 0100 0000 0000  .4..$...8.......
 0007de60: 0100 0000 2400 0000 c400 0000 0000 0000  ....$...........
@@ -32277,15 +32277,15 @@
 0007e140: 0100 0000 2e01 0000 4c94 0100 0000 0000  ........L.......
 0007e150: e934 0000 2401 0000 4c94 0100 0000 0000  .4..$...L.......
 0007e160: 0100 0000 2400 0000 fc00 0000 0000 0000  ....$...........
 0007e170: 0100 0000 4e01 0000 4c94 0100 0000 0000  ....N...L.......
 0007e180: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 0007e190: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 0007e1a0: fc34 0000 6400 0000 0000 0000 0000 0000  .4..d...........
-0007e1b0: 0335 0000 6600 0100 8935 3864 0000 0000  .5..f....58d....
+0007e1b0: 0335 0000 6600 0100 c1b1 3d64 0000 0000  .5..f.....=d....
 0007e1c0: 0100 0000 2e01 0000 4895 0100 0000 0000  ........H.......
 0007e1d0: 9435 0000 2401 0000 4895 0100 0000 0000  .5..$...H.......
 0007e1e0: 0100 0000 2400 0000 1c00 0000 0000 0000  ....$...........
 0007e1f0: 0100 0000 4e01 0000 4895 0100 0000 0000  ....N...H.......
 0007e200: 0100 0000 2e01 0000 6495 0100 0000 0000  ........d.......
 0007e210: ae35 0000 2401 0000 6495 0100 0000 0000  .5..$...d.......
 0007e220: 0100 0000 2400 0000 7400 0000 0000 0000  ....$...t.......
@@ -32767,15 +32767,15 @@
 0007ffe0: 0100 0000 2400 0000 0400 0000 0000 0000  ....$...........
 0007fff0: 0100 0000 4e01 0000 0839 0200 0000 0000  ....N....9......
 00080000: ca3f 0000 2000 0000 0000 0000 0000 0000  .?.. ...........
 00080010: e43f 0000 2000 0000 0000 0000 0000 0000  .?.. ...........
 00080020: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 00080030: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 00080040: f83f 0000 6400 0000 0000 0000 0000 0000  .?..d...........
-00080050: 0040 0000 6600 0100 8935 3864 0000 0000  .@..f....58d....
+00080050: 0040 0000 6600 0100 c0b1 3d64 0000 0000  .@..f.....=d....
 00080060: 0100 0000 2e01 0000 0c39 0200 0000 0000  .........9......
 00080070: 9240 0000 2401 0000 0c39 0200 0000 0000  .@..$....9......
 00080080: 0100 0000 2400 0000 2400 0000 0000 0000  ....$...$.......
 00080090: 0100 0000 4e01 0000 0c39 0200 0000 0000  ....N....9......
 000800a0: 0100 0000 2e01 0000 3039 0200 0000 0000  ........09......
 000800b0: 9f40 0000 2401 0000 3039 0200 0000 0000  .@..$...09......
 000800c0: 0100 0000 2400 0000 3000 0000 0000 0000  ....$...0.......
@@ -32863,15 +32863,15 @@
 000805e0: 0100 0000 2e01 0000 d840 0200 0000 0000  .........@......
 000805f0: bc41 0000 2401 0000 d840 0200 0000 0000  .A..$....@......
 00080600: 0100 0000 2400 0000 3002 0000 0000 0000  ....$...0.......
 00080610: 0100 0000 4e01 0000 d840 0200 0000 0000  ....N....@......
 00080620: 0100 0000 6401 0000 0000 0000 0000 0000  ....d...........
 00080630: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 00080640: ca41 0000 6400 0000 0000 0000 0000 0000  .A..d...........
-00080650: d441 0000 6600 0100 8835 3864 0000 0000  .A..f....58d....
+00080650: d441 0000 6600 0100 bfb1 3d64 0000 0000  .A..f.....=d....
 00080660: 0100 0000 2e01 0000 0843 0200 0000 0000  .........C......
 00080670: 6842 0000 2401 0000 0843 0200 0000 0000  hB..$....C......
 00080680: 0100 0000 2400 0000 3c00 0000 0000 0000  ....$...<.......
 00080690: 0100 0000 4e01 0000 0843 0200 0000 0000  ....N....C......
 000806a0: 0100 0000 2e01 0000 4443 0200 0000 0000  ........DC......
 000806b0: 7642 0000 2401 0000 4443 0200 0000 0000  vB..$...DC......
 000806c0: 0100 0000 2400 0000 4000 0000 0000 0000  ....$...@.......
@@ -34536,29 +34536,29 @@
 00086e70: 0000 0941 0001 0000 0000 0a45 fade 0c02  ...A.......E....
 00086e80: 0000 0909 0002 0400 0000 0002 0000 0129  ...............)
 00086e90: 0000 0058 0000 0005 0000 003f 0003 ee50  ...X.......?...P
 00086ea0: 2002 000c 0000 0000 0000 0000 0000 0000   ...............
 00086eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00086ec0: 0000 0000 0000 0000 0002 8000 0000 0000  ................
 00086ed0: 0000 0000 6c69 6279 6170 692d 3535 3535  ....libyapi-5555
-00086ee0: 3439 3434 6166 3366 3566 3961 3031 3365  4944af3f5f9a013e
-00086ef0: 3363 3566 6263 6534 3336 3762 3634 3262  3c5fbce4367b642b
-00086f00: 3230 3335 00c6 dc9c 8e50 8ccb 383c 8c74  2035.....P..8<.t
+00086ee0: 3439 3434 3565 3765 3239 3533 6231 3861  49445e7e2953b18a
+00086ef0: 3334 3037 6262 3063 6236 3966 3537 3636  3407bb0cb69f5766
+00086f00: 6637 6637 00c6 dc9c 8e50 8ccb 383c 8c74  f7f7.....P..8<.t
 00086f10: 84e8 3d73 a81a c271 ac0d c9ba 1ea2 efca  ..=s...q........
 00086f20: 12de fda0 c600 0000 0000 0000 0000 0000  ................
 00086f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00086f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00086f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00086f60: 0000 0000 0098 7920 904e ab65 0e75 788c  ......y .N.e.ux.
 00086f70: 054a a0b0 524e 6a80 bfc7 1aa3 2df8 d237  .J..RNj.....-..7
 00086f80: a617 43f9 8600 0000 0000 0000 0000 0000  ..C.............
 00086f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00086fa0: 0000 0000 00cf 56db e449 157b 2253 f1f0  ......V..I.{"S..
-00086fb0: 9521 9389 6cc2 f627 1f01 118e 7f55 fcb7  .!..l..'.....U..
-00086fc0: ebac dfc4 d0ad 7fac b258 6fc6 e966 c004  .........Xo..f..
+00086fa0: 0000 0000 00ff 8e61 4c20 2d6a ee95 c69e  .......aL -j....
+00086fb0: ca96 6cb7 1c5e 49f1 5a49 1fcb 41d1 b94b  ..l..^I.ZI..A..K
+00086fc0: 0ea5 32b8 67ad 7fac b258 6fc6 e966 c004  ..2.g....Xo..f..
 00086fd0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00086fe0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00086ff0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00087000: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00087010: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00087020: 8b48 892c a76e ca70 026b 7fe2 a7fd 6d1f  .H.,.n.p.k....m.
 00087030: de24 682f 2cf0 6bab a3f7 3b6a 4cda b5e0  .$h/,.k...;jL...
@@ -34576,17 +34576,17 @@
 000870f0: 830f c95e ec5c 65f5 c24b 5bfa 39a1 013b  ...^.\e..K[.9..;
 00087100: ad4f 3d1b 887e 9b0f b5f3 686b 0e59 9de0  .O=..~....hk.Y..
 00087110: f489 6de7 9c6b 2964 46cb 319e 2870 6606  ..m..k)dF.1.(pf.
 00087120: 87bb 93c1 5964 c154 c8e2 b9d8 32da 0abb  ....Yd.T....2...
 00087130: 5ce0 d7e7 3182 dbd0 455c 6555 d61c 7a5e  \...1...E\eU..z^
 00087140: ce5a 443f 24bc b961 b551 b5d7 8bf1 ddcb  .ZD?$..a.Q......
 00087150: d3b7 791a 26c4 c8de e4cf 2ee7 55af 8218  ..y.&.......U...
-00087160: 9812 a82e 42c1 1c4d a771 e006 2bc3 81d2  ....B..M.q..+...
-00087170: 8fa7 4094 6cb3 b0a9 0a1f 655f 079f c86c  ..@.l.....e_...l
-00087180: b0e5 c24e 8320 c783 84f6 113d ec63 0f1a  ...N. .....=.c..
+00087160: 9812 a82e 4249 1773 6ff6 1186 b62e 7bba  ....BI.so.....{.
+00087170: 74af 2c4c b980 170a fec3 6371 112f 2536  t.,L......cq./%6
+00087180: a8a0 fbcc cd20 c783 84f6 113d ec63 0f1a  ..... .....=.c..
 00087190: 50be 3b34 f9a9 cea6 3ab8 b69d 31e0 c953  P.;4....:...1..S
 000871a0: 94d2 9a20 4342 50c4 40f0 d6f3 8e4a bc5a  ... CBP.@....J.Z
 000871b0: 80ce 5d1f c3ab b2ea 0d14 6484 cdac 60b3  ..].......d...`.
 000871c0: 81d3 3377 5d0d faa1 d84b 8464 1a9b b05e  ..3w]....K.d...^
 000871d0: 167f b418 9155 6778 e160 2bcb 9ce9 cbcf  .....Ugx.`+.....
 000871e0: e736 8132 4e0f a1b7 3fbf 2348 50c1 6876  .6.2N...?.#HP.hv
 000871f0: 98e3 b30f e7a3 872e 8462 3890 70dd 8e00  .........b8.p...
@@ -34626,17 +34626,17 @@
 00087410: fec2 8e46 5d92 2be5 849b 4173 6b63 eadd  ...F].+...Askc..
 00087420: e502 357b 6868 d3b9 8b0f 540a 7465 c5e5  ..5{hh....T.te..
 00087430: 2ed7 6bbc 4a9c 6add 6529 b05f 1dd5 d595  ..k.J.j.e)._....
 00087440: 60cc 430e 2bdc 81cb 6582 7f13 d81f 7567  `.C.+...e.....ug
 00087450: b48a eeaf 05f4 14ef b6e2 f301 10ee 5de1  ..............].
 00087460: 82a4 7056 4e0b f899 d649 85bd b7e1 18d8  ..pVN....I......
 00087470: 6dd9 084a 63e1 da7f e005 78ed 22a6 1364  m..Jc.....x."..d
-00087480: 630e fd2a 5ef8 2d9d 2828 70c2 e875 2720  c..*^.-.((p..u' 
-00087490: 7c02 ec9a 403f ccca 0556 299c aab6 e9b6  |...@?...V).....
-000874a0: bd6d 584b abc2 5911 53be 2c0f 09ee 11b2  .mXK..Y.S.,.....
+00087480: 630e fd2a 5ee7 784f 36c4 d2fd 83d7 32be  c..*^.xO6.....2.
+00087490: 8b74 b54d 7400 7f88 a63a a09a 81e2 c7c2  .t.Mt....:......
+000874a0: a551 86a8 99c2 5911 53be 2c0f 09ee 11b2  .Q....Y.S.,.....
 000874b0: f6b4 372b 57ac 6925 1301 3c30 31b0 2e60  ..7+W.i%..<01..`
 000874c0: 635e d8f4 30ad 7fac b258 6fc6 e966 c004  c^..0....Xo..f..
 000874d0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 000874e0: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 000874f0: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00087500: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00087510: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
@@ -34648,29 +34648,29 @@
 00087570: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 00087580: 8b48 892c a7ad 7fac b258 6fc6 e966 c004  .H.,.....Xo..f..
 00087590: d7d1 d16b 024f 5805 ff7c b47c 7a85 dabd  ...k.OX..|.|z...
 000875a0: 8b48 892c a790 d9f7 1992 4e3b 3d8e df4c  .H.,......N;=..L
 000875b0: 1b89 6ca4 e79d d1a5 907d eea2 841d 1399  ..l......}......
 000875c0: d852 63ef 0152 9c2a f894 8fc9 a1b3 4561  .Rc..R.*......Ea
 000875d0: 7ae1 dff9 22a7 45af 4eeb 9287 7ebc 6e59  z...".E.N...~.nY
-000875e0: 5258 ef32 7860 cc11 a017 ef36 2835 76e4  RX.2x`.....6(5v.
-000875f0: 2aa0 be44 f10e a5ee 7cd7 2ad2 1007 0308  *..D....|.*.....
-00087600: bdfa 153d fa22 d4eb 495b 3992 7778 d585  ...=."..I[9.wx..
-00087610: 7292 4917 71e1 71ea 8472 564f 6ba4 87bd  r.I.q.q..rVOk...
-00087620: a7bc d4c7 4c85 ab3a bd01 e46d 8926 d722  ....L..:...m.&."
-00087630: 52a6 aa8e da50 9601 9475 da9c a38f db26  R....P...u.....&
-00087640: 442c fe12 b0e9 b4eb cb26 6f8b 9795 ff6d  D,.......&o....m
-00087650: 1b44 ae59 37a2 f263 da2f a010 3e44 f7a8  .D.Y7..c./..>D..
-00087660: 3bfa 2612 2e42 7d53 1813 d2e0 c710 d987  ;.&..B}S........
-00087670: 13d8 3d90 157e 0868 85e8 8269 e060 bf51  ..=..~.h...i.`.Q
-00087680: 77d7 0217 2035 1833 058f 3c99 2b77 74a6  w... 5.3..<.+wt.
+000875e0: 5258 ef32 7841 d2ed 941c bca2 41e0 21ea  RX.2xA......A.!.
+000875f0: 839c 4a94 d651 d307 f8bb 977a c9bf b044  ..J..Q.....z...D
+00087600: f68d c798 7815 793c 3a32 1f81 e1d9 777d  ....x.y<:2....w}
+00087610: a024 b8aa d413 0541 d2a0 d7dd e851 c9db  .$.....A.....Q..
+00087620: 2fda e45a 5bb3 017c 9e49 9db5 ec48 c8f2  /..Z[..|.I...H..
+00087630: 1319 94b7 2cc6 a479 594c a9a9 b705 1117  ....,..yYL......
+00087640: 000f c76c 9a9b 6e74 9d65 5b24 5f37 145a  ...l..nt.e[$_7.Z
+00087650: 2663 3cfd e619 6e01 e38c f25a faeb 0b5d  &c<...n....Z...]
+00087660: c8da 9612 3e07 6fcf 8dee 58e1 baf9 febe  ....>.o...X.....
+00087670: 98c2 ecd3 b2dd 87df 3a6b 26db 1666 bac9  ........:k&..f..
+00087680: 52f0 058e c235 1833 058f 3c99 2b77 74a6  R....5.3..<.+wt.
 00087690: 397d 0a7a e4e5 43c2 e8d4 8557 b1db df24  9}.z..C....W...$
-000876a0: ceef 14c3 c0e9 53a4 3d6f e4f7 85c4 929d  ......S.=o......
-000876b0: 9cd7 ea52 b29b 719d da84 772f 193a 0b10  ...R..q...w/.:..
-000876c0: 660c da23 ee37 b246 ef83 33ec 6219 c732  f..#.7.F..3.b..2
+000876a0: ceef 14c3 c083 9062 56f0 ccf8 61a9 3d10  .......bV...a.=.
+000876b0: 0889 b00b cb9e b45e a085 4f2a d6eb 41de  .......^..O*..A.
+000876c0: 9040 aada 7337 b246 ef83 33ec 6219 c732  .@..s7.F..3.b..2
 000876d0: 89b5 14f7 a904 06d4 ec94 b867 6b30 bef7  ...........gk0..
 000876e0: 73c6 6067 d7d9 b853 3c98 c61b 8e51 30eb  s.`g...S<....Q0.
 000876f0: 8b99 b3be f22d 94b8 c775 e061 ff90 fd64  .....-...u.a...d
 00087700: 8876 fb6e ae20 b520 a04d db54 4466 c1ab  .v.n. . .M.TDf..
 00087710: 24af 7a9f f842 249c 56bd 3443 1560 6c4c  $.z..B$.V.4C.`lL
 00087720: 6dcf d243 be23 dd4e efee 2b4f 1019 6b69  m..C.#.N..+O..ki
 00087730: 3782 6597 adcb 4696 98c4 c849 6e07 cb12  7.e...F....In...
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/yapi.dll` & `yoctopuce-1.10.54070/yoctopuce/cdll/yapi.dll`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 00000090: b0e9 f7a9 ae82 f4a8 b0e9 f1a9 3982 f4a8  ............9...
 000000a0: b0e9 f0a9 b682 f4a8 9fdc f7a9 b282 f4a8  ................
 000000b0: 9fdc f1a9 bf82 f4a8 9fdc f0a9 b482 f4a8  ................
 000000c0: b0e9 f5a9 ad82 f4a8 a482 f5a8 2c82 f4a8  ............,...
 000000d0: 0edc fca9 aa82 f4a8 0edc f4a9 a582 f4a8  ................
 000000e0: 0edc 0ba8 a582 f4a8 0edc f6a9 a582 f4a8  ................
 000000f0: 5269 6368 a482 f4a8 0000 0000 0000 0000  Rich............
-00000100: 5045 0000 4c01 0600 f735 3864 0000 0000  PE..L....58d....
+00000100: 5045 0000 4c01 0600 30b2 3d64 0000 0000  PE..L...0.=d....
 00000110: 0000 0000 e000 0221 0b01 0e00 00e2 0300  .......!........
 00000120: 0024 0500 0000 0000 ed6d 0200 0010 0000  .$.......m......
 00000130: 0000 0400 0000 0010 0010 0000 0002 0000  ................
 00000140: 0600 0000 0000 0000 0600 0000 0000 0000  ................
-00000150: 0050 0900 0004 0000 e243 0500 0200 4001  .P.......C....@.
+00000150: 0050 0900 0004 0000 fe05 0600 0200 4001  .P............@.
 00000160: 0000 1000 0010 0000 0000 1000 0010 0000  ................
 00000170: 0000 0000 1000 0000 f09a 0400 3811 0000  ............8...
 00000180: 28ac 0400 6400 0000 0000 0900 7803 0000  (...d.......x...
 00000190: 0000 0000 0000 0000 00e8 0400 f82c 0000  .............,..
 000001a0: 0010 0900 5837 0000 f08f 0400 1c00 0000  ....X7..........
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 1090 0400 4000 0000  ............@...
@@ -17569,16 +17569,16 @@
 00044a00: 6861 7320 636c 6f73 6520 7468 6520 636f  has close the co
 00044a10: 6e6e 6563 7469 6f6e 0000 0000 0000 0000  nnection........
 00044a20: 4745 5420 2f61 7069 2f6d 6f64 756c 652f  GET /api/module/
 00044a30: 6669 726d 7761 7265 5265 6c65 6173 652e  firmwareRelease.
 00044a40: 6a73 6f6e 200d 0a0d 0a00 0000 456e 756d  json .......Enum
 00044a50: 6572 6174 696f 6e20 6661 696c 6564 2066  eration failed f
 00044a60: 6f72 2025 733a 2564 2028 2573 2900 0000  or %s:%d (%s)...
-00044a70: 312e 3130 2e35 3430 3337 0000 4170 7220  1.10.54037..Apr 
-00044a80: 3133 2032 3032 3320 3139 3a30 323a 3536  13 2023 19:02:56
+00044a70: 312e 3130 2e35 3430 3730 0000 4170 7220  1.10.54070..Apr 
+00044a80: 3137 2032 3032 3320 3232 3a35 343a 3136  17 2023 22:54:16
 00044a90: 0000 0000 596f 6374 6f70 7563 6500 0000  ....Yoctopuce...
 00044aa0: 2573 3a2f 2f25 733a 2564 2573 2573 0000  %s://%s:%d%s%s..
 00044ab0: 4e6f 2066 756e 6374 696f 6e20 6f66 2074  No function of t
 00044ac0: 6861 7420 636c 6173 7300 0000 200d 0a0d  hat class... ...
 00044ad0: 0a00 0000 4163 6365 7373 2064 656e 6965  ....Access denie
 00044ae0: 643a 2061 646d 696e 2063 7265 6465 6e74  d: admin credent
 00044af0: 6961 6c73 2072 6571 7569 7265 6400 0000  ials required...
@@ -17801,15 +17801,15 @@
 00045880: 6d61 6e79 207a 6f6e 6573 2069 6e20 2e62  many zones in .b
 00045890: 796e 2066 696c 6500 496e 636f 7272 6563  yn file.Incorrec
 000458a0: 7420 6669 6c65 2073 697a 6520 6f72 2063  t file size or c
 000458b0: 6f72 7275 7074 2066 696c 6500 496e 7661  orrupt file.Inva
 000458c0: 6c69 6420 7072 6f67 7261 6d6d 696e 6720  lid programming 
 000458d0: 746f 6f6c 7320 7265 7669 7369 6f6e 206f  tools revision o
 000458e0: 7220 636f 7272 7570 7420 6669 6c65 0000  r corrupt file..
-000458f0: 3534 3033 3700 0000 5468 6973 2066 6972  54037...This fir
+000458f0: 3534 3037 3000 0000 5468 6973 2066 6972  54070...This fir
 00045900: 6d77 6172 6520 6973 2074 6f6f 2072 6563  mware is too rec
 00045910: 656e 742c 2070 6c65 6173 6520 7570 6772  ent, please upgr
 00045920: 6164 6520 796f 7572 2056 6972 7475 616c  ade your Virtual
 00045930: 4875 6220 6f72 2059 6f63 746f 7075 6365  Hub or Yoctopuce
 00045940: 206c 6962 7261 7279 0000 0000 546f 6f20   library....Too 
 00045950: 6d61 6e79 2052 4f4d 207a 6f6e 6573 2069  many ROM zones i
 00045960: 6e20 2e62 796e 2066 696c 6500 546f 6f20  n .byn file.Too 
@@ -18265,15 +18265,15 @@
 00047580: 0000 0000 0000 0080 0000 0000 0000 1000  ................
 00047590: 0000 0000 0000 e0c3 0000 0000 0000 e043  ...............C
 000475a0: 0000 0000 0000 f043 0000 00f0 ffff ef47  .......C.......G
 000475b0: 0000 00f0 ffff 0f38 0000 0000 0000 6045  .......8......`E
 000475c0: 0810 0000 0000 0001 0000 0000 0000 f020  ............... 
 000475d0: 3304 0000 3f04 0000 0008 0000 ff17 0000  3...?...........
 000475e0: 3f13 0000 0000 0000 0000 0000 0000 0000  ?...............
-000475f0: 0000 0000 f735 3864 0000 0000 0d00 0000  .....58d........
+000475f0: 0000 0000 30b2 3d64 0000 0000 0d00 0000  ....0.=d........
 00047600: ac02 0000 6c91 0400 6c77 0400 0000 0000  ....l...lw......
 00047610: 5c00 0000 0000 0000 0000 0000 0000 0000  \...............
 00047620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00047630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00047640: 0000 0000 0000 0000 0000 0000 04c0 0410  ................
 00047650: 5091 0410 0700 0000 0002 0410 0000 0000  P...............
 00047660: 0000 0000 0000 0000 0001 0000 0000 0000  ................
@@ -18441,15 +18441,15 @@
 00048080: d0ff ffff 0000 0000 feff ffff f8e8 0310  ................
 00048090: fce8 0310 0000 0000 bfde 0310 0000 0000  ................
 000480a0: a49a 0410 0200 0000 b09a 0410 cc9a 0410  ................
 000480b0: 0000 0000 98ca 0410 0000 0000 ffff ffff  ................
 000480c0: 0000 0000 0c00 0000 60de 0310 0000 0000  ........`.......
 000480d0: b8ca 0410 0000 0000 ffff ffff 0000 0000  ................
 000480e0: 0c00 0000 93de 0310 0000 0000 0000 0000  ................
-000480f0: 0000 0000 f735 3864 0000 0000 aa9f 0400  .....58d........
+000480f0: 0000 0000 2fb2 3d64 0000 0000 aa9f 0400  ..../.=d........
 00048100: 0100 0000 7500 0000 7500 0000 189b 0400  ....u...u.......
 00048110: ec9c 0400 c09e 0400 70cd 0000 90cd 0000  ........p.......
 00048120: b0cd 0000 60ce 0000 a0cf 0000 70d0 0000  ....`.......p...
 00048130: 40d1 0000 10d2 0000 c0d3 0000 80d4 0000  @...............
 00048140: 10d5 0000 60d5 0000 b0d5 0000 00d6 0000  ....`...........
 00048150: 50d6 0000 70d6 0000 90d6 0000 a0d6 0000  P...p...........
 00048160: c0d6 0000 e0d6 0000 00d7 0000 10d7 0000  ................
@@ -19167,29 +19167,29 @@
 0004ade0: 4e00 1300 0100 4600 6900 6c00 6500 4400  N.....F.i.l.e.D.
 0004adf0: 6500 7300 6300 7200 6900 7000 7400 6900  e.s.c.r.i.p.t.i.
 0004ae00: 6f00 6e00 0000 0000 5900 6f00 6300 7400  o.n.....Y.o.c.t.
 0004ae10: 6f00 7000 7500 6300 6500 2000 7900 4100  o.p.u.c.e. .y.A.
 0004ae20: 5000 4900 2000 6400 6c00 6c00 0000 0000  P.I. .d.l.l.....
 0004ae30: 2c00 0600 0100 4600 6900 6c00 6500 5600  ,.....F.i.l.e.V.
 0004ae40: 6500 7200 7300 6900 6f00 6e00 0000 0000  e.r.s.i.o.n.....
-0004ae50: 3500 3400 3000 3300 3700 0000 2a00 0500  5.4.0.3.7...*...
+0004ae50: 3500 3400 3000 3700 3000 0000 2a00 0500  5.4.0.7.0...*...
 0004ae60: 0100 4900 6e00 7400 6500 7200 6e00 6100  ..I.n.t.e.r.n.a.
 0004ae70: 6c00 4e00 6100 6d00 6500 0000 7900 6100  l.N.a.m.e...y.a.
 0004ae80: 7000 6900 0000 0000 3a00 0900 0100 4f00  p.i.....:.....O.
 0004ae90: 7200 6900 6700 6900 6e00 6100 6c00 4600  r.i.g.i.n.a.l.F.
 0004aea0: 6900 6c00 6500 6e00 6100 6d00 6500 0000  i.l.e.n.a.m.e...
 0004aeb0: 7900 6100 7000 6900 2e00 6400 6c00 6c00  y.a.p.i...d.l.l.
 0004aec0: 0000 0000 3e00 0f00 0100 5000 7200 6f00  ....>.....P.r.o.
 0004aed0: 6400 7500 6300 7400 4e00 6100 6d00 6500  d.u.c.t.N.a.m.e.
 0004aee0: 0000 0000 5900 6f00 6300 7400 6f00 7000  ....Y.o.c.t.o.p.
 0004aef0: 7500 6300 6500 2000 7900 4100 5000 4900  u.c.e. .y.A.P.I.
 0004af00: 0000 0000 3000 0600 0100 5000 7200 6f00  ....0.....P.r.o.
 0004af10: 6400 7500 6300 7400 5600 6500 7200 7300  d.u.c.t.V.e.r.s.
-0004af20: 6900 6f00 6e00 0000 3500 3400 3000 3300  i.o.n...5.4.0.3.
-0004af30: 3700 0000 4400 0000 0100 5600 6100 7200  7...D.....V.a.r.
+0004af20: 6900 6f00 6e00 0000 3500 3400 3000 3700  i.o.n...5.4.0.7.
+0004af30: 3000 0000 4400 0000 0100 5600 6100 7200  0...D.....V.a.r.
 0004af40: 4600 6900 6c00 6500 4900 6e00 6600 6f00  F.i.l.e.I.n.f.o.
 0004af50: 0000 0000 2400 0400 0000 5400 7200 6100  ....$.....T.r.a.
 0004af60: 6e00 7300 6c00 6100 7400 6900 6f00 6e00  n.s.l.a.t.i.o.n.
 0004af70: 0000 0000 0904 e404 0000 0000 0000 0000  ................
 0004af80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0004af90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0004afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -20097,17 +20097,17 @@
 0004e800: f82c 0000 0002 0200 3082 2ce9 0609 2a86  .,......0.,...*.
 0004e810: 4886 f70d 0107 02a0 822c da30 822c d602  H........,.0.,..
 0004e820: 0101 310f 300d 0609 6086 4801 6503 0402  ..1.0...`.H.e...
 0004e830: 0105 0030 5c06 0a2b 0601 0401 8237 0201  ...0\..+.....7..
 0004e840: 04a0 4e30 4c30 1706 0a2b 0601 0401 8237  ..N0L0...+.....7
 0004e850: 0201 0f30 0903 0100 a004 a202 8000 3031  ...0..........01
 0004e860: 300d 0609 6086 4801 6503 0402 0105 0004  0...`.H.e.......
-0004e870: 205d 2ea1 7078 df19 9a55 c1be e8e6 3075   ]..px...U....0u
-0004e880: b730 73ca d71e 8208 c5c1 01ae 0148 3c30  .0s..........H<0
-0004e890: 83a0 8211 ed30 8205 6f30 8204 57a0 0302  .....0..o0..W...
+0004e870: 20e6 d199 a175 b59f 6bbe e189 0661 d9d7   ....u..k....a..
+0004e880: 56fd ec5a 7f17 e23e 70c2 3e2e 6acf 76e3  V..Z...>p.>.j.v.
+0004e890: 8fa0 8211 ed30 8205 6f30 8204 57a0 0302  .....0..o0..W...
 0004e8a0: 0102 0210 48fc 93b4 6055 948d 36a7 c98a  ....H...`U..6...
 0004e8b0: 89d6 9416 300d 0609 2a86 4886 f70d 0101  ....0...*.H.....
 0004e8c0: 0c05 0030 7b31 0b30 0906 0355 0406 1302  ...0{1.0...U....
 0004e8d0: 4742 311b 3019 0603 5504 080c 1247 7265  GB1.0...U....Gre
 0004e8e0: 6174 6572 204d 616e 6368 6573 7465 7231  ater Manchester1
 0004e8f0: 1030 0e06 0355 0407 0c07 5361 6c66 6f72  .0...U....Salfor
 0004e900: 6431 1a30 1806 0355 040a 0c11 436f 6d6f  d1.0...U....Como
@@ -20402,61 +20402,61 @@
 0004fb10: 86f7 0d01 0903 310c 060a 2b06 0104 0182  ......1...+.....
 0004fb20: 3702 0104 301c 060a 2b06 0104 0182 3702  7...0...+.....7.
 0004fb30: 010b 310e 300c 060a 2b06 0104 0182 3702  ..1.0...+.....7.
 0004fb40: 0115 302c 060a 2b06 0104 0182 3702 010c  ..0,..+.....7...
 0004fb50: 311e 301c a01a 8018 0079 0061 0070 0069  1.0......y.a.p.i
 0004fb60: 0020 0033 0032 0020 0062 0069 0074 0073  . .3.2. .b.i.t.s
 0004fb70: 302f 0609 2a86 4886 f70d 0109 0431 2204  0/..*.H......1".
-0004fb80: 20f0 5fea 865f 81b0 e86b 847a 7a3b 1972   ._.._...k.zz;.r
-0004fb90: 2ebe 8890 4ff1 da3f 13ec a486 32e9 6bde  ....O..?....2.k.
-0004fba0: 2830 0d06 092a 8648 86f7 0d01 0101 0500  (0...*.H........
-0004fbb0: 0482 0200 3407 d16a fb7e d0dc e67a 40b7  ....4..j.~...z@.
-0004fbc0: c9da 6efb 136a 3be7 8445 384e 83fb 44f3  ..n..j;..E8N..D.
-0004fbd0: bbf9 77e4 fa4c 8c91 abc5 5453 3edc 7913  ..w..L....TS>.y.
-0004fbe0: 2979 39e0 22f5 bc43 0876 a8ee bcf6 40c7  )y9."..C.v....@.
-0004fbf0: 7ec5 1542 cfeb 6b10 042d 69e9 df1b 3ed2  ~..B..k..-i...>.
-0004fc00: 0ef5 44ba 90ad c3e4 4f47 3bf1 4938 9ba1  ..D.....OG;.I8..
-0004fc10: 1481 c8d2 a89b e553 db4f 4a1d bce7 b4ea  .......S.OJ.....
-0004fc20: d604 91a1 90bc 1f70 c114 08f9 1d67 9f1a  .......p.....g..
-0004fc30: ab56 cf03 7daa 6028 0d69 00b2 c639 59e5  .V..}.`(.i...9Y.
-0004fc40: 1b24 54ca f73a ae0f 7a56 c38c 7006 c2ad  .$T..:..zV..p...
-0004fc50: f5a5 5f64 86d9 339a f27c 734c d6e3 43c1  .._d..3..|sL..C.
-0004fc60: 93f5 442f 18f2 95a1 fbcc ed52 1415 2564  ..D/.......R..%d
-0004fc70: 7b49 f2dd f069 af8d 6803 6146 2588 4932  {I...i..h.aF%.I2
-0004fc80: 5ece b1e9 5dc4 720d 1f8f 04d8 fc8f 29c9  ^...].r.......).
-0004fc90: 05e0 2d87 3552 004a 66ee f6d1 5482 2ca9  ..-.5R.Jf...T.,.
-0004fca0: 80f1 e1ae c5a7 cb98 0868 c54d 89b8 a061  .........h.M...a
-0004fcb0: a831 7edd 8e21 e1ec 0fab efe8 2b1a e910  .1~..!......+...
-0004fcc0: 4b58 4a8f 6f68 5bff 2933 4f97 1ffb da77  KXJ.oh[.)3O....w
-0004fcd0: 0a54 f6cc d878 e149 444e d73e a589 e5bd  .T...x.IDN.>....
-0004fce0: b63a 955d aa1e b1fc 0584 b107 63ba 61af  .:.]........c.a.
-0004fcf0: 685f 166c d373 d006 6f70 1f3a 3350 953c  h_.l.s..op.:3P.<
-0004fd00: 0f4a b874 aeb2 d9c0 b837 3a6f cfd0 a319  .J.t.....7:o....
-0004fd10: 1d3f 5242 2158 d182 5dd0 cae5 ba4e 394c  .?RB!X..]....N9L
-0004fd20: eb85 3066 c30f 88be 4086 778d e0f2 669e  ..0f....@.w...f.
-0004fd30: e157 7f83 8037 cec4 ed7c a876 c799 52c7  .W...7...|.v..R.
-0004fd40: 93f6 84c3 d637 04ec c891 c2c5 07e9 7ada  .....7........z.
-0004fd50: 976c 93ad c066 8458 56c3 c8d0 f36b 0eb8  .l...f.XV....k..
-0004fd60: 93a6 4074 6209 2aab 769d 719e 86f2 59c6  ..@tb.*.v.q...Y.
-0004fd70: ca2d 15fb 9697 2c83 4105 ce7b e143 ce7b  .-....,.A..{.C.{
-0004fd80: 99c5 45ba d7c2 4863 6ac8 732b 7ad0 32b3  ..E...Hcj.s+z.2.
-0004fd90: 34b5 4306 38ff ad99 8c4b b6ca bf6d c0bf  4.C.8....K...m..
-0004fda0: 0898 284e 4799 da95 7d40 9925 7aa2 22dd  ..(NG...}@.%z.".
-0004fdb0: a827 3b60 a182 173d 3082 1739 060a 2b06  .';`...=0..9..+.
+0004fb80: 20aa acf2 ccdc 3377 7816 bf3c e180 3eb2   .....3wx..<..>.
+0004fb90: 77b6 ba57 559a 70fa 7b10 97a2 3957 ae88  w..WU.p.{...9W..
+0004fba0: fc30 0d06 092a 8648 86f7 0d01 0101 0500  .0...*.H........
+0004fbb0: 0482 0200 7f80 32d1 603d 5378 5402 c7cc  ......2.`=SxT...
+0004fbc0: a16c 30f6 a4df beae 8900 1dfc efc9 071c  .l0.............
+0004fbd0: 570d 4319 38ce 8f5b 4b95 6187 f8e4 208b  W.C.8..[K.a... .
+0004fbe0: c414 0ca2 4530 ff20 bc60 24c2 471e 1b84  ....E0. .`$.G...
+0004fbf0: b884 9137 f939 15da ce78 61ca 3073 1e3d  ...7.9...xa.0s.=
+0004fc00: 4d35 6e94 8b47 fd0b 3ec4 cae2 b0cb a294  M5n..G..>.......
+0004fc10: 3dfb 193a d1d3 6d3e 0210 fd50 801f 569e  =..:..m>...P..V.
+0004fc20: f97c 8678 72ff 2b69 62cf d304 6225 8d68  .|.xr.+ib...b%.h
+0004fc30: 43ed 73ed 0007 b556 a43f b5ed 2d89 d430  C.s....V.?..-..0
+0004fc40: 34db 4641 257d de4a bdc1 4280 30b8 cf2c  4.FA%}.J..B.0..,
+0004fc50: 27e5 8c00 0ef7 c2a5 ffed 21f5 5dd2 ce94  '.........!.]...
+0004fc60: 5a0d f31b 7339 92da d2ab 7f58 80b6 0360  Z...s9.....X...`
+0004fc70: 2314 b3e2 e95a 1acc df33 7b7a b33b 0afc  #....Z...3{z.;..
+0004fc80: 65ad c7ff 4013 dafe 857e b4ad 4bf0 e55b  e...@....~..K..[
+0004fc90: 6a2f 7926 1217 47f5 d678 a9b0 9b31 d3af  j/y&..G..x...1..
+0004fca0: f1be 3e1f 2b72 e51b 69df da2d 6d6c b30b  ..>.+r..i..-ml..
+0004fcb0: 0b31 d5b7 f800 3711 33f9 4fbd 4c85 cad5  .1....7.3.O.L...
+0004fcc0: f911 e5bd 36fc 9cff c338 9b36 fe87 9bf6  ....6....8.6....
+0004fcd0: eb18 f993 e8f7 a13d 6e71 9946 5b5e 7755  .......=nq.F[^wU
+0004fce0: 8a6a 766f 6a6e 098e cfb0 f213 ee80 79c1  .jvojn........y.
+0004fcf0: 3710 c858 90fb 1e9f 77d0 9324 4e18 d1da  7..X....w..$N...
+0004fd00: e776 f2c9 224e 41ce 514d 9956 755a 5998  .v.."NA.QM.VuZY.
+0004fd10: 4e0f 9cba 273e 7689 7ebb 266c 3ce4 cc80  N...'>v.~.&l<...
+0004fd20: d8ad 2f6b 39d5 3e9a d097 d8f5 0d8e 3658  ../k9.>.......6X
+0004fd30: c88a b07b 8b4a d520 84a7 024e 48d8 4120  ...{.J. ...NH.A 
+0004fd40: 23df 98a4 fabf 1b2e 2f44 b1c1 05e2 10d0  #......./D......
+0004fd50: d660 5c3b f350 58b6 5abf 1b85 14e8 4760  .`\;.PX.Z.....G`
+0004fd60: 3ba0 47d0 712b e4a3 91cf 596f 7a38 24bf  ;.G.q+....Yoz8$.
+0004fd70: 8c98 2e02 8621 ceb5 a20e 30ab 9ae0 c910  .....!....0.....
+0004fd80: 3c04 5125 180c c2f3 91c0 a836 b582 5d07  <.Q%.......6..].
+0004fd90: ca89 fb1b 5b16 b213 ce09 cf44 1dc3 a384  ....[......D....
+0004fda0: 6981 f217 aa99 5902 1983 936c 6f67 603f  i.....Y....log`?
+0004fdb0: 1083 a98b a182 173d 3082 1739 060a 2b06  .......=0..9..+.
 0004fdc0: 0104 0182 3703 0301 3182 1729 3082 1725  ....7...1..)0..%
 0004fdd0: 0609 2a86 4886 f70d 0107 02a0 8217 1630  ..*.H..........0
 0004fde0: 8217 1202 0103 310f 300d 0609 6086 4801  ......1.0...`.H.
 0004fdf0: 6503 0402 0105 0030 7706 0b2a 8648 86f7  e......0w..*.H..
 0004fe00: 0d01 0910 0104 a068 0466 3064 0201 0106  .......h.f0d....
 0004fe10: 0960 8648 0186 fd6c 0701 3031 300d 0609  .`.H...l..010...
-0004fe20: 6086 4801 6503 0402 0105 0004 205c cbac  `.H.e....... \..
-0004fe30: 3888 a1e3 9d3e d02c 7227 fa28 41b2 2f0d  8....>.,r'.(A./.
-0004fe40: bdf9 5b20 135d 9d47 a758 1d3f 3c02 1045  ..[ .].G.X.?<..E
-0004fe50: a8eb 6f0b 69ae 5bdc 096a 34d3 6bcf 6d18  ..o.i.[..j4.k.m.
-0004fe60: 0f32 3032 3330 3431 3331 3730 3533 315a  .20230413170531Z
+0004fe20: 6086 4801 6503 0402 0105 0004 20fc 19ba  `.H.e....... ...
+0004fe30: 8fb6 0a15 540e 0f89 cd59 f7df 4eb1 321b  ....T....Y..N.2.
+0004fe40: bb0b 50ba ebf6 21b0 984d 48e8 9102 1056  ..P...!..MH....V
+0004fe50: bd41 bd4e 7139 879b e935 df3f 779c 7318  .A.Nq9...5.?w.s.
+0004fe60: 0f32 3032 3330 3431 3732 3035 3635 335a  .20230417205653Z
 0004fe70: a082 1307 3082 06c0 3082 04a8 a003 0201  ....0...0.......
 0004fe80: 0202 100c 4d69 724b 94fa 3c2a 4a3d 2907  ....MirK..<*J=).
 0004fe90: 803d 5a30 0d06 092a 8648 86f7 0d01 010b  .=Z0...*.H......
 0004fea0: 0500 3063 310b 3009 0603 5504 0613 0255  ..0c1.0...U....U
 0004feb0: 5331 1730 1506 0355 040a 130e 4469 6769  S1.0...U....Digi
 0004fec0: 4365 7274 2c20 496e 632e 313b 3039 0603  Cert, Inc.1;09..
 0004fed0: 5504 0313 3244 6967 6943 6572 7420 5472  U...2DigiCert Tr
@@ -20766,51 +20766,51 @@
 000511d0: 5341 3430 3936 2053 4841 3235 3620 5469  SA4096 SHA256 Ti
 000511e0: 6d65 5374 616d 7069 6e67 2043 4102 100c  meStamping CA...
 000511f0: 4d69 724b 94fa 3c2a 4a3d 2907 803d 5a30  MirK..<*J=)..=Z0
 00051200: 0d06 0960 8648 0165 0304 0201 0500 a081  ...`.H.e........
 00051210: d130 1a06 092a 8648 86f7 0d01 0903 310d  .0...*.H......1.
 00051220: 060b 2a86 4886 f70d 0109 1001 0430 1c06  ..*.H........0..
 00051230: 092a 8648 86f7 0d01 0905 310f 170d 3233  .*.H......1...23
-00051240: 3034 3133 3137 3035 3331 5a30 2b06 0b2a  0413170531Z0+..*
+00051240: 3034 3137 3230 3536 3533 5a30 2b06 0b2a  0417205653Z0+..*
 00051250: 8648 86f7 0d01 0910 020c 311c 301a 3018  .H........1.0.0.
 00051260: 3016 0414 f387 224d 8633 8292 35a9 94bc  0....."M.3..5...
 00051270: bd8f 96e9 fe1c 7c73 302f 0609 2a86 4886  ......|s0/..*.H.
-00051280: f70d 0109 0431 2204 20c3 2343 1e50 69d9  .....1". .#C.Pi.
-00051290: 7289 4a79 2746 25c3 a9cf 13a1 eec8 cc05  r.Jy'F%.........
-000512a0: 2e14 c687 ec7b a745 8330 3706 0b2a 8648  .....{.E.07..*.H
+00051280: f70d 0109 0431 2204 200a 0f3f b9a7 fb8a  .....1". ..?....
+00051290: 74ff e5a5 9626 2094 ea7a bb19 c0b9 6881  t....& ..z....h.
+000512a0: 98ab 640c 1dbf b55b d930 3706 0b2a 8648  ..d....[.07..*.H
 000512b0: 86f7 0d01 0910 022f 3128 3026 3024 3022  ......./1(0&0$0"
 000512c0: 0420 c7f4 e1be 3228 8920 abe2 263a be1a  . ....2(. ..&:..
 000512d0: c4fc 4fe6 781c 2d64 d04c 8075 57a0 23b5  ..O.x.-d.L.uW.#.
 000512e0: b6fa 300d 0609 2a86 4886 f70d 0101 0105  ..0...*.H.......
-000512f0: 0004 8202 00bf cb1a 8ab8 c99c 3f5d 4b57  ............?]KW
-00051300: 2f93 c9cf 5f7d 6a58 5fa0 08fb 2fd6 5e30  /..._}jX_.../.^0
-00051310: 6108 06d2 1991 ddcd db13 d46c 58c2 e663  a..........lX..c
-00051320: 4e39 7893 93ee 1b51 0399 4c52 b08b 67b4  N9x....Q..LR..g.
-00051330: 8bbb 0954 0f7b c525 9402 10a2 a33b 876d  ...T.{.%.....;.m
-00051340: 5d2e a910 791c 9e91 7041 fc95 7022 ef6e  ]...y...pA..p".n
-00051350: 6410 51b8 f51a 34a3 1ccc c64f e95b ed18  d.Q...4....O.[..
-00051360: c0e8 d556 220c bcb1 c0e4 70eb 4f72 3c8a  ...V".....p.Or<.
-00051370: 6857 c724 fbb1 dfcc 212d 0230 29fa 3499  hW.$....!-.0).4.
-00051380: 79df ac75 893b 5376 763a a3c1 b0ff 1f81  y..u.;Svv:......
-00051390: 8358 ff9d 2d80 fe66 fdf8 0079 8e4b a585  .X..-..f...y.K..
-000513a0: b318 f9fb 839e 8b2f ebe9 2353 a476 e10e  ......./..#S.v..
-000513b0: f8e4 a44c 7c42 72b6 c4a1 bc76 25fd b778  ...L|Br....v%..x
-000513c0: 7997 cf1e 3536 8e44 4e1d 0ae4 2994 408c  y...56.DN...).@.
-000513d0: 86b2 efff b681 0347 bd06 40fd 498e ce59  .......G..@.I..Y
-000513e0: f22b 79a6 dcc7 5d25 0d86 7e1c 1b8d 9940  .+y...]%..~....@
-000513f0: eb28 7a57 1739 4865 8218 18d6 ac67 c51c  .(zW.9He.....g..
-00051400: c9ff bc3c 482b 21d1 0cae 518a d293 9572  ...<H+!...Q....r
-00051410: bade 026b 8009 5862 9b36 db9d 5474 88b3  ...k..Xb.6..Tt..
-00051420: 8910 939d c589 1c48 1cf1 edb0 fb9c dccf  .......H........
-00051430: 2a8e 9b20 13fd 68f6 a830 1ce1 1a75 e292  *.. ..h..0...u..
-00051440: 5ce0 6d2c 4b4c b6ef ea2b a0f4 7c1b 7c84  \.m,KL...+..|.|.
-00051450: 31b5 4d53 3684 f97c ff9b 2d77 a921 3c3f  1.MS6..|..-w.!<?
-00051460: fc37 fdcf df2f 1498 5f8e dc01 a675 f4a5  .7.../.._....u..
-00051470: da68 d442 2724 5de9 ad53 c2bf 223b 6d5b  .h.B'$]..S..";m[
-00051480: 69b5 4a49 26fe 9f2c cc10 d34c d855 09b2  i.JI&..,...L.U..
-00051490: 7798 4ca7 d197 723c bb32 edee 6623 8c70  w.L...r<.2..f#.p
-000514a0: a8d8 136d b3dd 2100 0295 f572 0e29 ac41  ...m..!....r.).A
-000514b0: 4b64 a887 cbe2 379f 04c4 83c4 2fdf 7c2e  Kd....7...../.|.
-000514c0: 0a75 9798 1fca 9a16 0256 2b09 afd7 51e9  .u.......V+...Q.
-000514d0: 5629 a16a 48dd e910 57d4 b504 8bed 5bea  V).jH...W.....[.
-000514e0: 885b 8c89 60ab f71d 4933 776d a305 df00  .[..`...I3wm....
-000514f0: 3a51 3c57 5400 0000                      :Q<WT...
+000512f0: 0004 8202 00c9 0a18 769d 2fa2 99e3 7d57  ........v./...}W
+00051300: d621 e523 e7f5 1a9c 0165 f17c 7b61 3945  .!.#.....e.|{a9E
+00051310: eb93 9e05 eb66 200e 3b86 f974 524d cc62  .....f .;..tRM.b
+00051320: e4dd 3719 e75c 6a30 6312 5488 f2ac 256f  ..7..\j0c.T...%o
+00051330: ba88 fc6b abb5 91d3 20e5 9a4b 872f 02bc  ...k.... ..K./..
+00051340: 54a9 dc43 d52e 9a08 40fe 588d 046b 111d  T..C....@.X..k..
+00051350: 5fa7 9568 30e3 2516 742f af0f f76a 3309  _..h0.%.t/...j3.
+00051360: b619 91ad bbbe 2320 b54f aa8a 13ba e55f  ......# .O....._
+00051370: 6e89 e2e3 c336 061e 4c87 36cb b8cf b9fa  n....6..L.6.....
+00051380: 9225 be8f 18c3 8290 ff59 1458 0c1b 85a7  .%.......Y.X....
+00051390: 313b 156b 32ab 80a4 8e7f 5a8d 1243 d91b  1;.k2.....Z..C..
+000513a0: 87e2 bfa0 f45d 67f1 d840 598f 46a5 c6c4  .....]g..@Y.F...
+000513b0: 4c29 f2bc b31c e226 48af 8457 c1d8 9ca3  L).....&H..W....
+000513c0: 1d06 2679 2e6d 4598 6b41 d751 0e69 045b  ..&y.mE.kA.Q.i.[
+000513d0: 4ca2 3501 3f47 7dcc 5925 a0b8 37eb 9973  L.5.?G}.Y%..7..s
+000513e0: 294f f98f 27de 96a9 49f2 b8bf 114f 9fbf  )O..'...I....O..
+000513f0: 930d 3f35 54cb 5fb0 f286 abe6 589d c1d3  ..?5T._.....X...
+00051400: 1c6e 4ec8 448d d28c 86cf e3c2 7baa 72c0  .nN.D.......{.r.
+00051410: 3640 25a0 222f c600 78da e4f9 e34c 25a6  6@%."/..x....L%.
+00051420: 6cd0 21f5 65cf 92fa 73ee 9644 b6ff 7d83  l.!.e...s..D..}.
+00051430: 156d 0141 0f3b 74e9 4cd5 3a50 c380 486c  .m.A.;t.L.:P..Hl
+00051440: ce16 4386 5b17 08cb 422b a438 43b1 361d  ..C.[...B+.8C.6.
+00051450: adbc f622 5a75 eec5 87ac e2af 6868 356e  ..."Zu......hh5n
+00051460: 71d9 6619 ef28 020d d807 3df4 6740 b194  q.f..(....=.g@..
+00051470: f58e 4d2c 1552 eb1c 51b7 a121 6a89 73a3  ..M,.R..Q..!j.s.
+00051480: a20c 6149 2993 0b12 4caf 7b8f 94ef 28df  ..aI)...L.{...(.
+00051490: 6fc9 8050 6519 890b b5c9 c9fb 1b26 1a92  o..Pe........&..
+000514a0: 9ef7 cf02 a0f9 b157 7b0d 38c2 9b47 d2e6  .......W{.8..G..
+000514b0: 6826 3fa2 c388 c81e f960 3ace 5ff4 556c  h&?......`:._.Ul
+000514c0: 7461 08ac 6c01 ce77 9047 0bd1 9539 d4ab  ta..l..w.G...9..
+000514d0: 6585 a143 743d e824 2b4e 695c 83e0 c9c7  e..Ct=.$+Ni\....
+000514e0: b87e 76c5 d4fa 7bdd 9ec5 96df 443d 4387  .~v...{.....D=C.
+000514f0: 0528 a07f 8f00 0000                      .(......
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/cdll/yapi64.dll` & `yoctopuce-1.10.54070/yoctopuce/cdll/yapi64.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018002d9dc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 13 17:05:31 2023
+Time/Date		Mon Apr 17 20:56:53 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	0
 SizeOfCode		0000000000046200
 SizeOfInitializedData	0000000000058c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000002d9dc
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		000a6000
 SizeOfHeaders		00000400
-CheckSum		0006d013
+CheckSum		00065bf1
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -208,15 +208,15 @@
  00058934	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .rdata at 0x180057df0
 
 The Export Tables (interpreted .rdata section contents)
 
 Export Flags 			0
-Time/Date stamp 		6438365a
+Time/Date stamp 		643db294
 Major/Minor 			0/0
 Name 				0000000000058106 yapi.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000004b
 	[Name Pointer/Ordinal] Table	0000004b
 Table Addresses
@@ -8761,15 +8761,15 @@
 	  020: 00 00 00 00 02 00 00 00 98 7d 05 00 c0 7d 05 00
 	  030: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  040: 20 ac 05 00 00 00 00 00 ff ff ff ff 00 00 00 00
 	  050: 18 00 00 00 00 55 04 00 00 00 00 00 00 00 00 00
 	  060: 00 00 00 00 00 00 00 00 48 ac 05 00 00 00 00 00
 	  070: ff ff ff ff 00 00 00 00 18 00 00 00 60 55 04 00
 	  080: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  090: 00 00 00 00 00 00 00 00 5a 36 38 64 00 00 00 00
+	  090: 00 00 00 00 00 00 00 00 94 b2 3d 64 00 00 00 00
 	  0a0: 06 81 05 00 01 00 00 00 4b 00 00 00 4b 00 00 00
 	  0b0: 18 7e 05 00 44 7f 05 00 70 80 05 00 b0 c2 01 00
 	  0c0: a0 d1 01 00 f0 ce 01 00 90 c2 01 00 c0 c3 01 00
 	  0d0: f0 e1 00 00 30 c3 01 00 f0 d7 01 00 10 d9 01 00
 	  0e0: d0 c8 01 00 d0 d9 01 00 00 10 00 00 70 eb 00 00
 	  0f0: 20 e7 00 00 f0 e1 00 00 60 eb 00 00 90 e7 00 00
 	  100: e0 e7 00 00 40 eb 00 00 a0 ea 00 00 50 8d 00 00
@@ -99881,27 +99881,28 @@
    180050f1e:	and    %ah,0x64253a73(%rip)        # 0x1e42a4997
    180050f24:	and    %ch,(%rax)
    180050f26:	and    $0x2973,%eax
    180050f2b:	add    %al,(%rax)
    180050f2d:	add    %al,(%rax)
    180050f2f:	add    %dh,(%rcx)
    180050f31:	cs xor %esi,(%rax)
-   180050f34:	cs xor $0x37333034,%eax
+   180050f34:	cs xor $0x30373034,%eax
    180050f3a:	add    %al,(%rax)
    180050f3c:	add    %al,(%rax)
    180050f3e:	add    %al,(%rax)
    180050f40:	rex.B jo 0x180050fb5
    180050f43:	and    %dh,(%rcx)
-   180050f45:	xor    (%rax),%esp
-   180050f47:	xor    (%rax),%dh
-   180050f49:	xor    (%rbx),%dh
-   180050f4b:	and    %dh,(%rcx)
-   180050f4d:	cmp    %edi,(%rdx)
-   180050f4f:	xor    %dh,(%rdx,%rdi,1)
-   180050f52:	xor    0x0(%rip),%esi        # 0x180050f58
+   180050f45:	(bad)
+   180050f46:	and    %dh,(%rdx)
+   180050f48:	xor    %dh,(%rdx)
+   180050f4a:	xor    (%rax),%esp
+   180050f4c:	xor    (%rdx),%dh
+   180050f4e:	cmp    0x36353a35(%rip),%dh        # 0x1b63a4989
+   180050f54:	add    %al,(%rax)
+   180050f56:	add    %al,(%rax)
    180050f58:	pop    %rcx
    180050f59:	outsl  %ds:(%rsi),(%dx)
    180050f5a:	movsxd 0x70(%rdi,%rbp,2),%esi
    180050f5e:	jne    0x180050fc3
    180050f60:	add    %al,%gs:(%rax)
    180050f63:	add    %al,(%rax)
    180050f65:	add    %al,(%rax)
@@ -101387,22 +101388,22 @@
    180051ed2:	and    %ch,0x72(%rdi)
    180051ed5:	and    %ah,0x6f(%rbx)
    180051ed8:	jb     0x180051f4c
    180051eda:	jne    0x180051f4c
    180051edc:	je     0x180051efe
    180051ede:	imul   $0x3500,0x0(%rbp,%riz,2),%bp
    180051ee5:	xor    $0x30,%al
-   180051ee7:	xor    (%rdi),%esi
-   180051ee9:	add    %al,(%rax)
-   180051eeb:	add    %al,(%rax)
-   180051eed:	add    %al,(%rax)
-   180051eef:	add    %dl,0x69(%rax,%rbp,2)
-   180051ef3:	jae    0x180051f15
-   180051ef5:	imul   $0x6177,0x6d(%rdx),%si
-   180051efb:	jb     0x180051f62
+   180051ee7:	(bad)
+   180051ee8:	xor    %al,(%rax)
+   180051eea:	add    %al,(%rax)
+   180051eec:	add    %al,(%rax)
+   180051eee:	add    %al,(%rax)
+   180051ef0:	push   %rsp
+   180051ef1:	push   $0x66207369
+   180051ef6:	imul   $0x65726177,0x6d(%rdx),%esi
    180051efd:	and    %ch,0x73(%rcx)
    180051f00:	and    %dh,0x6f(%rdi,%rbp,2)
    180051f04:	and    %dh,0x65(%rdx)
    180051f07:	movsxd 0x6e(%rbp),%esp
    180051f0a:	je     0x180051f38
    180051f0c:	and    %dh,0x6c(%rax)
    180051f0f:	gs (bad)
@@ -104506,16 +104507,17 @@
    180053d3c:	add    %al,-0x71(%rax)
    180053d3f:	rex add %al,(%rax)
    180053d42:	add    %al,(%rax)
    180053d44:	add    %al,(%rax)
    180053d46:	lock rex.XB add %al,(%r8)
 	...
    180053d52:	add    %al,(%rax)
-   180053d54:	pop    %rbx
-   180053d55:	ss cmp %ah,0x0(%rax,%rax,1)
+   180053d54:	xchg   %eax,%ebp
+   180053d55:	mov    $0x3d,%dl
+   180053d57:	add    %al,%fs:(%rax)
    180053d5a:	add    %al,(%rax)
    180053d5c:	or     $0xdc000000,%eax
    180053d61:	add    (%rax),%al
    180053d63:	add    %dh,0x5(%rdi,%rdi,1)
    180053d67:	add    %dh,0x5(%rbp,%riz,1)
    180053d6b:	add    %al,(%rax)
    180053d6d:	add    %al,(%rax)
@@ -111012,16 +111014,17 @@
    180057dcf:	incl   (%rax)
    180057dd1:	add    %al,(%rax)
    180057dd3:	add    %bl,(%rax)
    180057dd5:	add    %al,(%rax)
    180057dd7:	add    %ah,0x55(%rax)
    180057dda:	add    $0x0,%al
 	...
-   180057df4:	pop    %rdx
-   180057df5:	ss cmp %ah,0x0(%rax,%rax,1)
+   180057df4:	xchg   %eax,%esp
+   180057df5:	mov    $0x3d,%dl
+   180057df7:	add    %al,%fs:(%rax)
    180057dfa:	add    %al,(%rax)
    180057dfc:	(bad)
    180057dfd:	addl   $0x4b00,0x100(%rip)        # 0x180057f07
    180057e07:	add    %cl,0x0(%rbx)
    180057e0a:	add    %al,(%rax)
    180057e0c:	sbb    %bh,0x5(%rsi)
    180057e0f:	add    %al,0x5(%rdi,%rdi,2)
@@ -118280,16 +118283,16 @@
    1800a4253:	add    %ah,0x0(%rbp)
    1800a4256:	jb     0x1800a4258
    1800a4258:	jae    0x1800a425a
    1800a425a:	imul   $0x6e006f,(%rax),%eax
    1800a4260:	add    %al,(%rax)
    1800a4262:	add    %al,(%rax)
    1800a4264:	xor    $0x30003400,%eax
-   1800a4269:	add    %dh,(%rbx)
-   1800a426b:	add    %dh,(%rdi)
+   1800a4269:	add    %dh,(%rdi)
+   1800a426b:	add    %dh,(%rax)
    1800a426d:	add    %al,(%rax)
    1800a426f:	add    %ch,(%rdx)
    1800a4271:	add    %al,0x49000100(%rip)        # 0x1c90a4377
    1800a4277:	add    %ch,0x0(%rsi)
    1800a427a:	je     0x1800a427c
    1800a427c:	add    %dh,%gs:0x0(%rdx)
    1800a4280:	outsb  %ds:(%rsi),(%dx)
@@ -118374,16 +118377,16 @@
    1800a4340:	push   %rsi
    1800a4341:	add    %ah,0x0(%rbp)
    1800a4344:	jb     0x1800a4346
    1800a4346:	jae    0x1800a4348
    1800a4348:	imul   $0x6e006f,(%rax),%eax
    1800a434e:	add    %al,(%rax)
    1800a4350:	xor    $0x30003400,%eax
-   1800a4355:	add    %dh,(%rbx)
-   1800a4357:	add    %dh,(%rdi)
+   1800a4355:	add    %dh,(%rdi)
+   1800a4357:	add    %dh,(%rax)
    1800a4359:	add    %al,(%rax)
    1800a435b:	add    %al,0x0(%rax,%rax,1)
    1800a435f:	add    %al,(%rcx)
    1800a4361:	add    %dl,0x0(%rsi)
    1800a4364:	(bad)
    1800a4365:	add    %dh,0x0(%rdx)
    1800a4368:	rex.RX add %r13b,0x0(%rcx)
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_accelerometer.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_accelerometer.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_altitude.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_altitude.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_anbutton.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_anbutton.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_api.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # *********************************************************************
 # *
-# * $Id: yocto_api.py 53857 2023-04-04 15:04:32Z mvuilleu $
+# * $Id: yocto_api.py 54066 2023-04-17 14:22:16Z seb $
 # *
 # * High-level programming interface, common to all modules
 # *
 # * - - - - - - - - - License information: - - - - - - - - -
 # *
 # *  Copyright (C) 2011 and beyond by Yoctopuce Sarl, Switzerland.
 # *
@@ -904,15 +904,15 @@
     DETECT_NET = 2
     RESEND_MISSING_PKT = 4
     DETECT_ALL = DETECT_USB | DETECT_NET
 
     YOCTO_API_VERSION_STR = "1.10"
     YOCTO_API_VERSION_BCD = 0x0110
 
-    YOCTO_API_BUILD_NO = "54037"
+    YOCTO_API_BUILD_NO = "54070"
     YOCTO_DEFAULT_PORT = 4444
     YOCTO_VENDORID = 0x24e0
     YOCTO_DEVID_FACTORYBOOT = 1
 
     YOCTO_DEVID_BOOTLOADER = 2
     YOCTO_ERRMSG_LEN = 256
     YOCTO_MANUFACTURER_LEN = 20
@@ -1287,17 +1287,14 @@
         YAPI._yapiSetNetworkTimeout.argtypes = [ctypes.c_int]
         YAPI._yapiGetNetworkTimeout = YAPI._yApiCLib.yapiGetNetworkTimeout
         YAPI._yapiGetNetworkTimeout.restypes = ctypes.c_int
         YAPI._yapiGetNetworkTimeout.argtypes = []
         YAPI._yapiAddUdevRulesForYocto = YAPI._yApiCLib.yapiAddUdevRulesForYocto
         YAPI._yapiAddUdevRulesForYocto.restypes = ctypes.c_int
         YAPI._yapiAddUdevRulesForYocto.argtypes = [ctypes.c_int, ctypes.c_char_p]
-        YAPI._yapiGetNextHubRef = YAPI._yApiCLib.yapiGetNextHubRef
-        YAPI._yapiGetNextHubRef.restypes = ctypes.c_int
-        YAPI._yapiGetNextHubRef.argtypes = [ctypes.c_int]
     #--- (end of generated code: YFunction dlldef)
 
         YAPI._ydllLoaded = True
 
     # noinspection PyUnresolvedReferences,PyTypeChecker
     class yDeviceSt(ctypes.Structure):
         _pack_ = 1
```

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_arithmeticsensor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_arithmeticsensor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_audioin.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_audioin.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_audioout.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_audioout.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_bluetoothlink.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_bluetoothlink.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_buzzer.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_buzzer.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_carbondioxide.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_carbondioxide.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_cellular.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_cellular.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_colorled.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_colorled.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_colorledcluster.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_colorledcluster.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_compass.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_compass.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_current.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_current.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_currentloopoutput.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_currentloopoutput.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_daisychain.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_daisychain.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_datalogger.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_datalogger.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_digitalio.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_digitalio.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_display.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_display.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_dualpower.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_dualpower.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_files.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_files.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_genericsensor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_genericsensor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_gps.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_gps.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_groundspeed.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_groundspeed.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_gyro.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_gyro.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_hubport.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_hubport.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_humidity.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_humidity.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_i2cport.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_i2cport.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_inputcapture.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_inputcapture.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_inputchain.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_inputchain.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_latitude.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_latitude.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_led.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_led.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_lightsensor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_lightsensor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_longitude.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_longitude.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_magnetometer.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_magnetometer.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_messagebox.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_messagebox.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_motor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_motor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_multiaxiscontroller.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_multiaxiscontroller.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_multicellweighscale.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_multicellweighscale.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_multisenscontroller.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_multisenscontroller.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_network.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_network.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_oscontrol.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_oscontrol.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_power.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_power.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_poweroutput.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_poweroutput.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_powersupply.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_powersupply.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_pressure.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_pressure.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_proximity.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_proximity.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_pwminput.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_pwminput.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_pwmoutput.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_pwmoutput.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_pwmpowersource.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_pwmpowersource.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_quadraturedecoder.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_quadraturedecoder.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_rangefinder.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_rangefinder.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_realtimeclock.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_realtimeclock.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_refframe.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_refframe.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_relay.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_relay.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_segmenteddisplay.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_segmenteddisplay.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_serialport.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_serialport.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_servo.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_servo.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_spiport.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_spiport.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_steppermotor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_steppermotor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_temperature.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_temperature.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_tilt.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_tilt.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_tvoc.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_tvoc.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_voc.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_voc.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_voltage.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_voltage.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_voltageoutput.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_voltageoutput.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_wakeupmonitor.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_wakeupmonitor.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_wakeupschedule.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_wakeupschedule.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_watchdog.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_watchdog.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_weighscale.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_weighscale.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce/yocto_wireless.py` & `yoctopuce-1.10.54070/yoctopuce/yocto_wireless.py`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/yoctopuce.egg-info/PKG-INFO` & `yoctopuce-1.10.54070/yoctopuce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoctopuce
-Version: 1.10.54037
+Version: 1.10.54070
 Summary: Yoctopuce python API
 Home-page: https://www.yoctopuce.com
 Author: Yoctopuce
 Author-email: support@yoctopuce.com
 License: UNKNOWN
 Project-URL: Documentation, https://www.yoctopuce.com/EN/doc/reference/yoctolib-python-EN.html
 Project-URL: Source, https://github.com/yoctopuce/yoctolib_python
```

### Comparing `yoctopuce-1.10.54037/yoctopuce.egg-info/SOURCES.txt` & `yoctopuce-1.10.54070/yoctopuce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/LICENSE.txt` & `yoctopuce-1.10.54070/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/README.md` & `yoctopuce-1.10.54070/README.md`

 * *Files identical despite different names*

### Comparing `yoctopuce-1.10.54037/setup.py` & `yoctopuce-1.10.54070/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setuptools.setup(name='yoctopuce',
-      version='1.10.54037',
+      version='1.10.54070',
       packages=['yoctopuce'],
       description="Yoctopuce python API",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Yoctopuce",
       author_email="support@yoctopuce.com",
       url="https://www.yoctopuce.com",
```

### Comparing `yoctopuce-1.10.54037/PKG-INFO` & `yoctopuce-1.10.54070/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoctopuce
-Version: 1.10.54037
+Version: 1.10.54070
 Summary: Yoctopuce python API
 Home-page: https://www.yoctopuce.com
 Author: Yoctopuce
 Author-email: support@yoctopuce.com
 License: UNKNOWN
 Project-URL: Documentation, https://www.yoctopuce.com/EN/doc/reference/yoctolib-python-EN.html
 Project-URL: Source, https://github.com/yoctopuce/yoctolib_python
```

