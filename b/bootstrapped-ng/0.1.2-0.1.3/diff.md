# Comparing `tmp/bootstrapped-ng-0.1.2.tar.gz` & `tmp/bootstrapped-ng-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapped-ng-0.1.2.tar", last modified: Tue Apr 18 13:22:55 2023, max compression
+gzip compressed data, was "bootstrapped-ng-0.1.3.tar", last modified: Tue Apr 18 16:01:27 2023, max compression
```

## Comparing `bootstrapped-ng-0.1.2.tar` & `bootstrapped-ng-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/LICENSE-examples
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/bootstrapped/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/compare_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/bootstrapped/stats_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-18 13:22:55.000000 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-18 13:22:55.000000 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:22:55.000000 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 13:22:55.000000 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 13:22:55.000000 bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:22:55.064239 bootstrapped-ng-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-04-18 13:22:43.000000 bootstrapped-ng-0.1.2/tests/test_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/LICENSE-examples
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/bootstrapped/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/compare_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/bootstrapped/stats_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-18 16:01:27.000000 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-18 16:01:27.000000 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:01:27.000000 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 16:01:27.000000 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 16:01:27.000000 bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:01:27.393725 bootstrapped-ng-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-04-18 16:01:17.000000 bootstrapped-ng-0.1.3/tests/test_bootstrap.py
```

### Comparing `bootstrapped-ng-0.1.2/LICENSE` & `bootstrapped-ng-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/LICENSE-examples` & `bootstrapped-ng-0.1.3/LICENSE-examples`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/PKG-INFO` & `bootstrapped-ng-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapped-ng
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementations of the percentile based bootstrap - forked
 Home-page: https://github.com/athenianco/bootstrapped
 Author: Spencer Beecher
 Author-email: spencebeecher@gmail.com
 Maintainer: Vadim Markovtsev
 Maintainer-email: vadim@athenian.co
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bootstrapped-ng-0.1.2/README.rst` & `bootstrapped-ng-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/bootstrapped/bootstrap.py` & `bootstrapped-ng-0.1.3/bootstrapped/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
 def bootstrap(
     values,
     stat_func,
     denominator_values=None,
     alpha=0.05,
     num_iterations=10000,
-    iteration_batch_size=10,
+    iteration_batch_size=None,
     is_pivotal=True,
     num_threads=1,
     return_distribution=False,
 ):
     """Calculate the bootstrap estimate.
 
     Args:
@@ -351,15 +351,15 @@
             analysis slower. Defaults to 10000.
         iteration_batch_size: The bootstrap sample can generate very large
             matrices. This argument limits the memory footprint by
             batching bootstrap rounds. If unspecified the underlying code
             will produce a matrix of len(values) x num_iterations. If specified
             the code will produce sets of len(values) x iteration_batch_size
             (one at a time) until num_iterations have been simulated.
-            Defaults to 10. Passing None will calculate the full simulation in one step.
+            Defaults to None. Passing None will calculate the full simulation in one step.
         is_pivotal: if true, use the pivotal method for bootstrapping confidence
             intervals. If false, use the percentile method.
         num_threads: The number of therads to use. This speeds up calculation of
             the bootstrap. Defaults to 1. If -1 is specified then
             multiprocessing.cpu_count() is used instead.
     Returns:
         BootstrapResults representing CI and estimated value.
@@ -407,15 +407,15 @@
     ctrl,
     stat_func,
     compare_func,
     test_denominator=None,
     ctrl_denominator=None,
     alpha=0.05,
     num_iterations=10000,
-    iteration_batch_size=10,
+    iteration_batch_size=None,
     scale_test_by=1.0,
     is_pivotal=True,
     num_threads=1,
     return_distribution=False,
 ):
     """Calculate the bootstrap confidence intervals for an A/B test.
 
@@ -447,15 +447,15 @@
         num_iterations: number of bootstrap iterations to run. The higher this
             number the more sure you can be about the stability your bootstrap.
             By this - we mean the returned interval should be consistent across
             runs for the same input. This also consumes more memory and makes
             analysis slower.
         iteration_batch_size: The bootstrap sample can generate very large
             arrays. This function iteration_batch_size limits the memory
-            footprint by batching bootstrap rounds. Defaults to 10. Passing None
+            footprint by batching bootstrap rounds. Defaults to None. Passing None
             will attempt to calculate the full simulation in one step.
         scale_test_by: The ratio between test and control population
             sizes. Use this if your test and control split is different from a
             50/50 split. Defaults to 1.0.
         is_pivotal: if true, use the pivotal method for bootstrapping confidence
             intervals. If false, use the percentile method.
         num_threads: The number of therads to use. This speeds up calculation of
```

### Comparing `bootstrapped-ng-0.1.2/bootstrapped/compare_functions.py` & `bootstrapped-ng-0.1.3/bootstrapped/compare_functions.py`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/bootstrapped/permutation.py` & `bootstrapped-ng-0.1.3/bootstrapped/permutation.py`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/bootstrapped/power.py` & `bootstrapped-ng-0.1.3/bootstrapped/power.py`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/bootstrapped/stats_functions.py` & `bootstrapped-ng-0.1.3/bootstrapped/stats_functions.py`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/bootstrapped_ng.egg-info/PKG-INFO` & `bootstrapped-ng-0.1.3/bootstrapped_ng.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapped-ng
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementations of the percentile based bootstrap - forked
 Home-page: https://github.com/athenianco/bootstrapped
 Author: Spencer Beecher
 Author-email: spencebeecher@gmail.com
 Maintainer: Vadim Markovtsev
 Maintainer-email: vadim@athenian.co
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bootstrapped-ng-0.1.2/pyproject.toml` & `bootstrapped-ng-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/setup.py` & `bootstrapped-ng-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `bootstrapped-ng-0.1.2/tests/test_bootstrap.py` & `bootstrapped-ng-0.1.3/tests/test_bootstrap.py`

 * *Files identical despite different names*

