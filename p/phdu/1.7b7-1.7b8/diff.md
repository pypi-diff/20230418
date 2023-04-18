# Comparing `tmp/phdu-1.7b7.tar.gz` & `tmp/phdu-1.7b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.7b7.tar", last modified: Wed Mar 22 15:49:56 2023, max compression
+gzip compressed data, was "phdu-1.7b8.tar", last modified: Tue Apr 18 11:10:29 2023, max compression
```

## Comparing `phdu-1.7b7.tar` & `phdu-1.7b8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.713224 phdu-1.7b7/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.7b7/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-03-22 15:49:56.713224 phdu-1.7b7/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.7b7/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.706558 phdu-1.7b7/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.706558 phdu-1.7b7/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    13090 2023-03-22 15:49:01.000000 phdu-1.7b7/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.709891 phdu-1.7b7/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      853 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    26448 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.709891 phdu-1.7b7/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.713224 phdu-1.7b7/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.7b7/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3581 2023-03-22 15:47:48.000000 phdu-1.7b7/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-03-22 15:49:56.706558 phdu-1.7b7/phdu.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-03-22 15:49:56.000000 phdu-1.7b7/phdu.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-03-22 15:49:56.000000 phdu-1.7b7/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-03-22 15:49:56.000000 phdu-1.7b7/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-03-22 15:49:56.000000 phdu-1.7b7/phdu.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-03-22 15:49:56.000000 phdu-1.7b7/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-03-22 15:49:56.713224 phdu-1.7b7/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-03-22 15:49:20.000000 phdu-1.7b7/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.610703 phdu-1.7b8/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.7b8/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:10:29.610703 phdu-1.7b8/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.7b8/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.522699 phdu-1.7b8/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.7b8/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.7b8/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.7b8/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.7b8/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.7b8/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.7b8/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.566701 phdu-1.7b8/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.7b8/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.7b8/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.7b8/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    13090 2023-04-18 11:06:30.000000 phdu-1.7b8/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.7b8/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.586702 phdu-1.7b8/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.7b8/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.7b8/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      853 2022-11-08 18:00:22.000000 phdu-1.7b8/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.7b8/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    27651 2023-04-18 11:09:00.000000 phdu-1.7b8/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.7b8/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.7b8/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.594702 phdu-1.7b8/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.7b8/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.7b8/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.7b8/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.606703 phdu-1.7b8/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.7b8/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.7b8/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.7b8/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3581 2023-02-08 11:11:43.000000 phdu-1.7b8/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.550700 phdu-1.7b8/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-18 11:10:29.622704 phdu-1.7b8/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-18 11:09:57.000000 phdu-1.7b8/setup.py
```

### Comparing `phdu-1.7b7/LICENSE.md` & `phdu-1.7b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/PKG-INFO` & `phdu-1.7b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b7
+Version: 1.7b8
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b7/README.md` & `phdu-1.7b8/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/_helper.py` & `phdu-1.7b8/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/clustering.py` & `phdu-1.7b8/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/decomposition.py` & `phdu-1.7b8/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/np_utils.py` & `phdu-1.7b8/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/pd_utils.py` & `phdu-1.7b8/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/plots/base.py` & `phdu-1.7b8/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/plots/plotly_utils.py` & `phdu-1.7b8/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/script_fmt.py` & `phdu-1.7b8/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/_integration.py` & `phdu-1.7b8/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/_plots.py` & `phdu-1.7b8/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/bootstrap.py` & `phdu-1.7b8/phdu/stats/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     if shell == 'ZMQInteractiveShell': # script being run in Jupyter notebook
         from tqdm.notebook import tqdm
     elif shell == 'TerminalInteractiveShell': #script being run in iPython terminal
         from tqdm import tqdm
 except NameError:
     from tqdm import tqdm # Probably runing on standard python terminal.
 
-from ..np_utils import numpy_fill 
+from ..np_utils import numpy_fill
 from ._integration import simpson3oct_vec
 from . import conf_interval
-    
+
 @njit
 def resample_paired_nb(X, Y, func, output_len=1, R=int(1e5), seed=0):
     np.random.seed(seed)
-    N = X.size    
+    N = X.size
     data_paired = np.vstack((X, Y)).T
     idxs_resampling = np.random.randint(low=0, high=N, size=R*N)
-    data_resampled = data_paired[idxs_resampling].reshape(R, N, 2)    
+    data_resampled = data_paired[idxs_resampling].reshape(R, N, 2)
     stat = func(X, Y)
-    
+
     boot_sample = np.empty((R, output_len))
     for i, r in enumerate(data_resampled):
         x, y = r.T
         boot_sample[i] = func(x, y)
     return boot_sample
 
 @njit
@@ -71,45 +71,66 @@
             data_resampled[:,:,k] += h_k * np.random.standard_t(n_trimmed, R*N)
     return data_resampled
 
 @njit
 def resample_nb(X, func, output_len=1, R=int(1e5), seed=0, smooth=False, N=0):
     """X: array of shape (N_samples, n_vars)."""
     data_resampled = resample_nb_X(X, R=R, seed=seed, smooth=smooth, N=N)
-    
+
     boot_sample = np.empty((R, output_len))
     for i, r in enumerate(data_resampled):
         boot_sample[i] = func(r)
     return boot_sample
 
 @njit
+def resample_twosamples_nb(X1, X2, func, output_len=1, R=int(1e5), seed=0, smooth=False, N=0):
+    """Xi: array of shape (N_samples, n_vars)."""
+    data_resampled_1 = resample_nb_X(X1, R=R, seed=seed, smooth=smooth, N=N)
+    data_resampled_2 = resample_nb_X(X2, R=R, seed=seed, smooth=smooth, N=N)
+
+    boot_sample = np.empty((R, output_len))
+    for i, (r1, r2) in enumerate(zip(data_resampled_1, data_resampled_2)):
+        boot_sample[i] = func(r1, r2)
+    return boot_sample
+
+def resample_twosamples(X1, X2, func, output_len=1, R=int(1e5), seed=0, smooth=False, N=0):
+    """Xi: array of shape (N_samples, n_vars)."""
+    data_resampled_1 = resample_nb_X(X1, R=R, seed=seed, smooth=smooth, N=N)
+    data_resampled_2 = resample_nb_X(X2, R=R, seed=seed, smooth=smooth, N=N)
+
+    boot_sample = np.empty((R, output_len))
+    for i, (r1, r2) in enumerate(zip(data_resampled_1, data_resampled_2)):
+        boot_sample[i] = func(r1, r2)
+    return boot_sample
+
+@njit
 def _nb_mean(x):
     """
     njit version of numpy mean.
     """
     return np.mean(x)
 
 @njit
 def resample_block_nb(X, Y, func, output_len=1, R=int(1e5), seed=0, stack_data=True, aggregator=_nb_mean):
     """
-    X, Y:         ragged arrays or tuples. Each element is an array containing the data for a block. 
+    X, Y:         ragged arrays or tuples. Each element is an array containing the data for a block.
     func:         numba function f: X,Y  ->  Z,   Z: 1D array of size output_len.
     aggregator:   numba function for aggregating data from a block.
     """
     np.random.seed(seed)
     def stack(arr_list):
         return np.array([a for arr in arr_list for a in arr])
-    
+
     n_x = [len(x) for x in X]
     n_y = [len(y) for y in Y]
     idxs_resampling_x = [np.random.randint(low=0, high=n, size=R*n) for n in n_x]
     idxs_resampling_y = [np.random.randint(low=0, high=n, size=R*n) for n in n_y]
     X_resampled = [x[idxs_resampling].reshape(R, n) for x, n, idxs_resampling in zip(X, n_x, idxs_resampling_x)]
     Y_resampled = [y[idxs_resampling].reshape(R, n) for y, n, idxs_resampling in zip(Y, n_y, idxs_resampling_y)]
-    
+
     boot_sample = np.empty((R, output_len))
     if stack_data:
         for i in range(R):
             Xi = stack([x[i] for x in X_resampled])
             Yi = stack([y[i] for y in Y_resampled])
             boot_sample[i] = func(Xi, Yi)
     else:
@@ -121,43 +142,43 @@
 
 def resample(X, func, output_len=1, R=int(1e4), seed=0):
     """X: array of shape (N_samples, n_vars)."""
     np.random.seed(seed)
     N = X.shape[0]
     idxs_resampling = np.random.randint(low=0, high=N, size=R*N)
     data_resampled = X[idxs_resampling].reshape(R, N, X.shape[1])
-    
+
     boot_sample = np.empty((R, output_len))
     for i, r in enumerate(data_resampled):
         boot_sample[i] = func(r)
     return boot_sample
 
 
 def resample_block(X, Y, func, output_len=1, R=int(1e5), seed=0):
     """
-    X, Y:   ragged arrays or tuples. Each element is an array containing the data for a block. 
+    X, Y:   ragged arrays or tuples. Each element is an array containing the data for a block.
     func:   numba function f: X,Y  ->  Z,   Z: 1D array of size output_len.
     """
     np.random.seed(seed)
-    
+
     n_x = [len(x) for x in X]
     n_y = [len(y) for y in Y]
     idxs_resampling_x = [np.random.randint(low=0, high=n, size=R*n) for n in n_x]
     idxs_resampling_y = [np.random.randint(low=0, high=n, size=R*n) for n in n_y]
     X_resampled = [x[idxs_resampling].reshape(R, n) for x, n, idxs_resampling in zip(X, n_x, idxs_resampling_x)]
     Y_resampled = [y[idxs_resampling].reshape(R, n) for y, n, idxs_resampling in zip(Y, n_y, idxs_resampling_y)]
-    
+
     boot_sample = np.empty((R, output_len))
     for i in range(R):
         Xi = np.hstack([x[i] for x in X_resampled])
         Yi = np.hstack([y[i] for y in Y_resampled])
         boot_sample[i] = func(Xi, Yi)
     return boot_sample
 
-    
+
 @njit
 def jackknife_resampling(data):
     """Performs jackknife resampling on numpy arrays.
 
     Jackknife resampling is a technique to generate 'n' deterministic samples
     of size 'n-1' from a measured sample of size 'n'. The i-th
     sample  is generated by removing the i-th measurement
@@ -202,15 +223,15 @@
     in [0, 1].
     """
     B = a.shape[axis]
     if account_equal:
         return ((a < score).sum(axis=axis) + (a <= score).sum(axis=axis)) / (2 * B)
     else:
         return (a < score).sum(axis=axis) / B
-    
+
 def _resample(data, data2, use_numba, statistic, R, n_min=5, smooth=False, stack_data=True, aggregator=_nb_mean, **kwargs):
     """
     Resample using normal resampling if data2 is None.
     Else uses block resampling with data and data2.
     """
     if data2 is None:
         if data.ndim == 1:
@@ -224,76 +245,85 @@
         if N < n_min:
             warnings.warn(f"N={N} < n_min={n_min}. Avoiding computation (returning NaNs) ...")
             theta_hat_b = None
         else:
             resample_func = resample_nb if use_numba else resample
             theta_hat_b = resample_func(data, statistic, R=R, output_len=output_len, smooth=smooth, **kwargs).squeeze()
     else:
-        if stack_data:
-            sample_stat = statistic(np.hstack(data), np.hstack(data2))
+        is_block = isinstance(data, tuple)
+        if is_block:
+            if stack_data:
+                sample_stat = statistic(np.hstack(data), np.hstack(data2))
+            else:
+                sample_stat = statistic(np.array([aggregator(di) for di in data]), np.array([aggregator(di) for di in data2]))
+            total_N = lambda data: np.sum([d.shape[0] for d in data])
+            N = min([total_N(data), total_N(data2)])
+            resample_func = resample_block_nb if use_numba else resample_block
+            resample_kwargs = dict(stack_data=stack_data, aggregator=aggregator)
         else:
-            sample_stat = statistic(np.array([aggregator(di) for di in data]), np.array([aggregator(di) for di in data2]))
+            sample_stat = statistic(data, data2)
+            N = min([len(data), len(data2)])
+            resample_func = resample_twosamples_nb if use_numba else resample_twosamples
+            resample_kwargs = dict()
+
         if hasattr(sample_stat, "__len__"):
             output_len = len(sample_stat)
         else:
             output_len = 1
-        total_N = lambda data: np.sum([d.shape[0] for d in data])
-        N = min([total_N(data), total_N(data2)])
         if N < n_min:
             warnings.warn(f"N={N} < n_min={n_min}. Avoiding computation (returning NaNs) ...")
             theta_hat_b = None
         else:
-            resample_func = resample_block_nb if use_numba else resample_block
-            theta_hat_b = resample_func(data, data2, statistic, R=R, output_len=output_len, stack_data=stack_data, aggregator=aggregator, **kwargs).squeeze()
-            if stack_data:
+            theta_hat_b = resample_func(data, data2, statistic, R=R, output_len=output_len, **resample_kwargs, **kwargs).squeeze()
+            if stack_data and is_block:
                 data = np.hstack(data)
                 data2 = np.hstack(data2)
     return data, data2, theta_hat_b, sample_stat, N
-    
+
 def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=5, **kwargs):
     """
     If data2 is provided, assumes a block resampling and statistic takes two arguments.
     Optional kwargs for aggregating data, data2 before computing the statistic:
-            stack_data = False, 
+            stack_data = False,
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
     if alternative == 'two-sided':
         probs = np.array([alpha/2, 1 - alpha/2])
     elif alternative == 'less':
         probs = np.array([0, 1-alpha])
     elif alternative == 'greater':
         probs = np.array([alpha, 1])
     else:
         raise ValueError(f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'.")
-        
+
     data, data2, theta_hat_b, sample_stat, N = _resample(data, data2, use_numba, statistic, R=R, n_min=n_min, **kwargs)
-    
+
     if theta_hat_b is None:
         return np.array([np.NaN, np.NaN])
-        
+
     alpha_bca = _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba)[0]
-    
-    if np.isnan(alpha_bca).all(): 
+
+    if np.isnan(alpha_bca).all():
         warnings.warn('CI shows there is only one value. Check data.', RuntimeWarning)
         if data2 is None:
             sample_stat = statistic(data)
         else:
             sample_stat = statistic(data, data2)
         return np.array([sample_stat, sample_stat])
     else:
         return _compute_CI_percentile(theta_hat_b, alpha_bca, alternative)
     #elif alternative == 'two-sided':
     #    return  np.percentile(theta_hat_b, alpha_bca*100, axis=0)
     #elif alternative == 'less':
     #     return np.array([-np.inf, np.percentile(theta_hat_b, alpha_bca[0]*100, axis=0)])
     #elif alternative == 'greater':
     #    return np.array([np.percentile(theta_hat_b, alpha_bca[0]*100, axis=0), np.inf])
-    
+
 def _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba):
     """Bias-corrected and accelerated interval."""
     # calculate z0_hat
     if data2 is None:
         theta_hat = statistic(data)
     else:
         theta_hat = statistic(data, data2)
@@ -303,15 +333,15 @@
     # calculate a_hat
     if data2 is None:
         jackknife_computer = jackknife_stat_nb if use_numba else jackknife_stat
         theta_hat_jk = jackknife_computer(data, statistic)  # jackknife resample
     else:
         theta_hat_jk = jackknife_stat_two_samples(data, data2, statistic)
     n = theta_hat_jk.shape[0]
-    theta_hat_jk_dot = theta_hat_jk.mean(axis=0) 
+    theta_hat_jk_dot = theta_hat_jk.mean(axis=0)
 
     U = (n - 1) * (theta_hat_jk_dot - theta_hat_jk)
     num = (U**3).sum(axis=0) / n**3
     den = (U**2).sum(axis=0) / n**2
     a_hat = 1/6 * num / (den**(3/2))
 
     # calculate alpha_1, alpha_2
@@ -362,27 +392,27 @@
     return CIs
 
 def compute_CI_studentized(base, results, studentized_results, alpha=0.05, alternative='two-sided'):
     R, output_len = results.shape
     bootstrap_estimate = results.mean(axis=0)
     errors = results - bootstrap_estimate
     std_err = np.asarray(np.sqrt(np.diag(errors.T.dot(errors) / R)))
-    
+
     lower = np.empty((output_len))
     upper = np.empty((output_len))
     alpha_tails = alpha / 2 if alternative == 'two-sided' else alpha
     percentiles = 100 * np.array([[alpha_tails, 1.0 - alpha_tails]] * output_len)
     for i in range(output_len):
         lower[i], upper[i] = np.percentile(studentized_results[:, i], percentiles[i])
     if alternative == 'less':
         upper.fill(np.inf)
     elif alternative == 'greater':
         lower.fill(-1 * np.inf)
-        
-    # Basic and studentized use the lower empirical quantile to compute upper and vice versa.      
+
+    # Basic and studentized use the lower empirical quantile to compute upper and vice versa.
     lower_copy = lower + 0.0
     lower = base - upper * std_err
     upper = base - lower_copy * std_err
     CI = np.vstack((lower, upper)).T
     return CI
 
 def vs_integrand(x, f_linear):
@@ -391,15 +421,15 @@
     if np.isnan(clipped_f).any():
         clipped_f = numpy_fill(clipped_f)
     return 1 / clipped_f
 
 def cov(results, base=None, recenter=False):
     """
     reps : Number of bootstrap replications
-    recenter : Whether to center the bootstrap variance estimator on the average of the bootstrap samples (True), or 
+    recenter : Whether to center the bootstrap variance estimator on the average of the bootstrap samples (True), or
                        to center on the original sample estimate (False).
     """
     if recenter:
         errors = results - np.mean(results, 0)
     else:
         assert base is not None
         errors = results - base
@@ -410,23 +440,23 @@
     output_len = base.size
     studentized_results = np.empty((R, output_len))
     results = np.empty((R, output_len))
     se_bootstrap = np.empty((R, output_len))
     n = data.shape[0]
     if divide_by_se:
         def get_studentized(data_r, result, seed):
-            nested_resampling = resample_nb(data_r, statistic, R=studentized_reps, output_len=output_len, seed=seed, smooth=False)        
+            nested_resampling = resample_nb(data_r, statistic, R=studentized_reps, output_len=output_len, seed=seed, smooth=False)
             std_err = np.sqrt(np.diag(cov(nested_resampling, result, recenter=recenter)))
             err = result - base
             t_result = err /std_err
             return t_result, std_err
     else:
         def get_studentized(data_r, result, seed):
             return result - base, np.NaN
-    
+
     data_r = resample_nb_X(data, R=R, seed=seed, smooth=smooth)
     if se_func is None:
         for i, d_r in enumerate(data_r):
             result = statistic(d_r)
             t_result, std_err = get_studentized(d_r, result, i)
             results[i] = result
             studentized_results[i] = t_result # t = (x^ - x) / s
@@ -436,23 +466,23 @@
             result = statistic(d_r)
             se = se_func(d_r)
             results[i] = result
             studentized_results[i] = (result - base) / se
             se_bootstrap[i] = se
     return base, results, studentized_results, se_bootstrap
 
-def CI_studentized(data, statistic, R=int(1e5), alpha=0.05, alternative='two-sided', smooth=False, vs=False, 
-                   frac_g=2/3, frac_invert=1/10, studentized_reps=100, 
+def CI_studentized(data, statistic, R=int(1e5), alpha=0.05, alternative='two-sided', smooth=False, vs=False,
+                   frac_g=2/3, frac_invert=1/10, studentized_reps=100,
                    integration_precision=1e-4, **kwargs):
     assert alternative in ['two-sided', 'less', 'greater'], f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'."
     base, results, studentized_results, se_bootstrap = _bootstrap_studentized_resampling(data, statistic, smooth=smooth, R=R, studentized_reps=studentized_reps, **kwargs)
     if vs:
         g, lowess_linear_interp = vs_transform(data, results, se_bootstrap, precision=integration_precision, frac=frac_g)
         base_g, results_g, studentized_results_g, _ = _bootstrap_studentized_resampling(g, statistic, R=R, divide_by_se=False, smooth=False)
-        CI = invert_CI(compute_CI_studentized(base_g, results_g, studentized_results_g, alpha=alpha, alternative=alternative), 
+        CI = invert_CI(compute_CI_studentized(base_g, results_g, studentized_results_g, alpha=alpha, alternative=alternative),
                        data, g, lowess_linear_interp, frac=frac_invert, integration_precision=integration_precision)
     else:
         CI = compute_CI_studentized(base, results, studentized_results, alpha=alpha, alternative=alternative)
     return CI
 
 def _compute_CI_percentile(boot_sample, alpha, alternative):
     alpha_iter = isinstance(alpha, Iterable)
@@ -477,50 +507,50 @@
         CI = np.vstack((np.percentile(boot_sample, alpha_ptg[0] if alpha_iter else alpha_ptg, axis=0), np.inf * np.ones((output_len)))).T
     else:
         raise ValueError(f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'.")
     return CI
 
 def CI_percentile(data, statistic, data2=None, R=int(1e5), alpha=0.05, smooth=False, alternative='two-sided', n_min=3, use_numba=True, **kwargs):
     """
-    If data2 is provided, assumes a block resampling and statistic takes two arguments.
+    If data2 is provided, statistic takes two arguments and assumes block resampling if the input data are tuples.
     Optional kwargs for aggregating data, data2 before computing the statistic:
-            stack_data = False, 
+            stack_data = False,
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
     data, data2, boot_sample, sample_stat, N = _resample(data, data2, use_numba, statistic, R=R, n_min=n_min, smooth=smooth, **kwargs)
     if boot_sample is None:
         return np.array([np.NaN, np.NaN])
-    else:    
+    else:
         return _compute_CI_percentile(boot_sample, alpha, alternative)
 
 def CI_all(data, statistic, R=int(1e5), alpha=0.05, alternative='two-sided', coverage_iters=int(1e5), coverage_seed=42, avg_len=3, exclude=['studentized_vs', 'studentized_vs_smooth']):
     """
-    Computes all CIs. 
+    Computes all CIs.
     exclude: CIs to exclude. Available: percentile
                                         percentile_smooth
                                         bca
-                                        bca_smooth 
+                                        bca_smooth
                                         studentized
                                         studentized_smooth
                                         studentized_vs
                                         studentized_vs_smooth
     """
     specs = dict(percentile = (CI_percentile, {}),
                  percentile_smooth = (CI_percentile, dict(smooth=True)),
                  bca = (CI_bca, {}),
                  bca_smooth = (CI_bca, dict(smooth=True)),
                  studentized = (CI_studentized, {}),
                  studentized_smooth = (CI_studentized, dict(smooth=True)),
                  studentized_vs = (CI_studentized, dict(vs=True)),
                  studentized_vs_smooth = (CI_studentized, dict(vs=True, smooth=True))
                 )
-    specs = {k: v for k, v in specs.items() if k not in exclude} 
-    
+    specs = {k: v for k, v in specs.items() if k not in exclude}
+
     CIs = defaultdict(list)
     for label, (func, kws) in tqdm(specs.items()):
         CI = func(data, statistic, R=R, alpha=alpha, alternative=alternative, **kws)
         CIs['CI'].append(label)
         if CI.shape[0] == 1 or CI.ndim == 1:
             CI = CI.squeeze()
             CIs['low'].append(CI[0])
@@ -528,18 +558,18 @@
         else:
             CIs['low'].append(CI[:, 0])
             CIs['high'].append(CI[:, 1])
     return conf_interval.CI_specs(pd.DataFrame(CIs).set_index('CI'), data, statistic, coverage_iters=coverage_iters, seed=coverage_seed, avg_len=avg_len)
 
 def power_analysis_naive(data, statistic, low, high, N_values=np.array([5, 10, 25, 50, 100, 200]), R=int(1e4), seed=0):
     """
-    Naive bootstrap power and sample-size calculation for accepting H0. 
+    Naive bootstrap power and sample-size calculation for accepting H0.
     Computes violations on the low and high bound of H0.
     See Efron-Tshibirani: An introduction to the bootstrap,  p. 379-381.
-    
+
     Returns: dataframe with index=N_values, columns=[low_fails, high_fails, power].
     """
     results = defaultdict(list)
     n = data.shape[0]
     if n not in N_values:
         N_values = np.sort(np.hstack((n, N_values)))
     for N in N_values:
@@ -551,49 +581,49 @@
         results['violations-high'].append(fail_high)
         results['power'].append(power)
     return pd.DataFrame(results, index=N_values)
 
 def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0,
                    R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3)):
     """
-    Stable bootstrap power and sample-size calculation for accepting H0. 
+    Stable bootstrap power and sample-size calculation for accepting H0.
     Computes violations on the studentized equivalent for the low and high bound of H0.
     Takes into account the variability in the original sample (size n):   bootstrap estimate, SE of the bootstrap estimate.
                                      and in the future sample (size N):   bootstrap estimate.
     See Efron-Tshibirani: An introduction to the bootstrap,  p. 381-384.
-    
+
     Returns: dataframe with index=N_values, columns=[low_fails, high_fails, power].
     """
     n = data.shape[0]
     if n not in N_values:
         N_values = np.sort(np.hstack((n, N_values)))
     base = statistic(data)
-    se_estimate = np.sqrt(np.diag(cov(resample_nb(data, statistic, seed=seed, R=R_se, output_len=output_len), 
+    se_estimate = np.sqrt(np.diag(cov(resample_nb(data, statistic, seed=seed, R=R_se, output_len=output_len),
                                       base,
                                       recenter=recenter)
-                                 ))    
+                                 ))
     low_studentized = (base - low) / se_estimate
     high_studentized = (base - high) / se_estimate
-    
+
     # Estimation of SE (datasize = n). This is the computational bottleneck.
     data_n = resample_nb_X(data, R=R, seed=seed+1)
     se_estimate_n = np.empty((R, output_len))
     estimate_n = np.empty((R, output_len))
     for i, d_n in enumerate(tqdm(data_n)):
         estimate_n_i = statistic(d_n)
         nested_estimate_n = resample_nb(d_n, statistic, seed=seed+3+i, R=R_se_nested, output_len=output_len)
         estimate_n[i] = estimate_n_i
-        se_estimate_n[i] = np.sqrt(np.diag(cov(nested_estimate_n, estimate_n_i, recenter=recenter))) 
-        
+        se_estimate_n[i] = np.sqrt(np.diag(cov(nested_estimate_n, estimate_n_i, recenter=recenter)))
+
     # Violations of studentized endpoints.
     results = defaultdict(list)
     for N in N_values:
         estimate_N = resample_nb(data, statistic, N=N, R=R, seed=seed+2, output_len=output_len)
-        T = (estimate_n - estimate_N) / se_estimate_n           
+        T = (estimate_n - estimate_N) / se_estimate_n
         low_violations = (T >= low_studentized).mean()
         high_violations = (T <= high_studentized).mean()
         power = 1 - low_violations - high_violations
         results['violations-low'].append(low_violations)
         results['violations-high'].append(high_violations)
         results['power'].append(power)
-        
+
     return pd.DataFrame(results, index=N_values)
```

### Comparing `phdu-1.7b7/phdu/stats/conf_interval.py` & `phdu-1.7b8/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/corr.py` & `phdu-1.7b8/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/rtopy/_helper.py` & `phdu-1.7b8/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/rtopy/resample.py` & `phdu-1.7b8/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/stats/test/permutation.py` & `phdu-1.7b8/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu/storage.py` & `phdu-1.7b8/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/phdu.egg-info/PKG-INFO` & `phdu-1.7b8/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b7
+Version: 1.7b8
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b7/phdu.egg-info/SOURCES.txt` & `phdu-1.7b8/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.7b7/setup.py` & `phdu-1.7b8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.7.b7',
+    version='1.7.b8',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

