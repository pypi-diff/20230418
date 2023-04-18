# Comparing `tmp/kornia_moons-0.2.5.tar.gz` & `tmp/kornia_moons-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kornia_moons-0.2.5.tar", last modified: Mon Apr 17 12:10:11 2023, max compression
+gzip compressed data, was "kornia_moons-0.2.6.tar", last modified: Tue Apr 18 14:36:46 2023, max compression
```

## Comparing `kornia_moons-0.2.5.tar` & `kornia_moons-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.869689 kornia_moons-0.2.5/
--rw-r--r--   0 oldufo     (501) staff       (20)     2348 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 oldufo     (501) staff       (20)    11357 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/LICENSE
--rw-r--r--   0 oldufo     (501) staff       (20)      111 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/MANIFEST.in
--rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-17 12:10:11.869561 kornia_moons-0.2.5/PKG-INFO
--rw-r--r--   0 oldufo     (501) staff       (20)     1296 2023-04-17 11:47:08.000000 kornia_moons-0.2.5/README.md
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.868114 kornia_moons-0.2.5/kornia_moons/
--rw-r--r--   0 oldufo     (501) staff       (20)       22 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/__init__.py
--rw-r--r--   0 oldufo     (501) staff       (20)     6858 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/_modidx.py
--rw-r--r--   0 oldufo     (501) staff       (20)     1358 2023-04-17 09:31:18.000000 kornia_moons-0.2.5/kornia_moons/_nbdev.py
--rw-r--r--   0 oldufo     (501) staff       (20)     8614 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/feature.py
--rw-r--r--   0 oldufo     (501) staff       (20)    18988 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/viz.py
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.869395 kornia_moons-0.2.5/kornia_moons.egg-info/
--rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/PKG-INFO
--rw-r--r--   0 oldufo     (501) staff       (20)      436 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/SOURCES.txt
--rw-r--r--   0 oldufo     (501) staff       (20)        1 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/dependency_links.txt
--rw-r--r--   0 oldufo     (501) staff       (20)       46 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/entry_points.txt
--rw-r--r--   0 oldufo     (501) staff       (20)        1 2021-06-15 15:53:30.000000 kornia_moons-0.2.5/kornia_moons.egg-info/not-zip-safe
--rw-r--r--   0 oldufo     (501) staff       (20)       45 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/requires.txt
--rw-r--r--   0 oldufo     (501) staff       (20)       13 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/top_level.txt
--rw-r--r--   0 oldufo     (501) staff       (20)     2433 2023-04-17 12:06:09.000000 kornia_moons-0.2.5/settings.ini
--rw-r--r--   0 oldufo     (501) staff       (20)       38 2023-04-17 12:10:11.869726 kornia_moons-0.2.5/setup.cfg
--rw-r--r--   0 oldufo     (501) staff       (20)     2596 2023-04-17 09:31:18.000000 kornia_moons-0.2.5/setup.py
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-18 14:36:46.852065 kornia_moons-0.2.6/
+-rw-r--r--   0 oldufo     (501) staff       (20)     2348 2023-04-17 09:31:17.000000 kornia_moons-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 oldufo     (501) staff       (20)    11357 2023-04-17 09:31:17.000000 kornia_moons-0.2.6/LICENSE
+-rw-r--r--   0 oldufo     (501) staff       (20)      111 2023-04-17 09:31:17.000000 kornia_moons-0.2.6/MANIFEST.in
+-rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-18 14:36:46.851924 kornia_moons-0.2.6/PKG-INFO
+-rw-r--r--   0 oldufo     (501) staff       (20)     1296 2023-04-17 11:47:08.000000 kornia_moons-0.2.6/README.md
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-18 14:36:46.850676 kornia_moons-0.2.6/kornia_moons/
+-rw-r--r--   0 oldufo     (501) staff       (20)       22 2023-04-18 14:36:09.000000 kornia_moons-0.2.6/kornia_moons/__init__.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     7985 2023-04-18 14:36:09.000000 kornia_moons-0.2.6/kornia_moons/_modidx.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     1358 2023-04-17 09:31:18.000000 kornia_moons-0.2.6/kornia_moons/_nbdev.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     8614 2023-04-18 14:36:09.000000 kornia_moons-0.2.6/kornia_moons/feature.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     1301 2023-04-18 14:26:03.000000 kornia_moons-0.2.6/kornia_moons/line.py
+-rw-r--r--   0 oldufo     (501) staff       (20)    19274 2023-04-18 14:36:09.000000 kornia_moons-0.2.6/kornia_moons/viz.py
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-18 14:36:46.851741 kornia_moons-0.2.6/kornia_moons.egg-info/
+-rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/PKG-INFO
+-rw-r--r--   0 oldufo     (501) staff       (20)      457 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/SOURCES.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)        1 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/dependency_links.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)       46 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/entry_points.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)        1 2021-06-15 15:53:30.000000 kornia_moons-0.2.6/kornia_moons.egg-info/not-zip-safe
+-rw-r--r--   0 oldufo     (501) staff       (20)       45 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/requires.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)       13 2023-04-18 14:36:46.000000 kornia_moons-0.2.6/kornia_moons.egg-info/top_level.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)     2433 2023-04-18 14:36:06.000000 kornia_moons-0.2.6/settings.ini
+-rw-r--r--   0 oldufo     (501) staff       (20)       38 2023-04-18 14:36:46.852106 kornia_moons-0.2.6/setup.cfg
+-rw-r--r--   0 oldufo     (501) staff       (20)     2596 2023-04-17 09:31:18.000000 kornia_moons-0.2.6/setup.py
```

### Comparing `kornia_moons-0.2.5/CONTRIBUTING.md` & `kornia_moons-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.5/LICENSE` & `kornia_moons-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.5/PKG-INFO` & `kornia_moons-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kornia_moons
-Version: 0.2.5
+Version: 0.2.6
 Summary: Conversions between kornia and other computer vision libraries formats
 Home-page: https://github.com/ducha-aiki/kornia_moons/tree/master/
 Author: Dmytro Mishkin
 Author-email: ducha.aiki@gmail.com
 License: Apache Software License 2.0
 Keywords: kornia,python,pytorch,deep learning,computer vision
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kornia_moons-0.2.5/README.md` & `kornia_moons-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.5/kornia_moons/_modidx.py` & `kornia_moons-0.2.6/kornia_moons/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,23 @@
                                       'kornia_moons.feature.opencv_SIFT_kpts_from_laf': ( 'feature.html#opencv_sift_kpts_from_laf',
                                                                                           'kornia_moons/feature.py'),
                                       'kornia_moons.feature.opencv_kpts_from_laf': ( 'feature.html#opencv_kpts_from_laf',
                                                                                      'kornia_moons/feature.py'),
                                       'kornia_moons.feature.to_np': ('feature.html#to_np', 'kornia_moons/feature.py'),
                                       'kornia_moons.feature.to_numpy_image': ('feature.html#to_numpy_image', 'kornia_moons/feature.py'),
                                       'kornia_moons.feature.to_torch': ('feature.html#to_torch', 'kornia_moons/feature.py')},
+            'kornia_moons.line': { 'kornia_moons.line.LineFeature': ('line.html#linefeature', 'kornia_moons/line.py'),
+                                   'kornia_moons.line.LineFeature.__init__': ('line.html#linefeature.__init__', 'kornia_moons/line.py'),
+                                   'kornia_moons.line.LineFeature.detect_line_segments': ( 'line.html#linefeature.detect_line_segments',
+                                                                                           'kornia_moons/line.py'),
+                                   'kornia_moons.line.LineFeature.forward': ('line.html#linefeature.forward', 'kornia_moons/line.py'),
+                                   'kornia_moons.line.LineFeature.get_image_descriptors': ( 'line.html#linefeature.get_image_descriptors',
+                                                                                            'kornia_moons/line.py'),
+                                   'kornia_moons.line.LineFeature.match_lines': ( 'line.html#linefeature.match_lines',
+                                                                                  'kornia_moons/line.py')},
             'kornia_moons.viz': { 'kornia_moons.viz.draw_LAF_inliers_perspective_repjojected': ( 'viz.html#draw_laf_inliers_perspective_repjojected',
                                                                                                  'kornia_moons/viz.py'),
                                   'kornia_moons.viz.draw_LAF_matches': ('viz.html#draw_laf_matches', 'kornia_moons/viz.py'),
                                   'kornia_moons.viz.draw_LAF_matches_from_result_dict': ( 'viz.html#draw_laf_matches_from_result_dict',
                                                                                           'kornia_moons/viz.py'),
                                   'kornia_moons.viz.draw_epipolar_errors_in_single_image': ( 'viz.html#draw_epipolar_errors_in_single_image',
                                                                                              'kornia_moons/viz.py'),
```

### Comparing `kornia_moons-0.2.5/kornia_moons/_nbdev.py` & `kornia_moons-0.2.6/kornia_moons/_nbdev.py`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.5/kornia_moons/feature.py` & `kornia_moons-0.2.6/kornia_moons/feature.py`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.5/kornia_moons/viz.py` & `kornia_moons-0.2.6/kornia_moons/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 import matplotlib.pyplot as plt
 import torch.nn as nn
 from torch import allclose
 from typing import Union
 
 
-
 # %% ../viz.ipynb 6
 def visualize_LAF(img, LAF, img_idx = 0, color='r', linewidth=1,
                   draw_ori = True, fig=None,
                   ax = None, return_fig_ax = False, **kwargs):
     from kornia_moons.feature import to_numpy_image
     x, y = kornia.feature.laf.get_laf_pts_to_draw(kornia.feature.laf.scale_laf(LAF, 0.5), img_idx)
     if not draw_ori:
@@ -90,14 +89,15 @@
                                "feature_color": (0.2, 0.5, 1),
                                   "vertical": False}, 
                         Fm: Optional[np.array] = None, H: Optional[np.array] = None,
                         fig = None, ax: Optional = None,
                         return_fig_ax=False):
     '''This function draws LAFs, tentative matches, inliers epipolar lines (if F is provided),
     and image1 corners reprojection into image 2 (if H is provided)'''
+    from kornia_moons.feature import to_numpy_image, cv2_matches_from_kornia, to_np, to_torch
     if inlier_mask is not None:
         inlier_mask = np.array(inlier_mask).reshape(-1)
     img1 = to_numpy_image(img1)
     img2 = to_numpy_image(img2)
     
     h,w = img1.shape[:2]
     h2,w2 = img2.shape[:2]
@@ -253,14 +253,15 @@
                         H: np.array = None,
                         fig = None, ax: Optional = None,
                         return_fig_ax=False):
     '''This function draws tentative matches and inliers given the homography H'''
     import kornia as K
     import kornia.feature as KF
     import kornia.geometry as KG
+    from kornia_moons.feature import to_numpy_image, cv2_matches_from_kornia, to_np, to_torch
     inlier_mask = np.array(inlier_mask).reshape(-1)
     img1 = to_numpy_image(img1)
     img2 = to_numpy_image(img2)
     
     h,w = img1.shape[:2]
     h2,w2 = img2.shape[:2]
     
@@ -367,14 +368,16 @@
                                                      "figsize": (10,10),
                                                      "markersize": 8},
                                          img_index: int = 2,
                                          ax: Optional = None,
                                          title = None):
     '''This function draws epipolar errors in single image'''
     from kornia.geometry.epipolar import get_closest_point_on_epipolar_line
+    from kornia_moons.feature import to_numpy_image, cv2_matches_from_kornia, to_np, to_torch
+    
     img = to_numpy_image(img)
     pts1 = to_torch(kp1)[None]
     pts2 = to_torch(kp2)[None]
     Fm = to_torch(Fm1to2)
     if len(Fm.shape) == 2:
         Fm = Fm[None]
     assert img_index in [1,2]
```

### Comparing `kornia_moons-0.2.5/kornia_moons.egg-info/PKG-INFO` & `kornia_moons-0.2.6/kornia_moons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kornia-moons
-Version: 0.2.5
+Version: 0.2.6
 Summary: Conversions between kornia and other computer vision libraries formats
 Home-page: https://github.com/ducha-aiki/kornia_moons/tree/master/
 Author: Dmytro Mishkin
 Author-email: ducha.aiki@gmail.com
 License: Apache Software License 2.0
 Keywords: kornia,python,pytorch,deep learning,computer vision
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kornia_moons-0.2.5/settings.ini` & `kornia_moons-0.2.6/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = ducha-aiki
 description = Conversions between kornia and other computer vision libraries formats
 keywords = kornia, python, pytorch, deep learning, computer vision
 author = Dmytro Mishkin
 author_email = ducha.aiki@gmail.com
 copyright = Dmytro Mishkin
 branch = master
-version = 0.2.5
+version = 0.2.6
 min_python = 3.7
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `kornia_moons-0.2.5/setup.py` & `kornia_moons-0.2.6/setup.py`

 * *Files identical despite different names*

