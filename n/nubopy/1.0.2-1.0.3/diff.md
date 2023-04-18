# Comparing `tmp/nubopy-1.0.2.tar.gz` & `tmp/nubopy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nubopy-1.0.2.tar", last modified: Tue Apr 18 17:11:26 2023, max compression
+gzip compressed data, was "nubopy-1.0.3.tar", last modified: Tue Apr 18 17:15:33 2023, max compression
```

## Comparing `nubopy-1.0.2.tar` & `nubopy-1.0.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.318418 nubopy-1.0.2/
--rw-r--r--   0 mikediessner   (501) staff       (20)     1500 2023-03-16 09:32:23.000000 nubopy-1.0.2/LICENSE.md
--rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:11:26.318270 nubopy-1.0.2/PKG-INFO
--rw-r--r--   0 mikediessner   (501) staff       (20)     1683 2023-04-05 15:30:35.000000 nubopy-1.0.2/README.md
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.285482 nubopy-1.0.2/nubo/
--rw-r--r--   0 mikediessner   (501) staff       (20)       94 2023-02-28 09:35:10.000000 nubopy-1.0.2/nubo/__init__.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.287361 nubopy-1.0.2/nubo/acquisition/
--rw-r--r--   0 mikediessner   (501) staff       (20)      136 2023-03-07 13:05:46.000000 nubopy-1.0.2/nubo/acquisition/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1014 2023-03-30 17:33:30.000000 nubopy-1.0.2/nubo/acquisition/acquisition_function.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     4436 2023-04-06 08:23:23.000000 nubopy-1.0.2/nubo/acquisition/analytical.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     9239 2023-04-04 09:43:08.000000 nubopy-1.0.2/nubo/acquisition/monte_carlo.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.288750 nubopy-1.0.2/nubo/models/
--rw-r--r--   0 mikediessner   (501) staff       (20)       70 2023-03-03 10:04:54.000000 nubopy-1.0.2/nubo/models/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1833 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/models/fit.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2764 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/models/gaussian_process.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.294917 nubopy-1.0.2/nubo/optimisation/
--rw-r--r--   0 mikediessner   (501) staff       (20)      232 2023-03-31 10:52:35.000000 nubopy-1.0.2/nubo/optimisation/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     8268 2023-04-03 12:42:29.000000 nubopy-1.0.2/nubo/optimisation/adam.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2285 2023-04-03 12:42:54.000000 nubopy-1.0.2/nubo/optimisation/lbfgsb.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     3475 2023-04-03 12:42:41.000000 nubopy-1.0.2/nubo/optimisation/mixed.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     6995 2023-04-03 12:47:24.000000 nubopy-1.0.2/nubo/optimisation/multipoint.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2717 2023-04-18 16:22:14.000000 nubopy-1.0.2/nubo/optimisation/singlepoint.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2432 2023-04-03 12:47:44.000000 nubopy-1.0.2/nubo/optimisation/slsqp.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1325 2023-04-03 12:49:09.000000 nubopy-1.0.2/nubo/optimisation/utils.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.299525 nubopy-1.0.2/nubo/test_functions/
--rw-r--r--   0 mikediessner   (501) staff       (20)      359 2023-02-28 09:35:10.000000 nubopy-1.0.2/nubo/test_functions/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2800 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/ackley.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2530 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/dixonprice.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2419 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/griewank.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     7953 2023-03-29 09:52:55.000000 nubopy-1.0.2/nubo/test_functions/hartmann.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2661 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/levy.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2319 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/rastrigin.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2345 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/schwefel.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2217 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/sphere.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2276 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/sumsquares.py
--rw-r--r--   0 mikediessner   (501) staff       (20)      291 2023-03-08 10:27:07.000000 nubopy-1.0.2/nubo/test_functions/test_functions.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2440 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/test_functions/zakharov.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.307085 nubopy-1.0.2/nubo/utils/
--rw-r--r--   0 mikediessner   (501) staff       (20)      151 2023-03-14 10:12:07.000000 nubopy-1.0.2/nubo/utils/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1164 2023-03-16 09:32:23.000000 nubopy-1.0.2/nubo/utils/generate_inputs.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     3359 2023-03-29 09:52:55.000000 nubopy-1.0.2/nubo/utils/latin_hypercube.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1818 2023-03-23 09:40:34.000000 nubopy-1.0.2/nubo/utils/transform.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.311917 nubopy-1.0.2/nubopy.egg-info/
--rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:11:26.000000 nubopy-1.0.2/nubopy.egg-info/PKG-INFO
--rw-r--r--   0 mikediessner   (501) staff       (20)     1227 2023-04-18 17:11:26.000000 nubopy-1.0.2/nubopy.egg-info/SOURCES.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)        1 2023-04-18 17:11:26.000000 nubopy-1.0.2/nubopy.egg-info/dependency_links.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)        5 2023-04-18 17:11:26.000000 nubopy-1.0.2/nubopy.egg-info/top_level.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)      537 2023-04-18 17:11:07.000000 nubopy-1.0.2/pyproject.toml
--rw-r--r--   0 mikediessner   (501) staff       (20)       38 2023-04-18 17:11:26.318452 nubopy-1.0.2/setup.cfg
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:11:26.316956 nubopy-1.0.2/tests/
--rw-r--r--   0 mikediessner   (501) staff       (20)    16878 2023-03-29 11:44:07.000000 nubopy-1.0.2/tests/test_acquisition.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2876 2023-03-29 09:52:55.000000 nubopy-1.0.2/tests/test_models.py
--rw-r--r--   0 mikediessner   (501) staff       (20)    22786 2023-03-31 10:16:55.000000 nubopy-1.0.2/tests/test_optimisation.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     9449 2023-03-29 09:52:55.000000 nubopy-1.0.2/tests/test_test_functions.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     4123 2023-03-29 09:52:55.000000 nubopy-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.674484 nubopy-1.0.3/
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1500 2023-03-16 09:32:23.000000 nubopy-1.0.3/LICENSE.md
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:15:33.674281 nubopy-1.0.3/PKG-INFO
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1683 2023-04-05 15:30:35.000000 nubopy-1.0.3/README.md
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.644530 nubopy-1.0.3/nubo/
+-rw-r--r--   0 mikediessner   (501) staff       (20)       94 2023-02-28 09:35:10.000000 nubopy-1.0.3/nubo/__init__.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.646615 nubopy-1.0.3/nubo/acquisition/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      136 2023-03-07 13:05:46.000000 nubopy-1.0.3/nubo/acquisition/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1014 2023-03-30 17:33:30.000000 nubopy-1.0.3/nubo/acquisition/acquisition_function.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     4436 2023-04-06 08:23:23.000000 nubopy-1.0.3/nubo/acquisition/analytical.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     9239 2023-04-04 09:43:08.000000 nubopy-1.0.3/nubo/acquisition/monte_carlo.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.648111 nubopy-1.0.3/nubo/models/
+-rw-r--r--   0 mikediessner   (501) staff       (20)       70 2023-03-03 10:04:54.000000 nubopy-1.0.3/nubo/models/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1833 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/models/fit.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2764 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/models/gaussian_process.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.656055 nubopy-1.0.3/nubo/optimisation/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      232 2023-03-31 10:52:35.000000 nubopy-1.0.3/nubo/optimisation/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     8268 2023-04-03 12:42:29.000000 nubopy-1.0.3/nubo/optimisation/adam.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2285 2023-04-03 12:42:54.000000 nubopy-1.0.3/nubo/optimisation/lbfgsb.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     3475 2023-04-03 12:42:41.000000 nubopy-1.0.3/nubo/optimisation/mixed.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     6995 2023-04-03 12:47:24.000000 nubopy-1.0.3/nubo/optimisation/multipoint.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2717 2023-04-18 16:22:14.000000 nubopy-1.0.3/nubo/optimisation/singlepoint.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2432 2023-04-03 12:47:44.000000 nubopy-1.0.3/nubo/optimisation/slsqp.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1325 2023-04-03 12:49:09.000000 nubopy-1.0.3/nubo/optimisation/utils.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.667461 nubopy-1.0.3/nubo/test_functions/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      359 2023-02-28 09:35:10.000000 nubopy-1.0.3/nubo/test_functions/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2800 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/ackley.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2530 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/dixonprice.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2419 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/griewank.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     7953 2023-03-29 09:52:55.000000 nubopy-1.0.3/nubo/test_functions/hartmann.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2661 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/levy.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2319 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/rastrigin.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2345 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/schwefel.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2217 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/sphere.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2276 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/sumsquares.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)      291 2023-03-08 10:27:07.000000 nubopy-1.0.3/nubo/test_functions/test_functions.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2440 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/zakharov.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.669450 nubopy-1.0.3/nubo/utils/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      151 2023-03-14 10:12:07.000000 nubopy-1.0.3/nubo/utils/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1164 2023-03-16 09:32:23.000000 nubopy-1.0.3/nubo/utils/generate_inputs.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     3359 2023-03-29 09:52:55.000000 nubopy-1.0.3/nubo/utils/latin_hypercube.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1818 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/utils/transform.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.671485 nubopy-1.0.3/nubopy.egg-info/
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/PKG-INFO
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1256 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/SOURCES.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)        1 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/dependency_links.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)       27 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/requires.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)        5 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/top_level.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)      553 2023-04-18 17:15:26.000000 nubopy-1.0.3/pyproject.toml
+-rw-r--r--   0 mikediessner   (501) staff       (20)       38 2023-04-18 17:15:33.674520 nubopy-1.0.3/setup.cfg
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.673868 nubopy-1.0.3/tests/
+-rw-r--r--   0 mikediessner   (501) staff       (20)    16878 2023-03-29 11:44:07.000000 nubopy-1.0.3/tests/test_acquisition.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2876 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_models.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)    22786 2023-03-31 10:16:55.000000 nubopy-1.0.3/tests/test_optimisation.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     9449 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_test_functions.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     4123 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_utils.py
```

### Comparing `nubopy-1.0.2/LICENSE.md` & `nubopy-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/PKG-INFO` & `nubopy-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nubopy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A transparent Python package for Bayesian optimisation
 Author-email: Mike Diessner <m.diessner2@ncl.ac.uk>
 Project-URL: Homepage, https://mikediessner.github.io/nubo
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `nubopy-1.0.2/README.md` & `nubopy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/acquisition/acquisition_function.py` & `nubopy-1.0.3/nubo/acquisition/acquisition_function.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/acquisition/analytical.py` & `nubopy-1.0.3/nubo/acquisition/analytical.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/acquisition/monte_carlo.py` & `nubopy-1.0.3/nubo/acquisition/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/models/fit.py` & `nubopy-1.0.3/nubo/models/fit.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/models/gaussian_process.py` & `nubopy-1.0.3/nubo/models/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/adam.py` & `nubopy-1.0.3/nubo/optimisation/adam.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/lbfgsb.py` & `nubopy-1.0.3/nubo/optimisation/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/mixed.py` & `nubopy-1.0.3/nubo/optimisation/mixed.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/multipoint.py` & `nubopy-1.0.3/nubo/optimisation/multipoint.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/singlepoint.py` & `nubopy-1.0.3/nubo/optimisation/singlepoint.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/slsqp.py` & `nubopy-1.0.3/nubo/optimisation/slsqp.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/optimisation/utils.py` & `nubopy-1.0.3/nubo/optimisation/utils.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/ackley.py` & `nubopy-1.0.3/nubo/test_functions/ackley.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/dixonprice.py` & `nubopy-1.0.3/nubo/test_functions/dixonprice.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/griewank.py` & `nubopy-1.0.3/nubo/test_functions/griewank.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/hartmann.py` & `nubopy-1.0.3/nubo/test_functions/hartmann.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/levy.py` & `nubopy-1.0.3/nubo/test_functions/levy.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/rastrigin.py` & `nubopy-1.0.3/nubo/test_functions/rastrigin.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/schwefel.py` & `nubopy-1.0.3/nubo/test_functions/schwefel.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/sphere.py` & `nubopy-1.0.3/nubo/test_functions/sphere.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/sumsquares.py` & `nubopy-1.0.3/nubo/test_functions/sumsquares.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/test_functions/zakharov.py` & `nubopy-1.0.3/nubo/test_functions/zakharov.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/utils/generate_inputs.py` & `nubopy-1.0.3/nubo/utils/generate_inputs.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/utils/latin_hypercube.py` & `nubopy-1.0.3/nubo/utils/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubo/utils/transform.py` & `nubopy-1.0.3/nubo/utils/transform.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/nubopy.egg-info/PKG-INFO` & `nubopy-1.0.3/nubopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nubopy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A transparent Python package for Bayesian optimisation
 Author-email: Mike Diessner <m.diessner2@ncl.ac.uk>
 Project-URL: Homepage, https://mikediessner.github.io/nubo
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `nubopy-1.0.2/nubopy.egg-info/SOURCES.txt` & `nubopy-1.0.3/nubopy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,14 @@
 nubo/utils/__init__.py
 nubo/utils/generate_inputs.py
 nubo/utils/latin_hypercube.py
 nubo/utils/transform.py
 nubopy.egg-info/PKG-INFO
 nubopy.egg-info/SOURCES.txt
 nubopy.egg-info/dependency_links.txt
+nubopy.egg-info/requires.txt
 nubopy.egg-info/top_level.txt
 tests/test_acquisition.py
 tests/test_models.py
 tests/test_optimisation.py
 tests/test_test_functions.py
 tests/test_utils.py
```

### Comparing `nubopy-1.0.2/pyproject.toml` & `nubopy-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
-requires = ["setuptools", "torch", "gpytorch", "scipy", "numpy"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nubopy"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Mike Diessner", email="m.diessner2@ncl.ac.uk" },
 ]
 description = "A transparent Python package for Bayesian optimisation"
 readme = "README.md"
 requires-python = ">=3.7"
+dependencies = ["torch", "gpytorch", "scipy", "numpy"]
 classifiers = [
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
 "Homepage" = "https://mikediessner.github.io/nubo"
```

### Comparing `nubopy-1.0.2/tests/test_acquisition.py` & `nubopy-1.0.3/tests/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/tests/test_models.py` & `nubopy-1.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/tests/test_optimisation.py` & `nubopy-1.0.3/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/tests/test_test_functions.py` & `nubopy-1.0.3/tests/test_test_functions.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.2/tests/test_utils.py` & `nubopy-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

