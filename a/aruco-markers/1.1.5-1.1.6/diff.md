# Comparing `tmp/aruco_markers-1.1.5.tar.gz` & `tmp/aruco_markers-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruco_markers-1.1.5.tar", last modified: Tue Apr 18 07:42:44 2023, max compression
+gzip compressed data, was "aruco_markers-1.1.6.tar", last modified: Tue Apr 18 08:01:11 2023, max compression
```

## Comparing `aruco_markers-1.1.5.tar` & `aruco_markers-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.5/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14321 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/aruco_markers/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      332 2023-04-09 14:02:20.000000 aruco_markers-1.1.5/aruco_markers/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-07 11:30:34.000000 aruco_markers-1.1.5/aruco_markers/calibrate.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     8487 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/aruco_markers/camera.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7834 2023-04-18 07:08:11.000000 aruco_markers-1.1.5/aruco_markers/detect.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    15125 2023-04-18 07:40:47.000000 aruco_markers-1.1.5/aruco_markers/main.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-09 14:02:20.000000 aruco_markers-1.1.5/aruco_markers/marker.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-04-07 11:30:34.000000 aruco_markers-1.1.5/aruco_markers/utils.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/aruco_markers.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/entry_points.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-18 07:42:44.000000 aruco_markers-1.1.5/aruco_markers.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-18 07:41:44.000000 aruco_markers-1.1.5/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-18 07:42:44.991690 aruco_markers-1.1.5/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-18 07:41:38.000000 aruco_markers-1.1.5/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 08:01:11.219423 aruco_markers-1.1.6/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.6/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 08:01:11.219423 aruco_markers-1.1.6/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    14321 2023-04-18 07:40:47.000000 aruco_markers-1.1.6/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 08:01:11.219423 aruco_markers-1.1.6/aruco_markers/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      332 2023-04-09 14:02:20.000000 aruco_markers-1.1.6/aruco_markers/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-07 11:30:34.000000 aruco_markers-1.1.6/aruco_markers/calibrate.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     8487 2023-04-18 07:40:47.000000 aruco_markers-1.1.6/aruco_markers/camera.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7834 2023-04-18 07:08:11.000000 aruco_markers-1.1.6/aruco_markers/detect.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15128 2023-04-18 07:49:11.000000 aruco_markers-1.1.6/aruco_markers/main.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-09 14:02:20.000000 aruco_markers-1.1.6/aruco_markers/marker.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-04-07 11:30:34.000000 aruco_markers-1.1.6/aruco_markers/utils.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-18 08:01:11.219423 aruco_markers-1.1.6/aruco_markers.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15157 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/entry_points.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-18 08:01:11.000000 aruco_markers-1.1.6/aruco_markers.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-18 08:00:06.000000 aruco_markers-1.1.6/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-18 08:01:11.219423 aruco_markers-1.1.6/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-18 08:00:01.000000 aruco_markers-1.1.6/setup.py
```

### Comparing `aruco_markers-1.1.5/LICENSE` & `aruco_markers-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/PKG-INFO` & `aruco_markers-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruco_markers
-Version: 1.1.5
+Version: 1.1.6
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
```

### Comparing `aruco_markers-1.1.5/README.md` & `aruco_markers-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/aruco_markers/calibrate.py` & `aruco_markers-1.1.6/aruco_markers/calibrate.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/aruco_markers/camera.py` & `aruco_markers-1.1.6/aruco_markers/camera.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/aruco_markers/detect.py` & `aruco_markers-1.1.6/aruco_markers/detect.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/aruco_markers/main.py` & `aruco_markers-1.1.6/aruco_markers/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         action="store_true",
         default=False,
         help=helptxt("The camera is the ZEDm dual RGBD camera."),
     )
 
     rgbdside_param_default = "left"
     parser.add_argument(
-        "-s",
+        "-rs",
         "--rgbdside",
         type=str,
         choices=["left", "right"],
         default=rgbdside_param_default,
         help=helptxt(
             "The side of the RGBD camera used.",
             "When the camera is not RGBD, this argument is ignored.",
@@ -440,15 +440,15 @@
         default=False,
         help="Report the duration of each loop in the camera feed callback. "
         + "By default, the duration is not reported.",
     )
 
     rgbdside_param_default = "left"
     parser.add_argument(
-        "-s",
+        "-rs",
         "--rgbdside",
         type=str,
         choices=["left", "right"],
         default=rgbdside_param_default,
         help=helptxt(
             "The side of the RGBD camera used.",
             "When the camera is not RGBD, this argument is ignored.",
@@ -505,15 +505,15 @@
         action="store_true",
         default=False,
         help=helptxt("The camera is the ZEDm dual RGBD camera."),
     )
 
     rgbdside_param_default = "left"
     parser.add_argument(
-        "-s",
+        "-rs",
         "--rgbdside",
         type=str,
         choices=["left", "right"],
         default=rgbdside_param_default,
         help=helptxt(
             "The side of the RGBD camera used.",
             "When the camera is not RGBD, this argument is ignored.",
```

### Comparing `aruco_markers-1.1.5/aruco_markers/marker.py` & `aruco_markers-1.1.6/aruco_markers/marker.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.5/aruco_markers.egg-info/PKG-INFO` & `aruco_markers-1.1.6/aruco_markers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruco-markers
-Version: 1.1.5
+Version: 1.1.6
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
```

### Comparing `aruco_markers-1.1.5/pyproject.toml` & `aruco_markers-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruco_markers"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = " A compact Python package for handling ArUCo markers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aruco_markers-1.1.5/setup.py` & `aruco_markers-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="aruco_markers",
     description="A compact Python package for handling ArUCo markers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.1.5",
+    version="1.1.6",
     author="Christopher E. Mower",
     author_email="christopher.mower@kcl.ac.uk",
     url="https://github.com/cmower/aruco_markers",
     packages=["aruco_markers"],
     license="Apache License 2.0",
     entry_points={
         "console_scripts": [
```

