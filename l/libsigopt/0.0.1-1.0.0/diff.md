# Comparing `tmp/libsigopt-0.0.1.tar.gz` & `tmp/libsigopt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsigopt-0.0.1.tar", last modified: Fri Apr 14 20:21:09 2023, max compression
+gzip compressed data, was "libsigopt-1.0.0.tar", last modified: Tue Apr 18 18:07:45 2023, max compression
```

## Comparing `libsigopt-0.0.1.tar` & `libsigopt-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,63 @@
-drwxr-xr-x   0 dwanders   (503) staff       (20)        0 2023-04-14 20:21:09.850787 libsigopt-0.0.1/
--rw-r--r--   0 dwanders   (503) staff       (20)      506 2023-04-14 20:21:09.850478 libsigopt-0.0.1/PKG-INFO
-drwxr-xr-x   0 dwanders   (503) staff       (20)        0 2023-04-14 20:21:09.850082 libsigopt-0.0.1/libsigopt.egg-info/
--rw-r--r--   0 dwanders   (503) staff       (20)      506 2023-04-14 20:21:09.000000 libsigopt-0.0.1/libsigopt.egg-info/PKG-INFO
--rw-r--r--   0 dwanders   (503) staff       (20)      140 2023-04-14 20:21:09.000000 libsigopt-0.0.1/libsigopt.egg-info/SOURCES.txt
--rw-r--r--   0 dwanders   (503) staff       (20)        1 2023-04-14 20:21:09.000000 libsigopt-0.0.1/libsigopt.egg-info/dependency_links.txt
--rw-r--r--   0 dwanders   (503) staff       (20)        1 2023-04-14 20:21:09.000000 libsigopt-0.0.1/libsigopt.egg-info/top_level.txt
--rw-r--r--   0 dwanders   (503) staff       (20)       38 2023-04-14 20:21:09.850890 libsigopt-0.0.1/setup.cfg
--rw-r--r--   0 dwanders   (503) staff       (20)     1821 2023-04-14 20:19:29.000000 libsigopt-0.0.1/setup.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.113786 libsigopt-1.0.0/
+-rw-r--r--   0 sahowey    (502) staff       (20)    11347 2023-04-14 17:54:05.000000 libsigopt-1.0.0/LICENSE
+-rw-r--r--   0 sahowey    (502) staff       (20)      328 2023-04-18 18:07:45.113987 libsigopt-1.0.0/PKG-INFO
+-rw-r--r--   0 sahowey    (502) staff       (20)     1488 2023-04-14 17:54:05.000000 libsigopt-1.0.0/README.md
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.045828 libsigopt-1.0.0/libsigopt/
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.066012 libsigopt-1.0.0/libsigopt/aux/
+-rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/__init__.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1408 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/adapter_info_containers.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     2810 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/constant.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1556 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/errors.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1518 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/geometry_utils.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1542 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/multimetric.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     6642 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/samplers.py
+-rw-r--r--   0 sahowey    (502) staff       (20)      482 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/utils.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     3312 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/aux/validate_schema.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.093404 libsigopt-1.0.0/libsigopt/compute/
+-rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/__init__.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     2431 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/acquisition_function.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     9764 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/acquisition_function_optimization.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     7195 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/covariance.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    13250 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/covariance_base.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    43726 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/domain.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    21659 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/expected_improvement.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    13583 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/gaussian_process.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     6693 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/gaussian_process_sum.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     6971 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/log_likelihood.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.098620 libsigopt-1.0.0/libsigopt/compute/misc/
+-rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/misc/__init__.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     2589 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/misc/constant.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     6968 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/misc/data_containers.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    21711 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/misc/multimetric.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1677 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/multitask_acquisition_function.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     8117 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/multitask_covariance.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    10759 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/optimization.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     2390 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/optimization_auxiliary.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     3101 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/predictor.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     8221 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/probabilistic_failures.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     7117 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/python_utils.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     5481 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/search.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     7044 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/sigopt_parzen_estimator.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     9234 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/compute/vectorized_optimizers.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.102181 libsigopt-1.0.0/libsigopt/views/
+-rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/__init__.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.113069 libsigopt-1.0.0/libsigopt/views/rest/
+-rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/__init__.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1739 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/gp_ei_categorical.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     8227 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/gp_hyper_opt_multimetric.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    14887 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/gp_next_points_categorical.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     2372 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/multisolution_best_assignments.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1205 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/random_search_next_points.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     7630 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/search_next_points.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    15202 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/spe_next_points.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     5487 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/rest/spe_search_next_points.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    20677 2023-04-14 17:54:05.000000 libsigopt-1.0.0/libsigopt/views/view.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:07:45.057386 libsigopt-1.0.0/libsigopt.egg-info/
+-rw-r--r--   0 sahowey    (502) staff       (20)      328 2023-04-18 18:07:45.000000 libsigopt-1.0.0/libsigopt.egg-info/PKG-INFO
+-rw-r--r--   0 sahowey    (502) staff       (20)     1874 2023-04-18 18:07:45.000000 libsigopt-1.0.0/libsigopt.egg-info/SOURCES.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)        1 2023-04-18 18:07:45.000000 libsigopt-1.0.0/libsigopt.egg-info/dependency_links.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)       69 2023-04-18 18:07:45.000000 libsigopt-1.0.0/libsigopt.egg-info/requires.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)       10 2023-04-18 18:07:45.000000 libsigopt-1.0.0/libsigopt.egg-info/top_level.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)      588 2023-04-14 17:54:05.000000 libsigopt-1.0.0/pyproject.toml
+-rw-r--r--   0 sahowey    (502) staff       (20)       69 2023-04-14 17:54:05.000000 libsigopt-1.0.0/requirements.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)      655 2023-04-18 18:07:45.115014 libsigopt-1.0.0/setup.cfg
```

