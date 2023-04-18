# Comparing `tmp/kondo_ml-0.0.8.tar.gz` & `tmp/kondo_ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kondo_ml-0.0.8.tar", last modified: Mon Apr 17 10:41:55 2023, max compression
+gzip compressed data, was "kondo_ml-0.0.9.tar", last modified: Mon Apr 17 10:56:20 2023, max compression
```

## Comparing `kondo_ml-0.0.8.tar` & `kondo_ml-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.402038 kondo_ml-0.0.8/
--rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.8/LICENSE
--rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 10:41:55.401527 kondo_ml-0.0.8/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)      205 2023-04-17 09:22:08.000000 kondo_ml-0.0.8/README.md
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.379378 kondo_ml-0.0.8/kondo_ml/
--rw-r--r--   0 rueck      (501) staff       (20)      549 2023-04-17 10:40:11.000000 kondo_ml-0.0.8/kondo_ml/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.392388 kondo_ml-0.0.8/kondo_ml/instance_selection/
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.394260 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)     4281 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/datasets.py
--rw-r--r--   0 rueck      (501) staff       (20)    30415 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/linear.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.398197 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/
--rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
--rw-r--r--   0 rueck      (501) staff       (20)    42882 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/SELCON.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.400774 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/
--rw-r--r--   0 rueck      (501) staff       (20)    13594 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    14712 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
--rw-r--r--   0 rueck      (501) staff       (20)     4081 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/time_series.py
--rw-r--r--   0 rueck      (501) staff       (20)     1191 2023-04-17 09:53:23.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    21430 2023-04-17 10:38:50.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_drop.py
--rw-r--r--   0 rueck      (501) staff       (20)     5428 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_fish.py
--rw-r--r--   0 rueck      (501) staff       (20)     1911 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_fixed_time_window.py
--rw-r--r--   0 rueck      (501) staff       (20)      774 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_full_set.py
--rw-r--r--   0 rueck      (501) staff       (20)     3305 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_gradient_shapley.py
--rw-r--r--   0 rueck      (501) staff       (20)      705 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_local_outlier_factor.py
--rw-r--r--   0 rueck      (501) staff       (20)     2916 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_mutual_information.py
--rw-r--r--   0 rueck      (501) staff       (20)      736 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_random_selection.py
--rw-r--r--   0 rueck      (501) staff       (20)     3311 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_reg_CNN.py
--rw-r--r--   0 rueck      (501) staff       (20)     8488 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_reg_ENN.py
--rw-r--r--   0 rueck      (501) staff       (20)     1381 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/_selcon.py
--rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.8/kondo_ml/instance_selection/base.py
--rw-r--r--   0 rueck      (501) staff       (20)      462 2023-04-17 09:15:49.000000 kondo_ml-0.0.8/kondo_ml/kondo_ml.py
--rw-r--r--   0 rueck      (501) staff       (20)     2343 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/kondo_ml/utils.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:41:55.381984 kondo_ml-0.0.8/kondo_ml.egg-info/
--rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 10:41:55.000000 kondo_ml-0.0.8/kondo_ml.egg-info/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-17 10:41:55.000000 kondo_ml-0.0.8/kondo_ml.egg-info/SOURCES.txt
--rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-17 10:41:55.000000 kondo_ml-0.0.8/kondo_ml.egg-info/dependency_links.txt
--rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-17 10:41:55.000000 kondo_ml-0.0.8/kondo_ml.egg-info/requires.txt
--rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-17 10:41:55.000000 kondo_ml-0.0.8/kondo_ml.egg-info/top_level.txt
--rw-r--r--   0 rueck      (501) staff       (20)      620 2023-04-17 10:40:11.000000 kondo_ml-0.0.8/pyproject.toml
--rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-17 10:41:55.402202 kondo_ml-0.0.8/setup.cfg
--rw-r--r--   0 rueck      (501) staff       (20)     1605 2023-04-17 09:18:30.000000 kondo_ml-0.0.8/setup.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.408606 kondo_ml-0.0.9/
+-rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.9/LICENSE
+-rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 10:56:20.407969 kondo_ml-0.0.9/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)      205 2023-04-17 09:22:08.000000 kondo_ml-0.0.9/README.md
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.354074 kondo_ml-0.0.9/kondo_ml/
+-rw-r--r--   0 rueck      (501) staff       (20)      549 2023-04-17 10:55:31.000000 kondo_ml-0.0.9/kondo_ml/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.389672 kondo_ml-0.0.9/kondo_ml/instance_selection/
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.394055 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4281 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/datasets.py
+-rw-r--r--   0 rueck      (501) staff       (20)    30415 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/linear.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.400195 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/
+-rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
+-rw-r--r--   0 rueck      (501) staff       (20)    42882 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/SELCON.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.404641 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/
+-rw-r--r--   0 rueck      (501) staff       (20)    13594 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    14712 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4081 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/time_series.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1191 2023-04-17 09:53:23.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    21430 2023-04-17 10:38:50.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_drop.py
+-rw-r--r--   0 rueck      (501) staff       (20)     5428 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_fish.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1911 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_fixed_time_window.py
+-rw-r--r--   0 rueck      (501) staff       (20)      774 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_full_set.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3305 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_gradient_shapley.py
+-rw-r--r--   0 rueck      (501) staff       (20)      705 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_local_outlier_factor.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2916 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_mutual_information.py
+-rw-r--r--   0 rueck      (501) staff       (20)      736 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_random_selection.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3311 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_reg_CNN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     8488 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_reg_ENN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1381 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/_selcon.py
+-rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.9/kondo_ml/instance_selection/base.py
+-rw-r--r--   0 rueck      (501) staff       (20)      462 2023-04-17 09:15:49.000000 kondo_ml-0.0.9/kondo_ml/kondo_ml.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2343 2023-04-17 09:18:30.000000 kondo_ml-0.0.9/kondo_ml/utils.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 10:56:20.362425 kondo_ml-0.0.9/kondo_ml.egg-info/
+-rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 10:56:20.000000 kondo_ml-0.0.9/kondo_ml.egg-info/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-17 10:56:20.000000 kondo_ml-0.0.9/kondo_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-17 10:56:20.000000 kondo_ml-0.0.9/kondo_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 rueck      (501) staff       (20)       44 2023-04-17 10:56:20.000000 kondo_ml-0.0.9/kondo_ml.egg-info/requires.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-17 10:56:20.000000 kondo_ml-0.0.9/kondo_ml.egg-info/top_level.txt
+-rw-r--r--   0 rueck      (501) staff       (20)      634 2023-04-17 10:55:31.000000 kondo_ml-0.0.9/pyproject.toml
+-rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-17 10:56:20.408875 kondo_ml-0.0.9/setup.cfg
+-rw-r--r--   0 rueck      (501) staff       (20)     1619 2023-04-17 10:55:31.000000 kondo_ml-0.0.9/setup.py
```

### Comparing `kondo_ml-0.0.8/LICENSE` & `kondo_ml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/PKG-INFO` & `kondo_ml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kondo_ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.8.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.9.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `kondo_ml-0.0.8/kondo_ml/__init__.py` & `kondo_ml-0.0.9/kondo_ml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from kondo_ml.kondo_ml import KondoMLPackage
 
 __author__ = "Lukas Rücker"
 __email__ = "ruecker.lukas@gmail.com"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # module level doc-string
 __doc__ = """
 Kondo-ML
 ================
 
 Description
```

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/datasets.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/datasets.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/linear.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/linear.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/LinearRegression.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/model/SELCON.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/model/SELCON.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/SELCON/utils/time_series.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/SELCON/utils/time_series.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/__init__.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_drop.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_drop.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_fish.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_fish.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_fixed_time_window.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_fixed_time_window.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_full_set.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_full_set.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_gradient_shapley.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_gradient_shapley.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_local_outlier_factor.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_local_outlier_factor.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_mutual_information.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_mutual_information.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_random_selection.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_random_selection.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_reg_CNN.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_reg_CNN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_reg_ENN.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_reg_ENN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/_selcon.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/_selcon.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/instance_selection/base.py` & `kondo_ml-0.0.9/kondo_ml/instance_selection/base.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml/utils.py` & `kondo_ml-0.0.9/kondo_ml/utils.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/kondo_ml.egg-info/PKG-INFO` & `kondo_ml-0.0.9/kondo_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kondo-ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.8.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.9.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `kondo_ml-0.0.8/kondo_ml.egg-info/SOURCES.txt` & `kondo_ml-0.0.9/kondo_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.8/pyproject.toml` & `kondo_ml-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kondo_ml"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Lukas Rücker", email="ruecker.lukas@gmail.com" },
 ]
 description = "Python package for instance selection algorithms"
 readme = "README.md"
-dependencies = ['numpy','pandas','scikit-learn','torch']
+dependencies = ['numpy','pandas','scikit-learn','torch','mutual_info']
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `kondo_ml-0.0.8/setup.py` & `kondo_ml-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-    install_requires=["numpy", "pandas", "scikit-learn", "torch"],  # Dependencies
+    install_requires=["numpy", "pandas", "scikit-learn", "torch","mutual_info"],  # Dependencies
     python_requires=">=3.10",  # Minimum Python version
     name="kondo_ml",  # Package name
     version=new_version,  # Version
     author="L.Rücker",  # Author name
     author_email="ruecker.lukas@gmail.com",  # Author mail
     description="Python package for instance selection algorithms",  # Short package description
     long_description=long_description,  # Long package description
```

