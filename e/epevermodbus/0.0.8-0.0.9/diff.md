# Comparing `tmp/epevermodbus-0.0.8.tar.gz` & `tmp/epevermodbus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/epevermodbus-0.0.8.tar", last modified: Sun Aug  8 21:16:24 2021, max compression
+gzip compressed data, was "dist/epevermodbus-0.0.9.tar", last modified: Sun Aug  8 21:39:46 2021, max compression
```

## Comparing `epevermodbus-0.0.8.tar` & `epevermodbus-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:16:24.475314 epevermodbus-0.0.8/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2516 2021-08-08 21:16:24.475314 epevermodbus-0.0.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1533 2021-08-08 16:12:06.000000 epevermodbus-0.0.8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:16:24.471314 epevermodbus-0.0.8/epevermodbus/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       55 2021-08-08 14:52:32.000000 epevermodbus-0.0.8/epevermodbus/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2605 2021-08-08 16:13:08.000000 epevermodbus-0.0.8/epevermodbus/command_line.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9500 2021-08-08 21:16:03.000000 epevermodbus-0.0.8/epevermodbus/driver.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:16:24.471314 epevermodbus-0.0.8/epevermodbus.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2516 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      313 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2021-08-08 21:16:24.000000 epevermodbus-0.0.8/epevermodbus.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2021-08-08 21:16:24.475314 epevermodbus-0.0.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      707 2021-08-08 21:16:16.000000 epevermodbus-0.0.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:39:46.458648 epevermodbus-0.0.9/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3867 2021-08-08 21:39:46.458648 epevermodbus-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2804 2021-08-08 21:21:16.000000 epevermodbus-0.0.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:39:46.454648 epevermodbus-0.0.9/epevermodbus/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       55 2021-08-08 14:52:32.000000 epevermodbus-0.0.9/epevermodbus/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2872 2021-08-08 21:39:24.000000 epevermodbus-0.0.9/epevermodbus/command_line.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10056 2021-08-08 21:39:25.000000 epevermodbus-0.0.9/epevermodbus/driver.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2021-08-08 21:39:46.458648 epevermodbus-0.0.9/epevermodbus.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3867 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      313 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2021-08-08 21:39:46.000000 epevermodbus-0.0.9/epevermodbus.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2021-08-08 21:39:46.458648 epevermodbus-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      707 2021-08-08 21:26:08.000000 epevermodbus-0.0.9/setup.py
```

### Comparing `epevermodbus-0.0.8/epevermodbus/command_line.py` & `epevermodbus-0.0.9/epevermodbus/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     print("Solar power L:", controller.get_solar_power_l())
     print("Solar power H:", controller.get_solar_power_h())
     print("Load voltage:", controller.get_load_voltage())
     print("Load current:", controller.get_load_current())
     print("Load power:", controller.get_load_power())
     print("Load power L:", controller.get_load_power_l())
     print("Load power H:", controller.get_load_power_h())
-    print("Battery capacity:", controller.get_battery_capacity())
     print("Battery current L:", controller.get_battery_current_l())
     print("Battery current H:", controller.get_battery_current_h())
     print("Battery voltage:", controller.get_battery_voltage())
     print("Battery state of charge:", controller.get_battery_state_of_charge())
     print("Battery temperature:", controller.get_battery_temperature())
     print("Remote battery temperature:", controller.get_remote_battery_temperature())
     print("Controller temperature:", controller.get_controller_temperature())
@@ -48,11 +47,18 @@
     )
     print("Device over temperature:", controller.is_device_over_temperature())
     print("\n")
     print("Battery Parameters:")
     print("Rated charging current:", controller.get_rated_charging_current())
     print("Rated load current:", controller.get_rated_load_current())
     print("Battery real rated voltage:", controller.get_battery_real_rated_voltage())
+    print("Battery type:", controller.get_battery_type())
+    print("Battery capacity:", controller.get_battery_capacity())
+    print(
+        "Temperature compensation coefficient:",
+        controller.get_temperature_compensation_coefficient(),
+    )
+    print("Over voltage disconnect:", controller.get_over_voltage_disconnect())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `epevermodbus-0.0.8/epevermodbus/driver.py` & `epevermodbus-0.0.9/epevermodbus/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,14 @@
         """Load power L"""
         return self.retriable_read_register(0x310E, 2, 4)
 
     def get_load_power_h(self):
         """Load power H"""
         return self.retriable_read_register(0x310F, 2, 4)
 
-    def get_battery_capacity(self):
-        """Battery capacity in amp hours"""
-        return self.retriable_read_register(0x9001, 0, 3)
-
     def get_battery_current_l(self):
         """Battery current L"""
         return self.retriable_read_register(0x331B, 2, 4)
 
     def get_battery_current_h(self):
         """Battery current H"""
         return self.retriable_read_register(0x331C, 2, 4)
@@ -261,7 +257,25 @@
     def get_rated_load_current(self):
         """Rated load current"""
         return self.retriable_read_register(0x300E, 2, 4)
 
     def get_battery_real_rated_voltage(self):
         """Battery real rated voltage"""
         return self.retriable_read_register(0x311D, 2, 4)
+
+    def get_battery_type(self):
+        """Battery type"""
+        battery_type = self.retriable_read_register(0x9000, 2, 3)
+        battery_types = {0: "USER_DEFINED", 1: "SEALED", 2: "GEL", 3: "FLOODED"}
+        return battery_types[battery_type]
+
+    def get_battery_capacity(self):
+        """Battery capacity in amp hours"""
+        return self.retriable_read_register(0x9001, 0, 3)
+
+    def get_temperature_compensation_coefficient(self):
+        """Temperature compensation coefficient"""
+        return self.retriable_read_register(0x9002, 0, 3)
+
+    def get_over_voltage_disconnect(self):
+        """Over voltage disconnect"""
+        return self.retriable_read_register(0x9003, 2, 3)
```

### Comparing `epevermodbus-0.0.8/setup.py` & `epevermodbus-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="epevermodbus",
-    version="0.0.8",
+    version="0.0.9",
     description="",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/rosswarren/epevermodbus",
     author="Ross Warren",
     author_email="rosswarren4@gmail.com",
     license="MIT",
```

