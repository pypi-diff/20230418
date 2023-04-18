# Comparing `tmp/ms2query-0.7.3.2.tar.gz` & `tmp/ms2query-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-0.7.3.2.tar", last modified: Thu Mar 30 13:19:59 2023, max compression
+gzip compressed data, was "dist/ms2query-0.7.4.tar", last modified: Tue Apr 18 15:38:24 2023, max compression
```

## Comparing `ms2query-0.7.3.2.tar` & `ms2query-0.7.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/ms2query/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 13:19:58.000000 ms2query-0.7.3.2/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:59.000000 ms2query-0.7.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_use_files_without_spectrum_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-03-30 13:19:45.000000 ms2query-0.7.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-18 15:38:24.000000 ms2query-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-04-18 15:38:13.000000 ms2query-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-18 15:38:24.000000 ms2query-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-18 15:38:14.000000 ms2query-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_use_files_without_spectrum_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_utils.py
```

### Comparing `ms2query-0.7.3.2/PKG-INFO` & `ms2query-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 0.7.3.2
+Version: 0.7.4
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-0.7.3.2/README.md` & `ms2query-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/__init__.py` & `ms2query-0.7.4/ms2query/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-0.7.4/ms2query/benchmarking/collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-0.7.4/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-0.7.4/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-0.7.4/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-0.7.4/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/clean_and_filter_spectra.py` & `ms2query-0.7.4/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-0.7.4/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-0.7.4/ms2query/create_new_library/create_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/library_files_creator.py` & `ms2query-0.7.4/ms2query/create_new_library/library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/split_data_for_training.py` & `ms2query-0.7.4/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/train_models.py` & `ms2query-0.7.4/ms2query/create_new_library/train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/train_ms2deepscore.py` & `ms2query-0.7.4/ms2query/create_new_library/train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-0.7.4/ms2query/create_new_library/train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/ms2library.py` & `ms2query-0.7.4/ms2query/ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/old_query_from_sqlite_functions.py` & `ms2query-0.7.4/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/query_from_sqlite_database.py` & `ms2query-0.7.4/ms2query/query_from_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/results_table.py` & `ms2query-0.7.4/ms2query/results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/run_ms2query.py` & `ms2query-0.7.4/ms2query/run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query/utils.py` & `ms2query-0.7.4/ms2query/utils.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/ms2query.egg-info/PKG-INFO` & `ms2query-0.7.4/ms2query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 0.7.3.2
+Version: 0.7.4
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-0.7.3.2/ms2query.egg-info/SOURCES.txt` & `ms2query-0.7.4/ms2query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/setup.py` & `ms2query-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "h5py",
         "tensorflow-macos<2.9;platform_machine=='arm64'", #Add for Macos M1 chip compatability
         "tensorflow-metal==0.5.0;platform_machine=='arm64'",
         "tensorflow<2.9;platform_machine!='arm64'", #tensorflow <2.9 for change in error bar plotting
         "scikit-learn",
         "ms2deepscore<0.3.1",
         "gensim>=4.0.0",
-        "pandas>=1.2.5",
+        "pandas>=1.2.5,<2.0.0",
         "matchmsextras>=0.3.0,<0.4.0",
         "pubchempy", #This is a dependency for matchmsextras, which is missing in setup
         "tqdm",
         "matplotlib",
         "skl2onnx",
         "onnxruntime",
     ],
```

### Comparing `ms2query-0.7.3.2/tests/test_calculate_tanimoto_scores.py` & `ms2query-0.7.4/tests/test_calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_clean_and_filter_spectra.py` & `ms2query-0.7.4/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_collect_test_data_results.py` & `ms2query-0.7.4/tests/test_collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_library_files_creator.py` & `ms2query-0.7.4/tests/test_library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_ms2library.py` & `ms2query-0.7.4/tests/test_ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_results_table.py` & `ms2query-0.7.4/tests/test_results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_run_ms2query.py` & `ms2query-0.7.4/tests/test_run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_split_data_for_training.py` & `ms2query-0.7.4/tests/test_split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_sqlite.py` & `ms2query-0.7.4/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_train_models.py` & `ms2query-0.7.4/tests/test_train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_train_ms2deepscore.py` & `ms2query-0.7.4/tests/test_train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_train_ms2query_model.py` & `ms2query-0.7.4/tests/test_train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_use_files_without_spectrum_id.py` & `ms2query-0.7.4/tests/test_use_files_without_spectrum_id.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.3.2/tests/test_utils.py` & `ms2query-0.7.4/tests/test_utils.py`

 * *Files identical despite different names*

