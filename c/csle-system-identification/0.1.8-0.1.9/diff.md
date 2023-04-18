# Comparing `tmp/csle_system_identification-0.1.8.tar.gz` & `tmp/csle_system_identification-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.1.8.tar", last modified: Mon Mar 20 15:27:45 2023, max compression
+gzip compressed data, was "csle_system_identification-0.1.9.tar", last modified: Tue Mar 21 08:09:42 2023, max compression
```

## Comparing `csle_system_identification-0.1.8.tar` & `csle_system_identification-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.498621 csle_system_identification-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-03-20 15:27:45.498755 csle_system_identification-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4235 2023-01-11 18:45:47.000000 csle_system_identification-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      686 2023-02-12 08:59:32.000000 csle_system_identification-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1340 2023-03-20 15:27:45.499421 csle_system_identification-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.485827 csle_system_identification-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.489199 csle_system_identification-0.1.8/src/csle_system_identification/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_system_identification-0.1.8/src/csle_system_identification/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.492301 csle_system_identification-0.1.8/src/csle_system_identification/base/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2074 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.493306 csle_system_identification-0.1.8/src/csle_system_identification/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      688 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.494191 csle_system_identification-0.1.8/src/csle_system_identification/empirical/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/empirical/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     7135 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-r--r--   0 kimham     (501) staff       (20)    12807 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/emulator.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.494888 csle_system_identification-0.1.8/src/csle_system_identification/expectation_maximization/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/expectation_maximization/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     7380 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.496173 csle_system_identification-0.1.8/src/csle_system_identification/gp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/gp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     9700 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/gp/gp_regression_algorithm.py
--rw-r--r--   0 kimham     (501) staff       (20)      555 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.498226 csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2159 2022-12-07 07:23:42.000000 csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     2212 2022-11-28 13:00:49.000000 csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:27:45.491837 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-03-20 15:27:45.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     1412 2023-03-20 15:27:45.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:27:45.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:48.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      257 2023-03-20 15:27:45.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       27 2023-03-20 15:27:45.000000 csle_system_identification-0.1.8/src/csle_system_identification.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4235 2023-01-03 16:53:42.000000 csle_system_identification-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-02-11 20:28:41.000000 csle_system_identification-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1340 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_system_identification-0.1.9/src/csle_system_identification/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2074 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      688 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/empirical/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/empirical/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7135 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12807 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/emulator.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7380 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/gp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9700 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      555 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2022-12-03 16:48:17.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1412 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      257 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       27 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/top_level.txt
```

### Comparing `csle_system_identification-0.1.8/PKG-INFO` & `csle_system_identification-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.1.8/README.md` & `csle_system_identification-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/pyproject.toml` & `csle_system_identification-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/setup.cfg` & `csle_system_identification-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.8
-	csle-collector>=0.1.8
-	csle-attacker>=0.1.8
-	csle-defender>=0.1.8
+	csle-common>=0.1.9
+	csle-collector>=0.1.9
+	csle-attacker>=0.1.9
+	csle-defender>=0.1.9
 	gpytorch>=1.9.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
```

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.1.9/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.1.9/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.1.9/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/emulator.py` & `csle_system_identification-0.1.9/src/csle_system_identification/emulator.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py` & `csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.1.9/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.1.8/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.1.9/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

