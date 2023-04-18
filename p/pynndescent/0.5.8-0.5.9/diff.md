# Comparing `tmp/pynndescent-0.5.8.tar.gz` & `tmp/pynndescent-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynndescent-0.5.8.tar", last modified: Mon Oct 31 17:18:49 2022, max compression
+gzip compressed data, was "dist/pynndescent-0.5.9.tar", last modified: Tue Apr 18 01:00:38 2023, max compression
```

## Comparing `pynndescent-0.5.8.tar` & `pynndescent-0.5.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2022-10-31 17:18:49.269524 pynndescent-0.5.8/
--rw-r--r--   0 leland     (501) staff       (20)     3220 2021-03-26 04:21:30.000000 pynndescent-0.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 leland     (501) staff       (20)     2607 2021-03-26 04:21:30.000000 pynndescent-0.5.8/CONTRIBUTING.md
--rw-r--r--   0 leland     (501) staff       (20)     1319 2021-03-26 04:21:30.000000 pynndescent-0.5.8/LICENSE
--rw-r--r--   0 leland     (501) staff       (20)      130 2021-10-15 13:22:03.000000 pynndescent-0.5.8/MANIFEST.in
--rw-r--r--   0 leland     (501) staff       (20)     8639 2022-10-31 17:18:49.268779 pynndescent-0.5.8/PKG-INFO
--rw-r--r--   0 leland     (501) staff       (20)     5991 2021-10-15 14:18:17.000000 pynndescent-0.5.8/README.rst
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2022-10-31 17:18:49.251460 pynndescent-0.5.8/pynndescent/
--rw-r--r--   0 leland     (501) staff       (20)      615 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/__init__.py
--rw-r--r--   0 leland     (501) staff       (20)    24689 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/distances.py
--rw-r--r--   0 leland     (501) staff       (20)     7640 2022-03-22 13:31:45.000000 pynndescent-0.5.8/pynndescent/graph_utils.py
--rw-r--r--   0 leland     (501) staff       (20)    33571 2022-03-22 13:31:45.000000 pynndescent-0.5.8/pynndescent/optimal_transport.py
--rwxr-xr-x   0 leland     (501) staff       (20)    80594 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/pynndescent_.py
--rw-r--r--   0 leland     (501) staff       (20)    37762 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/rp_trees.py
--rw-r--r--   0 leland     (501) staff       (20)    32265 2022-05-20 16:37:16.000000 pynndescent-0.5.8/pynndescent/sparse.py
--rw-r--r--   0 leland     (501) staff       (20)    10206 2022-03-22 13:31:45.000000 pynndescent-0.5.8/pynndescent/sparse_nndescent.py
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2022-10-31 17:18:49.260563 pynndescent-0.5.8/pynndescent/tests/
--rw-r--r--   0 leland     (501) staff       (20)        0 2021-03-26 04:21:30.000000 pynndescent-0.5.8/pynndescent/tests/__init__.py
--rw-r--r--   0 leland     (501) staff       (20)     2837 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/tests/conftest.py
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2022-10-31 17:18:49.261247 pynndescent-0.5.8/pynndescent/tests/test_data/
--rw-r--r--   0 leland     (501) staff       (20)  1760128 2021-03-26 04:21:30.000000 pynndescent-0.5.8/pynndescent/tests/test_data/cosine_hang.npy
--rw-r--r--   0 leland     (501) staff       (20)    12766 2022-10-31 17:15:26.000000 pynndescent-0.5.8/pynndescent/tests/test_distances.py
--rw-r--r--   0 leland     (501) staff       (20)    22206 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/tests/test_pynndescent_.py
--rw-r--r--   0 leland     (501) staff       (20)     6951 2022-05-20 16:37:16.000000 pynndescent-0.5.8/pynndescent/tests/test_rank.py
--rw-r--r--   0 leland     (501) staff       (20)     2973 2021-03-26 04:21:30.000000 pynndescent-0.5.8/pynndescent/threaded_rp_trees.py
--rw-r--r--   0 leland     (501) staff       (20)    19788 2022-08-17 17:51:46.000000 pynndescent-0.5.8/pynndescent/utils.py
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2022-10-31 17:18:49.256981 pynndescent-0.5.8/pynndescent.egg-info/
--rw-r--r--   0 leland     (501) staff       (20)     8639 2022-10-31 17:18:48.000000 pynndescent-0.5.8/pynndescent.egg-info/PKG-INFO
--rw-r--r--   0 leland     (501) staff       (20)      778 2022-10-31 17:18:48.000000 pynndescent-0.5.8/pynndescent.egg-info/SOURCES.txt
--rw-r--r--   0 leland     (501) staff       (20)        1 2022-10-31 17:18:48.000000 pynndescent-0.5.8/pynndescent.egg-info/dependency_links.txt
--rw-r--r--   0 leland     (501) staff       (20)        1 2021-07-05 19:58:21.000000 pynndescent-0.5.8/pynndescent.egg-info/not-zip-safe
--rw-r--r--   0 leland     (501) staff       (20)      125 2022-10-31 17:18:48.000000 pynndescent-0.5.8/pynndescent.egg-info/requires.txt
--rw-r--r--   0 leland     (501) staff       (20)       12 2022-10-31 17:18:48.000000 pynndescent-0.5.8/pynndescent.egg-info/top_level.txt
--rw-r--r--   0 leland     (501) staff       (20)       78 2021-06-01 00:13:29.000000 pynndescent-0.5.8/requirements.txt
--rw-r--r--   0 leland     (501) staff       (20)       38 2022-10-31 17:18:49.269772 pynndescent-0.5.8/setup.cfg
--rw-r--r--   0 leland     (501) staff       (20)     1681 2022-10-31 17:16:31.000000 pynndescent-0.5.8/setup.py
+drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-04-18 01:00:38.490261 pynndescent-0.5.9/
+-rw-r--r--   0 leland     (501) staff       (20)     3220 2021-03-26 04:21:30.000000 pynndescent-0.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 leland     (501) staff       (20)     2607 2021-03-26 04:21:30.000000 pynndescent-0.5.9/CONTRIBUTING.md
+-rw-r--r--   0 leland     (501) staff       (20)     1319 2021-03-26 04:21:30.000000 pynndescent-0.5.9/LICENSE
+-rw-r--r--   0 leland     (501) staff       (20)      130 2021-10-15 13:22:03.000000 pynndescent-0.5.9/MANIFEST.in
+-rw-r--r--   0 leland     (501) staff       (20)     8601 2023-04-18 01:00:38.489979 pynndescent-0.5.9/PKG-INFO
+-rw-r--r--   0 leland     (501) staff       (20)     5991 2021-10-15 14:18:17.000000 pynndescent-0.5.9/README.rst
+drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-04-18 01:00:38.471215 pynndescent-0.5.9/pynndescent/
+-rw-r--r--   0 leland     (501) staff       (20)      615 2022-08-17 17:51:46.000000 pynndescent-0.5.9/pynndescent/__init__.py
+-rw-r--r--   0 leland     (501) staff       (20)    24602 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/distances.py
+-rw-r--r--   0 leland     (501) staff       (20)     7640 2022-03-22 13:31:45.000000 pynndescent-0.5.9/pynndescent/graph_utils.py
+-rw-r--r--   0 leland     (501) staff       (20)    33571 2022-03-22 13:31:45.000000 pynndescent-0.5.9/pynndescent/optimal_transport.py
+-rwxr-xr-x   0 leland     (501) staff       (20)    80628 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/pynndescent_.py
+-rw-r--r--   0 leland     (501) staff       (20)    39755 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/rp_trees.py
+-rw-r--r--   0 leland     (501) staff       (20)    32265 2022-05-20 16:37:16.000000 pynndescent-0.5.9/pynndescent/sparse.py
+-rw-r--r--   0 leland     (501) staff       (20)    10206 2022-03-22 13:31:45.000000 pynndescent-0.5.9/pynndescent/sparse_nndescent.py
+drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-04-18 01:00:38.477608 pynndescent-0.5.9/pynndescent/tests/
+-rw-r--r--   0 leland     (501) staff       (20)        0 2021-03-26 04:21:30.000000 pynndescent-0.5.9/pynndescent/tests/__init__.py
+-rw-r--r--   0 leland     (501) staff       (20)     3057 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/tests/conftest.py
+drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-04-18 01:00:38.489417 pynndescent-0.5.9/pynndescent/tests/test_data/
+-rw-r--r--   0 leland     (501) staff       (20)  1760128 2021-03-26 04:21:30.000000 pynndescent-0.5.9/pynndescent/tests/test_data/cosine_hang.npy
+-rw-r--r--   0 leland     (501) staff       (20)      384 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/tests/test_data/cosine_near_duplicates.npy
+-rw-r--r--   0 leland     (501) staff       (20)    12794 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/tests/test_distances.py
+-rw-r--r--   0 leland     (501) staff       (20)    22737 2023-04-18 00:59:36.000000 pynndescent-0.5.9/pynndescent/tests/test_pynndescent_.py
+-rw-r--r--   0 leland     (501) staff       (20)     6951 2022-05-20 16:37:16.000000 pynndescent-0.5.9/pynndescent/tests/test_rank.py
+-rw-r--r--   0 leland     (501) staff       (20)     2973 2021-03-26 04:21:30.000000 pynndescent-0.5.9/pynndescent/threaded_rp_trees.py
+-rw-r--r--   0 leland     (501) staff       (20)    19788 2022-08-17 17:51:46.000000 pynndescent-0.5.9/pynndescent/utils.py
+drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-04-18 01:00:38.475147 pynndescent-0.5.9/pynndescent.egg-info/
+-rw-r--r--   0 leland     (501) staff       (20)     8601 2023-04-18 01:00:38.000000 pynndescent-0.5.9/pynndescent.egg-info/PKG-INFO
+-rw-r--r--   0 leland     (501) staff       (20)      833 2023-04-18 01:00:38.000000 pynndescent-0.5.9/pynndescent.egg-info/SOURCES.txt
+-rw-r--r--   0 leland     (501) staff       (20)        1 2023-04-18 01:00:38.000000 pynndescent-0.5.9/pynndescent.egg-info/dependency_links.txt
+-rw-r--r--   0 leland     (501) staff       (20)        1 2021-07-05 19:58:21.000000 pynndescent-0.5.9/pynndescent.egg-info/not-zip-safe
+-rw-r--r--   0 leland     (501) staff       (20)      125 2023-04-18 01:00:38.000000 pynndescent-0.5.9/pynndescent.egg-info/requires.txt
+-rw-r--r--   0 leland     (501) staff       (20)       12 2023-04-18 01:00:38.000000 pynndescent-0.5.9/pynndescent.egg-info/top_level.txt
+-rw-r--r--   0 leland     (501) staff       (20)       78 2021-06-01 00:13:29.000000 pynndescent-0.5.9/requirements.txt
+-rw-r--r--   0 leland     (501) staff       (20)       38 2023-04-18 01:00:38.490377 pynndescent-0.5.9/setup.cfg
+-rw-r--r--   0 leland     (501) staff       (20)     1644 2023-04-18 00:59:36.000000 pynndescent-0.5.9/setup.py
```

### Comparing `pynndescent-0.5.8/CODE_OF_CONDUCT.md` & `pynndescent-0.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/CONTRIBUTING.md` & `pynndescent-0.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/LICENSE` & `pynndescent-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/PKG-INFO` & `pynndescent-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pynndescent
-Version: 0.5.8
+Version: 0.5.9
 Summary: Nearest Neighbor Descent
 Home-page: http://github.com/lmcinnes/pynndescent
 Author: Leland McInnes
 Author-email: leland.mcinnes@gmail.com
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: BSD
@@ -216,15 +216,14 @@
         
 Keywords: nearest neighbor,knn,ANN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
-Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `pynndescent-0.5.8/README.rst` & `pynndescent-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/__init__.py` & `pynndescent-0.5.9/pynndescent/__init__.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/distances.py` & `pynndescent-0.5.9/pynndescent/distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,23 +691,18 @@
 
     # average method
     return 0.5 * (count[dense] + count[dense - 1] + 1)
 
 
 @numba.njit(fastmath=True)
 def spearmanr(x, y):
-    a = np.column_stack((x, y))
+    x_rank = rankdata(x)
+    y_rank = rankdata(y)
 
-    n_vars = a.shape[1]
-
-    for i in range(n_vars):
-        a[:, i] = rankdata(a[:, i])
-    rs = np.corrcoef(a, rowvar=0)
-
-    return rs[1, 0]
+    return correlation(x_rank, y_rank)
 
 
 @numba.njit(nogil=True)
 def kantorovich(x, y, cost=_dummy_cost, max_iter=100000):
 
     row_mask = x != 0
     col_mask = y != 0
```

### Comparing `pynndescent-0.5.8/pynndescent/graph_utils.py` & `pynndescent-0.5.9/pynndescent/graph_utils.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/optimal_transport.py` & `pynndescent-0.5.9/pynndescent/optimal_transport.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/pynndescent_.py` & `pynndescent-0.5.9/pynndescent/pynndescent_.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,14 +772,15 @@
         ):
             self._angular_trees = True
         else:
             self._angular_trees = False
 
         if metric == "dot":
             data = normalize(data, norm="l2", copy=copy_on_normalize)
+            self._raw_data = data
 
         self.rng_state = current_random_state.randint(INT32_MIN, INT32_MAX, 3).astype(
             np.int64
         )
         self.search_rng_state = current_random_state.randint(
             INT32_MIN, INT32_MAX, 3
         ).astype(np.int64)
```

### Comparing `pynndescent-0.5.8/pynndescent/rp_trees.py` & `pynndescent-0.5.9/pynndescent/rp_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,26 @@
         elif margin > 0:
             side[i] = 0
             n_left += 1
         else:
             side[i] = 1
             n_right += 1
 
+    # If all points end up on one side, something went wrong numerically
+    # In this case, assign points randomly; they are likely very close anyway
+    if n_left == 0 or n_right == 0:
+        n_left = 0
+        n_right = 0
+        for i in range(indices.shape[0]):
+            side[i] = tau_rand_int(rng_state) % 2
+            if side[i] == 0:
+                n_left += 1
+            else:
+                n_right += 1
+
     # Now that we have the counts allocate arrays
     indices_left = np.empty(n_left, dtype=np.int32)
     indices_right = np.empty(n_right, dtype=np.int32)
 
     # Populate the arrays with graph_indices according to which side they fell on
     n_left = 0
     n_right = 0
@@ -244,14 +256,26 @@
         elif margin > 0:
             side[i] = 0
             n_left += 1
         else:
             side[i] = 1
             n_right += 1
 
+    # If all points end up on one side, something went wrong numerically
+    # In this case, assign points randomly; they are likely very close anyway
+    if n_left == 0 or n_right == 0:
+        n_left = 0
+        n_right = 0
+        for i in range(indices.shape[0]):
+            side[i] = tau_rand_int(rng_state) % 2
+            if side[i] == 0:
+                n_left += 1
+            else:
+                n_right += 1
+
     # Now that we have the counts allocate arrays
     indices_left = np.empty(n_left, dtype=np.int32)
     indices_right = np.empty(n_right, dtype=np.int32)
 
     # Populate the arrays with graph_indices according to which side they fell on
     n_left = 0
     n_right = 0
@@ -368,14 +392,26 @@
         elif margin > 0:
             side[i] = 0
             n_left += 1
         else:
             side[i] = 1
             n_right += 1
 
+    # If all points end up on one side, something went wrong numerically
+    # In this case, assign points randomly; they are likely very close anyway
+    if n_left == 0 or n_right == 0:
+        n_left = 0
+        n_right = 0
+        for i in range(indices.shape[0]):
+            side[i] = tau_rand_int(rng_state) % 2
+            if side[i] == 0:
+                n_left += 1
+            else:
+                n_right += 1
+
     # Now that we have the counts allocate arrays
     indices_left = np.empty(n_left, dtype=np.int32)
     indices_right = np.empty(n_right, dtype=np.int32)
 
     # Populate the arrays with graph_indices according to which side they fell on
     n_left = 0
     n_right = 0
@@ -475,14 +511,26 @@
         elif margin > 0:
             side[i] = 0
             n_left += 1
         else:
             side[i] = 1
             n_right += 1
 
+    # If all points end up on one side, something went wrong numerically
+    # In this case, assign points randomly; they are likely very close anyway
+    if n_left == 0 or n_right == 0:
+        n_left = 0
+        n_right = 0
+        for i in range(indices.shape[0]):
+            side[i] = abs(tau_rand_int(rng_state)) % 2
+            if side[i] == 0:
+                n_left += 1
+            else:
+                n_right += 1
+
     # Now that we have the counts allocate arrays
     indices_left = np.empty(n_left, dtype=np.int32)
     indices_right = np.empty(n_right, dtype=np.int32)
 
     # Populate the arrays with graph_indices according to which side they fell on
     n_left = 0
     n_right = 0
@@ -497,28 +545,28 @@
     hyperplane = np.vstack((hyperplane_inds, hyperplane_data))
 
     return indices_left, indices_right, hyperplane, hyperplane_offset
 
 
 @numba.njit(
     nogil=True,
-    cache=True,
     locals={"left_node_num": numba.types.int32, "right_node_num": numba.types.int32},
 )
 def make_euclidean_tree(
     data,
     indices,
     hyperplanes,
     offsets,
     children,
     point_indices,
     rng_state,
     leaf_size=30,
+    max_depth=100,
 ):
-    if indices.shape[0] > leaf_size:
+    if indices.shape[0] > leaf_size and max_depth > 0:
         (
             left_indices,
             right_indices,
             hyperplane,
             offset,
         ) = euclidean_random_projection_split(data, indices, rng_state)
 
@@ -527,27 +575,29 @@
             left_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         left_node_num = len(point_indices) - 1
 
         make_euclidean_tree(
             data,
             right_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         right_node_num = len(point_indices) - 1
 
         hyperplanes.append(hyperplane)
         offsets.append(offset)
         children.append((np.int32(left_node_num), np.int32(right_node_num)))
@@ -559,15 +609,14 @@
         point_indices.append(indices)
 
     return
 
 
 @numba.njit(
     nogil=True,
-    cache=True,
     locals={
         "children": numba.types.ListType(children_type),
         "left_node_num": numba.types.int32,
         "right_node_num": numba.types.int32,
     },
 )
 def make_angular_tree(
@@ -575,16 +624,17 @@
     indices,
     hyperplanes,
     offsets,
     children,
     point_indices,
     rng_state,
     leaf_size=30,
+    max_depth=100,
 ):
-    if indices.shape[0] > leaf_size:
+    if indices.shape[0] > leaf_size and max_depth > 0:
         (
             left_indices,
             right_indices,
             hyperplane,
             offset,
         ) = angular_random_projection_split(data, indices, rng_state)
 
@@ -593,27 +643,29 @@
             left_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         left_node_num = len(point_indices) - 1
 
         make_angular_tree(
             data,
             right_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         right_node_num = len(point_indices) - 1
 
         hyperplanes.append(hyperplane)
         offsets.append(offset)
         children.append((np.int32(left_node_num), np.int32(right_node_num)))
@@ -625,30 +677,30 @@
         point_indices.append(indices)
 
     return
 
 
 @numba.njit(
     nogil=True,
-    cache=True,
     locals={"left_node_num": numba.types.int32, "right_node_num": numba.types.int32},
 )
 def make_sparse_euclidean_tree(
     inds,
     indptr,
     data,
     indices,
     hyperplanes,
     offsets,
     children,
     point_indices,
     rng_state,
     leaf_size=30,
+    max_depth=100,
 ):
-    if indices.shape[0] > leaf_size:
+    if indices.shape[0] > leaf_size and max_depth > 0:
         (
             left_indices,
             right_indices,
             hyperplane,
             offset,
         ) = sparse_euclidean_random_projection_split(
             inds, indptr, data, indices, rng_state
@@ -661,14 +713,15 @@
             left_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         left_node_num = len(point_indices) - 1
 
         make_sparse_euclidean_tree(
             inds,
             indptr,
@@ -676,14 +729,15 @@
             right_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         right_node_num = len(point_indices) - 1
 
         hyperplanes.append(hyperplane)
         offsets.append(offset)
         children.append((np.int32(left_node_num), np.int32(right_node_num)))
@@ -695,30 +749,30 @@
         point_indices.append(indices)
 
     return
 
 
 @numba.njit(
     nogil=True,
-    cache=True,
     locals={"left_node_num": numba.types.int32, "right_node_num": numba.types.int32},
 )
 def make_sparse_angular_tree(
     inds,
     indptr,
     data,
     indices,
     hyperplanes,
     offsets,
     children,
     point_indices,
     rng_state,
     leaf_size=30,
+    max_depth=100,
 ):
-    if indices.shape[0] > leaf_size:
+    if indices.shape[0] > leaf_size and max_depth > 0:
         (
             left_indices,
             right_indices,
             hyperplane,
             offset,
         ) = sparse_angular_random_projection_split(
             inds, indptr, data, indices, rng_state
@@ -731,14 +785,15 @@
             left_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         left_node_num = len(point_indices) - 1
 
         make_sparse_angular_tree(
             inds,
             indptr,
@@ -746,14 +801,15 @@
             right_indices,
             hyperplanes,
             offsets,
             children,
             point_indices,
             rng_state,
             leaf_size,
+            max_depth - 1,
         )
 
         right_node_num = len(point_indices) - 1
 
         hyperplanes.append(hyperplane)
         offsets.append(offset)
         children.append((np.int32(left_node_num), np.int32(right_node_num)))
@@ -1043,15 +1099,14 @@
         return np.array([[-1]])
 
 
 @numba.njit()
 def recursive_convert(
     tree, hyperplanes, offsets, children, indices, node_num, leaf_start, tree_node
 ):
-
     if tree.children[tree_node][0] < 0:
         leaf_end = leaf_start + len(tree.indices[tree_node])
         children[node_num, 0] = -leaf_start
         children[node_num, 1] = -leaf_end
         indices[leaf_start:leaf_end] = tree.indices[tree_node]
         return node_num, leaf_end
     else:
@@ -1083,15 +1138,14 @@
         return node_num, leaf_start
 
 
 @numba.njit()
 def recursive_convert_sparse(
     tree, hyperplanes, offsets, children, indices, node_num, leaf_start, tree_node
 ):
-
     if tree.children[tree_node][0] < 0:
         leaf_end = leaf_start + len(tree.indices[tree_node])
         children[node_num, 0] = -leaf_start
         children[node_num, 1] = -leaf_end
         indices[leaf_start:leaf_end] = tree.indices[tree_node]
         return node_num, leaf_end
     else:
@@ -1172,28 +1226,26 @@
 FLAT_TREE_OFFSETS = 1
 FLAT_TREE_CHILDREN = 2
 FLAT_TREE_INDICES = 3
 FLAT_TREE_LEAF_SIZE = 4
 
 
 def denumbaify_tree(tree):
-
     result = (
         tree.hyperplanes,
         tree.offsets,
         tree.children,
         tree.indices,
         tree.leaf_size,
     )
 
     return result
 
 
 def renumbaify_tree(tree):
-
     result = FlatTree(
         tree[FLAT_TREE_HYPERPLANES],
         tree[FLAT_TREE_OFFSETS],
         tree[FLAT_TREE_CHILDREN],
         tree[FLAT_TREE_INDICES],
         tree[FLAT_TREE_LEAF_SIZE],
     )
```

### Comparing `pynndescent-0.5.8/pynndescent/sparse.py` & `pynndescent-0.5.9/pynndescent/sparse.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/sparse_nndescent.py` & `pynndescent-0.5.9/pynndescent/sparse_nndescent.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/tests/conftest.py` & `pynndescent-0.5.9/pynndescent/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,21 @@
 def cosine_hang_data():
     this_dir = os.path.dirname(os.path.abspath(__file__))
     data_path = os.path.join(this_dir, "test_data/cosine_hang.npy")
     return np.load(data_path)
 
 
 @pytest.fixture
+def cosine_near_duplicates_data():
+    this_dir = os.path.dirname(os.path.abspath(__file__))
+    data_path = os.path.join(this_dir, "test_data/cosine_near_duplicates.npy")
+    return np.load(data_path)
+
+
+@pytest.fixture
 def small_data():
     return np.random.uniform(40, 5, size=(20, 5))
 
 
 @pytest.fixture
 def sparse_small_data():
     # Too low dim might cause more than one empty row,
```

### Comparing `pynndescent-0.5.8/pynndescent/tests/test_data/cosine_hang.npy` & `pynndescent-0.5.9/pynndescent/tests/test_data/cosine_hang.npy`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/tests/test_distances.py` & `pynndescent-0.5.9/pynndescent/tests/test_distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         "braycurtis",
         "correlation",
     ],
 )
 def test_sparse_spatial_check(sparse_spatial_data, metric, decimal=6):
     if metric in spdist.sparse_named_distances:
         dist_matrix = pairwise_distances(
-            sparse_spatial_data.todense().astype(np.float32), metric=metric
+            np.asarray(sparse_spatial_data.todense()).astype(np.float32), metric=metric
         )
     if metric in ("braycurtis", "dice", "sokalsneath", "yule"):
         dist_matrix[np.where(~np.isfinite(dist_matrix))] = 0.0
     if metric in ("cosine", "correlation", "kulsinski", "russellrao"):
         dist_matrix[np.where(~np.isfinite(dist_matrix))] = 1.0
         # And because distance between all zero vectors should be zero
         dist_matrix[10, 11] = 0.0
@@ -170,15 +170,15 @@
         "russellrao",
         "sokalmichener",
         "sokalsneath",
     ],
 )
 def test_sparse_binary_check(sparse_binary_data, metric):
     if metric in spdist.sparse_named_distances:
-        dist_matrix = pairwise_distances(sparse_binary_data.todense(), metric=metric)
+        dist_matrix = pairwise_distances(np.asarray(sparse_binary_data.todense()), metric=metric)
     if metric in ("jaccard", "dice", "sokalsneath"):
         dist_matrix[np.where(~np.isfinite(dist_matrix))] = 0.0
     if metric in ("kulsinski", "russellrao"):
         dist_matrix[np.where(~np.isfinite(dist_matrix))] = 1.0
         # And because distance between all zero vectors should be zero
         dist_matrix[10, 11] = 0.0
         dist_matrix[11, 10] = 0.0
@@ -305,15 +305,15 @@
 
 def test_spearmanr():
     x = np.random.randn(100)
     y = np.random.randn(100)
 
     scipy_expected = stats.spearmanr(x, y)
     r = dist.spearmanr(x, y)
-    assert_array_almost_equal(r, scipy_expected.correlation)
+    assert_array_almost_equal(r, 1 - scipy_expected.correlation)
 
 
 def test_alternative_distances():
 
     for distname in dist.fast_distance_alternatives:
 
         true_dist = dist.named_distances[distname]
```

### Comparing `pynndescent-0.5.8/pynndescent/tests/test_pynndescent_.py` & `pynndescent-0.5.9/pynndescent/tests/test_pynndescent_.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,32 @@
 
     proportion_correct = num_correct / (data.shape[0] * n_neighbors)
     assert (
         proportion_correct >= 0.95
     ), "NN-descent did not get 95% accuracy on nearest neighbors"
 
 
+def test_rp_trees_should_not_stack_overflow_with_near_duplicate_data(seed, cosine_near_duplicates_data):
+
+    n_neighbors = 10
+    knn_indices, _ = NNDescent(
+        cosine_near_duplicates_data,
+        "cosine",
+        {},
+        n_neighbors,
+        random_state=np.random.RandomState(seed),
+        n_trees=20,
+    )._neighbor_graph
+
+    for i in range(cosine_near_duplicates_data.shape[0]):
+        assert len(knn_indices[i]) == len(
+            np.unique(knn_indices[i])
+        ), "Duplicate graph_indices in knn graph"
+
+
 def test_output_when_verbose_is_true(spatial_data, seed):
     out = io.StringIO()
     with redirect_stdout(out):
         _ = NNDescent(
             data=spatial_data,
             metric="euclidean",
             metric_kwds={},
```

### Comparing `pynndescent-0.5.8/pynndescent/tests/test_rank.py` & `pynndescent-0.5.9/pynndescent/tests/test_rank.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/threaded_rp_trees.py` & `pynndescent-0.5.9/pynndescent/threaded_rp_trees.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent/utils.py` & `pynndescent-0.5.9/pynndescent/utils.py`

 * *Files identical despite different names*

### Comparing `pynndescent-0.5.8/pynndescent.egg-info/PKG-INFO` & `pynndescent-0.5.9/pynndescent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pynndescent
-Version: 0.5.8
+Version: 0.5.9
 Summary: Nearest Neighbor Descent
 Home-page: http://github.com/lmcinnes/pynndescent
 Author: Leland McInnes
 Author-email: leland.mcinnes@gmail.com
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: BSD
@@ -216,15 +216,14 @@
         
 Keywords: nearest neighbor,knn,ANN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
-Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `pynndescent-0.5.8/pynndescent.egg-info/SOURCES.txt` & `pynndescent-0.5.9/pynndescent.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 pynndescent.egg-info/requires.txt
 pynndescent.egg-info/top_level.txt
 pynndescent/tests/__init__.py
 pynndescent/tests/conftest.py
 pynndescent/tests/test_distances.py
 pynndescent/tests/test_pynndescent_.py
 pynndescent/tests/test_rank.py
-pynndescent/tests/test_data/cosine_hang.npy
+pynndescent/tests/test_data/cosine_hang.npy
+pynndescent/tests/test_data/cosine_near_duplicates.npy
```

### Comparing `pynndescent-0.5.8/setup.py` & `pynndescent-0.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 def readme():
     with open("README.rst") as readme_file:
         return readme_file.read()
 
 
 configuration = {
     "name": "pynndescent",
-    "version": "0.5.8",
+    "version": "0.5.9",
     "description": "Nearest Neighbor Descent",
     "long_description": readme(),
     "classifiers": [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved",
-        "Programming Language :: C",
         "Programming Language :: Python",
         "Topic :: Software Development",
         "Topic :: Scientific/Engineering",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
```

