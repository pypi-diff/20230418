# Comparing `tmp/phdu-1.7b8.tar.gz` & `tmp/phdu-1.7b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.7b8.tar", last modified: Tue Apr 18 11:10:29 2023, max compression
+gzip compressed data, was "phdu-1.7b9.tar", last modified: Tue Apr 18 11:22:58 2023, max compression
```

## Comparing `phdu-1.7b8.tar` & `phdu-1.7b9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.610703 phdu-1.7b8/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.7b8/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:10:29.610703 phdu-1.7b8/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.7b8/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.522699 phdu-1.7b8/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.7b8/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.7b8/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.7b8/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.7b8/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.7b8/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.7b8/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.566701 phdu-1.7b8/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.7b8/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.7b8/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.7b8/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    13090 2023-04-18 11:06:30.000000 phdu-1.7b8/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.7b8/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.586702 phdu-1.7b8/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.7b8/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.7b8/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      853 2022-11-08 18:00:22.000000 phdu-1.7b8/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.7b8/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    27651 2023-04-18 11:09:00.000000 phdu-1.7b8/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.7b8/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.7b8/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.594702 phdu-1.7b8/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.7b8/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.7b8/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.7b8/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.606703 phdu-1.7b8/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.7b8/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.7b8/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.7b8/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3581 2023-02-08 11:11:43.000000 phdu-1.7b8/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:10:29.550700 phdu-1.7b8/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-18 11:10:29.000000 phdu-1.7b8/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-18 11:10:29.622704 phdu-1.7b8/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-18 11:09:57.000000 phdu-1.7b8/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.990646 phdu-1.7b9/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.7b9/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:22:57.990646 phdu-1.7b9/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.7b9/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.898642 phdu-1.7b9/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.7b9/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.7b9/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.7b9/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.7b9/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.7b9/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.7b9/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.938644 phdu-1.7b9/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.7b9/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.7b9/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.7b9/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    13090 2023-04-18 11:06:30.000000 phdu-1.7b9/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.7b9/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.966645 phdu-1.7b9/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.7b9/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.7b9/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      853 2022-11-08 18:00:22.000000 phdu-1.7b9/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.7b9/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    27790 2023-04-18 11:22:26.000000 phdu-1.7b9/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.7b9/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.7b9/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.974646 phdu-1.7b9/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.7b9/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.7b9/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.7b9/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.986646 phdu-1.7b9/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.7b9/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.7b9/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.7b9/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3581 2023-02-08 11:11:43.000000 phdu-1.7b9/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-18 11:22:57.926643 phdu-1.7b9/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-18 11:22:57.000000 phdu-1.7b9/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-18 11:22:57.998647 phdu-1.7b9/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-18 11:22:37.000000 phdu-1.7b9/setup.py
```

### Comparing `phdu-1.7b8/LICENSE.md` & `phdu-1.7b9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/PKG-INFO` & `phdu-1.7b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b8
+Version: 1.7b9
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b8/README.md` & `phdu-1.7b9/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/_helper.py` & `phdu-1.7b9/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/clustering.py` & `phdu-1.7b9/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/decomposition.py` & `phdu-1.7b9/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/np_utils.py` & `phdu-1.7b9/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/pd_utils.py` & `phdu-1.7b9/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/plots/base.py` & `phdu-1.7b9/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/plots/plotly_utils.py` & `phdu-1.7b9/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/script_fmt.py` & `phdu-1.7b9/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/_integration.py` & `phdu-1.7b9/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/_plots.py` & `phdu-1.7b9/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/bootstrap.py` & `phdu-1.7b9/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,14 +256,18 @@
             else:
                 sample_stat = statistic(np.array([aggregator(di) for di in data]), np.array([aggregator(di) for di in data2]))
             total_N = lambda data: np.sum([d.shape[0] for d in data])
             N = min([total_N(data), total_N(data2)])
             resample_func = resample_block_nb if use_numba else resample_block
             resample_kwargs = dict(stack_data=stack_data, aggregator=aggregator)
         else:
+            if data.ndim == 1:
+                data = data[:, None]
+            if data2.ndim == 1:
+                data2 = data2[:, None]
             sample_stat = statistic(data, data2)
             N = min([len(data), len(data2)])
             resample_func = resample_twosamples_nb if use_numba else resample_twosamples
             resample_kwargs = dict()
 
         if hasattr(sample_stat, "__len__"):
             output_len = len(sample_stat)
```

### Comparing `phdu-1.7b8/phdu/stats/conf_interval.py` & `phdu-1.7b9/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/corr.py` & `phdu-1.7b9/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/rtopy/_helper.py` & `phdu-1.7b9/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/rtopy/resample.py` & `phdu-1.7b9/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/stats/test/permutation.py` & `phdu-1.7b9/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu/storage.py` & `phdu-1.7b9/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/phdu.egg-info/PKG-INFO` & `phdu-1.7b9/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.7b8
+Version: 1.7b9
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.7b8/phdu.egg-info/SOURCES.txt` & `phdu-1.7b9/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.7b8/setup.py` & `phdu-1.7b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.7.b8',
+    version='1.7.b9',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

