# Comparing `tmp/satvis-0.1.5.tar.gz` & `tmp/satvis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satvis-0.1.5.tar", last modified: Tue Mar 14 20:03:31 2023, max compression
+gzip compressed data, was "satvis-0.2.0.tar", last modified: Tue Apr 18 19:48:25 2023, max compression
```

## Comparing `satvis-0.1.5.tar` & `satvis-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-03-14 20:03:31.285508 satvis-0.1.5/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1069 2022-11-14 19:16:32.000000 satvis-0.1.5/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-03-14 20:03:31.285508 satvis-0.1.5/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    12667 2022-11-16 20:21:06.000000 satvis-0.1.5/README.md
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1569 2023-03-14 20:00:14.000000 satvis-0.1.5/pyproject.toml
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-03-14 20:03:31.285508 satvis-0.1.5/satvis/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2022-11-15 17:08:14.000000 satvis-0.1.5/satvis/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3791 2022-12-16 19:14:03.000000 satvis-0.1.5/satvis/int_tree_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     9374 2022-12-16 19:13:58.000000 satvis-0.1.5/satvis/schedule_plots.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3967 2022-12-16 19:16:52.000000 satvis-0.1.5/satvis/vis_history.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    10871 2023-03-14 19:49:53.000000 satvis-0.1.5/satvis/visibility_func.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-03-14 20:03:31.285508 satvis-0.1.5/satvis.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-03-14 20:03:31.000000 satvis-0.1.5/satvis.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      449 2023-03-14 20:03:31.000000 satvis-0.1.5/satvis.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-03-14 20:03:31.000000 satvis-0.1.5/satvis.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2022-11-15 16:58:33.000000 satvis-0.1.5/satvis.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      269 2023-03-14 20:03:31.000000 satvis-0.1.5/satvis.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        7 2023-03-14 20:03:31.000000 satvis-0.1.5/satvis.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-03-14 20:03:31.285508 satvis-0.1.5/setup.cfg
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-03-14 20:03:31.285508 satvis-0.1.5/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1480 2022-12-16 19:13:45.000000 satvis-0.1.5/tests/test_int_tree_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3660 2022-12-16 19:22:11.000000 satvis-0.1.5/tests/test_schedule_plots.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1407 2022-12-16 19:13:36.000000 satvis-0.1.5/tests/test_vis_history.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     6898 2022-12-16 19:13:22.000000 satvis-0.1.5/tests/test_visibility_func.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1069 2022-11-14 19:16:32.000000 satvis-0.2.0/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-18 19:48:25.243433 satvis-0.2.0/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    12667 2022-11-16 20:21:06.000000 satvis-0.2.0/README.md
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1569 2023-04-18 19:46:26.000000 satvis-0.2.0/pyproject.toml
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/satvis/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2022-11-15 17:08:14.000000 satvis-0.2.0/satvis/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3791 2022-12-16 19:14:03.000000 satvis-0.2.0/satvis/int_tree_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     9374 2022-12-16 19:13:58.000000 satvis-0.2.0/satvis/schedule_plots.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3967 2022-12-16 19:16:52.000000 satvis-0.2.0/satvis/vis_history.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    11166 2023-04-18 19:45:28.000000 satvis-0.2.0/satvis/visibility_func.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/satvis.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    14358 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      449 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2022-11-15 16:58:33.000000 satvis-0.2.0/satvis.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      269 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        7 2023-04-18 19:48:25.000000 satvis-0.2.0/satvis.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-04-18 19:48:25.243433 satvis-0.2.0/setup.cfg
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-04-18 19:48:25.243433 satvis-0.2.0/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1480 2022-12-16 19:13:45.000000 satvis-0.2.0/tests/test_int_tree_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3660 2022-12-16 19:22:11.000000 satvis-0.2.0/tests/test_schedule_plots.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1407 2022-12-16 19:13:36.000000 satvis-0.2.0/tests/test_vis_history.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     7959 2023-04-18 19:42:38.000000 satvis-0.2.0/tests/test_visibility_func.py
```

### Comparing `satvis-0.1.5/LICENSE` & `satvis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/PKG-INFO` & `satvis-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satvis
-Version: 0.1.5
+Version: 0.2.0
 Summary: Satellite LOS visibility calculator
 Author-email: Dylan Penn <dylanrpenn@vt.edu>
 License: MIT License
         
         Copyright (c) 2022 Dylan R. Penn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `satvis-0.1.5/README.md` & `satvis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/pyproject.toml` & `satvis-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satvis"
-version = "0.1.5"
+version = "0.2.0"
 description = "Satellite LOS visibility calculator"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=2.8.5"
 classifiers = [
     "Programming Language :: Python :: 2",
     "License :: OSI Approved :: MIT License",
```

### Comparing `satvis-0.1.5/satvis/int_tree_converter.py` & `satvis-0.2.0/satvis/int_tree_converter.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/satvis/schedule_plots.py` & `satvis-0.2.0/satvis/schedule_plots.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/satvis/vis_history.py` & `satvis-0.2.0/satvis/vis_history.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/satvis/visibility_func.py` & `satvis-0.2.0/satvis/visibility_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,15 @@
 
 # Standard Library Imports
 from typing import Tuple
 from warnings import warn
 
 # Third Party Imports
 from intervaltree import Interval, IntervalTree
-from numpy import (
-    append,
-    arange,
-    arccos,
-    array,
-    dot,
-    isnan,
-    isreal,
-    nan,
-    ndarray,
-    sign,
-)
+from numpy import append, arange, arccos, array, dot, isreal, nan, ndarray, sign
 from numpy.linalg import norm
 from numpy.polynomial import Polynomial
 
 
 # %% Visibility function
 def visibilityFunc(
     r1: ndarray,
@@ -91,27 +80,19 @@
     phi = arccos(test_var)
 
     # %% If either point is far below  surface of body, abort and report not visible
     # check if points are far below surface of body
     r1_flag = False
     if RE_prime / r1_mag > (1 + eps):
         r1_flag = True
-        # print(
-        #     f"RE_prime/r1_mag={RE_prime/r1_mag}, (RE_prime={RE_prime}, r1_mag={r1_mag})"
-        # )
-        # raise ValueError("RE_prime > r1_mag")
         warn("RE_prime > r1_mag")
 
     r2_flag = False
     if RE_prime / r2_mag > (1 + eps):
         r2_flag = True
-        # print(
-        #     f"RE_prime/r2_mag={RE_prime/r2_mag}, (RE_prime={RE_prime}, r2_mag={r2_mag})"
-        # )
-        # raise ValueError("RE_prime > r2_mag")
         warn("RE_prime > r2_mag")
 
     # If either point is far below surface, v and alphas are undefined.
     # However, for v we don't want to return NaN, so just return a negative value
     # let the user know via the warnings above.
     if r1_flag or r2_flag:
         v = -1
@@ -209,15 +190,18 @@
 
             # print('i =' + str(i))
             # grab 4 time values
             tSnapshot = array([t[i - 3], t[i - 2], t[i - 1], t[i]])
             # grab 4 v values
             vSnapshot = array([v[i - 3], v[i - 2], v[i - 1], v[i]])
 
-            crossings = append(crossings, findCrossing(tSnapshot, vSnapshot, 3))
+            # Get new crossing.
+            new_crossings = findCrossing(tSnapshot, vSnapshot, 3)
+            single_crossing = trimCrossings(new_crossings)
+            crossings = append(crossings, single_crossing)
 
             # determine if zero-crossing was a rise or set time and assign
             # val to vector
             riseSet = append(riseSet, riseOrSet(v[i - 1]))
 
             # Construct interval tree for times when v > 0 (visibility
             # windows)
@@ -241,20 +225,36 @@
             if crossIndx >= 0 and sign(v[i]) == 1:
                 temp = Interval(crossings[crossIndx], t[i], id)
                 tree.add(temp)
 
     return crossings, riseSet, tree
 
 
+def trimCrossings(crossings: ndarray) -> ndarray:
+    """Trim extra (false) crossings from array."""
+
+    # Get new crossing; grab single element from new_crossings in case
+    # multiple crossings are returned. This happens in edge case where
+    # crossings occur between i=0/1 and i=1/2 or i=0/1, 1/2, and 2/3
+    if len(crossings) == 1:
+        # Single crossing detected, return input
+        c = crossings[0]
+    elif len(crossings) in [2, 3]:
+        # 2 or 3 crossings detected, return the 1st entry.
+        c = crossings[1]
+
+    return c
+
+
 def findCrossing(
     t: ndarray,
     v: ndarray,
     order: int,
 ) -> ndarray[float]:
-    """Fits a 3rd order polynomial to 4 points and finds root.
+    """Fits a N-order polynomial to 4 points and finds root.
 
     Args:
         t (`ndarray`): [4,] Time values.
         v (`ndarray`): [4,] Visibility function values.
         order (`int`): Order of polyfit.
 
     Returns:
```

### Comparing `satvis-0.1.5/satvis.egg-info/PKG-INFO` & `satvis-0.2.0/satvis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satvis
-Version: 0.1.5
+Version: 0.2.0
 Summary: Satellite LOS visibility calculator
 Author-email: Dylan Penn <dylanrpenn@vt.edu>
 License: MIT License
         
         Copyright (c) 2022 Dylan R. Penn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `satvis-0.1.5/tests/test_int_tree_converter.py` & `satvis-0.2.0/tests/test_int_tree_converter.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/tests/test_schedule_plots.py` & `satvis-0.2.0/tests/test_schedule_plots.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/tests/test_vis_history.py` & `satvis-0.2.0/tests/test_vis_history.py`

 * *Files identical despite different names*

### Comparing `satvis-0.1.5/tests/test_visibility_func.py` & `satvis-0.2.0/tests/test_visibility_func.py`

 * *Files 10% similar despite different names*

```diff
@@ -156,14 +156,42 @@
 
 [fig, ax] = plt.subplots()
 ax.plot(crossings, zeros(len(crossings)), marker="*", linestyle="None")
 ax.plot(crossings, riseSet, marker="|", linestyle="None")
 ax.plot(t, vis_a)
 ax.set_title("starts stradling 0 (--++++)")
 
+# Double-crossing in a window down-up  (+-+++)
+vis_a = array([1, -0.2, 0.5, 4, 2])
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n double crossing (+-+++)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
+# Double-crossing in a window up-down (-+---)
+vis_a = array([-1, 0.2, -0.5, -4, -2])
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n double crossing (-+---)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
+# Triple-crossing in a window down-up-down  (+-+--)
+vis_a = array([1, -0.2, 0.5, -4, -2])
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n triple crossing (+-+--)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
+# Triple-crossing in a window up-down-up  (-+-++)
+vis_a = array([-1, 0.2, -0.5, 4, 2])
+[crossings, riseSet, visTree] = zeroCrossingFit(vis_a, t, "der")
+print("\n triple crossing (-+-++)")
+print(f"crossings={crossings} \nriseSet={riseSet}")
+print(f"tree={visTree}")
+
 
 # %% Long time vector
 print("\nLong tests \n")
 tLong = linspace(0, 30, num=100)
 # multiple crossings, ends not visible
 vis5 = sin(tLong)
 [crossings, riseSet, visTree] = zeroCrossingFit(vis5, tLong, "der")
```

