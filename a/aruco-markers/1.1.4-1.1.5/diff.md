# Comparing `tmp/aruco_markers-1.1.4.tar.gz` & `tmp/aruco_markers-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruco_markers-1.1.4.tar", last modified: Sun Apr  9 13:52:29 2023, max compression
+gzip compressed data, was "aruco_markers-1.1.5.tar", last modified: Tue Apr 18 07:42:44 2023, max compression
```

## Comparing `aruco_markers-1.1.4.tar` & `aruco_markers-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.4/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14896 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14060 2023-04-09 13:51:07.000000 aruco_markers-1.1.4/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/aruco_markers/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      332 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/calibrate.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7714 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/camera.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7834 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/detect.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    13056 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/main.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/marker.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/utils.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/aruco_markers.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14896 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/entry_points.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-09 13:39:41.000000 aruco_markers-1.1.4/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-09 13:39:36.000000 aruco_markers-1.1.4/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.5/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    14321 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/aruco_markers/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      332 2023-04-09 14:02:20.000000 aruco_markers-1.1.5/aruco_markers/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-07 11:30:34.000000 aruco_markers-1.1.5/aruco_markers/calibrate.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     8487 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/aruco_markers/camera.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7834 2023-04-18 07:08:11.000000 aruco_markers-1.1.5/aruco_markers/detect.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15125 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/aruco_markers/main.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-09 14:02:20.000000 aruco_markers-1.1.5/aruco_markers/marker.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-04-07 11:30:34.000000 aruco_markers-1.1.5/aruco_markers/utils.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/aruco_markers.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/entry_points.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-18 07:41:44.000000 aruco_markers-1.1.5/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-18 07:41:38.000000 aruco_markers-1.1.5/setup.py
```

### Comparing `aruco_markers-1.1.4/LICENSE` & `aruco_markers-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.4/PKG-INFO` & `aruco_markers-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruco_markers
-Version: 1.1.4
+Version: 1.1.5
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
@@ -70,14 +70,15 @@
 All the data created by these commands are stored here, specified in the following sub-sections.
 
 The available commands are
 * `collect`: Collect data with checkerboard to calibrate a camera.
 * `calibrate`: Calibrate a camera.
 * `generate`: Generate marker tags.
 * `detect`: Detect marker poses from camera feed.
+* `server`: Start a camera server.
 
 The use of these commands are described below.
 In addition, you can access the documentation for ecah command by appending `--help`.
 For example
 ```
 $ aruco generate --help
 usage: aruco generate [OPTIONS]
@@ -203,15 +204,15 @@
 
 You should expect terminal output similar to the following.
 
 ```
 $ aruco collect --width 8 --height 6 --squaresize 25
 Press ESC to quit.
 Created HOMEDIR/aruco_markers_data
-Created HOMEDIR/home/cm22/aruco_markers_data/calibrate
+Created HOMEDIR/aruco_markers_data/calibrate
 Created HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 Data collection completed for the 'CAMERANAME' camera.
 Data saved in HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 ```
 
 In the above, `HOMEDIR` is your home directory, i.e. where ever `~/` is on you PC, and `CAMERANAME` is the camera name used for data collection.
 This should correspond to the camera you intend to calibrate (if you have more than one camera attached to your PC).
@@ -307,15 +308,15 @@
 
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
-Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
+Please see the examples, that show how to implement a simple pose estimator into [ROS 1](example/ros1_tf_publisher.py)/[ROS 2](example/ros2_tf_publisher.py).
 This example assumes you have calibrated your camera by running `aruco collect`, and `aruco calibrate` prior to running this script.
 
 # Build documentation
 
 The documentation is hosted [here](https://cmower.github.io/aruco_markers/).
 However, if you would like to build the documentation yourself, follow these steps.
 
@@ -330,14 +331,21 @@
 5. View documentation:
    - In a browser, open `html/index.html`
    - Build pdf (requires LaTeX)
 	 - `$ cd latex`
 	 - `$ make`
 	 - Open the file called `refman.pdf`
 
+# Supported cameras
+
+Generally, any camera that is accessible by the OpenCV `VideoCapture` class is supported.
+Others include
+
+* The [ZED-Mini](https://www.stereolabs.com/zed-mini/) RGBD camera.
+
 # Citing
 
 If you use `aruco_markers` in your work, please consider citing the following.
 
 ```bibtex
 @software{Mower2023
   title = "aruco_markers: A Compact Python Package for handling ArUCo markers",
```

### Comparing `aruco_markers-1.1.4/README.md` & `aruco_markers-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 All the data created by these commands are stored here, specified in the following sub-sections.
 
 The available commands are
 * `collect`: Collect data with checkerboard to calibrate a camera.
 * `calibrate`: Calibrate a camera.
 * `generate`: Generate marker tags.
 * `detect`: Detect marker poses from camera feed.
+* `server`: Start a camera server.
 
 The use of these commands are described below.
 In addition, you can access the documentation for ecah command by appending `--help`.
 For example
 ```
 $ aruco generate --help
 usage: aruco generate [OPTIONS]
@@ -184,15 +185,15 @@
 
 You should expect terminal output similar to the following.
 
 ```
 $ aruco collect --width 8 --height 6 --squaresize 25
 Press ESC to quit.
 Created HOMEDIR/aruco_markers_data
-Created HOMEDIR/home/cm22/aruco_markers_data/calibrate
+Created HOMEDIR/aruco_markers_data/calibrate
 Created HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 Data collection completed for the 'CAMERANAME' camera.
 Data saved in HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 ```
 
 In the above, `HOMEDIR` is your home directory, i.e. where ever `~/` is on you PC, and `CAMERANAME` is the camera name used for data collection.
 This should correspond to the camera you intend to calibrate (if you have more than one camera attached to your PC).
@@ -288,15 +289,15 @@
 
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
-Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
+Please see the examples, that show how to implement a simple pose estimator into [ROS 1](example/ros1_tf_publisher.py)/[ROS 2](example/ros2_tf_publisher.py).
 This example assumes you have calibrated your camera by running `aruco collect`, and `aruco calibrate` prior to running this script.
 
 # Build documentation
 
 The documentation is hosted [here](https://cmower.github.io/aruco_markers/).
 However, if you would like to build the documentation yourself, follow these steps.
 
@@ -311,14 +312,21 @@
 5. View documentation:
    - In a browser, open `html/index.html`
    - Build pdf (requires LaTeX)
 	 - `$ cd latex`
 	 - `$ make`
 	 - Open the file called `refman.pdf`
 
+# Supported cameras
+
+Generally, any camera that is accessible by the OpenCV `VideoCapture` class is supported.
+Others include
+
+* The [ZED-Mini](https://www.stereolabs.com/zed-mini/) RGBD camera.
+
 # Citing
 
 If you use `aruco_markers` in your work, please consider citing the following.
 
 ```bibtex
 @software{Mower2023
   title = "aruco_markers: A Compact Python Package for handling ArUCo markers",
```

### Comparing `aruco_markers-1.1.4/aruco_markers/calibrate.py` & `aruco_markers-1.1.5/aruco_markers/calibrate.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.4/aruco_markers/camera.py` & `aruco_markers-1.1.5/aruco_markers/camera.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,14 +113,45 @@
         self._img = cv2.imdecode(img_data, cv2.IMREAD_COLOR)
         return self._img
 
     def close(self):
         self.sock.close()
 
 
+class ZEDMCamera(cvCamera):
+    def __init__(self, index, side="left"):
+        super().__init__(index)
+        self.side = side
+
+        if side == "left":
+            self.extract = self.extract_left
+        elif side == "right":
+            self.extract = self.extract_right
+        else:
+            raise ValueError(f"did not recognize side '{side}'")
+
+    @property
+    def name(self):
+        return super().name + f"_zedm_{self.side}"
+
+    def extract_left(self, full_img):
+        return full_img[:, : self.width]
+
+    def extract_right(self, full_img):
+        return full_img[:, self.width :]
+
+    @property
+    def width(self):
+        return int(super().width / 2)
+
+    def read(self):
+        full_img = super().read()
+        return self.extract(full_img)
+
+
 class CameraViewerCallback(abc.ABC):
 
     """! Callback class for the camera viewer. You must implement the call method that inputs an image (from the interface) and outputs the image to be viewed."""
 
     def __init__(self):
         """! Initializer for the CameraViewerCallback class."""
         self.num_calls = 0
```

### Comparing `aruco_markers-1.1.4/aruco_markers/detect.py` & `aruco_markers-1.1.5/aruco_markers/detect.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.4/aruco_markers/main.py` & `aruco_markers-1.1.5/aruco_markers/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import sys
 import argparse
 from collections import OrderedDict
 
 from .marker import Marker
-from .camera import cvCamera, CameraViewer, ServerCameraViewerCallback, UDPSenderServer
+from .camera import (
+    cvCamera,
+    CameraViewer,
+    ServerCameraViewerCallback,
+    UDPSenderServer,
+    ZEDMCamera,
+)
 from .calibrate import collect_data, calibrate, Checkerboard
 from .detect import detect_poses_from_camera, DetectSingleMarkerPoseFromCameraCallback
 
 #
 # Helper variables/methods for setting up documentation
 #
 
@@ -261,18 +267,44 @@
         default=False,
         help=helptxt(
             "Report the duration of each loop in the camera feed callback.",
             "By default, the duration is not reported.",
         ),
     )
 
+    parser.add_argument(
+        "-z",
+        "--zedm",
+        action="store_true",
+        default=False,
+        help=helptxt("The camera is the ZEDm dual RGBD camera."),
+    )
+
+    rgbdside_param_default = "left"
+    parser.add_argument(
+        "-s",
+        "--rgbdside",
+        type=str,
+        choices=["left", "right"],
+        default=rgbdside_param_default,
+        help=helptxt(
+            "The side of the RGBD camera used.",
+            "When the camera is not RGBD, this argument is ignored.",
+            default=rgbdside_param_default,
+        ),
+    )
+
     args = parser.parse_args(argv)
 
     # Setup camera and checkerboard
-    camera = cvCamera(args.cameraindex)
+
+    if not args.zedm:
+        camera = cvCamera(args.cameraindex)
+    else:
+        camera = ZEDMCamera(args.cameraindex, side=args.rgbdside)
     checkerboard = Checkerboard(
         camera.name.replace(" ", "-"),  # ensure no space in name
         args.width,
         args.height,
         args.squaresize,
     )
 
@@ -390,26 +422,51 @@
         help=helptxt(
             "Marker index.",
             default=cameraindex_param_default,
         ),
     )
 
     parser.add_argument(
+        "-z",
+        "--zedm",
+        action="store_true",
+        default=False,
+        help=helptxt("The camera is the ZEDm dual RGBD camera."),
+    )
+
+    parser.add_argument(
         "-r",
         "--reportduration",
         action="store_true",
         default=False,
         help="Report the duration of each loop in the camera feed callback. "
         + "By default, the duration is not reported.",
     )
 
+    rgbdside_param_default = "left"
+    parser.add_argument(
+        "-s",
+        "--rgbdside",
+        type=str,
+        choices=["left", "right"],
+        default=rgbdside_param_default,
+        help=helptxt(
+            "The side of the RGBD camera used.",
+            "When the camera is not RGBD, this argument is ignored.",
+            default=rgbdside_param_default,
+        ),
+    )
+
     args = parser.parse_args(argv)
 
     # Run pose detection
-    camera = cvCamera(args.cameraindex)
+    if not args.zedm:
+        camera = cvCamera(args.cameraindex)
+    else:
+        camera = ZEDMCamera(args.cameraindex, side=args.rgbdside)
     callback = DetectSingleMarkerPoseFromCameraCallback(
         camera, args.dict, args.markerindex
     )
 
     detect_poses_from_camera(camera, callback, args.reportduration)
 
 
@@ -438,18 +495,43 @@
         default=compressionquality_param_default,
         help=helptxt(
             "Quality of the compression, in range 0 to 100.",
             default=compressionquality_param_default,
         ),
     )
 
+    parser.add_argument(
+        "-z",
+        "--zedm",
+        action="store_true",
+        default=False,
+        help=helptxt("The camera is the ZEDm dual RGBD camera."),
+    )
+
+    rgbdside_param_default = "left"
+    parser.add_argument(
+        "-s",
+        "--rgbdside",
+        type=str,
+        choices=["left", "right"],
+        default=rgbdside_param_default,
+        help=helptxt(
+            "The side of the RGBD camera used.",
+            "When the camera is not RGBD, this argument is ignored.",
+            default=rgbdside_param_default,
+        ),
+    )
+
     args = parser.parse_args(argv)
 
     # Setup camera
-    camera = cvCamera(args.cameraindex)
+    if not args.zedm:
+        camera = cvCamera(args.cameraindex)
+    else:
+        camera = ZEDMCamera(args.cameraindex, side=args.rgbdside)
 
     # Setup server and callback
     assert 0 <= args.compressionquality <= 100, (
         f"Compression quality argument outside of allowed range. "
         + "Got '{args.compressionquality}' expected in range 0 to 100."
     )
     sender_server = UDPSenderServer()
```

### Comparing `aruco_markers-1.1.4/aruco_markers/marker.py` & `aruco_markers-1.1.5/aruco_markers/marker.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.4/aruco_markers.egg-info/PKG-INFO` & `aruco_markers-1.1.5/aruco_markers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruco-markers
-Version: 1.1.4
+Version: 1.1.5
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
@@ -70,14 +70,15 @@
 All the data created by these commands are stored here, specified in the following sub-sections.
 
 The available commands are
 * `collect`: Collect data with checkerboard to calibrate a camera.
 * `calibrate`: Calibrate a camera.
 * `generate`: Generate marker tags.
 * `detect`: Detect marker poses from camera feed.
+* `server`: Start a camera server.
 
 The use of these commands are described below.
 In addition, you can access the documentation for ecah command by appending `--help`.
 For example
 ```
 $ aruco generate --help
 usage: aruco generate [OPTIONS]
@@ -203,15 +204,15 @@
 
 You should expect terminal output similar to the following.
 
 ```
 $ aruco collect --width 8 --height 6 --squaresize 25
 Press ESC to quit.
 Created HOMEDIR/aruco_markers_data
-Created HOMEDIR/home/cm22/aruco_markers_data/calibrate
+Created HOMEDIR/aruco_markers_data/calibrate
 Created HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 Data collection completed for the 'CAMERANAME' camera.
 Data saved in HOMEDIR/aruco_markers_data/calibrate/CAMERANAME
 ```
 
 In the above, `HOMEDIR` is your home directory, i.e. where ever `~/` is on you PC, and `CAMERANAME` is the camera name used for data collection.
 This should correspond to the camera you intend to calibrate (if you have more than one camera attached to your PC).
@@ -307,15 +308,15 @@
 
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
-Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
+Please see the examples, that show how to implement a simple pose estimator into [ROS 1](example/ros1_tf_publisher.py)/[ROS 2](example/ros2_tf_publisher.py).
 This example assumes you have calibrated your camera by running `aruco collect`, and `aruco calibrate` prior to running this script.
 
 # Build documentation
 
 The documentation is hosted [here](https://cmower.github.io/aruco_markers/).
 However, if you would like to build the documentation yourself, follow these steps.
 
@@ -330,14 +331,21 @@
 5. View documentation:
    - In a browser, open `html/index.html`
    - Build pdf (requires LaTeX)
 	 - `$ cd latex`
 	 - `$ make`
 	 - Open the file called `refman.pdf`
 
+# Supported cameras
+
+Generally, any camera that is accessible by the OpenCV `VideoCapture` class is supported.
+Others include
+
+* The [ZED-Mini](https://www.stereolabs.com/zed-mini/) RGBD camera.
+
 # Citing
 
 If you use `aruco_markers` in your work, please consider citing the following.
 
 ```bibtex
 @software{Mower2023
   title = "aruco_markers: A Compact Python Package for handling ArUCo markers",
```

### Comparing `aruco_markers-1.1.4/pyproject.toml` & `aruco_markers-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruco_markers"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = " A compact Python package for handling ArUCo markers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aruco_markers-1.1.4/setup.py` & `aruco_markers-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="aruco_markers",
     description="A compact Python package for handling ArUCo markers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.1.4",
+    version="1.1.5",
     author="Christopher E. Mower",
     author_email="christopher.mower@kcl.ac.uk",
     url="https://github.com/cmower/aruco_markers",
     packages=["aruco_markers"],
     license="Apache License 2.0",
     entry_points={
         "console_scripts": [
```

