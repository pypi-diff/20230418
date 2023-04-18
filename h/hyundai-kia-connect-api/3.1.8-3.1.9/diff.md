# Comparing `tmp/hyundai_kia_connect_api-3.1.8.tar.gz` & `tmp/hyundai_kia_connect_api-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.1.8.tar", last modified: Sun Apr  9 21:20:57 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.1.9.tar", last modified: Sun Apr  9 21:34:25 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.1.8.tar` & `hyundai_kia_connect_api-3.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:57.765149 hyundai_kia_connect_api-3.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30574 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 21:20:57.000000 hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-09 21:20:41.000000 hyundai_kia_connect_api-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:57.769149 hyundai_kia_connect_api-3.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-09 21:20:04.000000 hyundai_kia_connect_api-3.1.8/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:25.217684 hyundai_kia_connect_api-3.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30570 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 21:34:25.000000 hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-09 21:34:13.000000 hyundai_kia_connect_api-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:34:25.221684 hyundai_kia_connect_api-3.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-09 21:33:40.000000 hyundai_kia_connect_api-3.1.9/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.1.8/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/LICENSE` & `hyundai_kia_connect_api-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/PKG-INFO` & `hyundai_kia_connect_api-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.1.8/README.rst` & `hyundai_kia_connect_api-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/docs/Makefile` & `hyundai_kia_connect_api-3.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/docs/conf.py` & `hyundai_kia_connect_api-3.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/docs/installation.rst` & `hyundai_kia_connect_api-3.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/docs/make.bat` & `hyundai_kia_connect_api-3.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     temperature_range_c_new = [x * 0.5 for x in range(28, 64)]
     temperature_range_model_year = 2020
 
     def __init__(self, region: int, brand: int, language: str) -> None:
         self.vehicle_timezone = self.data_timezone
         self.LANGUAGE: str = language
         if BRANDS[brand] == BRAND_KIA:
-            self.BASE_URL: str = "www.kiaconnect.ca"
+            self.BASE_URL: str = "kiaconnect.ca"
         elif BRANDS[brand] == BRAND_HYUNDAI:
             self.BASE_URL: str = "mybluelink.ca"
         self.old_vehicle_status = {}
         self.API_URL: str = "https://" + self.BASE_URL + "/tods/api/"
         self.API_HEADERS = {
             "content-type": "application/json;charset=UTF-8",
             "accept": "application/json, text/plain, */*",
```

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.1.8/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.1.9/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/setup.py` & `hyundai_kia_connect_api-3.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.1.8",
+    version="3.1.9",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.1.8/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.1.9/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.1.8/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.1.9/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

