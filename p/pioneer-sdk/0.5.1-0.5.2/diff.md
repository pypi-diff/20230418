# Comparing `tmp/pioneer_sdk-0.5.1.tar.gz` & `tmp/pioneer_sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pioneer_sdk-0.5.1.tar", last modified: Tue Dec 27 10:55:16 2022, max compression
+gzip compressed data, was "pioneer_sdk-0.5.2.tar", last modified: Tue Apr 18 15:01:42 2023, max compression
```

## Comparing `pioneer_sdk-0.5.1.tar` & `pioneer_sdk-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 10:55:16.440299 pioneer_sdk-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1704 2022-12-27 10:55:16.440299 pioneer_sdk-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1183 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 10:55:16.436299 pioneer_sdk-0.5.1/pioneer_sdk/
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4751 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/camera.py
--rw-rw-rw-   0 root         (0) root         (0)     2981 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/generic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 10:55:16.440299 pioneer_sdk-0.5.1/pioneer_sdk/mavsub/
--rw-rw-rw-   0 root         (0) root         (0)    20412 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/mavsub/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/mavsub/wifi.py
--rw-rw-rw-   0 root         (0) root         (0)    25026 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/piosdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 10:55:16.440299 pioneer_sdk-0.5.1/pioneer_sdk/tools/
--rw-rw-rw-   0 root         (0) root         (0)      423 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/tools/lua.py
--rwxrwxrwx   0 root         (0) root         (0)   149144 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/tools/luac
--rw-rw-rw-   0 root         (0) root         (0)   190976 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/pioneer_sdk/tools/luac.exe
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 10:55:16.436299 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1704 2022-12-27 10:55:16.000000 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2022-12-27 10:55:16.000000 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 10:55:16.000000 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2022-12-27 10:55:16.000000 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-12-27 10:55:16.000000 pioneer_sdk-0.5.1/pioneer_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 10:55:16.440299 pioneer_sdk-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2022-12-27 10:55:01.000000 pioneer_sdk-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:01:42.024376 pioneer_sdk-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-04-18 15:01:42.024376 pioneer_sdk-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:01:42.020376 pioneer_sdk-0.5.2/pioneer_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/camera.py
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/generic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:01:42.020376 pioneer_sdk-0.5.2/pioneer_sdk/mavsub/
+-rw-rw-rw-   0 root         (0) root         (0)    20412 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/mavsub/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/mavsub/wifi.py
+-rw-rw-rw-   0 root         (0) root         (0)    25026 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/piosdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:01:42.024376 pioneer_sdk-0.5.2/pioneer_sdk/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/tools/lua.py
+-rwxrwxrwx   0 root         (0) root         (0)   149144 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/tools/luac
+-rw-rw-rw-   0 root         (0) root         (0)   190976 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/pioneer_sdk/tools/luac.exe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:01:42.020376 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-04-18 15:01:41.000000 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-18 15:01:41.000000 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:01:41.000000 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-18 15:01:41.000000 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-18 15:01:41.000000 pioneer_sdk-0.5.2/pioneer_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:01:42.024376 pioneer_sdk-0.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-18 15:01:26.000000 pioneer_sdk-0.5.2/setup.py
```

### Comparing `pioneer_sdk-0.5.1/LICENSE.txt` & `pioneer_sdk-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/PKG-INFO` & `pioneer_sdk-0.5.2/pioneer_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pioneer_sdk
-Version: 0.5.1
+Name: pioneer-sdk
+Version: 0.5.2
 Summary: Programming tools for programming geoscan pioneer drone
 Home-page: https://github.com/geoscan/pioneer_sdk
 Author: geoscan
 Author-email: info@geoscan.aero
 License: MIT
 Keywords: mavlink,pioneer,geoscan
 Platform: UNKNOWN
```

### Comparing `pioneer_sdk-0.5.1/README.md` & `pioneer_sdk-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/camera.py` & `pioneer_sdk-0.5.2/pioneer_sdk/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,24 @@
         return frame
 
 
 class VideoStream:
     def __init__(self, logger=True):
         self.camera = Camera(log_connection=logger)
         self.logger = logger
-        self._vidio_stream = None
+        self._video_stream = None
         self._stop = threading.Event()
         self._stop.set()
 
     def start(self):
         if not self._stop.is_set():
             return
         self._stop.clear()
-        self._vidio_stream = threading.Thread(target=self._stream, daemon=True)
-        self._vidio_stream.start()
+        self._video_stream = threading.Thread(target=self._stream, daemon=True)
+        self._video_stream.start()
 
     def stop(self):
         self._stop.set()
 
     def _stream(self):
         """
         Continuously receives JPEG frames from ESP32, parses them, and renders it using standard OpenCV's image rendering
```

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/generic.py` & `pioneer_sdk-0.5.2/pioneer_sdk/generic.py`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/mavsub/ftp.py` & `pioneer_sdk-0.5.2/pioneer_sdk/mavsub/ftp.py`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/mavsub/wifi.py` & `pioneer_sdk-0.5.2/pioneer_sdk/mavsub/wifi.py`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/piosdk.py` & `pioneer_sdk-0.5.2/pioneer_sdk/piosdk.py`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/tools/luac` & `pioneer_sdk-0.5.2/pioneer_sdk/tools/luac`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk/tools/luac.exe` & `pioneer_sdk-0.5.2/pioneer_sdk/tools/luac.exe`

 * *Files identical despite different names*

### Comparing `pioneer_sdk-0.5.1/pioneer_sdk.egg-info/PKG-INFO` & `pioneer_sdk-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pioneer-sdk
-Version: 0.5.1
+Name: pioneer_sdk
+Version: 0.5.2
 Summary: Programming tools for programming geoscan pioneer drone
 Home-page: https://github.com/geoscan/pioneer_sdk
 Author: geoscan
 Author-email: info@geoscan.aero
 License: MIT
 Keywords: mavlink,pioneer,geoscan
 Platform: UNKNOWN
```

### Comparing `pioneer_sdk-0.5.1/setup.py` & `pioneer_sdk-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
   name='pioneer_sdk',
   packages=['pioneer_sdk', 'pioneer_sdk.mavsub', 'pioneer_sdk.tools'],
   include_package_data=True,
-  version='0.5.1',
+  version='0.5.2',
   license='MIT',
   description='Programming tools for programming geoscan pioneer drone',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='geoscan',
   author_email='info@geoscan.aero',
   url='https://github.com/geoscan/pioneer_sdk',
   keywords=['mavlink', 'pioneer', 'geoscan'],
   setup_requires=['wheel'],
   install_requires=[
-          'pymavlink',
-          'pyserial',
-          'future',
-          'numpy',
-          'opencv-contrib-python'
+          'pymavlink==2.4.37',
+          'pyserial==3.5',
+          'future==0.18.3',
+          'numpy==1.21.2',
+          'opencv-contrib-python==4.7.0.72'
       ],
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
   python_requires='>=3.7',
```

