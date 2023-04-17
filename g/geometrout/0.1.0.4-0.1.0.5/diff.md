# Comparing `tmp/geometrout-0.1.0.4.tar.gz` & `tmp/geometrout-0.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometrout-0.1.0.4.tar", last modified: Mon Feb 13 20:50:07 2023, max compression
+gzip compressed data, was "geometrout-0.1.0.5.tar", last modified: Mon Apr 17 22:40:15 2023, max compression
```

## Comparing `geometrout-0.1.0.4.tar` & `geometrout-0.1.0.5.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     2327 2023-02-05 17:13:44.000000 geometrout-0.1.0.4/LICENSE
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       85 2021-11-19 05:57:07.000000 geometrout-0.1.0.4/README.md
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/geometrout/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      100 2023-02-04 23:16:47.000000 geometrout-0.1.0.4/geometrout/__init__.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     1853 2021-11-19 06:36:16.000000 geometrout-0.1.0.4/geometrout/pointcloud.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)    20151 2023-02-13 20:44:40.000000 geometrout-0.1.0.4/geometrout/primitive.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)    10397 2023-02-13 20:42:48.000000 geometrout-0.1.0.4/geometrout/transform.py
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/geometrout.egg-info/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-02-13 20:50:07.000000 geometrout-0.1.0.4/geometrout.egg-info/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      331 2023-02-13 20:50:07.000000 geometrout-0.1.0.4/geometrout.egg-info/SOURCES.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)        1 2023-02-13 20:50:07.000000 geometrout-0.1.0.4/geometrout.egg-info/dependency_links.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       20 2023-02-13 20:50:07.000000 geometrout-0.1.0.4/geometrout.egg-info/requires.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       11 2023-02-13 20:50:07.000000 geometrout-0.1.0.4/geometrout.egg-info/top_level.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       90 2021-12-28 21:19:21.000000 geometrout-0.1.0.4/pyproject.toml
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      394 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/setup.cfg
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-02-13 20:50:07.757498 geometrout-0.1.0.4/tests/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     1293 2023-02-04 19:24:42.000000 geometrout-0.1.0.4/tests/test_transform.py
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     2327 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/LICENSE
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/PKG-INFO
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       85 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/README.md
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/geometrout/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      100 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/__init__.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     1853 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/pointcloud.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)    22362 2023-04-14 20:57:49.000000 geometrout-0.1.0.5/geometrout/primitive.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)    10397 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/transform.py
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/geometrout.egg-info/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/PKG-INFO
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      307 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/SOURCES.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)        1 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/dependency_links.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       20 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/requires.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       11 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/top_level.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       90 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/pyproject.toml
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      394 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/setup.cfg
```

### Comparing `geometrout-0.1.0.4/LICENSE` & `geometrout-0.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.4/geometrout/pointcloud.py` & `geometrout-0.1.0.5/geometrout/pointcloud.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.4/geometrout/primitive.py` & `geometrout-0.1.0.5/geometrout/primitive.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,23 +79,59 @@
 def _cuboid_sample_volume(pose_matrix, dims, num_points):
     random_points = np.random.uniform(-1.0, 1.0, (num_points, 3))
     random_points = random_points * dims / 2
     _transform(random_points, pose_matrix)
     return random_points
 
 
+@nb.njit
+def np_apply_along_axis(func1d, axis, arr):
+    assert arr.ndim == 2
+    assert axis in [0, 1]
+    if axis == 0:
+        result = np.empty(arr.shape[1])
+        for i in range(len(result)):
+            result[i] = func1d(arr[:, i])
+    else:
+        result = np.empty(arr.shape[0])
+        for i in range(len(result)):
+            result[i] = func1d(arr[i, :])
+    return result
+
+
+@nb.njit
+def np_mean(array, axis):
+    return np_apply_along_axis(np.mean, axis, array)
+
+
+@nb.njit
+def np_std(array, axis):
+    return np_apply_along_axis(np.std, axis, array)
+
+
 @nb.jit(nopython=True, cache=True)
 def _cuboid_sdf(inverse_pose_matrix, dims, point):
-    homog_point = np.ones(4)
-    homog_point[:3] = point
-    projected_point = (inverse_pose_matrix @ homog_point)[:3]
-    distance = np.abs(projected_point) - (dims / 2)
-    outside = np.linalg.norm(np.maximum(distance, np.zeros(3)))
-    inner_max_distance = np.max(distance)
-    inside = np.minimum(inner_max_distance, 0)
+    assert point.ndim < 3
+    if point.ndim == 1:
+        homog_point = np.ones(4)
+        homog_point[:3] = point
+        projected_point = (inverse_pose_matrix @ homog_point)[:3]
+        distance = np.abs(projected_point) - (dims / 2)
+        outside = np.linalg.norm(np.maximum(distance, np.zeros(3)))
+        inner_max_distance = np.max(distance)
+        inside = np.minimum(inner_max_distance, 0)
+    elif point.ndim == 2:
+        homog_point = np.ones((point.shape[0], 4))
+        homog_point[:, :3] = point
+        projected_point = (inverse_pose_matrix @ homog_point.T)[:3, :].T
+        distance = np.abs(projected_point) - (dims / 2)
+        _outside = np.power(np.maximum(distance, np.zeros((1, 3))), 2)
+        outside = np.sqrt(_outside[:, 0] + _outside[:, 1] + _outside[:, 2])
+        inner_max_distance = np_apply_along_axis(np.max, 1, distance)
+        inside = np.minimum(inner_max_distance, 0)
     return outside + inside
 
 
 @nb.jit(nopython=True, cache=True)
 def _cuboid_corners(pose_matrix, dims):
     x_front, x_back = (
         dims[0] / 2,
@@ -177,15 +213,15 @@
                 f"    dims={self.dims},",
                 f"    quaternion={self.pose.so3.wxyz},",
                 ")",
             ]
         )
 
     @staticmethod
-    def unit(cls):
+    def unit():
         return Cuboid(
             center=np.array([0.0, 0.0, 0.0]),
             dims=np.array([1.0, 1.0, 1.0]),
             quaternion=np.array([1.0, 0.0, 0.0, 0.0]),
         )
 
     @staticmethod
@@ -247,15 +283,15 @@
         return _cuboid_sample_volume(self.pose.matrix, self.dims, num_points)
 
     def sdf(self, point):
         """
         :param point: Point in 3D for which we want the sdf
         :return: The sdf value of that point
         """
-        return _cuboid_sdf(self.pose.inverse.matrix, point)
+        return _cuboid_sdf(self.pose.inverse.matrix, self.dims, point)
 
     @property
     def center(self):
         """
         :return: The center of the object as a list
         """
         return self.pose.pos
@@ -284,15 +320,19 @@
 @nb.jit(nopython=True, cache=True)
 def _sphere_volume(radius):
     return 4 / 3 * np.pi * radius**3
 
 
 @nb.jit(nopython=True, cache=True)
 def _sphere_sdf(center, radius, point):
-    return np.linalg.norm(point - center) - radius
+    assert point.ndim < 3
+    if point.ndim == 1:
+        return np.linalg.norm(point - center) - radius
+    distance2 = np.power(point - center, 2)
+    return np.sqrt(distance2[:, 0] + distance2[:, 1] + distance2[:, 2]) - radius
 
 
 @nb.jit(nopython=True, cache=True)
 def _sphere_sample_surface(center, radius, num_points, noise):
     assert (
         noise >= 0
     ), "Noise parameter should be a radius of the uniform distribution added to the random points"
@@ -407,29 +447,48 @@
 @nb.jit(nopython=True, cache=True)
 def _cylinder_volume(radius, height):
     return height * np.pi * radius**2
 
 
 @nb.jit(nopython=True, cache=True)
 def _cylinder_sdf(inverse_pose_matrix, radius, height, point):
-    homog_point = np.ones(4)
-    homog_point[:3] = np.asarray(point)
-    projected_point = (inverse_pose_matrix @ homog_point)[:3]
-    surface_distance_xy = np.linalg.norm(projected_point[:2])
-    z_distance = projected_point[2]
-
-    # After having the z distance, we can reduce this problem to a
-    # 2D box computation with size height and width 2 * radius
-    half_extent_2d = np.array([radius, height / 2])
-    point_2d = np.array([surface_distance_xy, z_distance])
-    distance_2d = np.abs(point_2d) - half_extent_2d
-
-    outside = np.linalg.norm(np.maximum(distance_2d, np.zeros(2)))
-    inner_max_distance_2d = np.max(distance_2d)
-    inside = np.minimum(inner_max_distance_2d, 0)
+    assert point.ndim < 3
+    if point.ndim == 1:
+        homog_point = np.ones(4)
+        homog_point[:3] = np.asarray(point)
+        projected_point = (inverse_pose_matrix @ homog_point)[:3]
+        surface_distance_xy = np.linalg.norm(projected_point[:2])
+        z_distance = projected_point[2]
+
+        # After having the z distance, we can reduce this problem to a
+        # 2D box computation with size height and width 2 * radius
+        half_extent_2d = np.array([radius, height / 2])
+        point_2d = np.array([surface_distance_xy, z_distance])
+        distance_2d = np.abs(point_2d) - half_extent_2d
+
+        outside = np.linalg.norm(np.maximum(distance_2d, np.zeros(2)))
+        inner_max_distance_2d = np.max(distance_2d)
+        inside = np.minimum(inner_max_distance_2d, 0)
+    else:
+        homog_point = np.ones((point.shape[0], 4))
+        homog_point[:, :3] = point
+        projected_point = (inverse_pose_matrix @ homog_point.T)[:3, :].T
+        xy2 = np.power(projected_point[:, :2], 2)
+        surface_distance_xy = np.sqrt(xy2[:, 0] + xy2[:, 1])
+        z_distance = projected_point[:, 2]
+
+        half_extent_2d = np.array([radius, height / 2])
+        point_2d = np.stack((surface_distance_xy, z_distance), axis=1)
+        distance_2d = np.abs(point_2d) - half_extent_2d
+
+        _outside = np.power(np.maximum(distance_2d, np.zeros(2)), 2)
+        outside = np.sqrt(_outside[:, 0] + _outside[:, 1])
+        inner_max_distance_2d = np_apply_along_axis(np.max, 1, distance_2d)
+        inside = np.minimum(inner_max_distance_2d, 0)
+
     return outside + inside
 
 
 @nb.jit(nopython=True, cache=True)
 def _cylinder_sample_surface(pose_matrix, radius, height, num_points, noise):
     assert (
         noise >= 0
```

### Comparing `geometrout-0.1.0.4/geometrout/transform.py` & `geometrout-0.1.0.5/geometrout/transform.py`

 * *Files identical despite different names*

