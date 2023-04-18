# Comparing `tmp/sigoptlite-0.1.1.tar.gz` & `tmp/sigoptlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigoptlite-0.1.1.tar", last modified: Wed Mar 29 22:30:54 2023, max compression
+gzip compressed data, was "sigoptlite-0.1.2.tar", last modified: Tue Apr 18 18:21:51 2023, max compression
```

## Comparing `sigoptlite-0.1.1.tar` & `sigoptlite-0.1.2.tar`

### file list

```diff
@@ -1,65 +1,30 @@
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.699959 sigoptlite-0.1.1/
--rw-r--r--   0 sahowey    (502) staff       (20)      293 2023-03-29 22:30:54.700117 sigoptlite-0.1.1/PKG-INFO
--rw-r--r--   0 sahowey    (502) staff       (20)     5984 2023-03-28 22:09:08.000000 sigoptlite-0.1.1/README.md
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.677426 sigoptlite-0.1.1/lite_sigoptaux/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1408 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/adapter_info_containers.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2806 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/constant.py
--rw-r--r--   0 sahowey    (502) staff       (20)    43446 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/domain.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1518 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/geometry_utils.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1472 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/importances.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1518 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/multimetric.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6643 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/lite_sigoptaux/samplers.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.687177 sigoptlite-0.1.1/lite_sigoptcompute/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2432 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/acquisition_function.py
--rw-r--r--   0 sahowey    (502) staff       (20)     9767 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/acquisition_function_optimization.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7093 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/covariance.py
--rw-r--r--   0 sahowey    (502) staff       (20)    13260 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/covariance_base.py
--rw-r--r--   0 sahowey    (502) staff       (20)    23077 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/expected_improvement.py
--rw-r--r--   0 sahowey    (502) staff       (20)    13596 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/gaussian_process.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6653 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/gaussian_process_sum.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6941 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/log_likelihood.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.689333 sigoptlite-0.1.1/lite_sigoptcompute/misc/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/misc/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2585 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/misc/constant.py
--rw-r--r--   0 sahowey    (502) staff       (20)     6917 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/misc/data_containers.py
--rw-r--r--   0 sahowey    (502) staff       (20)    21649 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/misc/multimetric.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1678 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/multitask_acquisition_function.py
--rw-r--r--   0 sahowey    (502) staff       (20)     8108 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/multitask_covariance.py
--rw-r--r--   0 sahowey    (502) staff       (20)    10761 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/optimization.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2390 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/optimization_auxiliary.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3058 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/predictor.py
--rw-r--r--   0 sahowey    (502) staff       (20)     8222 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/probabilistic_failures.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7106 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/python_utils.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5483 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/search.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7054 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/sigopt_parzen_estimator.py
--rw-r--r--   0 sahowey    (502) staff       (20)     9101 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/vectorized_optimizers.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.690172 sigoptlite-0.1.1/lite_sigoptcompute/views/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/__init__.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.693761 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/
--rw-r--r--   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     1772 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/gp_ei_categorical.py
--rw-r--r--   0 sahowey    (502) staff       (20)     8187 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/gp_hyper_opt_multimetric.py
--rw-r--r--   0 sahowey    (502) staff       (20)    14914 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/gp_next_points_categorical.py
--rw-r--r--   0 sahowey    (502) staff       (20)     2384 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/multisolution_best_assignments.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7652 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/search_next_points.py
--rw-r--r--   0 sahowey    (502) staff       (20)    15229 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/spe_next_points.py
--rw-r--r--   0 sahowey    (502) staff       (20)     5516 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/rest/spe_search_next_points.py
--rw-r--r--   0 sahowey    (502) staff       (20)    20705 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/lite_sigoptcompute/views/view.py
--rw-r--r--   0 sahowey    (502) staff       (20)       81 2023-03-29 19:01:51.000000 sigoptlite-0.1.1/pyproject.toml
--rw-r--r--   0 sahowey    (502) staff       (20)      511 2023-03-29 22:30:54.700847 sigoptlite-0.1.1/setup.cfg
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.697076 sigoptlite-0.1.1/sigoptlite/
--rw-r--r--   0 sahowey    (502) staff       (20)      118 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/sigoptlite/__init__.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3730 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/sigoptlite/best_assignments.py
--rw-r--r--   0 sahowey    (502) staff       (20)     3730 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/sigoptlite/broker.py
--rw-r--r--   0 sahowey    (502) staff       (20)    33390 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/sigoptlite/builders.py
--rw-r--r--   0 sahowey    (502) staff       (20)     4695 2023-03-29 22:30:46.000000 sigoptlite-0.1.1/sigoptlite/driver.py
--rw-r--r--   0 sahowey    (502) staff       (20)     7523 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/sigoptlite/models.py
--rw-r--r--   0 sahowey    (502) staff       (20)    17763 2023-03-29 22:30:45.000000 sigoptlite-0.1.1/sigoptlite/sources.py
-drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-03-29 22:30:54.699623 sigoptlite-0.1.1/sigoptlite.egg-info/
--rw-r--r--   0 sahowey    (502) staff       (20)      293 2023-03-29 22:30:54.000000 sigoptlite-0.1.1/sigoptlite.egg-info/PKG-INFO
--rw-r--r--   0 sahowey    (502) staff       (20)     2032 2023-03-29 22:30:54.000000 sigoptlite-0.1.1/sigoptlite.egg-info/SOURCES.txt
--rw-r--r--   0 sahowey    (502) staff       (20)        1 2023-03-29 22:30:54.000000 sigoptlite-0.1.1/sigoptlite.egg-info/dependency_links.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       57 2023-03-29 22:30:54.000000 sigoptlite-0.1.1/sigoptlite.egg-info/requires.txt
--rw-r--r--   0 sahowey    (502) staff       (20)       45 2023-03-29 22:30:54.000000 sigoptlite-0.1.1/sigoptlite.egg-info/top_level.txt
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:21:51.336054 sigoptlite-0.1.2/
+-rw-r--r--   0 sahowey    (502) staff       (20)    11347 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/LICENSE
+-rw-r--r--   0 sahowey    (502) staff       (20)      315 2023-04-18 18:21:51.336252 sigoptlite-0.1.2/PKG-INFO
+-rw-r--r--   0 sahowey    (502) staff       (20)     6010 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/README.md
+-rw-r--r--   0 sahowey    (502) staff       (20)      612 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/pyproject.toml
+-rw-r--r--   0 sahowey    (502) staff       (20)       34 2023-04-18 18:11:27.000000 sigoptlite-0.1.2/requirements.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)      611 2023-04-18 18:21:51.337103 sigoptlite-0.1.2/setup.cfg
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:21:51.322979 sigoptlite-0.1.2/sigoptlite/
+-rw-r--r--   0 sahowey    (502) staff       (20)      118 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/__init__.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     3729 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/best_assignments.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     4187 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/broker.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     9661 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/builders.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     4695 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/driver.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     7800 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/models.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    17560 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/sources.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    22605 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/sigoptlite/validators.py
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:21:51.327595 sigoptlite-0.1.2/sigoptlite.egg-info/
+-rw-r--r--   0 sahowey    (502) staff       (20)      315 2023-04-18 18:21:51.000000 sigoptlite-0.1.2/sigoptlite.egg-info/PKG-INFO
+-rw-r--r--   0 sahowey    (502) staff       (20)      565 2023-04-18 18:21:51.000000 sigoptlite-0.1.2/sigoptlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)        1 2023-04-18 18:21:51.000000 sigoptlite-0.1.2/sigoptlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)       34 2023-04-18 18:21:51.000000 sigoptlite-0.1.2/sigoptlite.egg-info/requires.txt
+-rw-r--r--   0 sahowey    (502) staff       (20)       11 2023-04-18 18:21:51.000000 sigoptlite-0.1.2/sigoptlite.egg-info/top_level.txt
+drwxr-xr-x   0 sahowey    (502) staff       (20)        0 2023-04-18 18:21:51.335383 sigoptlite-0.1.2/test/
+-rw-r--r--   0 sahowey    (502) staff       (20)    18391 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_adapter.py
+-rw-r--r--   0 sahowey    (502) staff       (20)      834 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_broker.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    12701 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_builders.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     3778 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_compute_mode.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     1612 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_driver.py
+-rw-r--r--   0 sahowey    (502) staff       (20)    14788 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_models.py
+-rw-r--r--   0 sahowey    (502) staff       (20)     3944 2023-04-13 17:33:17.000000 sigoptlite-0.1.2/test/test_sources.py
```

### Comparing `sigoptlite-0.1.1/README.md` & `sigoptlite-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Copyright © 2023 Intel Corporation
 
 SPDX-License-Identifier: Apache License 2.0
 -->
 
 # SigOpt-Lite
 
-SigOpt-Lite is an open source tool for locally running a lightweight version of [SigOpt](https://www.sigopt.com). Sigopt-Lite contains all the computation elements of SigOpt-Server, but bypasses the need to set up servers and Docker. SigOpt-Lite gives access to the SigOpt Core Module functionality; to learn more about that, visit the [SigOpt documentation](https://docs.sigopt.com/intro/sigopt-api-modules). To learn about how to host your own SigOpt server, visit our [SigOpt-Server documentation](../#README.md) or [the official SigOpt OSS site (sigopt.org)](https://sigopt.org/).
+SigOpt-Lite is an open source tool for locally running a lightweight version of [SigOpt](https://www.sigopt.com). Sigopt-Lite contains all the computation elements of SigOpt-Server, but bypasses the need to set up servers and Docker. SigOpt-Lite gives access to the SigOpt Core Module functionality; to learn more about that, visit the [SigOpt documentation](https://docs.sigopt.com/intro/sigopt-api-modules). To learn about how to host your own SigOpt server, visit the [SigOpt-Server repository](https://github.com/sigopt/sigopt-server) or [the official SigOpt OSS site (sigopt.org)](https://sigopt.org/).
 
 ## Installation
 
 Executing the following command will install both the `sigopt` client (to interact with SigOpt) and the `sigoptlite` driver (to run the computations locally).
 
 ```bash
 pip install 'sigopt[lite]'
@@ -36,15 +36,15 @@
   parameters=[
     dict(name="x0", type="double", bounds=dict(min=0, max=1)),
     dict(name="x1", type="int", bounds=dict(min=0, max=10)),
   ],
   metrics=[
     dict(
       name="f",
-      objective="mimize",
+      objective="minimize",
     )
   ],
   observation_budget=20,
 )
 e = conn.experiments().create(**experiment_meta)
 suggestion = conn.experiments(e.id).suggestions().create()
 conn.experiments(e.id).observations().create(
@@ -83,15 +83,15 @@
 
 ### Limitations
 
 The following behavior limitations are strictly enforced in SigOpt-Lite.
 
 - SigOpt-Lite can only run one Experiment at a time: the Experiment ID for the sole experiment is `"-1"`.
 - SigOpt-Lite supports no [parallelism](https://docs.sigopt.com/advanced_experimentation/parallelism): an observation must be reported for the open suggestion before creating another unique suggestion. Parallel suggestions can be accessed through an account at [sigopt.com](https://app.sigopt.com/signup) or through the open source SigOpt-Server.
-- SigOpt-Lite does not support [Grid Searh](https://docs.sigopt.com/intro/main-concepts/random_search#grid-search).
+- SigOpt-Lite does not support [Grid Search](https://docs.sigopt.com/intro/main-concepts/random_search#grid-search).
 
 ### Recommended Limitations
 
 The following set of soft limitations are recommended by the SigOpt research team to ensure a pleasant experience using SigOpt-Lite.
 
 - Maximum number of parameters <= 100
 - Maximum number of observations <= 10,000
```

### Comparing `sigoptlite-0.1.1/lite_sigoptcompute/views/view.py` & `sigoptlite-0.1.2/test/test_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,508 +1,411 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: Apache License 2.0
-import logging
-from dataclasses import asdict
-
 import numpy
+import pytest
 
-from lite_sigoptcompute.covariance import COVARIANCE_TYPES_TO_CLASSES
-from lite_sigoptcompute.expected_improvement import (
-  AugmentedExpectedImprovement,
-  ExpectedImprovement,
-  ExpectedImprovementWithFailures,
-  ExpectedParallelImprovement,
-  ExpectedParallelImprovementWithFailures,
-)
-from lite_sigoptcompute.gaussian_process import GaussianProcess
-from lite_sigoptcompute.gaussian_process_sum import GaussianProcessSum
-from lite_sigoptcompute.misc.constant import (
-  CONSTANT_LIAR_MIN,
-  DEFAULT_CONSTANT_LIAR_LIE_NOISE_VARIANCE,
-  DEFAULT_COVARIANCE_KERNEL,
-  DEFAULT_TASK_COVARIANCE_KERNEL,
-)
-from lite_sigoptcompute.misc.data_containers import HistoricalData, MultiMetricMidpointInfo, SingleMetricMidpointInfo
-from lite_sigoptcompute.misc.multimetric import (
-  CONVEX_COMBINATION,
-  EPSILON_CONSTRAINT,
-  MULTIMETRIC_INFO_NOT_MULTIMETRIC,
-  PROBABILISTIC_FAILURES,
-  filter_multimetric_points_sampled,
-  find_epsilon_constraint_value,
-  form_multimetric_info_from_phase,
-  identify_multimetric_phase,
-)
-from lite_sigoptcompute.multitask_covariance import MultitaskTensorCovariance
-from lite_sigoptcompute.probabilistic_failures import (
-  ProbabilisticFailures,
-  ProbabilisticFailuresCDF,
-  ProductOfListOfProbabilisticFailures,
+from libsigopt.aux.adapter_info_containers import DomainInfo
+from libsigopt.aux.constant import (
+  CATEGORICAL_EXPERIMENT_PARAMETER_NAME,
+  DOUBLE_EXPERIMENT_PARAMETER_NAME,
+  INT_EXPERIMENT_PARAMETER_NAME,
+  MULTISOLUTION_QUANTILE_FOR_SEARCH_THRESHOLD,
+  QUANTIZED_EXPERIMENT_PARAMETER_NAME,
+  ParameterPriorNames,
 )
-from lite_sigoptcompute.python_utils import validate_polynomial_indices
 
-from lite_sigoptaux.adapter_info_containers import GPModelInfo
-from lite_sigoptaux.constant import PARALLEL_CONSTANT_LIAR
-from lite_sigoptaux.domain import CategoricalDomain
-
-
-_UNSET = object()
-# Level of noise at which Augmented Expected Improvement should be used
-AUGMENTED_EI_THRESHOLD = 1e-7
-
-
-def filter_points_sampled(points_sampled, metrics_info):
-  optimized_metrics_index = numpy.asarray(metrics_info.optimized_metrics_index)
-  has_optimization_metrics = metrics_info.has_optimization_metrics
-  has_constraint_metrics = metrics_info.has_constraint_metrics
-  constraint_metrics_index = False
-  if has_constraint_metrics:
-    constraint_metrics_index = numpy.asarray(metrics_info.constraint_metrics_index)
-
-  return (
-    points_sampled.points,
-    points_sampled.values[:, optimized_metrics_index] if has_optimization_metrics else _UNSET,
-    points_sampled.value_vars[:, optimized_metrics_index] if has_optimization_metrics else _UNSET,
-    points_sampled.values[:, constraint_metrics_index] if has_constraint_metrics else _UNSET,
-    points_sampled.value_vars[:, constraint_metrics_index] if has_constraint_metrics else _UNSET,
-    points_sampled.failures,
-    points_sampled.task_costs,
-  )
+from sigoptlite.builders import LocalExperimentBuilder
+from sigoptlite.models import dataclass_to_dict
+from sigoptlite.sources import BaseOptimizationSource
+
+from test.base_test import UnitTestsBase
+from test.constants import (
+  DEFAULT_METRICS,
+  DEFAULT_METRICS_MULTIPLE,
+  DEFAULT_PARAMETERS,
+  EXPERIMENT_META_WITH_CONSTRAINTS,
+  PARAMETER_BETA_PRIOR,
+  PARAMETER_CATEGORICAL,
+  PARAMETER_DOUBLE,
+  PARAMETER_INT,
+  PARAMETER_NORMAL_PRIOR,
+)
 
 
-def form_one_hot_points_with_tasks(domain, points, task_costs=None):
-  assert isinstance(domain, CategoricalDomain)
-  one_hot_points = numpy.array([domain.map_categorical_point_to_one_hot(p) for p in points])
-  if task_costs is not None and one_hot_points.size:
-    one_hot_points = numpy.concatenate((one_hot_points, task_costs[:, None]), axis=1)
-  return one_hot_points
-
-
-def form_metric_midpoint_info(points_sampled_values, points_sampled_failures, metric_objectives):
-  if len(points_sampled_values.shape) == 1:
-    mmi = SingleMetricMidpointInfo(points_sampled_values, points_sampled_failures, metric_objectives)
-  else:
-    mmi = MultiMetricMidpointInfo(points_sampled_values, points_sampled_failures, metric_objectives)
-  return mmi
-
-
-def identify_scaled_values_exceeding_scaled_upper_thresholds(scaled_values, scaled_upper_thresholds):
-  within_bounds = numpy.full(len(scaled_values), True, dtype=bool)
-  for i, scaled_upper_threshold in enumerate(scaled_upper_thresholds):
-    if not numpy.isnan(scaled_upper_threshold):
-      within_bounds = numpy.logical_and(within_bounds, scaled_values[:, i] < scaled_upper_threshold)
-  return numpy.logical_not(within_bounds)
-
-
-def get_relevant_expected_improvement(predictor):
-  # If mean of sample variances is above threshold we use Augmented Expected Improvement
-  noise_variance = numpy.mean(predictor.points_sampled_noise_variance)
-  if noise_variance > AUGMENTED_EI_THRESHOLD:
-    return AugmentedExpectedImprovement(predictor)
-  else:
-    return ExpectedImprovement(predictor)
-
-
-class View(object):
-  view_name = None
-
-  def __init__(self, params, logging_service=None):
-    self.params = params
-    self.log = (logging_service or logging).getLogger(__name__)
-    self.tag = self.params["tag"]
-
-    self.domain = CategoricalDomain(**asdict(self.params["domain_info"]))
-    self.task_options = numpy.array(self.params["task_options"])
-    self.task_cost_populated = self.task_options.size
-
-    self.optimized_metrics_index = _UNSET
-    self.optimized_metrics_objectives = _UNSET
-    self._mmi = _UNSET
-    self.optimized_metrics_thresholds = _UNSET
-    self.scaled_optimized_lie_values = _UNSET
-
-    self.constraint_metrics_index = _UNSET
-    self.constraint_metrics_objectives = _UNSET
-    self._constraint_mmi = _UNSET
-    self.scaled_constraint_lie_values = _UNSET
-
-    self.has_optimization_metrics = self.params["metrics_info"].has_optimization_metrics
-    self.has_constraint_metrics = self.params["metrics_info"].has_constraint_metrics
-
-    if not self.has_optimization_metrics:
-      assert len(self.params["metrics_info"].optimized_metrics_index) == 0
-    assert self.has_optimization_metrics or self.has_constraint_metrics
-
-    (
-      self.points_sampled_points,
-      self.points_sampled_for_af_values,
-      self.points_sampled_for_af_value_vars,
-      self.points_sampled_for_pf_values,
-      self.points_sampled_for_pf_value_vars,
-      self.points_sampled_failures,
-      self.points_sampled_task_costs,
-    ) = filter_points_sampled(
-      self.params["points_sampled"],
-      self.params["metrics_info"],
-    )
-    if not self.task_cost_populated:
-      assert self.points_sampled_task_costs is None
-
-    if self.has_optimization_metrics:
-      self._preprocess_optimization_metrics()
-
-    if self.has_constraint_metrics:
-      self._preprocess_constraint_metrics()
-
-    # Convert to one hot point space
-    self.one_hot_points_sampled_points = form_one_hot_points_with_tasks(
-      self.domain,
-      self.points_sampled_points,
-      self.points_sampled_task_costs,
-    )
-
-    self._one_hot_points_being_sampled_points = _UNSET
-    self._one_hot_points_to_evaluate_points = _UNSET
-    self.dim_with_task = self.one_hot_points_sampled_points.shape[1]
-    assert self.dim_with_task == self.domain.one_hot_dim + (1 if self.task_cost_populated else 0)
-
-    self.form_multimetric_info()
-
-  # TODO: these two preprocess functions have a lot of overlap, consolidate this later.
-  def _preprocess_optimization_metrics(self):
-    self.optimized_metrics_index = self.params["metrics_info"].optimized_metrics_index
-    assert len(self.optimized_metrics_index) >= 1
-    self.optimized_metrics_objectives = numpy.asarray(
-      self.params["metrics_info"].objectives,
-      dtype=str,
-    )[self.optimized_metrics_index].tolist()
-    assert len(self.optimized_metrics_objectives) == len(self.optimized_metrics_index)
-    self._mmi = form_metric_midpoint_info(
-      self.points_sampled_for_af_values,
-      self.points_sampled_failures,
-      self.optimized_metrics_objectives,
-    )
-
-    # invert and scale points_sampled_value and points_sampled_value_vars
-    self.scaled_optimized_lie_values = self._mmi.relative_objective_value(
-      self._mmi.compute_lie_value(CONSTANT_LIAR_MIN)
-    )
-    self.points_sampled_for_af_values = self._mmi.relative_objective_value(self.points_sampled_for_af_values)
-    self.points_sampled_for_af_values[self.points_sampled_failures] = self.scaled_optimized_lie_values
-    self.points_sampled_for_af_value_vars = self._mmi.relative_objective_variance(self.points_sampled_for_af_value_vars)
-    unscaled_optimized_metrics_thresholds = numpy.asarray(
-      self.params["metrics_info"].user_specified_thresholds,
-      dtype=float,
-    )[self.optimized_metrics_index]
-    self.optimized_metrics_thresholds = self._mmi.relative_objective_value(unscaled_optimized_metrics_thresholds)
-
-  def _preprocess_constraint_metrics(self):
-    self.constraint_metrics_index = self.params["metrics_info"].constraint_metrics_index
-    assert len(self.constraint_metrics_index) >= 1
-    self.constraint_metrics_objectives = numpy.asarray(
-      self.params["metrics_info"].objectives,
-      dtype=str,
-    )[self.constraint_metrics_index].tolist()
-    assert len(self.constraint_metrics_objectives) == len(self.constraint_metrics_index)
-    self._constraint_mmi = form_metric_midpoint_info(
-      self.points_sampled_for_pf_values,
-      self.points_sampled_failures,
-      self.constraint_metrics_objectives,
-    )
-    self.scaled_constraint_lie_values = self._constraint_mmi.relative_objective_value(
-      self._constraint_mmi.compute_lie_value(CONSTANT_LIAR_MIN)
-    )
-    self.points_sampled_for_pf_values = self._constraint_mmi.relative_objective_value(self.points_sampled_for_pf_values)
-    self.points_sampled_for_pf_values[self.points_sampled_failures] = self.scaled_constraint_lie_values
-    self.points_sampled_for_pf_value_vars = self._constraint_mmi.relative_objective_variance(
-      self.points_sampled_for_pf_value_vars
-    )
-    unscaled_constraint_thresholds = numpy.asarray(
-      self.params["metrics_info"].user_specified_thresholds,
-      dtype=float,
-    )[self.constraint_metrics_index]
-    self.constraint_thresholds = self._constraint_mmi.relative_objective_value(unscaled_constraint_thresholds)
-
-  @property
-  def one_hot_points_to_evaluate_points(self):
-    if self._one_hot_points_to_evaluate_points is _UNSET:
-      self._one_hot_points_to_evaluate_points = form_one_hot_points_with_tasks(
-        self.domain,
-        self.params["points_to_evaluate"].points,
-        self.params["points_to_evaluate"].task_costs if self.task_cost_populated else None,
-      )
-    return self._one_hot_points_to_evaluate_points
-
-  @property
-  def one_hot_points_being_sampled_points(self):
-    if self._one_hot_points_being_sampled_points is _UNSET:
-      self._one_hot_points_being_sampled_points = form_one_hot_points_with_tasks(
-        self.domain,
-        self.params["points_being_sampled"].points,
-        self.params["points_being_sampled"].task_costs if self.task_cost_populated else None,
-      )
-    return self._one_hot_points_being_sampled_points
-
-  def create_sigoptcompute_log_line(self, log_type, content):
-    self.log.info(
-      "%s",
-      dict(
-        endpoint=self.view_name,
-        type=log_type,
-        content=content,
+class TestAdapter(UnitTestsBase):
+  @pytest.fixture
+  def experiment(self):
+    experiment_meta = dict(
+      parameters=[
+        PARAMETER_DOUBLE,
+        PARAMETER_INT,
+        PARAMETER_CATEGORICAL,
+      ],
+      metrics=DEFAULT_METRICS_MULTIPLE,
+      observation_budget=50,
+    )
+    return LocalExperimentBuilder(experiment_meta)
+
+  def test_observations_to_points(self, experiment):
+    observations = [
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 5.5, "i1": 15, "c1": "c"},
+        values=[dict(name="y1", value=1.1), dict(name="y2", value=2.2)],
       ),
-    )
-
-  def call(self):
-    self.create_sigoptcompute_log_line("params", self.params)
-    response = self.view()
-    self.create_sigoptcompute_log_line("return", response)
-    return response
-
-  def view(self):
-    raise NotImplementedError()
-
-  def form_multimetric_info(self):
-    if not self.params["metrics_info"].requires_pareto_frontier_optimization:
-      self.multimetric_info = MULTIMETRIC_INFO_NOT_MULTIMETRIC
-      return
-
-    num_open_suggestions = 0
-    if "points_being_sampled" in self.params:
-      num_open_suggestions = len(self.one_hot_points_being_sampled_points)
-    phase, kwargs = identify_multimetric_phase(
-      self.params["metrics_info"].has_optimized_metric_thresholds,
-      self.params["metrics_info"].observation_budget,
-      len(self.params["points_sampled"].points),
-      numpy.sum(self.params["points_sampled"].failures),
-      num_open_suggestions,
-    )
-    self.multimetric_info = form_multimetric_info_from_phase(phase, kwargs)
-
-
-class GPView(View):
-  def __init__(self, params, logging_service=None):
-    super().__init__(params, logging_service)
-    assert isinstance(self.params["model_info"], GPModelInfo)
-    self._polynomial_indices = _UNSET
-
-  @property
-  def polynomial_indices(self):
-    if self._polynomial_indices is _UNSET:
-      self._polynomial_indices = self._compute_polynomial_indices()
-    return self._polynomial_indices
-
-  def _compute_polynomial_indices(self):
-    return validate_polynomial_indices(
-      self.params["model_info"].nonzero_mean_info["poly_indices"],
-      self.params["model_info"].nonzero_mean_info["mean_type"],
-      self.dim_with_task,
-    )
-
-  def form_one_hot_covariance_base(self, domain, hyperparameter_dict):
-    assert isinstance(domain, CategoricalDomain)
-    length_scales = hyperparameter_dict["length_scales"]
-
-    one_hot_length_scales = domain.map_categorical_length_scales_to_one_hot(length_scales)
-    hyperparameters = (
-      [hyperparameter_dict["alpha"]]
-      + one_hot_length_scales
-      + ([] if hyperparameter_dict["task_length"] is None else [hyperparameter_dict["task_length"]])
-    )
-
-    physical_covariance_class = COVARIANCE_TYPES_TO_CLASSES[DEFAULT_COVARIANCE_KERNEL]
-    if self.task_cost_populated:
-      task_covariance_class = COVARIANCE_TYPES_TO_CLASSES[DEFAULT_TASK_COVARIANCE_KERNEL]
-      covariance = MultitaskTensorCovariance(hyperparameters, physical_covariance_class, task_covariance_class)
-    else:
-      covariance = physical_covariance_class(hyperparameters)
-
-    return covariance
-
-  def form_single_gaussian_process(
-    self,
-    filtered_one_hot_points_sampled_points,
-    filtered_points_sampled_values,
-    filtered_points_sampled_value_vars,
-    filtered_scaled_lie_value,
-    hyperparameter_dict,
-  ):
-    one_hot_historical_data = HistoricalData(self.dim_with_task)
-    one_hot_historical_data.append_historical_data(
-      filtered_one_hot_points_sampled_points,
-      filtered_points_sampled_values,
-      filtered_points_sampled_value_vars,
-    )
-    if self.params["parallelism"] == PARALLEL_CONSTANT_LIAR:
-      one_hot_historical_data.append_lies(
-        self.one_hot_points_being_sampled_points,
-        filtered_scaled_lie_value,
-        DEFAULT_CONSTANT_LIAR_LIE_NOISE_VARIANCE,
-      )
-
-    one_hot_covariance = self.form_one_hot_covariance_base(
-      self.domain,
-      hyperparameter_dict,
-    )
-
-    gaussian_process = GaussianProcess(
-      covariance=one_hot_covariance,
-      historical_data=one_hot_historical_data,
-      mean_poly_indices=self.polynomial_indices,
-      tikhonov_param=hyperparameter_dict["tikhonov"],
-    )
-    return gaussian_process
-
-  def form_gaussian_process_for_acquisition_function(self):
-    (
-      filtered_one_hot_points_sampled_points,
-      filtered_points_sampled_values,
-      filtered_points_sampled_value_vars,
-      filtered_scaled_lie_value,
-    ) = filter_multimetric_points_sampled(
-      self.multimetric_info,
-      self.one_hot_points_sampled_points,
-      self.points_sampled_for_af_values,
-      self.points_sampled_for_af_value_vars,
-      self.points_sampled_failures,
-      self.scaled_optimized_lie_values,
-    )
-    num_models = filtered_points_sampled_values.ndim
-    if self.multimetric_info.method == CONVEX_COMBINATION:
-      gaussian_process_list = []
-      for i, metric_index in enumerate(self.optimized_metrics_index):
-        gp = self.form_single_gaussian_process(
-          filtered_one_hot_points_sampled_points,
-          filtered_points_sampled_values[:, i],
-          filtered_points_sampled_value_vars[:, i],
-          filtered_scaled_lie_value[i],
-          self.params["model_info"].hyperparameters[metric_index],
-        )
-        gaussian_process_list.append(gp)
-      weights = numpy.copy(self.multimetric_info.params.weights)
-      main_gaussian_process = GaussianProcessSum(gaussian_process_list, weights)
-    else:
-      assert num_models == 1
-      optimization_model_index = 0
-      if self.params["metrics_info"].requires_pareto_frontier_optimization:
-        optimization_model_index = self.multimetric_info.params.optimizing_metric
-      metric_index = self.optimized_metrics_index[optimization_model_index]
-      main_gaussian_process = self.form_single_gaussian_process(
-        filtered_one_hot_points_sampled_points,
-        filtered_points_sampled_values,
-        filtered_points_sampled_value_vars,
-        filtered_scaled_lie_value,
-        self.params["model_info"].hyperparameters[metric_index],
-      )
-    return main_gaussian_process
-
-  def _form_gp_for_probabilistic_failures(self, relative_index, for_af_values=True):
-    metric_indexes = self.optimized_metrics_index
-    points_sampled_values = self.points_sampled_for_af_values
-    points_sampled_value_vars = self.points_sampled_for_af_value_vars
-    scaled_lie_values = self.scaled_optimized_lie_values
-    if for_af_values:
-      assert relative_index in (0, 1)
-    else:
-      assert relative_index in range(len(self.constraint_metrics_index))
-      metric_indexes = self.constraint_metrics_index
-      points_sampled_values = self.points_sampled_for_pf_values
-      points_sampled_value_vars = self.points_sampled_for_pf_value_vars
-      scaled_lie_values = self.scaled_constraint_lie_values
-
-    return self.form_single_gaussian_process(
-      self.one_hot_points_sampled_points,
-      points_sampled_values[:, relative_index],
-      points_sampled_value_vars[:, relative_index],
-      scaled_lie_values[relative_index],
-      self.params["model_info"].hyperparameters[metric_indexes[relative_index]],
-    )
-
-  # TODO(RTL-85): I think a lot of this workflow can be cleanup up with find_epsilon_constraint_value better now
-  def _form_probabilistic_failures_for_pareto_frontier_optimization(self):
-    multimetric_info = self.multimetric_info
-    if multimetric_info.method not in (PROBABILISTIC_FAILURES, EPSILON_CONSTRAINT):
-      return []
-
-    constraint_metrics_index = multimetric_info.params.constraint_metric
-    constraint_threshold = find_epsilon_constraint_value(
-      multimetric_info.params.epsilon,
-      constraint_metrics_index,
-      self.points_sampled_for_af_values,
-      self.optimized_metrics_thresholds,
-    )
-
-    threshold_0 = threshold_1 = None
-    if not numpy.any(numpy.isnan(self.optimized_metrics_thresholds)) and len(self.optimized_metrics_thresholds) == 2:
-      threshold_0, threshold_1 = self.optimized_metrics_thresholds
-    if constraint_metrics_index == 0:
-      threshold_0 = constraint_threshold
-    else:
-      threshold_1 = constraint_threshold
-
-    pof_0 = None
-    if threshold_0 is not None:
-      gp = self._form_gp_for_probabilistic_failures(0, for_af_values=True)
-      pof_0 = ProbabilisticFailures(gp, threshold_0)
-
-    pof_1 = None
-    if threshold_1 is not None:
-      gp = self._form_gp_for_probabilistic_failures(1, for_af_values=True)
-      pof_1 = ProbabilisticFailures(gp, threshold_1)
-
-    if pof_0 is None:
-      return [pof_1]
-    if pof_1 is None:
-      return [pof_0]
-    return [pof_0, pof_1]
-
-  def _form_list_of_probabilistic_failures_for_constraint_metrics(self):
-    list_of_probabilistic_failures = []
-
-    for i in range(len(self.constraint_metrics_index)):
-      gp = self._form_gp_for_probabilistic_failures(i, for_af_values=False)
-      threshold = self.constraint_thresholds[i]
-      pof = ProbabilisticFailuresCDF(gp, threshold)
-      list_of_probabilistic_failures.append(pof)
-
-    return list_of_probabilistic_failures
-
-  def form_probabilistic_failures_model(self):
-    if not (
-      self.multimetric_info.method in (PROBABILISTIC_FAILURES, EPSILON_CONSTRAINT) or self.has_constraint_metrics
-    ):
-      return None
-
-    list_of_failures = self._form_probabilistic_failures_for_pareto_frontier_optimization()
-    if self.has_constraint_metrics:
-      list_of_failures.extend(self._form_list_of_probabilistic_failures_for_constraint_metrics())
-
-    return ProductOfListOfProbabilisticFailures(list_of_failures)
-
-  def _form_parallel_ei(self, gaussian_process, probabilistic_failures):
-    num_to_sample = self.params.get("num_to_sample", 1)
-    assert num_to_sample == 1, "Currently capping number of qEI suggestions to 1"
-    if probabilistic_failures:
-      self.tag.update({"failure_model_info": probabilistic_failures.info_for_logs})
-      return ExpectedParallelImprovementWithFailures(
-        predictor=gaussian_process,
-        num_points_to_sample=num_to_sample,
-        failure_model=probabilistic_failures,
-        points_being_sampled=self.one_hot_points_being_sampled_points,
-      )
-    return ExpectedParallelImprovement(
-      predictor=gaussian_process,
-      num_points_to_sample=num_to_sample,
-      points_being_sampled=self.one_hot_points_being_sampled_points,
-    )
-
-  def form_acquisition_function(self, gaussian_process, probabilistic_failures, use_parallel_ei):
-    if use_parallel_ei:
-      return self._form_parallel_ei(gaussian_process, probabilistic_failures)
-    if probabilistic_failures:
-      self.tag.update({"failure_model_info": probabilistic_failures.info_for_logs})
-      return ExpectedImprovementWithFailures(
-        predictor=gaussian_process,
-        failure_model=probabilistic_failures,
-      )
-    return get_relevant_expected_improvement(gaussian_process)
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 7.5, "i1": 18, "c1": "a"},
+        values=[dict(name="y1", value=3.3), dict(name="y2", value=4.4)],
+      ),
+    ]
+    adapter = BaseOptimizationSource(experiment)
+    points_container = adapter.make_points_sampled(experiment, observations)
+    expected_points = numpy.array(
+      [
+        [5.5, 15, 3],
+        [7.5, 18, 1],
+      ]
+    )
+    assert numpy.all(points_container.points == expected_points)
+    expected_values = numpy.array(
+      [
+        [1.1, 2.2],
+        [3.3, 4.4],
+      ]
+    )
+    assert numpy.all(points_container.values == expected_values)
+    expected_value_vars = numpy.zeros((2, 2))
+    assert numpy.all(points_container.value_vars == expected_value_vars)
+    assert numpy.all(points_container.failures == numpy.array([False] * 2))
+
+  def test_observations_to_points_with_variance(self, experiment):
+    observations = [
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 5.5, "i1": 15, "c1": "c"},
+        values=[
+          dict(name="y1", value=1.1, value_stddev=1e-1),
+          dict(name="y2", value=2.2, value_stddev=1e-2),
+        ],
+      ),
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 7.5, "i1": 18, "c1": "a"},
+        values=[
+          dict(name="y1", value=3.3, value_stddev=1e-3),
+          dict(name="y2", value=4.4, value_stddev=1e-4),
+        ],
+      ),
+    ]
+    adapter = BaseOptimizationSource(experiment)
+    points_container = adapter.make_points_sampled(experiment, observations)
+    expected_value_vars = numpy.array(
+      [
+        [1e-1, 1e-2],
+        [1e-3, 1e-4],
+      ]
+    )
+    assert numpy.all(points_container.value_vars == expected_value_vars)
+
+  def test_observations_to_points_with_failures(self, experiment):
+    observations = [
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 5.5, "i1": 15, "c1": "c"},
+        failed=True,
+      ),
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 7.5, "i1": 18, "c1": "a"},
+        failed=True,
+      ),
+    ]
+    adapter = BaseOptimizationSource(experiment)
+    points_container = adapter.make_points_sampled(experiment, observations)
+    assert numpy.all(points_container.failures == numpy.array([True] * 2))
+
+  def test_observations_with_task(self):
+    experiment_meta = self.get_experiment_feature("multitask")
+    experiment = LocalExperimentBuilder(experiment_meta)
+    observations = [
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 5.5, "l1": 1, "i1": 15, "c1": "c", "g1": 0.3},
+        values=[dict(name="y1", value=1.1)],
+        task={"name": "cheap", "cost": 0.1},
+      ),
+      self.make_observation(
+        experiment=experiment,
+        assignments={"d1": 7.5, "l1": 1, "i1": 18, "c1": "a", "g1": 0.1},
+        values=[dict(name="y1", value=3.3)],
+        task={"name": "expensive", "cost": 1},
+      ),
+    ]
+    adapter = BaseOptimizationSource(experiment)
+    points_container = adapter.make_points_sampled(experiment, observations)
+    expected_task_costs = numpy.array([0.1, 1])
+    assert len(points_container.task_costs) == 2
+    assert numpy.all(points_container.task_costs == expected_task_costs)
+
+
+class TestGenerateDomainInfo(UnitTestsBase):
+  def test_generate_domain_info(self):
+    experiment_meta = dict(
+      parameters=DEFAULT_PARAMETERS,
+      metrics=DEFAULT_METRICS,
+    )
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    domain_info = adapter.form_domain_info(local_experiment)
+    expected_domain_info = DomainInfo(
+      constraint_list=[],
+      domain_components=[
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 10]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [-5, 0]},
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [10, 20]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2, 3]},
+        {"var_type": QUANTIZED_EXPERIMENT_PARAMETER_NAME, "elements": [0.01, 0.1, 0.3, 0.9]},
+      ],
+      force_hitandrun_sampling=False,
+      priors=None,
+    )
+    assert domain_info == expected_domain_info
+
+  def test_generate_domain_info_priors(self):
+    experiment_meta_with_priors = dict(
+      parameters=[
+        PARAMETER_NORMAL_PRIOR,
+        PARAMETER_BETA_PRIOR,
+        PARAMETER_DOUBLE,
+      ],
+      metrics=DEFAULT_METRICS,
+    )
+    local_experiment = LocalExperimentBuilder(experiment_meta_with_priors)
+    adapter = BaseOptimizationSource(local_experiment)
+    domain_info = adapter.form_domain_info(local_experiment)
+    expected_domain_info = DomainInfo(
+      constraint_list=[],
+      domain_components=[
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 10]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 10]},
+      ],
+      force_hitandrun_sampling=False,
+      priors=[
+        {"name": ParameterPriorNames.NORMAL, "params": {"mean": 5, "scale": 2}},
+        {"name": ParameterPriorNames.BETA, "params": {"shape_a": 1, "shape_b": 10}},
+        {"name": None, "params": None},
+      ],
+    )
+    assert domain_info == expected_domain_info
+
+  def test_generate_domain_info_constraints(self):
+    local_experiment = LocalExperimentBuilder(EXPERIMENT_META_WITH_CONSTRAINTS)
+    adapter = BaseOptimizationSource(local_experiment)
+    domain_info = adapter.form_domain_info(local_experiment)
+    expected_domain_info = DomainInfo(
+      constraint_list=[
+        {"weights": [1, 0, 2, 0, 0, 0], "rhs": 0.5, "var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME},
+        {"weights": [0, -3, 0, -4, 0, 0], "rhs": -0.9, "var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME},
+        {"weights": [0, 0, 0, 0, 1, 1], "rhs": 10, "var_type": INT_EXPERIMENT_PARAMETER_NAME},
+      ],
+      domain_components=[
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [0, 10]},
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [0, 10]},
+      ],
+      force_hitandrun_sampling=True,
+      priors=None,
+    )
+    assert domain_info == expected_domain_info
+
+
+class TestFormMetricsInfo(UnitTestsBase):
+  def get_points_sampled(self, experiment, num_observations):
+    observations = self.make_random_observations(experiment, num_observations)
+    points_sampled = BaseOptimizationSource.make_points_sampled(experiment, observations)
+    return points_sampled
+
+  def test_form_metrics_info_single(self):
+    experiment_meta = self.get_experiment_feature("default")
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment)
+    assert not metrics_info.requires_pareto_frontier_optimization
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [None]
+    assert not metrics_info.has_optimized_metric_thresholds
+    assert not metrics_info.has_constraint_metrics
+    assert metrics_info.objectives == ["maximize"]
+    assert metrics_info.optimized_metrics_index == [0]
+    assert metrics_info.constraint_metrics_index == []
+    assert metrics_info.has_optimization_metrics
+
+  def test_form_metrics_info_multi(self):
+    experiment_meta = self.get_experiment_feature("multimetric")
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment)
+    assert metrics_info.requires_pareto_frontier_optimization
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [None, None]
+    assert not metrics_info.has_optimized_metric_thresholds
+    assert not metrics_info.has_constraint_metrics
+    assert metrics_info.objectives == ["maximize", "minimize"]
+    assert metrics_info.optimized_metrics_index == [0, 1]
+    assert metrics_info.constraint_metrics_index == []
+    assert metrics_info.has_optimization_metrics
+
+  def test_form_metrics_info_metric_thresholds(self):
+    experiment_meta = self.get_experiment_feature("metric_threshold")
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment)
+    assert metrics_info.requires_pareto_frontier_optimization
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [0.5, None]
+    assert metrics_info.has_optimized_metric_thresholds
+    assert not metrics_info.has_constraint_metrics
+    assert metrics_info.objectives == ["maximize", "minimize"]
+    assert metrics_info.optimized_metrics_index == [0, 1]
+    assert metrics_info.constraint_metrics_index == []
+    assert metrics_info.has_optimization_metrics
+
+  def test_form_metrics_info_one_constraint(self):
+    experiment_meta = self.get_experiment_feature("metric_constraint")
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment)
+    assert not metrics_info.requires_pareto_frontier_optimization
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [0.5, None]
+    assert not metrics_info.has_optimized_metric_thresholds
+    assert metrics_info.has_constraint_metrics
+    assert metrics_info.objectives == ["maximize", "minimize"]
+    assert metrics_info.optimized_metrics_index == [1]
+    assert metrics_info.constraint_metrics_index == [0]
+    assert metrics_info.has_optimization_metrics
+
+  def test_form_metrics_info_search(self):
+    experiment_meta = self.get_experiment_feature("search")
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment)
+    assert not metrics_info.requires_pareto_frontier_optimization
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [0.25, 0.75]
+    assert not metrics_info.has_optimized_metric_thresholds
+    assert metrics_info.has_constraint_metrics
+    assert metrics_info.objectives == ["maximize", "minimize"]
+    assert metrics_info.optimized_metrics_index == []
+    assert metrics_info.constraint_metrics_index == [0, 1]
+    assert not metrics_info.has_optimization_metrics
+
+  @pytest.mark.parametrize("objective", ["maximize", "minimize"])
+  def test_form_metrics_info_multisolution_experiment(self, objective):
+    experiment_meta = self.get_experiment_feature("multisolution")
+    experiment_meta["metrics"][0]["objective"] = objective
+    local_experiment = LocalExperimentBuilder(experiment_meta)
+    num_observations = 11
+    points_sampled = self.get_points_sampled(local_experiment, num_observations)
+    quantile = MULTISOLUTION_QUANTILE_FOR_SEARCH_THRESHOLD
+    if objective == "minimize":
+      quantile = 1 - quantile
+    expected_threshold = numpy.quantile(
+      points_sampled.values[~points_sampled.failures, 0],
+      quantile,
+    )
+    adapter = BaseOptimizationSource(local_experiment)
+    metrics_info = adapter.form_metrics_info(local_experiment, points_sampled)
+    assert metrics_info.observation_budget == experiment_meta["observation_budget"]
+    assert metrics_info.user_specified_thresholds == [expected_threshold]
+    assert metrics_info.optimized_metrics_index == []
+    assert metrics_info.objectives == [objective]
+    assert metrics_info.constraint_metrics_index == [0]
+    assert not metrics_info.has_optimized_metric_thresholds
+    assert metrics_info.has_constraint_metrics
+
+
+class TestConditionals(UnitTestsBase):
+  def assert_parameter_list_are_equal(self, original_list, condional_list):
+    assert len(original_list) == len(condional_list)
+    for org_param, cond_param in zip(original_list, condional_list):
+      orginal_dict, condional_dict = dataclass_to_dict(org_param), dataclass_to_dict(cond_param)
+      orginal_dict["conditions"] = {}
+      assert orginal_dict == condional_dict
+
+  def test_create_unconditioned_experiment_from_conditionals(self):
+    experiment_meta = self.get_experiment_feature("conditionals")
+    original_experiment = LocalExperimentBuilder(experiment_meta)
+    unconditioned_exp = BaseOptimizationSource.apply_conditional_transformation_to_experiment(original_experiment)
+    assert [p.name for p in unconditioned_exp.parameters] == ["a", "b", "c", "x"]
+    self.assert_parameter_list_are_equal(original_experiment.parameters, unconditioned_exp.parameters[:-1])
+    assert all(not bool(p.conditions) for p in unconditioned_exp.parameters)
+    domain_info = BaseOptimizationSource.form_domain_info(unconditioned_exp)
+    expected_domain_info = DomainInfo(
+      constraint_list=[],
+      domain_components=[
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [1, 50]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [-50, 0]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2, 3]},
+      ],
+      force_hitandrun_sampling=False,
+      priors=None,
+    )
+    assert domain_info == expected_domain_info
+    base_source = BaseOptimizationSource(original_experiment)
+    assert base_source.experiment == unconditioned_exp
+    assert base_source.form_domain_info(base_source.experiment) == expected_domain_info
+
+  def test_create_unconditioned_experiment_from_multiconditional(self):
+    experiment_meta = self.get_experiment_feature("multiconditional")
+    original_experiment = LocalExperimentBuilder(experiment_meta)
+    unconditioned_exp = BaseOptimizationSource.apply_conditional_transformation_to_experiment(original_experiment)
+    assert [p.name for p in unconditioned_exp.parameters] == ["a", "b", "c", "d", "x", "y", "z"]
+    self.assert_parameter_list_are_equal(original_experiment.parameters, unconditioned_exp.parameters[:-3])
+    assert all(not bool(p.conditions) for p in unconditioned_exp.parameters)
+    domain_info = BaseOptimizationSource.form_domain_info(unconditioned_exp)
+    expected_domain_info = DomainInfo(
+      constraint_list=[],
+      domain_components=[
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [1, 50]},
+        {"var_type": DOUBLE_EXPERIMENT_PARAMETER_NAME, "elements": [-50, 0]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2]},
+        {"var_type": INT_EXPERIMENT_PARAMETER_NAME, "elements": [0, 1]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2, 3]},
+        {"var_type": CATEGORICAL_EXPERIMENT_PARAMETER_NAME, "elements": [1, 2]},
+      ],
+      force_hitandrun_sampling=False,
+      priors=None,
+    )
+    assert domain_info == expected_domain_info
+    base_source = BaseOptimizationSource(original_experiment)
+    assert base_source.experiment == unconditioned_exp
+    assert base_source.form_domain_info(base_source.experiment) == expected_domain_info
+
+  @pytest.mark.parametrize(
+    "unconditioned_assignments,expected_assignments",
+    [
+      (dict(a=1, b=-50.0, c="d", x="1"), dict(a=1, x="1")),
+      (dict(a=1, b=-50.0, c="d", x="5"), dict(a=1, b=-50.0, x="5")),
+      (dict(a=1, b=-50.0, c="d", x="10"), dict(a=1, b=-50.0, c="d", x="10")),
+    ],
+  )
+  def test_unconditioned_suggestions_from_conditionals(self, unconditioned_assignments, expected_assignments):
+    experiment_meta = self.get_experiment_feature("conditionals")
+    original_experiment = LocalExperimentBuilder(experiment_meta)
+    base_source = BaseOptimizationSource(original_experiment)
+    # pylint: disable=protected-access
+    assert base_source._original_experiment == original_experiment
+    assert base_source._original_experiment.is_conditional
+    # pylint: enable=protected-access
+    assert not base_source.experiment.is_conditional
+    unconditioned_suggestion = self.make_suggestion(assignments=unconditioned_assignments)
+    suggestion = base_source.remove_transformations_from_source_suggestion(unconditioned_suggestion)
+    assert suggestion.assignments == expected_assignments
```

### Comparing `sigoptlite-0.1.1/sigoptlite/best_assignments.py` & `sigoptlite-0.1.2/sigoptlite/best_assignments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: Apache License 2.0
-from lite_sigoptaux.constant import MULTISOLUTION_TOP_OBSERVATIONS_FRACTION
-from lite_sigoptaux.multimetric import find_pareto_frontier_observations_for_maximization
+from libsigopt.aux.constant import MULTISOLUTION_TOP_OBSERVATIONS_FRACTION
+from libsigopt.aux.multimetric import find_pareto_frontier_observations_for_maximization
+
 from sigoptlite.sources import BaseOptimizationSource
 
 
 class BestAssignmentsLogger(object):
   def __init__(self, experiment):
     self.experiment = experiment
     self.full_task_cost = None
```

### Comparing `sigoptlite-0.1.1/sigoptlite/broker.py` & `sigoptlite-0.1.2/sigoptlite/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: Apache License 2.0
-from lite_sigoptaux.constant import DEFAULT_USE_SPE_AFTER_THIS_MANY_OBSERVATIONS, DEFAULT_USE_SPE_BEYOND_THIS_MANY_DIMENSIONS
+from libsigopt.aux.constant import (
+  DEFAULT_USE_SPE_AFTER_THIS_MANY_OBSERVATIONS,
+  DEFAULT_USE_SPE_BEYOND_THIS_MANY_DIMENSIONS,
+)
+
 from sigoptlite.builders import LocalObservationBuilder
 from sigoptlite.models import LocalSuggestion, dataclass_to_dict
 from sigoptlite.sources import GPSource, RandomSearchSource, SPESource
 
 
 class Broker(object):
   def __init__(self, experiment, force_spe=False):
@@ -45,26 +49,18 @@
 
     return dict(
       observation_budget_consumed=observation_budget_consumed,
       observation_count=observation_count,
     )
 
   def create_observation(self, assignments=None, values=None, suggestion=None, failed=False, task=None):
-    if not (bool(not assignments) ^ bool(not suggestion)):
-      raise ValueError("Need to pass in an assignments dictionary or a suggestion id to create an observation")
+    self.validate_observation_assignments_and_suggestions(assignments, suggestion)
 
     if assignments is None:
-      if self.stored_suggestion is None:
-        raise ValueError("There is no stored suggestion to use. Please create a suggestion")
-
-      if suggestion != self.stored_suggestion.id:
-        raise ValueError(
-          f"The suggestion you provided: {suggestion} does not match the suggestion stored: {self.stored_suggestion.id}"
-        )
-
+      self.validate_observation_with_suggestion_id(suggestion)
       assignments = self.stored_suggestion.assignments
       if self.stored_suggestion.task is not None:
         task = dataclass_to_dict(self.stored_suggestion.task)
 
     observation = LocalObservationBuilder(
       input_dict=dict(
         assignments=assignments,
@@ -98,7 +94,22 @@
       id=str(self.suggestion_id),
       assignments=suggestion_data.assignments,
       task=suggestion_data.task,
     )
     self.stored_suggestion = suggestion_to_serve
     self.suggestion_id += 1
     return suggestion_to_serve
+
+  def validate_observation_assignments_and_suggestions(self, suggestion_id, assignments):
+    if (assignments is None) and (suggestion_id is None):
+      raise ValueError("Need to pass in an assignments dictionary or a suggestion id to create an observation")
+    if (assignments is not None) and (suggestion_id is not None):
+      raise ValueError("Cannot specify `suggestion` and `assignments`.")
+
+  def validate_observation_with_suggestion_id(self, suggestion_id):
+    if self.stored_suggestion is None:
+      raise ValueError("There is no stored suggestion to use. Please create a suggestion")
+    if suggestion_id != self.stored_suggestion.id:
+      raise ValueError(
+        f"The suggestion you provided: {suggestion_id} does not match the suggestion stored:"
+        f" {self.stored_suggestion.id}"
+      )
```

### Comparing `sigoptlite-0.1.1/sigoptlite/driver.py` & `sigoptlite-0.1.2/sigoptlite/driver.py`

 * *Files identical despite different names*

### Comparing `sigoptlite-0.1.1/sigoptlite/models.py` & `sigoptlite-0.1.2/sigoptlite/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: Apache License 2.0
 from dataclasses import asdict, dataclass, field
 from typing import List
 
-from lite_sigoptaux.constant import (
+from libsigopt.aux.constant import (
   CATEGORICAL_EXPERIMENT_PARAMETER_NAME,
   DOUBLE_EXPERIMENT_PARAMETER_NAME,
+  INT_EXPERIMENT_PARAMETER_NAME,
   ParameterPriorNames,
+  ParameterTransformationNames,
 )
 
 
 FIXED_EXPERIMENT_ID = "-1"
 
 
 def dataclass_to_dict(obj):
@@ -67,54 +69,58 @@
   name: str
   cost: float
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalParameterPrior:
   name: str
-  mean: float = None
-  scale: float = None
-  shape_a: float = None
-  shape_b: float = None
+  mean: float | None = None
+  scale: float | None = None
+  shape_a: float | None = None
+  shape_b: float | None = None
 
   @property
   def is_beta(self):
     return self.name == ParameterPriorNames.BETA
 
   @property
   def is_normal(self):
     return self.name == ParameterPriorNames.NORMAL
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalParameter:
   name: str
   type: str
-  bounds: LocalBounds = None
+  bounds: LocalBounds | None = None
   categorical_values: List[LocalCategoricalValue] = field(default_factory=list)
   conditions: List[LocalCondition] = field(default_factory=list)
   grid: List[float] = field(default_factory=list)
-  prior: LocalParameterPrior = None
-  transformation: str = None
+  prior: LocalParameterPrior | None = None
+  transformation: str | None = None
+
+  @property
+  def is_int(self):
+    return self.type == INT_EXPERIMENT_PARAMETER_NAME
 
   @property
   def is_categorical(self):
     return self.type == CATEGORICAL_EXPERIMENT_PARAMETER_NAME
 
   @property
   def is_double(self):
     return self.type == DOUBLE_EXPERIMENT_PARAMETER_NAME
 
   @property
   def has_prior(self):
     return self.prior is not None
 
   @property
-  def has_transformation(self):
-    return self.transformation is not None
+  def has_log_transformation(self):
+    return self.transformation == ParameterTransformationNames.LOG
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalConditional:
   name: str
   values: List[LocalConditionalValue]
 
@@ -133,15 +139,15 @@
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalMetric:
   name: str
   objective: str = "maximize"
   strategy: str = "optimize"
-  threshold: float = None
+  threshold: float | None = None
 
   @property
   def is_optimized(self):
     return self.strategy == "optimize"
 
   @property
   def is_constraint(self):
@@ -156,17 +162,17 @@
 class LocalExperiment:
   id: str = FIXED_EXPERIMENT_ID
   parameters: List[LocalParameter]
   metrics: List[LocalMetric]
   conditionals: List[LocalConditional] = field(default_factory=list)
   linear_constraints: List[LocalLinearConstraint] = field(default_factory=list)
   metadata = None
-  name: str = None
+  name: str | None = None
   num_solutions: int = 1
-  observation_budget: int = None
+  observation_budget: int | None = None
   parallel_bandwidth: int = 1
   tasks: List[LocalTask] = field(default_factory=list)
   type: str = "offline"
 
   @property
   def dimension(self):
     return len(self.parameters)
@@ -216,23 +222,23 @@
   pass
 
 
 @dataclass(frozen=True, kw_only=True)
 class MetricEvaluation:
   name: str
   value: float
-  value_stddev: float = None
+  value_stddev: float | None = None
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalObservation:
   assignments: LocalAssignments
   metric_evaluations: dict = field(default_factory=dict)
   failed: bool = False
-  task: LocalTask = None
+  task: LocalTask | None = None
 
   def get_client_observation(self, experiment):
     return dict(
       assignments=dict(self.assignments),
       values=None if self.failed else [dataclass_to_dict(me) for me in self.get_metric_evaluations(experiment)],
       task=dataclass_to_dict(self.task) if self.task else None,
       failed=self.failed,
@@ -268,16 +274,16 @@
       for metric in experiment.metrics
     )
 
 
 @dataclass(frozen=True, kw_only=True)
 class LocalSuggestion:
   assignments: LocalAssignments
-  id: str = None
-  task: LocalTask = None
+  id: str | None = None
+  task: LocalTask | None = None
 
   def __post_init__(self):
     object.__setattr__(self, "assignments", LocalAssignments(self.assignments))
 
   def get_assignments(self, experiment):
     parameters = experiment.parameters
     conditionals = experiment.conditionals
```

### Comparing `sigoptlite-0.1.1/sigoptlite/sources.py` & `sigoptlite-0.1.2/sigoptlite/sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # Copyright © 2022 Intel Corporation
 #
 # SPDX-License-Identifier: Apache License 2.0
-from dataclasses import asdict
-
 import numpy
 
-from lite_sigoptcompute.views.rest.gp_hyper_opt_multimetric import GpHyperOptMultimetricView
-from lite_sigoptcompute.views.rest.gp_next_points_categorical import GpNextPointsCategorical
-from lite_sigoptcompute.views.rest.multisolution_best_assignments import MultisolutionBestAssignments
-from lite_sigoptcompute.views.rest.search_next_points import SearchNextPoints
-from lite_sigoptcompute.views.rest.spe_next_points import SPENextPoints
-from lite_sigoptcompute.views.rest.spe_search_next_points import SPESearchNextPoints
-
-from lite_sigoptaux.adapter_info_containers import DomainInfo, GPModelInfo, MetricsInfo, PointsContainer
-from lite_sigoptaux.constant import (
+from libsigopt.aux.adapter_info_containers import DomainInfo, GPModelInfo, MetricsInfo, PointsContainer
+from libsigopt.aux.constant import (
   CATEGORICAL_EXPERIMENT_PARAMETER_NAME,
   DEFAULT_HYPERPARAMETER_ALPHA,
   DEFAULT_HYPERPARAMETER_TASK_LENGTH_SCALE,
-  DOUBLE_EXPERIMENT_PARAMETER_NAME,
-  INT_EXPERIMENT_PARAMETER_NAME,
   MAX_SIMULTANEOUS_AF_POINTS,
   MULTISOLUTION_QUANTILE_FOR_SEARCH_THRESHOLD,
   PARALLEL_CONSTANT_LIAR,
   QUANTIZED_EXPERIMENT_PARAMETER_NAME,
   ConstraintType,
-  ParameterPriorNames,
-  ParameterTransformationNames,
 )
-from lite_sigoptaux.domain import CategoricalDomain
+from libsigopt.aux.errors import SigoptComputeError
+from libsigopt.views.rest.gp_hyper_opt_multimetric import GpHyperOptMultimetricView
+from libsigopt.views.rest.gp_next_points_categorical import GpNextPointsCategorical
+from libsigopt.views.rest.multisolution_best_assignments import MultisolutionBestAssignments
+from libsigopt.views.rest.random_search_next_points import RandomSearchNextPoints
+from libsigopt.views.rest.search_next_points import SearchNextPoints
+from libsigopt.views.rest.spe_next_points import SPENextPoints
+from libsigopt.views.rest.spe_search_next_points import SPESearchNextPoints
+
 from sigoptlite.builders import create_experiment_from_template
 from sigoptlite.models import LocalSuggestion, dataclass_to_dict, replacement_value_if_missing
 
 
 EMPTY_POINTS_CONTAINER = PointsContainer(points=numpy.array([]))
 
 
@@ -39,14 +34,21 @@
   def __init__(self, experiment):
     self._original_experiment = experiment
     self.experiment = self.apply_transformations_to_experiment(experiment)
 
   def next_point(self, observations):
     raise NotImplementedError()
 
+  @classmethod
+  def call_libsigopt_views(cls, view_endpoint, view_input):
+    try:
+      return view_endpoint(view_input).call()
+    except (ValueError, IndexError, numpy.linalg.LinAlgError) as e:
+      raise SigoptComputeError(e) from e
+
   def apply_transformations_to_experiment(self, original_experiment):
     if not original_experiment.is_conditional:
       return original_experiment
     return self.apply_conditional_transformation_to_experiment(original_experiment)
 
   def remove_transformations_from_source_suggestion(self, source_suggestion):
     if not self._original_experiment.is_conditional:
@@ -141,15 +143,15 @@
       "domain_info": cls.form_domain_info(experiment),
       "metrics_info": cls.form_basic_metric_info(experiment),
       "num_solutions": experiment.num_solutions,
       "points_sampled": points_sampled,
       "tag": {},
       "task_options": [t.cost for t in experiment.tasks],
     }
-    response = MultisolutionBestAssignments(view_input).view()
+    response = cls.call_libsigopt_views(MultisolutionBestAssignments, view_input)
     best_indices = [int(i) for i in response["best_indices"] if i is not None]
     return best_indices
 
   @classmethod
   def form_metrics_info(cls, experiment, points_sampled=None):
     metrics_info = cls.form_basic_metric_info(experiment)
     if experiment.num_solutions == 1:
@@ -206,37 +208,37 @@
       objectives=objectives,
       optimized_metrics_index=optimized_metrics_index,
       constraint_metrics_index=constraint_metrics_index,
     )
 
   @staticmethod
   def pe_parameter_info(parameter):
-    if parameter.type == CATEGORICAL_EXPERIMENT_PARAMETER_NAME:
+    if parameter.is_categorical:
       elements = list(range(1, len(parameter.categorical_values) + 1))
     elif parameter.grid:
       elements = parameter.grid
     else:
       elements = [parameter.bounds.min, parameter.bounds.max]
-    var_type = parameter.type if not parameter.grid else QUANTIZED_EXPERIMENT_PARAMETER_NAME
-
-    if parameter.transformation == ParameterTransformationNames.LOG:
-      assert parameter.type == DOUBLE_EXPERIMENT_PARAMETER_NAME or parameter.grid
+    if parameter.has_log_transformation:
+      assert parameter.is_double or parameter.grid
       elements = numpy.log10(elements).tolist()
+
+    var_type = parameter.type if not parameter.grid else QUANTIZED_EXPERIMENT_PARAMETER_NAME
     return var_type, elements
 
   @staticmethod
   def parameter_to_prior_info(parameter):
-    if parameter.prior and parameter.prior.name == ParameterPriorNames.NORMAL:
-      name = ParameterPriorNames.NORMAL
+    if parameter.prior and parameter.prior.is_normal:
+      name = parameter.prior.name
       params = {
         "mean": parameter.prior.mean,
         "scale": parameter.prior.scale,
       }
-    elif parameter.prior and parameter.prior.name == ParameterPriorNames.BETA:
-      name = ParameterPriorNames.BETA
+    elif parameter.prior and parameter.prior.is_beta:
+      name = parameter.prior.name
       params = {
         "shape_a": parameter.prior.shape_a,
         "shape_b": parameter.prior.shape_b,
       }
     else:
       name = None
       params = None
@@ -252,47 +254,47 @@
       nonzero_coef_map = {a.name: a.weight for a in constraint.terms}
       constraint_vec = [0] * experiment.dimension
       var_type = None
 
       for index, p in enumerate(experiment.parameters):
         if p.name in nonzero_coef_map:
           constraint_vec[index] = nonzero_coef_map[p.name]
-          assert p.type in (DOUBLE_EXPERIMENT_PARAMETER_NAME, INT_EXPERIMENT_PARAMETER_NAME)
+          assert p.is_double or p.is_int
           var_type = p.type
 
       sign = -1 if constraint.type == ConstraintType.less_than else 1
       weights = [sign * v for v in constraint_vec]
       rhs = sign * constraint.threshold
       constraint_list.append({"weights": weights, "rhs": rhs, "var_type": var_type})
     return constraint_list
 
   @staticmethod
   def make_assignments_from_point(experiment, point):
     parameters = experiment.parameters
     assignments = {}
     for assignment, parameter in zip(point, parameters):
-      if parameter.transformation == ParameterTransformationNames.LOG:
+      if parameter.has_log_transformation:
         assignment = 10**assignment
-      if parameter.type in (INT_EXPERIMENT_PARAMETER_NAME, CATEGORICAL_EXPERIMENT_PARAMETER_NAME):
+      if parameter.is_categorical or parameter.is_int:
         assignment = round(assignment)
-      if parameter.type == CATEGORICAL_EXPERIMENT_PARAMETER_NAME:
+      if parameter.is_categorical:
         assignment = next(cv.name for cv in parameter.categorical_values if cv.enum_index == assignment)
       assignments[parameter.name] = assignment
     return assignments
 
   @staticmethod
   def get_point_from_assignments(experiment, assignments):
     point = numpy.empty(experiment.dimension)
     for i, parameter in enumerate(experiment.parameters):
       parameter_value = assignments.get(parameter.name, None)
       if parameter_value is None:
         parameter_value = replacement_value_if_missing(parameter)
-      if parameter.transformation == ParameterTransformationNames.LOG:
+      if parameter.has_log_transformation:
         parameter_value = numpy.log10(parameter_value)
-      elif parameter.type == CATEGORICAL_EXPERIMENT_PARAMETER_NAME:
+      elif parameter.is_categorical:
         parameter_value = next(cv.enum_index for cv in parameter.categorical_values if cv.name == parameter_value)
       point[i] = parameter_value
     return point
 
   @staticmethod
   def convert_conditional_to_categorical_parameter(conditional):
     return dict(
@@ -333,15 +335,15 @@
       "domain_info": self.form_domain_info(self.experiment),
       "model_info": self.form_gp_model_info(observations, hyperparameters),
       "points_sampled": self.make_points_sampled(self.experiment, observations),
       "tag": {},
       "metrics_info": self.form_metrics_info(self.experiment),
       "task_options": [t.cost for t in self.experiment.tasks],
     }
-    response = GpHyperOptMultimetricView(view_input).view()
+    response = self.call_libsigopt_views(GpHyperOptMultimetricView, view_input)
     self.hyperparameters = response["hyperparameter_dict"]
     return self.hyperparameters
 
   def next_point(self, observations):
     assert self.hyperparameters is not None
     points_sampled = self.make_points_sampled(self.experiment, observations)
     view_input = {
@@ -352,18 +354,19 @@
       "points_sampled": points_sampled,
       "points_being_sampled": EMPTY_POINTS_CONTAINER,
       "tag": {},
       "metrics_info": self.form_metrics_info(self.experiment, points_sampled),
       "task_options": [t.cost for t in self.experiment.tasks],
     }
     if self.experiment.is_search or self.experiment.is_multisolution:
-      response = SearchNextPoints(view_input).view()
+      view_endpoint = SearchNextPoints
     else:
-      response = GpNextPointsCategorical(view_input).view()
+      view_endpoint = GpNextPointsCategorical
 
+    response = self.call_libsigopt_views(view_endpoint, view_input)
     suggested_points = [[float(coord) for coord in point] for point in response["points_to_sample"]]
     task_cost = None
     if self.experiment.is_multitask:
       task_cost = response["task_costs"][0]
 
     return suggested_points[0], task_cost
 
@@ -378,21 +381,21 @@
       "length_scales": [[cls.default_lengthscales(p)] for p in experiment.parameters],
       "tikhonov": None,
       "task_length": DEFAULT_HYPERPARAMETER_TASK_LENGTH_SCALE if experiment.is_multitask else None,
     }
 
   @staticmethod
   def default_lengthscales(parameter):
-    if parameter.type == CATEGORICAL_EXPERIMENT_PARAMETER_NAME:
+    if parameter.is_categorical:
       return None
     if parameter.grid:
       return max(numpy.diff(parameter.grid))
     edge_length = parameter.bounds.max - parameter.bounds.min
     default = 0.1 * edge_length
-    if parameter.type == INT_EXPERIMENT_PARAMETER_NAME:
+    if parameter.is_int:
       default = max(default, 0.5)
     return default
 
 
 class SPESource(BaseOptimizationSource):
   def next_point(self, observations):
     points_sampled = self.make_points_sampled(self.experiment, observations[::-1])
@@ -402,34 +405,36 @@
       "points_sampled": points_sampled,
       "points_being_sampled": EMPTY_POINTS_CONTAINER,
       "tag": {},
       "metrics_info": self.form_metrics_info(self.experiment, points_sampled),
       "task_options": [t.cost for t in self.experiment.tasks],
     }
     if self.experiment.is_search or self.experiment.is_multisolution:
-      response = SPESearchNextPoints(view_input).view()
+      view_endpoint = SPESearchNextPoints
     else:
-      response = SPENextPoints(view_input).view()
-    suggested_points = [[float(coord) for coord in point] for point in response["points_to_sample"]]
+      view_endpoint = SPENextPoints
 
+    response = self.call_libsigopt_views(view_endpoint, view_input)
+    suggested_points = [[float(coord) for coord in point] for point in response["points_to_sample"]]
     task_cost = None
     if self.experiment.is_multitask:
       task_cost = response["task_costs"][0]
 
     return suggested_points[0], task_cost
 
 
 class RandomSearchSource(BaseOptimizationSource):
   def next_point(self, _):
-    domain_info = self.form_domain_info(self.experiment)
-    domain = CategoricalDomain(**asdict(domain_info))
-    if domain_info.priors and not domain_info.constraint_list:
-      samples = domain.generate_random_points_according_to_priors(1)
-    else:
-      samples = domain.generate_quasi_random_points_in_domain(1)
+    view_input = {
+      "domain_info": self.form_domain_info(self.experiment),
+      "num_to_sample": 1,
+      "tag": {},
+      "task_options": [t.cost for t in self.experiment.tasks],
+    }
+    response = self.call_libsigopt_views(RandomSearchNextPoints, view_input)
+    suggested_points = [[float(coord) for coord in point] for point in response["points_to_sample"]]
 
     task_cost = None
     if self.experiment.is_multitask:
-      tasks_costs = [t.cost for t in self.experiment.tasks]
-      task_cost = numpy.random.choice(tasks_costs)
+      task_cost = response["task_costs"][0]
 
-    return samples[0], task_cost
+    return suggested_points[0], task_cost
```

