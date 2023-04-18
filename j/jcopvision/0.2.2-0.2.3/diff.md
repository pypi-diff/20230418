# Comparing `tmp/jcopvision-0.2.2.tar.gz` & `tmp/jcopvision-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcopvision-0.2.2.tar", last modified: Tue Feb 21 07:29:53 2023, max compression
+gzip compressed data, was "jcopvision-0.2.3.tar", last modified: Tue Apr 18 17:30:55 2023, max compression
```

## Comparing `jcopvision-0.2.2.tar` & `jcopvision-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.167055 jcopvision-0.2.2/
--rw-r--r--   0 bmduser    (501) staff       (20)     1513 2023-02-10 18:31:03.000000 jcopvision-0.2.2/LICENSE
--rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-02-21 07:29:53.167212 jcopvision-0.2.2/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      283 2023-02-10 18:31:03.000000 jcopvision-0.2.2/README.md
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.156121 jcopvision-0.2.2/jcopvision/
--rw-r--r--   0 bmduser    (501) staff       (20)       80 2023-02-21 07:22:48.000000 jcopvision-0.2.2/jcopvision/__init__.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.159876 jcopvision-0.2.2/jcopvision/draw/
--rw-r--r--   0 bmduser    (501) staff       (20)      157 2023-02-21 07:03:57.000000 jcopvision-0.2.2/jcopvision/draw/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2595 2023-02-17 17:03:21.000000 jcopvision-0.2.2/jcopvision/draw/bbox.py
--rw-r--r--   0 bmduser    (501) staff       (20)      982 2023-02-17 17:03:25.000000 jcopvision-0.2.2/jcopvision/draw/circle.py
--rw-r--r--   0 bmduser    (501) staff       (20)      850 2023-02-17 17:03:56.000000 jcopvision-0.2.2/jcopvision/draw/imshow.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1471 2023-02-21 07:25:20.000000 jcopvision-0.2.2/jcopvision/draw/text.py
--rw-r--r--   0 bmduser    (501) staff       (20)      146 2023-02-17 11:27:53.000000 jcopvision-0.2.2/jcopvision/exception.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.161562 jcopvision-0.2.2/jcopvision/image_processing/
--rw-r--r--   0 bmduser    (501) staff       (20)      137 2023-02-17 17:21:06.000000 jcopvision-0.2.2/jcopvision/image_processing/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1360 2023-02-17 17:04:55.000000 jcopvision-0.2.2/jcopvision/image_processing/blending.py
--rw-r--r--   0 bmduser    (501) staff       (20)      415 2023-02-17 17:05:43.000000 jcopvision-0.2.2/jcopvision/image_processing/enhancement.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1888 2023-02-17 17:06:45.000000 jcopvision-0.2.2/jcopvision/image_processing/masking.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.163527 jcopvision-0.2.2/jcopvision/io/
--rw-r--r--   0 bmduser    (501) staff       (20)      161 2023-02-17 17:20:33.000000 jcopvision-0.2.2/jcopvision/io/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      701 2023-02-17 17:12:22.000000 jcopvision-0.2.2/jcopvision/io/jupyter.py
--rw-r--r--   0 bmduser    (501) staff       (20)     4347 2023-02-21 06:58:23.000000 jcopvision-0.2.2/jcopvision/io/reader.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1527 2023-02-17 17:08:47.000000 jcopvision-0.2.2/jcopvision/io/utils.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3026 2023-02-17 17:16:45.000000 jcopvision-0.2.2/jcopvision/io/writer.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.166657 jcopvision-0.2.2/jcopvision/utils/
--rw-r--r--   0 bmduser    (501) staff       (20)      434 2023-02-17 17:28:50.000000 jcopvision-0.2.2/jcopvision/utils/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      260 2023-02-17 17:23:09.000000 jcopvision-0.2.2/jcopvision/utils/background.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2018 2023-02-17 17:23:57.000000 jcopvision-0.2.2/jcopvision/utils/bbox.py
--rw-r--r--   0 bmduser    (501) staff       (20)      524 2023-02-17 17:24:40.000000 jcopvision-0.2.2/jcopvision/utils/color.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1810 2023-02-17 17:26:23.000000 jcopvision-0.2.2/jcopvision/utils/filter.py
--rw-r--r--   0 bmduser    (501) staff       (20)      505 2023-02-17 17:26:44.000000 jcopvision-0.2.2/jcopvision/utils/image.py
--rw-r--r--   0 bmduser    (501) staff       (20)      537 2023-02-17 17:27:38.000000 jcopvision-0.2.2/jcopvision/utils/landmark.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-02-21 07:29:53.157830 jcopvision-0.2.2/jcopvision.egg-info/
--rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-02-21 07:29:53.000000 jcopvision-0.2.2/jcopvision.egg-info/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      857 2023-02-21 07:29:53.000000 jcopvision-0.2.2/jcopvision.egg-info/SOURCES.txt
--rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-02-21 07:29:53.000000 jcopvision-0.2.2/jcopvision.egg-info/dependency_links.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       38 2023-02-21 07:29:53.000000 jcopvision-0.2.2/jcopvision.egg-info/requires.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       11 2023-02-21 07:29:53.000000 jcopvision-0.2.2/jcopvision.egg-info/top_level.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-02-21 07:29:53.167817 jcopvision-0.2.2/setup.cfg
--rw-r--r--   0 bmduser    (501) staff       (20)     1093 2023-02-10 18:31:03.000000 jcopvision-0.2.2/setup.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.375317 jcopvision-0.2.3/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1513 2023-02-10 18:31:03.000000 jcopvision-0.2.3/LICENSE
+-rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-18 17:30:55.375424 jcopvision-0.2.3/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      283 2023-02-10 18:31:03.000000 jcopvision-0.2.3/README.md
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.367180 jcopvision-0.2.3/jcopvision/
+-rw-r--r--   0 bmduser    (501) staff       (20)       80 2023-04-18 16:38:02.000000 jcopvision-0.2.3/jcopvision/__init__.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.370400 jcopvision-0.2.3/jcopvision/draw/
+-rw-r--r--   0 bmduser    (501) staff       (20)      192 2023-04-18 17:18:39.000000 jcopvision-0.2.3/jcopvision/draw/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2660 2023-04-18 17:10:33.000000 jcopvision-0.2.3/jcopvision/draw/bbox.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1142 2023-04-18 17:10:47.000000 jcopvision-0.2.3/jcopvision/draw/circle.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      850 2023-02-17 17:03:56.000000 jcopvision-0.2.3/jcopvision/draw/imshow.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1230 2023-04-18 17:17:49.000000 jcopvision-0.2.3/jcopvision/draw/line.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1544 2023-04-18 17:10:58.000000 jcopvision-0.2.3/jcopvision/draw/text.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      146 2023-02-17 11:27:53.000000 jcopvision-0.2.3/jcopvision/exception.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.371468 jcopvision-0.2.3/jcopvision/image_processing/
+-rw-r--r--   0 bmduser    (501) staff       (20)      137 2023-02-17 17:21:06.000000 jcopvision-0.2.3/jcopvision/image_processing/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1360 2023-02-17 17:04:55.000000 jcopvision-0.2.3/jcopvision/image_processing/blending.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      415 2023-02-17 17:05:43.000000 jcopvision-0.2.3/jcopvision/image_processing/enhancement.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1888 2023-02-17 17:06:45.000000 jcopvision-0.2.3/jcopvision/image_processing/masking.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.373167 jcopvision-0.2.3/jcopvision/io/
+-rw-r--r--   0 bmduser    (501) staff       (20)      161 2023-02-17 17:20:33.000000 jcopvision-0.2.3/jcopvision/io/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      701 2023-02-17 17:12:22.000000 jcopvision-0.2.3/jcopvision/io/jupyter.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     4347 2023-02-21 06:58:23.000000 jcopvision-0.2.3/jcopvision/io/reader.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1527 2023-02-17 17:08:47.000000 jcopvision-0.2.3/jcopvision/io/utils.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3026 2023-02-17 17:16:45.000000 jcopvision-0.2.3/jcopvision/io/writer.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.375069 jcopvision-0.2.3/jcopvision/utils/
+-rw-r--r--   0 bmduser    (501) staff       (20)      436 2023-04-18 16:49:05.000000 jcopvision-0.2.3/jcopvision/utils/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      260 2023-02-17 17:23:09.000000 jcopvision-0.2.3/jcopvision/utils/background.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2018 2023-02-17 17:23:57.000000 jcopvision-0.2.3/jcopvision/utils/bbox.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      860 2023-04-18 17:08:49.000000 jcopvision-0.2.3/jcopvision/utils/color.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1810 2023-02-17 17:26:23.000000 jcopvision-0.2.3/jcopvision/utils/filter.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      505 2023-04-18 17:00:09.000000 jcopvision-0.2.3/jcopvision/utils/image.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      537 2023-02-17 17:27:38.000000 jcopvision-0.2.3/jcopvision/utils/landmark.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.368567 jcopvision-0.2.3/jcopvision.egg-info/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      881 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/SOURCES.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/dependency_links.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       38 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/requires.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       11 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/top_level.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-04-18 17:30:55.375878 jcopvision-0.2.3/setup.cfg
+-rw-r--r--   0 bmduser    (501) staff       (20)     1093 2023-02-10 18:31:03.000000 jcopvision-0.2.3/setup.py
```

### Comparing `jcopvision-0.2.2/LICENSE` & `jcopvision-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/PKG-INFO` & `jcopvision-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopvision
-Version: 0.2.2
+Version: 0.2.3
 Summary: J.COp Vision consists of helper tools for computer vision
 Home-page: https://github.com/WiraDKP/jcopvision
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: computer vision dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopvision-0.2.2/jcopvision/draw/bbox.py` & `jcopvision-0.2.3/jcopvision/draw/bbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from jcopvision.utils import denormalize_image, idx2color
+from jcopvision.utils import denormalize_image, parse_color
 
 __all__ = ["draw_single_bbox"]
 
 
 def draw_single_bbox(frame, bbox, color=-1, label=None, conf=None, thickness=1, font=cv2.FONT_HERSHEY_SIMPLEX, fontsize=0.5, fontcolor=(0, 0, 0)):
     '''
     Draw a bounding box with its label
@@ -21,18 +21,19 @@
     === Input ===
     frame: array
         image / frame to be drawn
 
     bbox: (int, int, int, int) or (float, float, float, float)
         4 values representing (xmin, ymin, xmax, ymax)
 
-    color: int or (int, int, int)
+    color: int or (int, int, int) or str
         The color of the bounding box
-        If int, it would be map to default colormap using jcopvision.utils.idx2color. Use -1 for random color.
+        If int, it would be map to default colormap using jcopvision.utils.parse_color. Use -1 for random color.
         If (int, int, int), color in BGR format
+        If str, it will be parsed such in matplotlib colors. Hex code is also accepted
 
     label: str
         A text or class label. It will be added to the inner top left of the bounding box
 
     conf: float
         The prediction confidence (0 to 1)
 
@@ -55,16 +56,15 @@
     === Return ===
     frame: array
         annotated image / frame
     '''
     frame = frame.copy()
     frame = denormalize_image(frame)
 
-    if isinstance(color, int):
-        color = idx2color(color)
+    color = parse_color(color)
 
     bbox = np.array(bbox).astype(int)
     pt1 = tuple(bbox[:2])
     pt2 = tuple(bbox[2:])
 
     cv2.rectangle(frame, pt1, pt2, color, thickness)
```

### Comparing `jcopvision-0.2.2/jcopvision/draw/circle.py` & `jcopvision-0.2.3/jcopvision/draw/circle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from jcopvision.utils import denormalize_image, idx2color
+from jcopvision.utils import denormalize_image, parse_color, denormalize_landmark
 
 __all__ = ["draw_single_circle"]
 
 
 def draw_single_circle(frame, center, radius, color=-1, thickness=1):
     '''
     Draw a circle
@@ -13,29 +13,31 @@
     === Input ===
     frame: array
         image / frame to be drawn
 
     center: (int, int) or (float, float)
         location to draw the circle.
 
-    color: int or (int, int, int)
-        The color of the circle
-        If int, it would be map to default colormap using jcopvision.utils.idx2color. Use -1 for random color.
+    color: int or (int, int, int) or str
+        The color of the bounding box
+        If int, it would be map to default colormap using jcopvision.utils.parse_color. Use -1 for random color.
         If (int, int, int), color in BGR format
+        If str, it will be parsed such in matplotlib colors. Hex code is also accepted
 
     thickness: int
         The circle and text thickness
 
 
     === Return ===
     frame: array
         annotated image / frame
     '''
     frame = frame.copy()
     frame = denormalize_image(frame)
 
-    if isinstance(color, int):
-        color = idx2color(color)
+    color = parse_color(color)
+
+    if not isinstance(center[0], int):
+        center = tuple(denormalize_landmark(frame, center).astype(int))    
 
-    center = tuple(np.array(center).astype(int))
     cv2.circle(frame, center, radius, color, thickness)
     return frame
```

### Comparing `jcopvision-0.2.2/jcopvision/draw/imshow.py` & `jcopvision-0.2.3/jcopvision/draw/imshow.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/draw/text.py` & `jcopvision-0.2.3/jcopvision/draw/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cv2
-from jcopvision.utils import denormalize_image, idx2color, denormalize_landmark
+from jcopvision.utils import denormalize_image, parse_color, denormalize_landmark
 
 __all__ = ["add_text"]
 
 
 def add_text(frame, text, position=(0.05, 0.1), size=1, thickness=2, color=-1, font=cv2.FONT_HERSHEY_DUPLEX, line_type=cv2.LINE_AA):
     '''
     Add text
@@ -23,18 +23,19 @@
 
     size: int
         font scale factor (multiplied to font base size)
 
     thickness: int
         Text thickness in px        
 
-    color: int or (int, int, int)
-        The color of the Text
-        If int, it would be map to default colormap using jcopvision.utils.idx2color. Use -1 for random color.
+    color: int or (int, int, int) or str
+        The color of the bounding box
+        If int, it would be map to default colormap using jcopvision.utils.parse_color. Use -1 for random color.
         If (int, int, int), color in BGR format
+        If str, it will be parsed such in matplotlib colors. Hex code is also accepted
 
     font: cv2.FONT
         opencv font
 
     line_type: cv2.LINE
         opencv line type    
 
@@ -42,15 +43,14 @@
     === Return ===
     frame: array
         annotated image / frame
     '''
     frame = frame.copy()
     frame = denormalize_image(frame)
 
-    if isinstance(color, int):
-        color = idx2color(color)
+    color = parse_color(color)
 
     if not isinstance(position[0], int):
         position = tuple(denormalize_landmark(frame, position).astype(int))
     
     frame = cv2.putText(frame, text, position, font, size, color, thickness, line_type)    
     return frame
```

### Comparing `jcopvision-0.2.2/jcopvision/image_processing/blending.py` & `jcopvision-0.2.3/jcopvision/image_processing/blending.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/image_processing/masking.py` & `jcopvision-0.2.3/jcopvision/image_processing/masking.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/io/jupyter.py` & `jcopvision-0.2.3/jcopvision/io/jupyter.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/io/reader.py` & `jcopvision-0.2.3/jcopvision/io/reader.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/io/utils.py` & `jcopvision-0.2.3/jcopvision/io/utils.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/io/writer.py` & `jcopvision-0.2.3/jcopvision/io/writer.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/utils/bbox.py` & `jcopvision-0.2.3/jcopvision/utils/bbox.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/utils/filter.py` & `jcopvision-0.2.3/jcopvision/utils/filter.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision/utils/landmark.py` & `jcopvision-0.2.3/jcopvision/utils/landmark.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.2/jcopvision.egg-info/PKG-INFO` & `jcopvision-0.2.3/jcopvision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopvision
-Version: 0.2.2
+Version: 0.2.3
 Summary: J.COp Vision consists of helper tools for computer vision
 Home-page: https://github.com/WiraDKP/jcopvision
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: computer vision dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopvision-0.2.2/jcopvision.egg-info/SOURCES.txt` & `jcopvision-0.2.3/jcopvision.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 jcopvision.egg-info/dependency_links.txt
 jcopvision.egg-info/requires.txt
 jcopvision.egg-info/top_level.txt
 jcopvision/draw/__init__.py
 jcopvision/draw/bbox.py
 jcopvision/draw/circle.py
 jcopvision/draw/imshow.py
+jcopvision/draw/line.py
 jcopvision/draw/text.py
 jcopvision/image_processing/__init__.py
 jcopvision/image_processing/blending.py
 jcopvision/image_processing/enhancement.py
 jcopvision/image_processing/masking.py
 jcopvision/io/__init__.py
 jcopvision/io/jupyter.py
```

### Comparing `jcopvision-0.2.2/setup.py` & `jcopvision-0.2.3/setup.py`

 * *Files identical despite different names*

