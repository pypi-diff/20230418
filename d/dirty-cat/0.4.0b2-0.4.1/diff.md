# Comparing `tmp/dirty_cat-0.4.0b2.tar.gz` & `tmp/dirty_cat-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirty_cat-0.4.0b2.tar", last modified: Wed Feb  1 10:15:35 2023, max compression
+gzip compressed data, was "dirty_cat-0.4.1.tar", last modified: Tue Apr 18 15:59:32 2023, max compression
```

## Comparing `dirty_cat-0.4.0b2.tar` & `dirty_cat-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.110334 dirty_cat-0.4.0b2/
--rw-rw-r--   0 soda      (1000) soda      (1000)     1530 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/LICENSE.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)     4722 2023-02-01 10:15:35.110334 dirty_cat-0.4.0b2/PKG-INFO
--rw-rw-r--   0 soda      (1000) soda      (1000)     3750 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/README.rst
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/benchmarks/
--rw-rw-r--   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    15804 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/bench_minhash.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     2248 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/encoders_time_memory_bench.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     6887 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/fuzzy_join_benchmark.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     2882 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/fuzzy_join_full_benchmark.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     1637 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/get_results.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     5991 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/similarity_scores_time_benchmark.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     4079 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/supervectorizer_tuning.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/benchmarks/utils/
--rw-rw-r--   0 soda      (1000) soda      (1000)      157 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/utils/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      657 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/utils/_argparser.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     1847 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/utils/_various.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     7777 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/benchmarks/utils/monitor.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/dirty_cat/
--rw-rw-r--   0 soda      (1000) soda      (1000)        8 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/VERSION.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)     1083 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      937 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_check_dependencies.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    10221 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_datetime_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     8406 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_deduplicate.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     2927 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_fast_hash.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     7248 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_feature_augmenter.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    10428 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_fuzzy_join.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    40454 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_gap_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    11776 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_minhash_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    25006 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_similarity_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     3471 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_string_distances.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    28755 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_super_vectorizer.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    11772 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_target_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     1877 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/_utils.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/dirty_cat/datasets/
--rw-rw-r--   0 soda      (1000) soda      (1000)      700 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    24948 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/_fetching.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     2093 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/_generating.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      561 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/_utils.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/dirty_cat/datasets/tests/
--rw-rw-r--   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/tests/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    15293 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/tests/test_fetching.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      574 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/tests/test_generating.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      565 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/datasets/tests/test_utils.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.110334 dirty_cat-0.4.0b2/dirty_cat/tests/
--rw-rw-r--   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/__init__.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    11246 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_datetime_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     4678 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_deduplicate.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     8006 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_docstrings.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      533 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_fast_hash.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     2137 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_feature_augmenter.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     7252 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_fuzzy_join.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     6998 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_gap_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     8625 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_minhash_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    12571 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_similarity_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      704 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_sklearn.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     1356 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_string_distances.py
--rw-rw-r--   0 soda      (1000) soda      (1000)    14669 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_super_vectorizer.py
--rw-rw-r--   0 soda      (1000) soda      (1000)     9323 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_target_encoder.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      290 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/test_utils.py
--rw-rw-r--   0 soda      (1000) soda      (1000)      829 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/dirty_cat/tests/utils.py
-drwxrwxr-x   0 soda      (1000) soda      (1000)        0 2023-02-01 10:15:35.106334 dirty_cat-0.4.0b2/dirty_cat.egg-info/
--rw-rw-r--   0 soda      (1000) soda      (1000)     4722 2023-02-01 10:15:34.000000 dirty_cat-0.4.0b2/dirty_cat.egg-info/PKG-INFO
--rw-rw-r--   0 soda      (1000) soda      (1000)     1895 2023-02-01 10:15:35.000000 dirty_cat-0.4.0b2/dirty_cat.egg-info/SOURCES.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)        1 2023-02-01 10:15:34.000000 dirty_cat-0.4.0b2/dirty_cat.egg-info/dependency_links.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)      475 2023-02-01 10:15:34.000000 dirty_cat-0.4.0b2/dirty_cat.egg-info/requires.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)       21 2023-02-01 10:15:34.000000 dirty_cat-0.4.0b2/dirty_cat.egg-info/top_level.txt
--rw-rw-r--   0 soda      (1000) soda      (1000)      450 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/pyproject.toml
--rw-rw-r--   0 soda      (1000) soda      (1000)     2237 2023-02-01 10:15:35.110334 dirty_cat-0.4.0b2/setup.cfg
--rw-rw-r--   0 soda      (1000) soda      (1000)       70 2023-02-01 10:15:26.000000 dirty_cat-0.4.0b2/setup.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.082035 dirty_cat-0.4.1/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1559 2022-12-15 14:22:51.000000 dirty_cat-0.4.1/LICENSE.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     4720 2023-04-18 15:59:32.082035 dirty_cat-0.4.1/PKG-INFO
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     3839 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/README.rst
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.070035 dirty_cat-0.4.1/benchmarks/
+-rw-r--r--   0 lboulard  (1000) lboulard  (1000)     4980 2022-11-18 17:28:09.000000 dirty_cat-0.4.1/benchmarks/3_compare_encoders_perfs.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)        0 2022-12-14 14:00:43.000000 dirty_cat-0.4.1/benchmarks/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    15649 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/bench_minhash_batch.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    13490 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/benchmark_fuzzy_join_hash.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2333 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/benchmarks/encoders_time_memory_bench.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     7315 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/fuzzy_join_benchmark.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2982 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/benchmarks/fuzzy_join_full_benchmark.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1690 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/benchmarks/get_results.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     6203 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/benchmarks/similarity_scores_time_benchmark.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     4225 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/benchmarks/tablevectorizer_tuning.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.070035 dirty_cat-0.4.1/benchmarks/utils/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      143 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/utils/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      679 2023-01-06 13:56:48.000000 dirty_cat-0.4.1/benchmarks/utils/_argparser.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1847 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/utils/_various.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8816 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/benchmarks/utils/monitor.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.074035 dirty_cat-0.4.1/dirty_cat/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)        7 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/VERSION.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1166 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/dirty_cat/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      967 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/dirty_cat/_check_dependencies.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    10907 2023-03-02 10:15:26.000000 dirty_cat-0.4.1/dirty_cat/_datetime_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     9046 2023-03-02 10:15:26.000000 dirty_cat-0.4.1/dirty_cat/_deduplicate.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     3017 2022-12-16 17:31:29.000000 dirty_cat-0.4.1/dirty_cat/_fast_hash.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8254 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/_feature_augmenter.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    18067 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/_fuzzy_join.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    41950 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/_gap_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    12509 2023-03-02 10:15:26.000000 dirty_cat-0.4.1/dirty_cat/_minhash_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    26501 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/_similarity_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     3586 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/dirty_cat/_string_distances.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    34461 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/_table_vectorizer.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    12494 2023-03-02 10:15:26.000000 dirty_cat-0.4.1/dirty_cat/_target_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1945 2023-01-06 13:56:48.000000 dirty_cat-0.4.1/dirty_cat/_utils.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.074035 dirty_cat-0.4.1/dirty_cat/datasets/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      927 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/datasets/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    31058 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/datasets/_fetching.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2153 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/datasets/_generating.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8165 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/datasets/_ken_embeddings.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      579 2022-12-15 14:22:51.000000 dirty_cat-0.4.1/dirty_cat/datasets/_utils.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.078035 dirty_cat-0.4.1/dirty_cat/datasets/tests/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)        0 2022-09-15 13:17:28.000000 dirty_cat-0.4.1/dirty_cat/datasets/tests/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     6376 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/datasets/tests/test_fetching.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      603 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/datasets/tests/test_generating.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1850 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/datasets/tests/test_ken_embeddings.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      583 2022-12-16 17:32:43.000000 dirty_cat-0.4.1/dirty_cat/datasets/tests/test_utils.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.082035 dirty_cat-0.4.1/dirty_cat/tests/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)        0 2022-12-15 14:22:51.000000 dirty_cat-0.4.1/dirty_cat/tests/__init__.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    11601 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/test_datetime_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     4802 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/test_deduplicate.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8868 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/dirty_cat/tests/test_docstrings.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      550 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/dirty_cat/tests/test_fast_hash.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2229 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/test_feature_augmenter.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    11813 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/tests/test_fuzzy_join.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8975 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/tests/test_gap_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     8806 2023-03-02 10:15:26.000000 dirty_cat-0.4.1/dirty_cat/tests/test_minhash_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    12968 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/test_similarity_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      737 2023-02-28 10:29:29.000000 dirty_cat-0.4.1/dirty_cat/tests/test_sklearn.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     1407 2022-12-15 14:22:51.000000 dirty_cat-0.4.1/dirty_cat/tests/test_string_distances.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)    20940 2023-04-18 15:53:14.000000 dirty_cat-0.4.1/dirty_cat/tests/test_table_vectorizer.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     9613 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/test_target_encoder.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      305 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/dirty_cat/tests/test_utils.py
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      858 2023-02-13 14:34:50.000000 dirty_cat-0.4.1/dirty_cat/tests/utils.py
+drwxrwxr-x   0 lboulard  (1000) lboulard  (1000)        0 2023-04-18 15:59:32.074035 dirty_cat-0.4.1/dirty_cat.egg-info/
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     4720 2023-04-18 15:59:31.000000 dirty_cat-0.4.1/dirty_cat.egg-info/PKG-INFO
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2066 2023-04-18 15:59:31.000000 dirty_cat-0.4.1/dirty_cat.egg-info/SOURCES.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)        1 2023-04-18 15:59:31.000000 dirty_cat-0.4.1/dirty_cat.egg-info/dependency_links.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      528 2023-04-18 15:59:31.000000 dirty_cat-0.4.1/dirty_cat.egg-info/requires.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)       21 2023-04-18 15:59:31.000000 dirty_cat-0.4.1/dirty_cat.egg-info/top_level.txt
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)      478 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/pyproject.toml
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)     2295 2023-04-18 15:59:32.082035 dirty_cat-0.4.1/setup.cfg
+-rw-rw-r--   0 lboulard  (1000) lboulard  (1000)       75 2022-12-15 14:25:59.000000 dirty_cat-0.4.1/setup.py
```

### Comparing `dirty_cat-0.4.0b2/LICENSE.txt` & `dirty_cat-0.4.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2018-2022, The dirty_cat developers.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2018-2022, The dirty_cat developers.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `dirty_cat-0.4.0b2/PKG-INFO` & `dirty_cat-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirty_cat
-Version: 0.4.0b2
+Version: 0.4.1
 Summary: Machine learning with dirty categories.
 Author: Patricio Cerda
 Author-email: patricio.cerda@inria.fr
 License: BSD
 Project-URL: Homepage, https://dirty-cat.github.io/
 Project-URL: Source, https://github.com/dirty-cat/dirty_cat
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
 
 If you like the package, please *spread the word*, and ⭐ `the repository <https://github.com/dirty-cat/dirty_cat/>`_!
 
 What can `dirty_cat` do?
 ------------------------
 
-`dirty_cat` provides tools (``SuperVectorizer``, ``fuzzy_join``...) and
+`dirty_cat` provides tools (``TableVectorizer``, ``fuzzy_join``...) and
 encoders (``GapEncoder``, ``MinHashEncoder``...) for **morphological similarities**,
 for which we usually identify three common cases: **similarities, typos and variations**
 
 `The first example notebook <https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html>`_
 goes in-depth on how to identify and deal with dirty data using the `dirty_cat` library.
 
 What `dirty_cat` does not
```

### Comparing `dirty_cat-0.4.0b2/README.rst` & `dirty_cat-0.4.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-`dirty_cat`
-===========
-
-.. image:: https://dirty-cat.github.io/stable/_static/dirty_cat.svg
-   :align: center
-   :alt: dirty_cat logo
-
-
-|py_ver| |pypi_var| |pypi_dl| |codecov| |circleci| |black|
-
-.. |py_ver| image:: https://img.shields.io/pypi/pyversions/dirty_cat
-.. |pypi_var| image:: https://img.shields.io/pypi/v/dirty_cat?color=informational
-.. |pypi_dl| image:: https://img.shields.io/pypi/dm/dirty_cat
-.. |codecov| image:: https://img.shields.io/codecov/c/github/dirty-cat/dirty_cat/main
-.. |circleci| image:: https://img.shields.io/circleci/build/github/dirty-cat/dirty_cat/main?label=CircleCI
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-
-`dirty_cat <https://dirty-cat.github.io/>`_ is a Python library
-that facilitates machine-learning on dirty categorical variables.
-
-For a detailed description of the problem of encoding dirty categorical data, see
-`Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
-and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
-
-If you like the package, please *spread the word*, and ⭐ `the repository <https://github.com/dirty-cat/dirty_cat/>`_!
-
-What can `dirty_cat` do?
-------------------------
-
-`dirty_cat` provides tools (``SuperVectorizer``, ``fuzzy_join``...) and
-encoders (``GapEncoder``, ``MinHashEncoder``...) for **morphological similarities**,
-for which we usually identify three common cases: **similarities, typos and variations**
-
-`The first example notebook <https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html>`_
-goes in-depth on how to identify and deal with dirty data using the `dirty_cat` library.
-
-What `dirty_cat` does not
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-`Semantic similarities <https://en.wikipedia.org/wiki/Semantic_similarity>`_
-are currently not supported.
-For example, the similarity between *car* and *automobile* is outside the reach
-of the methods implemented here.
-
-This kind of problem is tackled by
-`Natural Language Processing <https://en.wikipedia.org/wiki/Natural_language_processing>`_
-methods.
-
-`dirty_cat` can still help with handling typos and variations in this kind of setting.
-
-Installation
-------------
-
-dirty_cat can be easily installed via `pip`::
-
-    pip install dirty_cat
-
-Dependencies
-~~~~~~~~~~~~
-
-Dependencies and minimal versions are listed in the `setup <https://github.com/dirty-cat/dirty_cat/blob/main/setup.cfg#L26>`_ file.
-
-Related projects
-----------------
-
-Are listed on the `dirty_cat's website <https://dirty-cat.github.io/stable/#related-projects>`_
-
-Contributing
-------------
-
-If you want to encourage development of `dirty_cat`,
-the best thing to do is to *spread the word*!
-
-If you encounter an issue while using `dirty_cat`, please
-`open an issue <https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue>`_ and/or
-`submit a pull request <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>`_.
-Don't hesitate, you're helping to make this project better for everyone!
-
-Additional resources
---------------------
-
-* `Introductory video (YouTube) <https://youtu.be/_GNaaeEI2tg>`_
-* `Overview poster for EuroSciPy 2022 (Google Drive) <https://drive.google.com/file/d/1TtmJ3VjASy6rGlKe0txKacM-DdvJdIvB/view?usp=sharing>`_
-
-References
-----------
-
-.. [1] Patricio Cerda, Gaël Varoquaux, Balázs Kégl. Similarity encoding for learning with dirty categorical variables. 2018. Machine Learning journal, Springer.
-.. [2] Patricio Cerda, Gaël Varoquaux. Encoding high-cardinality string categorical variables. 2020. IEEE Transactions on Knowledge & Data Engineering.
+`dirty_cat`
+===========
+
+.. image:: https://dirty-cat.github.io/stable/_static/dirty_cat.svg
+   :align: center
+   :alt: dirty_cat logo
+
+
+|py_ver| |pypi_var| |pypi_dl| |codecov| |circleci| |black|
+
+.. |py_ver| image:: https://img.shields.io/pypi/pyversions/dirty_cat
+.. |pypi_var| image:: https://img.shields.io/pypi/v/dirty_cat?color=informational
+.. |pypi_dl| image:: https://img.shields.io/pypi/dm/dirty_cat
+.. |codecov| image:: https://img.shields.io/codecov/c/github/dirty-cat/dirty_cat/main
+.. |circleci| image:: https://img.shields.io/circleci/build/github/dirty-cat/dirty_cat/main?label=CircleCI
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+`dirty_cat <https://dirty-cat.github.io/>`_ is a Python library
+that facilitates machine-learning on dirty categorical variables.
+
+For a detailed description of the problem of encoding dirty categorical data, see
+`Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
+and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
+
+If you like the package, please *spread the word*, and ⭐ `the repository <https://github.com/dirty-cat/dirty_cat/>`_!
+
+What can `dirty_cat` do?
+------------------------
+
+`dirty_cat` provides tools (``TableVectorizer``, ``fuzzy_join``...) and
+encoders (``GapEncoder``, ``MinHashEncoder``...) for **morphological similarities**,
+for which we usually identify three common cases: **similarities, typos and variations**
+
+`The first example notebook <https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html>`_
+goes in-depth on how to identify and deal with dirty data using the `dirty_cat` library.
+
+What `dirty_cat` does not
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+`Semantic similarities <https://en.wikipedia.org/wiki/Semantic_similarity>`_
+are currently not supported.
+For example, the similarity between *car* and *automobile* is outside the reach
+of the methods implemented here.
+
+This kind of problem is tackled by
+`Natural Language Processing <https://en.wikipedia.org/wiki/Natural_language_processing>`_
+methods.
+
+`dirty_cat` can still help with handling typos and variations in this kind of setting.
+
+Installation
+------------
+
+dirty_cat can be easily installed via `pip`::
+
+    pip install dirty_cat
+
+Dependencies
+~~~~~~~~~~~~
+
+Dependencies and minimal versions are listed in the `setup <https://github.com/dirty-cat/dirty_cat/blob/main/setup.cfg#L26>`_ file.
+
+Related projects
+----------------
+
+Are listed on the `dirty_cat's website <https://dirty-cat.github.io/stable/#related-projects>`_
+
+Contributing
+------------
+
+If you want to encourage development of `dirty_cat`,
+the best thing to do is to *spread the word*!
+
+If you encounter an issue while using `dirty_cat`, please
+`open an issue <https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue>`_ and/or
+`submit a pull request <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>`_.
+Don't hesitate, you're helping to make this project better for everyone!
+
+Additional resources
+--------------------
+
+* `Introductory video (YouTube) <https://youtu.be/_GNaaeEI2tg>`_
+* `Overview poster for EuroSciPy 2022 (Google Drive) <https://drive.google.com/file/d/1TtmJ3VjASy6rGlKe0txKacM-DdvJdIvB/view?usp=sharing>`_
+
+References
+----------
+
+.. [1] Patricio Cerda, Gaël Varoquaux, Balázs Kégl. Similarity encoding for learning with dirty categorical variables. 2018. Machine Learning journal, Springer.
+.. [2] Patricio Cerda, Gaël Varoquaux. Encoding high-cardinality string categorical variables. 2020. IEEE Transactions on Knowledge & Data Engineering.
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/bench_minhash.py` & `dirty_cat-0.4.1/benchmarks/bench_minhash_batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,470 +1,451 @@
-#################
-# The MinHashEncoder version used for the benchmark
-# On the main branch, we only kept the best version of the MinHashEncoder
-# which is the batched version
-# with batch_per_job=1
-# (the batch_per_job parameter has no effect on the results)
-#################
-
-from typing import Callable, Collection, Dict, List, Literal, Tuple
-
-import numpy as np
-from joblib import Parallel, delayed, effective_n_jobs
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils import gen_even_slices, murmurhash3_32
-
-from dirty_cat._fast_hash import ngram_min_hash
-from dirty_cat._string_distances import get_unique_ngrams
-from dirty_cat._utils import LRUDict, check_input
-
-NoneType = type(None)
-
-
-# Ignore lines too long, as links in the docstring cannot be cut.
-# flake8: noqa: E501
-
-
-class MinHashEncoder(BaseEstimator, TransformerMixin):
-    """
-    Encode string categorical features as a numeric array, minhash method
-    applied to ngram decomposition of strings based on ngram decomposition
-    of the string.
-
-    Parameters
-    ----------
-    n_components : int, default=30
-        The number of dimension of encoded strings. Numbers around 300 tend to
-        lead to good prediction performance, but with more computational cost.
-    ngram_range : typing.Tuple[int, int], default=(2, 4)
-        The lower and upper boundary of the range of n-values for different
-        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
-        will be used.
-    hashing : typing.Literal["fast", "murmur"], default=fast
-        Hashing function. fast is faster but
-        might have some concern with its entropy.
-    minmax_hash : bool, default=False
-        if True, return min hash and max hash concatenated.
-    handle_missing : typing.Literal["error", "zero_impute"], default=zero_impute
-        Whether to raise an error or encode missing values (NaN) with
-        vectors filled with zeros.
-    batch: bool, default=False
-        If False, parallelize the computation of the hash of each unique
-        element. If True, parallelize the computation of the hash of each
-        batch of elements.
-    batch_per_job: int, default=1
-        Number of batches to be processed in each job.
-    n_jobs : int, default=None
-        The number of jobs to run in parallel.
-        The hash computations for all unique elements are parallelized.
-        None means 1 unless in a
-        `joblib.parallel_backend context <https://joblib.readthedocs.io/en/latest/parallel.html>`_.
-        -1 means using all processors.
-        See `Scikit-learn Glossary <https://scikit-learn.org/stable/glossary.html#term-n_jobs>`_
-        for more details.
-
-    Attributes
-    ----------
-    hash_dict_ : LRUDict
-        Computed hashes.
-
-    Examples
-    --------
-    >>> enc = MinHashEncoder(n_components=5)
-
-    Let's encode the following non-normalized data:
-
-    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['London']]
-
-    >>> enc.fit(X)
-    MinHashEncoder()
-
-    The encoded data with 5 components are:
-
-    >>> enc.transform(X)
-    array([[-1.78337518e+09, -1.58827021e+09, -1.66359234e+09,
-            -1.81988679e+09, -1.96259387e+09],
-           [-8.48046971e+08, -1.76657887e+09, -1.55891205e+09,
-            -1.48574446e+09, -1.68729890e+09],
-           [-1.97582893e+09, -2.09500033e+09, -1.59652117e+09,
-            -1.81759383e+09, -2.09569333e+09],
-           [-1.97582893e+09, -2.09500033e+09, -1.53072052e+09,
-            -1.45918266e+09, -1.58098831e+09]])
-
-    References
-    ----------
-    For a detailed description of the method, see
-    `Encoding high-cardinality string categorical variables
-    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
-
-    """
-
-    hash_dict_: LRUDict
-
-    _capacity: int = 2**10
-
-    def __init__(
-        self,
-        n_components: int = 30,
-        ngram_range: Tuple[int, int] = (2, 4),
-        hashing: Literal["fast", "murmur"] = "fast",
-        minmax_hash: bool = False,
-        handle_missing: Literal["error", "zero_impute"] = "zero_impute",
-        batch: bool = False,
-        batch_per_job: int = 1,
-        n_jobs: int = None,
-    ):
-        self.ngram_range = ngram_range
-        self.n_components = n_components
-        self.hashing = hashing
-        self.minmax_hash = minmax_hash
-        self.handle_missing = handle_missing
-        self.batch = batch
-        self.batch_per_job = batch_per_job
-        self.n_jobs = n_jobs
-
-    def _more_tags(self) -> Dict[str, List[str]]:
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def _get_murmur_hash(self, string: str) -> np.array:
-        """
-        Encode a string using murmur hashing function.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-
-        Returns
-        -------
-        ndarray of shape (n_components, )
-            The encoded string.
-        """
-        min_hashes = np.ones(self.n_components) * np.infty
-        grams = get_unique_ngrams(string, self.ngram_range)
-        if len(grams) == 0:
-            grams = get_unique_ngrams(" Na ", self.ngram_range)
-        for gram in grams:
-            hash_array = np.array(
-                [
-                    murmurhash3_32("".join(gram), seed=d, positive=True)
-                    for d in range(self.n_components)
-                ]
-            )
-            min_hashes = np.minimum(min_hashes, hash_array)
-        return min_hashes / (2**32 - 1)
-
-    def _get_fast_hash(self, string: str) -> np.array:
-        """
-        Encode a string with fast hashing function.
-        fast hashing supports both min_hash and minmax_hash encoding.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-
-        Returns
-        -------
-        ndarray of shape (n_components, )
-            The encoded string, using specified encoding scheme.
-        """
-        if self.minmax_hash:
-            return np.concatenate(
-                [
-                    ngram_min_hash(string, self.ngram_range, seed, return_minmax=True)
-                    for seed in range(self.n_components // 2)
-                ]
-            )
-        else:
-            return np.array(
-                [
-                    ngram_min_hash(string, self.ngram_range, seed)
-                    for seed in range(self.n_components)
-                ]
-            )
-
-    def _compute_hash(
-        self, string: str, hash_func: Callable[[str], np.ndarray]
-    ) -> np.ndarray:
-        """Function called to compute the hash of a string.
-
-        Check if the string is in the hash dictionary, if not, scompute the hash using
-        the specified hashing function and add it to the dictionary.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-        hash_func : callable
-            Hashing function to use on the string.
-
-        Returns
-        -------
-        np.array of shape (n_components, )
-            The encoded string, using specified encoding scheme.
-        """
-        if string not in self.hash_dict_:
-            if string == "NAN":  # true if x is a missing value
-                self.hash_dict_[string] = np.zeros(self.n_components)
-            else:
-                self.hash_dict_[string] = hash_func(string)
-        return self.hash_dict_[string]
-
-    def _compute_hash_batched(
-        self, batch: Collection[str], hash_func: Callable[[str], np.ndarray]
-    ):
-        """Function called to compute the hashes of a batch of strings.
-
-        Check if the string is in the hash dictionary, if not, compute the hash using
-        the specified hashing function and add it to the dictionary.
-
-        Parameters
-        ----------
-        batch : iterable of str
-            The batch of strings to encode.
-        hash_func : callable
-            Hashing function to use on the string.
-
-        Returns
-        -------
-        np.array of shape (n_samples, n_components)
-            The encoded strings, using specified encoding scheme.
-        """
-        res = np.zeros((len(batch), self.n_components))
-        for i, string in enumerate(batch):
-            if string not in self.hash_dict_:
-                if string == "NAN":  # true if x is a missing value
-                    self.hash_dict_[string] = np.zeros(self.n_components)
-                else:
-                    self.hash_dict_[string] = hash_func(string)
-            res[i] = self.hash_dict_[string]
-        return res
-
-    def fit(self, X, y=None) -> "MinHashEncoder":
-        """
-        Fit the MinHashEncoder to X. In practice, just initializes a dictionary
-        to store encodings to speed up computation.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
-            The string data to encode. Only here for compatibility.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        MinHashEncoder
-            The fitted MinHashEncoder instance.
-        """
-        if self.hashing not in ["fast", "murmur"]:
-            raise ValueError(
-                f"Got hashing={self.hashing!r}, "
-                'but expected any of {"fast", "murmur"}. '
-            )
-        if self.handle_missing not in ["error", "zero_impute"]:
-            raise ValueError(
-                f"Got handle_missing={self.handle_missing!r}, but expected "
-                'any of {"error", "zero_impute"}. '
-            )
-        self.hash_dict_ = LRUDict(capacity=self._capacity)
-        return self
-
-    def transform(self, X) -> np.array:
-        """
-        Transform X using specified encoding scheme.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
-            The string data to encode.
-
-        Returns
-        -------
-        ndarray of shape (n_samples, n_components)
-            Transformed input.
-        """
-        X = check_input(X)
-        if self.minmax_hash:
-            if self.n_components % 2 != 0:
-                raise ValueError(
-                    "n_components should be even when using"
-                    f"minmax_hash encoding, got {self.n_components}"
-                )
-        if self.hashing == "murmur":
-            if self.minmax_hash:
-                raise ValueError(
-                    "minmax_hash encoding is not supported"
-                    "with the murmur hashing function"
-                )
-        if self.handle_missing not in ["error", "zero_impute"]:
-            raise ValueError(
-                "handle_missing should be either "
-                f"'error' or 'zero_impute', got {self.handle_missing!r}"
-            )
-
-        # Handle missing values
-        missing_mask = (
-            ~(X == X)  # Find np.nan
-            | (X == None)  # Find None. Note: `X is None` doesn't work.
-            | (X == "")  # Find empty strings
-        )
-
-        if missing_mask.any():  # contains at least one missing value
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='zero_impute' to encode with missing values"
-                )
-            elif self.handle_missing == "zero_impute":
-                # NANs will be replaced by zeroes in _compute_hash
-                X[missing_mask] = "NAN"
-
-        if self.hashing == "fast":
-            hash_func = self._get_fast_hash
-        elif self.hashing == "murmur":
-            hash_func = self._get_murmur_hash
-        else:
-            raise ValueError(
-                "Hashing function should be either 'fast' or 'murmur', "
-                f"got {self.hashing!r}"
-            )
-
-        # Compute the hashes for unique values
-        unique_x, indices_x = np.unique(X, return_inverse=True)
-        n_jobs = effective_n_jobs(self.n_jobs)
-
-        if self.batch:
-            unique_x_trans = Parallel(n_jobs=n_jobs)(
-                delayed(self._compute_hash_batched)(
-                    unique_x[idx_slice],
-                    hash_func,
-                )
-                for idx_slice in gen_even_slices(
-                    len(unique_x), n_jobs * self.batch_per_job
-                )
-            )
-            # Match the hashes of the unique value to the original values
-            X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
-                len(X), X.shape[1] * self.n_components
-            )
-        else:
-            unique_x_trans = Parallel(n_jobs=n_jobs)(
-                delayed(self._compute_hash)(x, hash_func) for x in unique_x
-            )
-            # Match the hashes of the unique value to the original values
-            X_out = np.stack(unique_x_trans)[indices_x].reshape(
-                len(X), X.shape[1] * self.n_components
-            )
-
-        return X_out.astype(np.float64)  # The output is an int32 before conversion
-
-
-import pickle
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-from argparse import ArgumentParser
-
-from pathlib import Path
-
-from utils import monitor, parse_func_repr, find_result, default_parser
-from dirty_cat.tests.utils import generate_data
-
-benchmark_name = "minhash_batch_comparison"
-
-
-@monitor(
-    memory=True,
-    time=True,
-    parametrize={
-        "dataset_size": ["medium"],
-        "batched": [True, False],
-        "n_jobs": [1, 4, 8, 16, 32, 64],
-        "batch_per_job": [1, 2, 4],
-    },
-    save_as=benchmark_name,
-    repeat=10,
-)
-def benchmark(
-    dataset_size: str,
-    batched: bool,
-    n_jobs: int,
-    batch_per_job: int,
-) -> None:
-    X = data[dataset_size]
-    MinHashEncoder(batch=batched, n_jobs=n_jobs, batch_per_job=batch_per_job).fit(
-        X
-    ).transform(X)
-
-
-def plot(res: pd.DataFrame):
-    sns.set_theme(style="ticks", palette="pastel")
-
-    rows = []
-    for i, ser in res.iterrows():
-        times = eval(str(ser["time"]))
-        memories = eval(str(ser["memory"]))
-        _, _, kwargs = parse_func_repr(ser["call"])
-        for time, memory in zip(times, memories):
-            rows.append(
-                (
-                    kwargs["batched"],
-                    kwargs["batch_per_job"],
-                    kwargs["n_jobs"],
-                    time,
-                    memory,
-                )
-            )
-
-    df = pd.DataFrame(
-        rows, columns=["batched", "batch_per_job", "n_jobs", "time", "memory"]
-    )
-
-    # Create a new columns merging batched and batch_per_job
-    # If batch is False, ignore batch_per_job
-    df["config"] = df.apply(
-        lambda row: f"batched={row['batched']}, batch_per_job={row['batch_per_job']}"
-        if row["batched"] == "True"
-        else "batched=False",
-        axis=1,
-    )
-
-    sns.boxplot(x="n_jobs", y="time", hue="config", data=df)
-    plt.show()
-
-
-if __name__ == "__main__":
-    _args = ArgumentParser(
-        description="Benchmark for the batch feature of the MinHashEncoder.",
-        parents=[default_parser],
-    ).parse_args()
-
-    # Generate the data if not already on disk, and keep them in memory.
-    data = {}  # Will hold the datasets in memory.
-    _data_info = {
-        "small": 10_000,
-        "medium": 100_000,
-    }
-    for name, size in _data_info.items():
-        data_file = Path(f"data_{name}.pkl")
-        if data_file.is_file():
-            with data_file.open("rb") as fl:
-                data.update({name: pickle.load(fl)})
-        else:
-            with data_file.open("wb") as fl:
-                _gen = generate_data(size).reshape(-1, 1)
-                pickle.dump(_gen, fl)
-                data.update({name: _gen})
-
-    if _args.run:
-        df = benchmark()
-    else:
-        result_file = find_result(benchmark_name)
-        df = pd.read_csv(result_file)
-
-    if _args.plot:
-        plot(df)
+"""
+The MinHashEncoder version used for the benchmark.
+On the main branch, we only kept the best version of the MinHashEncoder
+which is the batched version with batch_per_job=1
+(the batch_per_job parameter has no effect on the results)
+"""
+
+from typing import Callable, Collection, Dict, List, Literal, Tuple
+
+import numpy as np
+from joblib import Parallel, delayed, effective_n_jobs
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils import gen_even_slices, murmurhash3_32
+
+from dirty_cat._fast_hash import ngram_min_hash
+from dirty_cat._string_distances import get_unique_ngrams
+from dirty_cat._utils import LRUDict, check_input
+
+NoneType = type(None)
+
+
+# Ignore lines too long, as links in the docstring cannot be cut.
+# flake8: noqa: E501
+
+
+class MinHashEncoder(BaseEstimator, TransformerMixin):
+    """
+    Encode string categorical features as a numeric array, minhash method
+    applied to ngram decomposition of strings based on ngram decomposition
+    of the string.
+
+    Parameters
+    ----------
+    n_components : int, default=30
+        The number of dimension of encoded strings. Numbers around 300 tend to
+        lead to good prediction performance, but with more computational cost.
+    ngram_range : typing.Tuple[int, int], default=(2, 4)
+        The lower and upper boundary of the range of n-values for different
+        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
+        will be used.
+    hashing : typing.Literal["fast", "murmur"], default=fast
+        Hashing function. fast is faster but
+        might have some concern with its entropy.
+    minmax_hash : bool, default=False
+        if True, return min hash and max hash concatenated.
+    handle_missing : typing.Literal["error", "zero_impute"], default=zero_impute
+        Whether to raise an error or encode missing values (NaN) with
+        vectors filled with zeros.
+    batch: bool, default=False
+        If False, parallelize the computation of the hash of each unique
+        element. If True, parallelize the computation of the hash of each
+        batch of elements.
+    batch_per_job: int, default=1
+        Number of batches to be processed in each job.
+    n_jobs : int, default=None
+        The number of jobs to run in parallel.
+        The hash computations for all unique elements are parallelized.
+        None means 1 unless in a
+        `joblib.parallel_backend context <https://joblib.readthedocs.io/en/latest/parallel.html>`_.
+        -1 means using all processors.
+        See `Scikit-learn Glossary <https://scikit-learn.org/stable/glossary.html#term-n_jobs>`_
+        for more details.
+
+    Attributes
+    ----------
+    hash_dict_ : LRUDict
+        Computed hashes.
+
+    Examples
+    --------
+    >>> enc = MinHashEncoder(n_components=5)
+
+    Let's encode the following non-normalized data:
+
+    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['London']]
+
+    >>> enc.fit(X)
+    MinHashEncoder()
+
+    The encoded data with 5 components are:
+
+    >>> enc.transform(X)
+    array([[-1.78337518e+09, -1.58827021e+09, -1.66359234e+09,
+            -1.81988679e+09, -1.96259387e+09],
+           [-8.48046971e+08, -1.76657887e+09, -1.55891205e+09,
+            -1.48574446e+09, -1.68729890e+09],
+           [-1.97582893e+09, -2.09500033e+09, -1.59652117e+09,
+            -1.81759383e+09, -2.09569333e+09],
+           [-1.97582893e+09, -2.09500033e+09, -1.53072052e+09,
+            -1.45918266e+09, -1.58098831e+09]])
+
+    References
+    ----------
+    For a detailed description of the method, see
+    `Encoding high-cardinality string categorical variables
+    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
+
+    """
+
+    hash_dict_: LRUDict
+
+    _capacity: int = 2**10
+
+    def __init__(
+        self,
+        n_components: int = 30,
+        ngram_range: Tuple[int, int] = (2, 4),
+        hashing: Literal["fast", "murmur"] = "fast",
+        minmax_hash: bool = False,
+        handle_missing: Literal["error", "zero_impute"] = "zero_impute",
+        batch: bool = False,
+        batch_per_job: int = 1,
+        n_jobs: int = None,
+    ):
+        self.ngram_range = ngram_range
+        self.n_components = n_components
+        self.hashing = hashing
+        self.minmax_hash = minmax_hash
+        self.handle_missing = handle_missing
+        self.batch = batch
+        self.batch_per_job = batch_per_job
+        self.n_jobs = n_jobs
+
+    def _more_tags(self) -> Dict[str, List[str]]:
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {"X_types": ["categorical"]}
+
+    def _get_murmur_hash(self, string: str) -> np.array:
+        """
+        Encode a string using murmur hashing function.
+
+        Parameters
+        ----------
+        string : str
+            The string to encode.
+
+        Returns
+        -------
+        ndarray of shape (n_components, )
+            The encoded string.
+        """
+        min_hashes = np.ones(self.n_components) * np.infty
+        grams = get_unique_ngrams(string, self.ngram_range)
+        if len(grams) == 0:
+            grams = get_unique_ngrams(" Na ", self.ngram_range)
+        for gram in grams:
+            hash_array = np.array(
+                [
+                    murmurhash3_32("".join(gram), seed=d, positive=True)
+                    for d in range(self.n_components)
+                ]
+            )
+            min_hashes = np.minimum(min_hashes, hash_array)
+        return min_hashes / (2**32 - 1)
+
+    def _get_fast_hash(self, string: str) -> np.array:
+        """
+        Encode a string with fast hashing function.
+        fast hashing supports both min_hash and minmax_hash encoding.
+
+        Parameters
+        ----------
+        string : str
+            The string to encode.
+
+        Returns
+        -------
+        ndarray of shape (n_components, )
+            The encoded string, using specified encoding scheme.
+        """
+        if self.minmax_hash:
+            return np.concatenate(
+                [
+                    ngram_min_hash(string, self.ngram_range, seed, return_minmax=True)
+                    for seed in range(self.n_components // 2)
+                ]
+            )
+        else:
+            return np.array(
+                [
+                    ngram_min_hash(string, self.ngram_range, seed)
+                    for seed in range(self.n_components)
+                ]
+            )
+
+    def _compute_hash(
+        self, string: str, hash_func: Callable[[str], np.ndarray]
+    ) -> np.ndarray:
+        """Function called to compute the hash of a string.
+
+        Check if the string is in the hash dictionary, if not, scompute the hash using
+        the specified hashing function and add it to the dictionary.
+
+        Parameters
+        ----------
+        string : str
+            The string to encode.
+        hash_func : callable
+            Hashing function to use on the string.
+
+        Returns
+        -------
+        np.array of shape (n_components, )
+            The encoded string, using specified encoding scheme.
+        """
+        if string not in self.hash_dict_:
+            if string == "NAN":  # true if x is a missing value
+                self.hash_dict_[string] = np.zeros(self.n_components)
+            else:
+                self.hash_dict_[string] = hash_func(string)
+        return self.hash_dict_[string]
+
+    def _compute_hash_batched(
+        self, batch: Collection[str], hash_func: Callable[[str], np.ndarray]
+    ):
+        """Function called to compute the hashes of a batch of strings.
+
+        Check if the string is in the hash dictionary, if not, compute the hash using
+        the specified hashing function and add it to the dictionary.
+
+        Parameters
+        ----------
+        batch : iterable of str
+            The batch of strings to encode.
+        hash_func : callable
+            Hashing function to use on the string.
+
+        Returns
+        -------
+        np.array of shape (n_samples, n_components)
+            The encoded strings, using specified encoding scheme.
+        """
+        res = np.zeros((len(batch), self.n_components))
+        for i, string in enumerate(batch):
+            if string not in self.hash_dict_:
+                if string == "NAN":  # true if x is a missing value
+                    self.hash_dict_[string] = np.zeros(self.n_components)
+                else:
+                    self.hash_dict_[string] = hash_func(string)
+            res[i] = self.hash_dict_[string]
+        return res
+
+    def fit(self, X, y=None) -> "MinHashEncoder":
+        """
+        Fit the MinHashEncoder to X. In practice, just initializes a dictionary
+        to store encodings to speed up computation.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, ) or (n_samples, 1)
+            The string data to encode. Only here for compatibility.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        MinHashEncoder
+            The fitted MinHashEncoder instance.
+        """
+        if self.hashing not in ["fast", "murmur"]:
+            raise ValueError(
+                f"Got hashing={self.hashing!r}, "
+                'but expected any of {"fast", "murmur"}. '
+            )
+        if self.handle_missing not in ["error", "zero_impute"]:
+            raise ValueError(
+                f"Got handle_missing={self.handle_missing!r}, but expected "
+                'any of {"error", "zero_impute"}. '
+            )
+        self.hash_dict_ = LRUDict(capacity=self._capacity)
+        return self
+
+    def transform(self, X) -> np.array:
+        """
+        Transform X using specified encoding scheme.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, ) or (n_samples, 1)
+            The string data to encode.
+
+        Returns
+        -------
+        ndarray of shape (n_samples, n_components)
+            Transformed input.
+        """
+        X = check_input(X)
+        if self.minmax_hash:
+            if self.n_components % 2 != 0:
+                raise ValueError(
+                    "n_components should be even when using"
+                    f"minmax_hash encoding, got {self.n_components}"
+                )
+        if self.hashing == "murmur":
+            if self.minmax_hash:
+                raise ValueError(
+                    "minmax_hash encoding is not supported"
+                    "with the murmur hashing function"
+                )
+        if self.handle_missing not in ["error", "zero_impute"]:
+            raise ValueError(
+                "handle_missing should be either "
+                f"'error' or 'zero_impute', got {self.handle_missing!r}"
+            )
+
+        # Handle missing values
+        missing_mask = (
+            ~(X == X)  # Find np.nan
+            | (X == None)  # Find None. Note: `X is None` doesn't work.
+            | (X == "")  # Find empty strings
+        )
+
+        if missing_mask.any():  # contains at least one missing value
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='zero_impute' to encode with missing values"
+                )
+            elif self.handle_missing == "zero_impute":
+                # NANs will be replaced by zeroes in _compute_hash
+                X[missing_mask] = "NAN"
+
+        if self.hashing == "fast":
+            hash_func = self._get_fast_hash
+        elif self.hashing == "murmur":
+            hash_func = self._get_murmur_hash
+        else:
+            raise ValueError(
+                "Hashing function should be either 'fast' or 'murmur', "
+                f"got {self.hashing!r}"
+            )
+
+        # Compute the hashes for unique values
+        unique_x, indices_x = np.unique(X, return_inverse=True)
+        n_jobs = effective_n_jobs(self.n_jobs)
+
+        if self.batch:
+            unique_x_trans = Parallel(n_jobs=n_jobs)(
+                delayed(self._compute_hash_batched)(
+                    unique_x[idx_slice],
+                    hash_func,
+                )
+                for idx_slice in gen_even_slices(
+                    len(unique_x), n_jobs * self.batch_per_job
+                )
+            )
+            # Match the hashes of the unique value to the original values
+            X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
+                len(X), X.shape[1] * self.n_components
+            )
+        else:
+            unique_x_trans = Parallel(n_jobs=n_jobs)(
+                delayed(self._compute_hash)(x, hash_func) for x in unique_x
+            )
+            # Match the hashes of the unique value to the original values
+            X_out = np.stack(unique_x_trans)[indices_x].reshape(
+                len(X), X.shape[1] * self.n_components
+            )
+
+        return X_out.astype(np.float64)  # The output is an int32 before conversion
+
+
+import pickle
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+from argparse import ArgumentParser
+
+from pathlib import Path
+
+from utils import monitor, find_result, default_parser
+from dirty_cat.tests.utils import generate_data
+
+benchmark_name = "minhash_batch_comparison"
+
+
+@monitor(
+    memory=True,
+    time=True,
+    parametrize={
+        "dataset_size": ["medium"],
+        "batched": [True, False],
+        "n_jobs": [1, 4, 8, 16, 32, 64],
+        "batch_per_job": [1, 2, 4],
+    },
+    save_as=benchmark_name,
+    repeat=10,
+)
+def benchmark(
+    dataset_size: str,
+    batched: bool,
+    n_jobs: int,
+    batch_per_job: int,
+) -> None:
+    X = data[dataset_size]
+    MinHashEncoder(batch=batched, n_jobs=n_jobs, batch_per_job=batch_per_job).fit(
+        X
+    ).transform(X)
+
+
+def plot(df: pd.DataFrame):
+    sns.set_theme(style="ticks", palette="pastel")
+
+    # Create a new columns merging batched and batch_per_job
+    # If batch is False, ignore batch_per_job
+    df["config"] = df.apply(
+        lambda row: f"batched={row['batched']}, batch_per_job={row['batch_per_job']}"
+        if row["batched"]
+        else "batched=False",
+        axis=1,
+    )
+
+    sns.boxplot(x="n_jobs", y="time", hue="config", data=df)
+    # Log scale for the y-axis
+    plt.yscale("log")
+    plt.show()
+
+
+if __name__ == "__main__":
+    _args = ArgumentParser(
+        description="Benchmark for the batch feature of the MinHashEncoder.",
+        parents=[default_parser],
+    ).parse_args()
+
+    # Generate the data if not already on disk, and keep them in memory.
+    data = {}  # Will hold the datasets in memory.
+    _data_info = {
+        "small": 10_000,
+        "medium": 100_000,
+    }
+    for name, size in _data_info.items():
+        data_file = Path(f"data_{name}.pkl")
+        if data_file.is_file():
+            with data_file.open("rb") as fl:
+                data.update({name: pickle.load(fl)})
+        else:
+            with data_file.open("wb") as fl:
+                _gen = generate_data(size).reshape(-1, 1)
+                pickle.dump(_gen, fl)
+                data.update({name: _gen})
+
+    if _args.run:
+        df = benchmark()
+    else:
+        result_file = find_result(benchmark_name)
+        df = pd.read_csv(result_file)
+
+    if _args.plot:
+        plot(df)
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/encoders_time_memory_bench.py` & `dirty_cat-0.4.1/benchmarks/encoders_time_memory_bench.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# Inspired from :
-# https://github.com/scikit-learn/scikit-learn/blob/main/benchmarks/bench_text_vectorizers.py
-# plot run time and memory usage of the different encoders using the SuperVectorizer method
-# test if auto_cast=True plays an important role
-
-"""
-
-To run this benchmark, you will need,
-
- * dirty_cat
- * pandas
- * memory_profiler
-
-"""
-import timeit
-import itertools
-
-import numpy as np
-import pandas as pd
-from memory_profiler import memory_usage
-
-from dirty_cat.datasets import fetch_traffic_violations
-
-from dirty_cat import SimilarityEncoder, GapEncoder, MinHashEncoder
-from dirty_cat import SuperVectorizer
-
-n_repeat = 3
-
-
-def run_encoders(Encoder, X, **params):
-    def f():
-        enc = Encoder(**params)
-        enc.fit_transform(X)
-
-    return f
-
-
-data = fetch_traffic_violations()
-
-X = data[1][:5000]
-y = data[2][:5000]
-
-print("=" * 80 + "\n#" + "    Dirty_cat encoders benchmark" + "\n" + "=" * 80 + "\n")
-print(f"Using a subset of the traffic violations dataset ({len(X)} observations).")
-print("This benchmarks runs in ~1 min ...")
-
-res = []
-
-for Encoder, (auto_cast, high_card_cat_transformer) in itertools.product(
-    [SuperVectorizer],
-    [
-        (True, SimilarityEncoder()),
-        (True, GapEncoder()),
-        (True, MinHashEncoder()),
-        (False, SimilarityEncoder()),
-        (False, GapEncoder()),
-        (False, MinHashEncoder()),
-    ],
-):
-    params = {
-        "auto_cast": auto_cast,
-        "high_card_cat_transformer": high_card_cat_transformer,
-    }
-    bench = {"encoder": Encoder}
-    bench.update(params)
-    dt = timeit.repeat(run_encoders(Encoder, X, **params), number=1, repeat=n_repeat)
-    bench["time"] = f"{np.mean(dt):.3f} (+-{np.std(dt):.3f})"
-
-    mem_usage = memory_usage(run_encoders(Encoder, X, **params))
-
-    bench["memory"] = f"{np.max(mem_usage):.1f}"
-
-    res.append(bench)
-
-df = pd.DataFrame(res).set_index(["auto_cast", "high_card_cat_transformer", "encoder"])
-
-print("\n========== Run time performance (sec) ===========\n")
-print(
-    "Computing the mean and the standard deviation "
-    f"of the run time over {n_repeat} runs...\n"
-)
-print(df["time"].unstack(level=-1))
-
-print("\n=============== Memory usage (MB) ===============\n")
-print(df["memory"].unstack(level=-1))
+# Inspired from :
+# https://github.com/scikit-learn/scikit-learn/blob/main/benchmarks/bench_text_vectorizers.py
+# plot run time and memory usage of the different encoders using the TableVectorizer method
+# test if auto_cast=True plays an important role
+
+"""
+
+To run this benchmark, you will need,
+
+ * dirty_cat
+ * pandas
+ * memory_profiler
+
+"""
+import timeit
+import itertools
+
+import numpy as np
+import pandas as pd
+from memory_profiler import memory_usage
+
+from dirty_cat.datasets import fetch_traffic_violations
+
+from dirty_cat import SimilarityEncoder, GapEncoder, MinHashEncoder
+from dirty_cat import TableVectorizer
+
+n_repeat = 3
+
+
+def run_encoders(Encoder, X, **params):
+    def f():
+        enc = Encoder(**params)
+        enc.fit_transform(X)
+
+    return f
+
+
+data = fetch_traffic_violations()
+
+X = data[1][:5000]
+y = data[2][:5000]
+
+print("=" * 80 + "\n#" + "    Dirty_cat encoders benchmark" + "\n" + "=" * 80 + "\n")
+print(f"Using a subset of the traffic violations dataset ({len(X)} observations).")
+print("This benchmarks runs in ~1 min ...")
+
+res = []
+
+for Encoder, (auto_cast, high_card_cat_transformer) in itertools.product(
+    [TableVectorizer],
+    [
+        (True, SimilarityEncoder()),
+        (True, GapEncoder()),
+        (True, MinHashEncoder()),
+        (False, SimilarityEncoder()),
+        (False, GapEncoder()),
+        (False, MinHashEncoder()),
+    ],
+):
+    params = {
+        "auto_cast": auto_cast,
+        "high_card_cat_transformer": high_card_cat_transformer,
+    }
+    bench = {"encoder": Encoder}
+    bench.update(params)
+    dt = timeit.repeat(run_encoders(Encoder, X, **params), number=1, repeat=n_repeat)
+    bench["time"] = f"{np.mean(dt):.3f} (+-{np.std(dt):.3f})"
+
+    mem_usage = memory_usage(run_encoders(Encoder, X, **params))
+
+    bench["memory"] = f"{np.max(mem_usage):.1f}"
+
+    res.append(bench)
+
+df = pd.DataFrame(res).set_index(["auto_cast", "high_card_cat_transformer", "encoder"])
+
+print("\n========== Run time performance (sec) ===========\n")
+print(
+    "Computing the mean and the standard deviation "
+    f"of the run time over {n_repeat} runs...\n"
+)
+print(df["time"].unstack(level=-1))
+
+print("\n=============== Memory usage (MB) ===============\n")
+print(df["memory"].unstack(level=-1))
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/fuzzy_join_benchmark.py` & `dirty_cat-0.4.1/benchmarks/fuzzy_join_benchmark.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,233 @@
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-from itertools import product
-
-from thefuzz.fuzz import partial_ratio, WRatio, ratio
-from thefuzz import process
-from autofj import AutoFJ
-from dirty_cat._fuzzy_join import fuzzy_join
-
-
-def fetch_data(dataset_name):
-    """Fetch datasets from https://github.com/chu-data-lab/AutomaticFuzzyJoin/tree/master/src/autofj/benchmark
-    """
-    repository = "chu-data-lab/AutomaticFuzzyJoin"
-    base_url = f"https://raw.githubusercontent.com/{repository}/master/src/autofj/benchmark/{dataset_name}"  # noqa
-    left = pd.read_csv(f"{base_url}/left.csv")
-    right = pd.read_csv(f"{base_url}/right.csv")
-    gt = pd.read_csv(f"{base_url}/gt.csv")
-    return left, right, gt
-
-
-def thefuzz_merge(df_1, df_2, key1, key2, threshold=90, limit=2, scorer=partial_ratio):
-    """
-    Merging using thefuzz
-
-    Parameters:
-        df_1: the left table to join
-        df_2: the right table to join
-        key1: key column of the left table
-        key2: key column of the right table
-        threshold: how close the matches should be to return a match, based on Levenshtein distance
-        limit: the amount of matches that will get returned, these are sorted high to low
-
-    Return:
-        dataframe with boths keys and matches
-    """
-    s = df_2[key2].tolist()
-
-    m = df_1[key1].apply(lambda x: process.extract(x, s, limit=limit, scorer=scorer))
-    df_1["matches"] = m
-
-    m2 = df_1["matches"].apply(
-        lambda x: ", ".join([i[0] for i in x if i[1] >= threshold])
-    )
-
-    df_1["matches"] = m2
-
-    return df_1[df_1["matches"] != ""]
-
-
-def test_autofj(left, right, gt, target):
-    """Merging using AutomaticFuzzyJoin"""
-    autofj = AutoFJ(precision_target=target, verbose=True)
-    LR_joins = autofj.join(left, right, id_column="id")
-
-    gt_joins = gt[["id_l", "id_r"]].values
-    LR_joins = LR_joins[["id_l", "id_r"]].values
-    p, r, f1 = evaluate(LR_joins, gt_joins)
-    print("Precision:", p, "Recall:", r, "F1:", f1)
-    return LR_joins, gt_joins
-
-
-def evaluate(pred_joins, gt_joins):
-    """Evaluate the performance of fuzzy joins
-
-    Parameters
-    ----------
-    pred_joins: list
-        A list of tuple pairs (id_l, id_r) that are predicted to be matches
-
-    gt_joins:
-        The ground truth matches
-
-    Returns
-    -------
-    precision: float
-        Precision score
-
-    recall: float
-        Recall score
-
-    f1: float
-        F1 score
-    """
-    pred = {(le, ri) for le, ri in pred_joins}
-    gt = {(le, ri) for le, ri in gt_joins}
-
-    tp = pred.intersection(gt)
-    precision = len(tp) / len(pred)
-    recall = len(tp) / len(gt)
-    # print('Precision', precision, 'Recall', recall)
-    if precision > 0 or recall > 0:
-        f1 = 2 * precision * recall / (precision + recall)
-    else:
-        f1 = 0
-    return precision, recall, f1
-
-
-def fuzzy_join_precision_recall(
-    left, right, gt, left_col, right_col, analyzer, ngram_range
-):
-    joined_fj = fuzzy_join(
-        right,
-        left,
-        left_on=left_col,
-        right_on=right_col,
-        analyzer=analyzer,
-        ngram_range=ngram_range,
-        return_score=True,
-    )
-    pr_list = []
-    re_list = []
-    f1_list = []
-    pr, re, f1 = evaluate(
-        list(zip(joined_fj["title_r"], joined_fj["title_l"])),
-        list(zip(gt["title_l"], gt["title_r"])),
-    )
-    pr_list.append(pr)
-    re_list.append(re)
-    f1_list.append(f1)
-    return pr_list, re_list, f1_list
-
-
-def thefuzz_precision_recall(
-    left, right, gt, left_col, right_col, scorer=partial_ratio
-):
-    pr_list = []
-    re_list = []
-    f1_list = []
-    for threshold in range(60, 99, 15):
-        joined = thefuzz_merge(
-            left,
-            right,
-            left_col,
-            right_col,
-            threshold=threshold,
-            limit=1,
-            scorer=scorer,
-        )
-        pr, re, f1 = evaluate(
-            list(zip(joined[left_col], joined["matches"])),
-            list(zip(gt["title_l"], gt["title_r"])),
-        )
-        pr_list.append(pr)
-        re_list.append(re)
-        f1_list.append(f1)
-    return pr_list, re_list, f1_list
-
-
-def autofj_precision_recall(left, right, gt, n_points=20):
-    pr_list = []
-    re_list = []
-    f1_list = []
-    for target in np.linspace(0.6, 1, n_points):
-        autofj = AutoFJ(precision_target=target, verbose=True)
-        LR_joins = autofj.join(left, right, id_column="id")
-        if len(LR_joins) != 0:
-            gt_joins = gt[["id_l", "id_r"]].values
-            LR_joins = LR_joins[["id_l", "id_r"]].values
-            p, r, f1 = evaluate(LR_joins, gt_joins)
-            pr_list.append(p)
-            re_list.append(r)
-            f1_list.append(f1)
-            # print("Precision:", p, "Recall:", r, "F1:", f1)
-    return pr_list, re_list, f1_list
-
-
-def best_precision_recall(pr_list, re_list, n_bins=13):
-    bins = np.digitize(re_list, np.quantile(re_list, np.linspace(0, 1, n_bins)))
-    res_pr = np.zeros(n_bins - 1)
-    res_re = np.zeros(n_bins - 1)
-    for i in range(1, n_bins):
-        mask = bins == i
-        # print("Recall:", re_list[mask], "Precision:", pr_list[mask])
-        if len(pr_list[mask]) > 0:
-            res_pr[i - 1] = np.nanmax(pr_list[mask])
-            res_re[i - 1] = np.nanmean(re_list[mask])
-        else:
-            res_pr[i - 1] = np.nan
-            res_re[i - 1] = np.nan
-    return res_pr, res_re
-
-
-left_1, right_1, gt_1 = fetch_data("Country")
-
-pr_list = []
-re_list = []
-for analyzer, max_n_gram in product(["char", "char_wb"], [3, 4, 5]):
-    if analyzer == "word" and max_n_gram > 2:
-        continue
-    precision, recall, f1 = fuzzy_join_precision_recall(
-        left=left_1,
-        right=right_1,
-        gt=gt_1,
-        left_col="title",
-        right_col="title",
-        analyzer=analyzer,
-        ngram_range=(2, max_n_gram),
-    )
-    pr_list.extend(precision)
-    re_list.extend(recall)
-    # plt.plot(recall, precision,
-    #         label=f"fuzzy_join_{analyzer}_{max_n_gram}_{similarity}")
-
-pr_list, re_list = best_precision_recall(np.array(pr_list), np.array(re_list))
-plt.plot(re_list, pr_list, label="fuzzy_join")
-
-pr_list_fw = []
-re_list_fw = []
-for scorer in partial_ratio, ratio, WRatio:
-    precision_fw, recall_fw, f1_fw = thefuzz_precision_recall(
-        left_1, right_1, gt_1, "title", "title", scorer=scorer
-    )
-    pr_list_fw.extend(precision_fw)
-    re_list_fw.extend(recall_fw)
-
-pr_list_fw, re_list_fw = best_precision_recall(
-    np.array(pr_list_fw), np.array(re_list_fw)
-)
-plt.plot(re_list_fw, pr_list_fw, label="thefuzz")
-# plt.plot(recall_fw, precision_fw, label=f'thefuzz_{scorer.__name__}')
-
-precision_fj, recall_fj, f1_fj = autofj_precision_recall(left_1, right_1, gt_1)
-plt.plot(recall_fj, precision_fj, label="autofj")
-
-plt.xlabel("Recall")
-plt.ylabel("Precision")
-plt.legend()
-plt.title("Best Precision / recall on Country")
-plt.savefig("precision_recall.png")
-# plt.show()
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from itertools import product
+
+from thefuzz.fuzz import partial_ratio, WRatio, ratio
+from thefuzz import process
+from autofj import AutoFJ
+from dirty_cat._fuzzy_join import fuzzy_join
+
+
+def fetch_data(dataset_name):
+    """Fetch datasets from https://github.com/chu-data-lab/AutomaticFuzzyJoin/tree/master/src/autofj/benchmark
+    """
+    repository = "chu-data-lab/AutomaticFuzzyJoin"
+    base_url = f"https://raw.githubusercontent.com/{repository}/master/src/autofj/benchmark/{dataset_name}"  # noqa
+    left = pd.read_csv(f"{base_url}/left.csv")
+    right = pd.read_csv(f"{base_url}/right.csv")
+    gt = pd.read_csv(f"{base_url}/gt.csv")
+    return left, right, gt
+
+
+def thefuzz_merge(df_1, df_2, key1, key2, threshold=90, limit=2, scorer=partial_ratio):
+    """
+    Merging using thefuzz
+
+    Parameters:
+        df_1: the left table to join
+        df_2: the right table to join
+        key1: key column of the left table
+        key2: key column of the right table
+        threshold: how close the matches should be to return a match, based on Levenshtein distance
+        limit: the amount of matches that will get returned, these are sorted high to low
+
+    Return:
+        dataframe with boths keys and matches
+    """
+    s = df_2[key2].tolist()
+
+    m = df_1[key1].apply(lambda x: process.extract(x, s, limit=limit, scorer=scorer))
+    df_1["matches"] = m
+
+    m2 = df_1["matches"].apply(
+        lambda x: ", ".join([i[0] for i in x if i[1] >= threshold])
+    )
+
+    df_1["matches"] = m2
+
+    return df_1[df_1["matches"] != ""]
+
+
+def test_autofj(left, right, gt, target):
+    """Merging using AutomaticFuzzyJoin"""
+    autofj = AutoFJ(precision_target=target, verbose=True)
+    LR_joins = autofj.join(left, right, id_column="id")
+
+    gt_joins = gt[["id_l", "id_r"]].values
+    LR_joins = LR_joins[["id_l", "id_r"]].values
+    p, r, f1 = evaluate(LR_joins, gt_joins)
+    print("Precision:", p, "Recall:", r, "F1:", f1)
+    return LR_joins, gt_joins
+
+
+def evaluate(pred_joins, gt_joins):
+    """Evaluate the performance of fuzzy joins
+
+    Parameters
+    ----------
+    pred_joins: list
+        A list of tuple pairs (id_l, id_r) that are predicted to be matches
+
+    gt_joins:
+        The ground truth matches
+
+    Returns
+    -------
+    precision: float
+        Precision score
+
+    recall: float
+        Recall score
+
+    f1: float
+        F1 score
+    """
+    pred = {(le, ri) for le, ri in pred_joins}
+    gt = {(le, ri) for le, ri in gt_joins}
+
+    tp = pred.intersection(gt)
+    precision = len(tp) / len(pred)
+    recall = len(tp) / len(gt)
+    # print('Precision', precision, 'Recall', recall)
+    if precision > 0 or recall > 0:
+        f1 = 2 * precision * recall / (precision + recall)
+    else:
+        f1 = 0
+    return precision, recall, f1
+
+
+def fuzzy_join_precision_recall(
+    left, right, gt, left_col, right_col, analyzer, ngram_range
+):
+    joined_fj = fuzzy_join(
+        right,
+        left,
+        left_on=left_col,
+        right_on=right_col,
+        analyzer=analyzer,
+        ngram_range=ngram_range,
+        return_score=True,
+    )
+    pr_list = []
+    re_list = []
+    f1_list = []
+    pr, re, f1 = evaluate(
+        list(zip(joined_fj["title_r"], joined_fj["title_l"])),
+        list(zip(gt["title_l"], gt["title_r"])),
+    )
+    pr_list.append(pr)
+    re_list.append(re)
+    f1_list.append(f1)
+    return pr_list, re_list, f1_list
+
+
+def thefuzz_precision_recall(
+    left, right, gt, left_col, right_col, scorer=partial_ratio
+):
+    pr_list = []
+    re_list = []
+    f1_list = []
+    for threshold in range(60, 99, 15):
+        joined = thefuzz_merge(
+            left,
+            right,
+            left_col,
+            right_col,
+            threshold=threshold,
+            limit=1,
+            scorer=scorer,
+        )
+        pr, re, f1 = evaluate(
+            list(zip(joined[left_col], joined["matches"])),
+            list(zip(gt["title_l"], gt["title_r"])),
+        )
+        pr_list.append(pr)
+        re_list.append(re)
+        f1_list.append(f1)
+    return pr_list, re_list, f1_list
+
+
+def autofj_precision_recall(left, right, gt, n_points=20):
+    pr_list = []
+    re_list = []
+    f1_list = []
+    for target in np.linspace(0.6, 1, n_points):
+        autofj = AutoFJ(precision_target=target, verbose=True)
+        LR_joins = autofj.join(left, right, id_column="id")
+        if len(LR_joins) != 0:
+            gt_joins = gt[["id_l", "id_r"]].values
+            LR_joins = LR_joins[["id_l", "id_r"]].values
+            p, r, f1 = evaluate(LR_joins, gt_joins)
+            pr_list.append(p)
+            re_list.append(r)
+            f1_list.append(f1)
+            # print("Precision:", p, "Recall:", r, "F1:", f1)
+    return pr_list, re_list, f1_list
+
+
+def best_precision_recall(pr_list, re_list, n_bins=13):
+    bins = np.digitize(re_list, np.quantile(re_list, np.linspace(0, 1, n_bins)))
+    res_pr = np.zeros(n_bins - 1)
+    res_re = np.zeros(n_bins - 1)
+    for i in range(1, n_bins):
+        mask = bins == i
+        # print("Recall:", re_list[mask], "Precision:", pr_list[mask])
+        if len(pr_list[mask]) > 0:
+            res_pr[i - 1] = np.nanmax(pr_list[mask])
+            res_re[i - 1] = np.nanmean(re_list[mask])
+        else:
+            res_pr[i - 1] = np.nan
+            res_re[i - 1] = np.nan
+    return res_pr, res_re
+
+
+if __name__ == "__main__":
+    left_1, right_1, gt_1 = fetch_data("Country")
+
+    pr_list = []
+    re_list = []
+    for analyzer, max_n_gram in product(["char", "char_wb"], [3, 4, 5]):
+        if analyzer == "word" and max_n_gram > 2:
+            continue
+        precision, recall, f1 = fuzzy_join_precision_recall(
+            left=left_1,
+            right=right_1,
+            gt=gt_1,
+            left_col="title",
+            right_col="title",
+            analyzer=analyzer,
+            ngram_range=(2, max_n_gram),
+        )
+        pr_list.extend(precision)
+        re_list.extend(recall)
+        # plt.plot(recall, precision,
+        #         label=f"fuzzy_join_{analyzer}_{max_n_gram}_{similarity}")
+
+    pr_list, re_list = best_precision_recall(np.array(pr_list), np.array(re_list))
+    plt.plot(re_list, pr_list, label="fuzzy_join")
+
+    pr_list_fw = []
+    re_list_fw = []
+    for scorer in partial_ratio, ratio, WRatio:
+        precision_fw, recall_fw, f1_fw = thefuzz_precision_recall(
+            left_1, right_1, gt_1, "title", "title", scorer=scorer
+        )
+        pr_list_fw.extend(precision_fw)
+        re_list_fw.extend(recall_fw)
+
+    pr_list_fw, re_list_fw = best_precision_recall(
+        np.array(pr_list_fw), np.array(re_list_fw)
+    )
+    plt.plot(re_list_fw, pr_list_fw, label="thefuzz")
+    # plt.plot(recall_fw, precision_fw, label=f'thefuzz_{scorer.__name__}')
+
+    precision_fj, recall_fj, f1_fj = autofj_precision_recall(left_1, right_1, gt_1)
+    plt.plot(recall_fj, precision_fj, label="autofj")
+
+    plt.xlabel("Recall")
+    plt.ylabel("Precision")
+    plt.legend()
+    plt.title("Best Precision / recall on Country")
+    plt.savefig("precision_recall.png")
+    # plt.show()
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/similarity_scores_time_benchmark.py` & `dirty_cat-0.4.1/benchmarks/similarity_scores_time_benchmark.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-"""
-Benchmark time consumption and scores for K-means and most frequent strategies.
-
-We use the traffic_violations dataset to benchmark the different dimensionality
-reduction strategies used in similarity encoding.
-
-Parameters that are modified:
-- Number of rows in datasets: 10k, 20k, 50k, 100k and nuniques.
-- Hashing dimensions: 2 ** 14, 2 ** 16, 2 ** 18, 2 ** 20
-- Ngram-range: (3, 3), (2, 4)
-"""
-
-# We filter out the warning asking us to specify the solver in the logistic_regression
-import warnings
-
-warnings.simplefilter(action="ignore", category=FutureWarning)
-
-from time import time
-
-import matplotlib.pyplot as plt
-import pandas as pd
-import seaborn as sns
-from sklearn import linear_model, model_selection
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import OneHotEncoder
-
-from dirty_cat import SimilarityEncoder
-from dirty_cat.datasets import fetch_traffic_violations
-
-
-data = fetch_traffic_violations()
-
-col_to_ohe = [
-    "alcohol",
-    "arrest_type",
-    "belts",
-    "commercial_license",
-    "commercial_vehicle",
-    "fatal",
-    "gender",
-    "hazmat",
-    "property_damage",
-    "race",
-    "work_zone",
-]
-
-col_to_pass = ["year"]
-
-col_to_enc = ["description"]
-
-# Get the data and remove missing values:
-X = data[1][col_to_enc + col_to_ohe + col_to_pass]
-mask = X.isna()[col_to_pass].copy()
-X.dropna(subset=col_to_pass, inplace=True)
-
-y = data[2][~mask[mask.columns[0]]]
-
-X.reset_index(inplace=True, drop=True)
-y.reset_index(inplace=True, drop=True)
-
-transformers = [
-    ("one_hot", OneHotEncoder(sparse=False, handle_unknown="ignore"), col_to_ohe),
-    ("pass", "passthrough", col_to_pass),
-]
-
-
-def benchmark(
-    X_b,
-    y_b,
-    strat="k-means",
-    limit=50000,
-    n_proto=100,
-    hash_dim=None,
-    ngram_range=(3, 3),
-):
-    X_b = X_b[:limit].copy()
-    y_b = y_b[:limit].copy()
-
-    if strat == "k-means":
-        sim_enc = SimilarityEncoder(
-            ngram_range=ngram_range,
-            categories="k-means",
-            hashing_dim=hash_dim,
-            n_prototypes=n_proto,
-            random_state=3498,
-        )
-    else:
-        sim_enc = SimilarityEncoder(
-            ngram_range=ngram_range,
-            categories="most_frequent",
-            hashing_dim=hash_dim,
-            n_prototypes=n_proto,
-            random_state=3498,
-        )
-
-    column_trans = ColumnTransformer(
-        transformers=transformers + [("sim_enc", sim_enc, ["description"])],
-        remainder="drop",
-    )
-
-    t0 = time()
-    X_enc = column_trans.fit_transform(X_b)
-    t1 = time()
-    t_score_1 = t1 - t0
-
-    model = linear_model.LogisticRegression()
-
-    t0 = time()
-    m_score = model_selection.cross_val_score(model, X_enc, y_b, cv=20)
-    t1 = time()
-    t_score_2 = t1 - t0
-    return t_score_1, m_score, t_score_2
-
-
-def plot(bench, title=""):
-    sns.set(style="ticks", palette="muted")
-    hash_dims = ["Count", "2 ** 14", "2 ** 16", "2 ** 18", "2 ** 20"]
-    scores = []
-    vectorizer = []
-    strategy = []
-
-    for i, e in enumerate(bench):
-        vectorizer.extend([hash_dims[i % 5]] * (2 * len(e[0][1])))
-        strategy.extend(["k-means"] * len(e[0][1]))
-        strategy.extend(["most-frequent"] * len(e[1][1]))
-        scores.extend(e[0][1])
-        scores.extend(e[1][1])
-
-    df = pd.DataFrame(columns=["vectorizer", "strategy", "score"])
-    df["vectorizer"] = vectorizer
-    df["strategy"] = strategy
-    df["score"] = scores
-
-    first = plt.figure()
-    ax = sns.boxplot(x="vectorizer", y="score", hue="strategy", data=df)
-    ax.set(
-        title=title,
-        xlabel="Vectorizer used",
-        ylabel="Mean score on 10 cross validations",
-    )
-    ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
-    first.tight_layout()
-
-    vectorizer.clear()
-    scores.clear()
-    strategy.clear()
-    times = []
-
-    for i, e in enumerate(bench):
-        vectorizer.extend([hash_dims[i % 5]] * 4)
-        strategy.extend(["K-means vect", "K-means X-val", "MF vect", "MF X-val"])
-        times.extend([e[0][0], e[0][2] / 20, e[1][0], e[1][2] / 20])
-
-    df = pd.DataFrame(columns=["vectorizer", "strategy/operation", "time"])
-    df["vectorizer"] = vectorizer
-    df["strategy/operation"] = strategy
-    df["time"] = times
-
-    second = plt.figure()
-    ax1 = sns.barplot(x="vectorizer", y="time", hue="strategy/operation", data=df)
-    ax1.set(title=title, xlabel="Vectorizer used", ylabel="Time in seconds")
-    ax1.legend(loc="center left", bbox_to_anchor=(1, 0.5))
-    second.tight_layout()
-
-    title = title.replace(" ", "_").replace(":", "-").replace(",", "_").lower()
-    first.savefig(title + "_score.png")
-    second.savefig(title + "_time.png")
-    # first.show()
-    # second.show(t)
-
-
-def loop(proto):
-    limits = sorted([X["description"].nunique(), 10000, 20000, 50000, 100000])
-    hash_dims = [None, 2**14, 2**16, 2**18, 2**20]
-    bench = list()
-    ngram = [(3, 3), (2, 4)]
-    for limit in limits:
-        for r in ngram:
-            for h in hash_dims:
-                bench.append(
-                    (
-                        benchmark(
-                            X,
-                            y,
-                            strat="k-means",
-                            limit=limit,
-                            n_proto=proto,
-                            hash_dim=h,
-                            ngram_range=r,
-                        ),
-                        benchmark(
-                            X,
-                            y,
-                            strat="most-frequent",
-                            limit=limit,
-                            n_proto=proto,
-                            hash_dim=h,
-                            ngram_range=r,
-                        ),
-                    )
-                )
-            title = "N-gram range: %s, Rows: %d, Prototypes: %d, 20 CV" % (
-                r.__str__(),
-                limit,
-                proto,
-            )
-            plot(bench, title)
-            bench.clear()
-
-
-if __name__ == "__main__":
-    loop(100)
+"""
+Benchmark time consumption and scores for K-means and most frequent strategies.
+
+We use the traffic_violations dataset to benchmark the different dimensionality
+reduction strategies used in similarity encoding.
+
+Parameters that are modified:
+- Number of rows in datasets: 10k, 20k, 50k, 100k and nuniques.
+- Hashing dimensions: 2 ** 14, 2 ** 16, 2 ** 18, 2 ** 20
+- Ngram-range: (3, 3), (2, 4)
+"""
+
+# We filter out the warning asking us to specify the solver in the logistic_regression
+import warnings
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+
+from time import time
+
+import matplotlib.pyplot as plt
+import pandas as pd
+import seaborn as sns
+from sklearn import linear_model, model_selection
+from sklearn.compose import ColumnTransformer
+from sklearn.preprocessing import OneHotEncoder
+
+from dirty_cat import SimilarityEncoder
+from dirty_cat.datasets import fetch_traffic_violations
+
+
+data = fetch_traffic_violations()
+
+col_to_ohe = [
+    "alcohol",
+    "arrest_type",
+    "belts",
+    "commercial_license",
+    "commercial_vehicle",
+    "fatal",
+    "gender",
+    "hazmat",
+    "property_damage",
+    "race",
+    "work_zone",
+]
+
+col_to_pass = ["year"]
+
+col_to_enc = ["description"]
+
+# Get the data and remove missing values:
+X = data[1][col_to_enc + col_to_ohe + col_to_pass]
+mask = X.isna()[col_to_pass].copy()
+X.dropna(subset=col_to_pass, inplace=True)
+
+y = data[2][~mask[mask.columns[0]]]
+
+X.reset_index(inplace=True, drop=True)
+y.reset_index(inplace=True, drop=True)
+
+transformers = [
+    ("one_hot", OneHotEncoder(sparse=False, handle_unknown="ignore"), col_to_ohe),
+    ("pass", "passthrough", col_to_pass),
+]
+
+
+def benchmark(
+    X_b,
+    y_b,
+    strat="k-means",
+    limit=50000,
+    n_proto=100,
+    hash_dim=None,
+    ngram_range=(3, 3),
+):
+    X_b = X_b[:limit].copy()
+    y_b = y_b[:limit].copy()
+
+    if strat == "k-means":
+        sim_enc = SimilarityEncoder(
+            ngram_range=ngram_range,
+            categories="k-means",
+            hashing_dim=hash_dim,
+            n_prototypes=n_proto,
+            random_state=3498,
+        )
+    else:
+        sim_enc = SimilarityEncoder(
+            ngram_range=ngram_range,
+            categories="most_frequent",
+            hashing_dim=hash_dim,
+            n_prototypes=n_proto,
+            random_state=3498,
+        )
+
+    column_trans = ColumnTransformer(
+        transformers=transformers + [("sim_enc", sim_enc, ["description"])],
+        remainder="drop",
+    )
+
+    t0 = time()
+    X_enc = column_trans.fit_transform(X_b)
+    t1 = time()
+    t_score_1 = t1 - t0
+
+    model = linear_model.LogisticRegression()
+
+    t0 = time()
+    m_score = model_selection.cross_val_score(model, X_enc, y_b, cv=20)
+    t1 = time()
+    t_score_2 = t1 - t0
+    return t_score_1, m_score, t_score_2
+
+
+def plot(bench, title=""):
+    sns.set(style="ticks", palette="muted")
+    hash_dims = ["Count", "2 ** 14", "2 ** 16", "2 ** 18", "2 ** 20"]
+    scores = []
+    vectorizer = []
+    strategy = []
+
+    for i, e in enumerate(bench):
+        vectorizer.extend([hash_dims[i % 5]] * (2 * len(e[0][1])))
+        strategy.extend(["k-means"] * len(e[0][1]))
+        strategy.extend(["most-frequent"] * len(e[1][1]))
+        scores.extend(e[0][1])
+        scores.extend(e[1][1])
+
+    df = pd.DataFrame(columns=["vectorizer", "strategy", "score"])
+    df["vectorizer"] = vectorizer
+    df["strategy"] = strategy
+    df["score"] = scores
+
+    first = plt.figure()
+    ax = sns.boxplot(x="vectorizer", y="score", hue="strategy", data=df)
+    ax.set(
+        title=title,
+        xlabel="Vectorizer used",
+        ylabel="Mean score on 10 cross validations",
+    )
+    ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+    first.tight_layout()
+
+    vectorizer.clear()
+    scores.clear()
+    strategy.clear()
+    times = []
+
+    for i, e in enumerate(bench):
+        vectorizer.extend([hash_dims[i % 5]] * 4)
+        strategy.extend(["K-means vect", "K-means X-val", "MF vect", "MF X-val"])
+        times.extend([e[0][0], e[0][2] / 20, e[1][0], e[1][2] / 20])
+
+    df = pd.DataFrame(columns=["vectorizer", "strategy/operation", "time"])
+    df["vectorizer"] = vectorizer
+    df["strategy/operation"] = strategy
+    df["time"] = times
+
+    second = plt.figure()
+    ax1 = sns.barplot(x="vectorizer", y="time", hue="strategy/operation", data=df)
+    ax1.set(title=title, xlabel="Vectorizer used", ylabel="Time in seconds")
+    ax1.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+    second.tight_layout()
+
+    title = title.replace(" ", "_").replace(":", "-").replace(",", "_").lower()
+    first.savefig(title + "_score.png")
+    second.savefig(title + "_time.png")
+    # first.show()
+    # second.show(t)
+
+
+def loop(proto):
+    limits = sorted([X["description"].nunique(), 10000, 20000, 50000, 100000])
+    hash_dims = [None, 2**14, 2**16, 2**18, 2**20]
+    bench = list()
+    ngram = [(3, 3), (2, 4)]
+    for limit in limits:
+        for r in ngram:
+            for h in hash_dims:
+                bench.append(
+                    (
+                        benchmark(
+                            X,
+                            y,
+                            strat="k-means",
+                            limit=limit,
+                            n_proto=proto,
+                            hash_dim=h,
+                            ngram_range=r,
+                        ),
+                        benchmark(
+                            X,
+                            y,
+                            strat="most-frequent",
+                            limit=limit,
+                            n_proto=proto,
+                            hash_dim=h,
+                            ngram_range=r,
+                        ),
+                    )
+                )
+            title = "N-gram range: %s, Rows: %d, Prototypes: %d, 20 CV" % (
+                r.__str__(),
+                limit,
+                proto,
+            )
+            plot(bench, title)
+            bench.clear()
+
+
+if __name__ == "__main__":
+    loop(100)
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/supervectorizer_tuning.py` & `dirty_cat-0.4.1/benchmarks/tablevectorizer_tuning.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-"""
-Performs a GridSearch to find the best parameters for the SuperVectorizer
-among a selection.
-"""
-
-import logging
-import pandas as pd
-
-from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
-from sklearn.model_selection import GridSearchCV
-from sklearn.pipeline import Pipeline
-
-from dirty_cat import SuperVectorizer
-from dirty_cat.datasets import (
-    fetch_open_payments,
-    fetch_drug_directory,
-    fetch_road_safety,
-    fetch_midwest_survey,
-    fetch_medical_charge,
-    fetch_employee_salaries,
-    fetch_traffic_violations,
-)
-
-from pathlib import Path
-from functools import wraps
-from datetime import datetime
-from typing import List, Tuple
-
-
-def get_classification_datasets() -> List[Tuple[dict, str]]:
-    return [
-        (fetch_open_payments(), "open_payments"),
-        # (fetch_drug_directory(), 'drug_directory),
-        (fetch_road_safety(), "road_safety"),
-        (fetch_midwest_survey(), "midwest_survey"),
-        (fetch_traffic_violations(), "traffic_violations"),
-    ]
-
-
-def get_regression_datasets() -> List[Tuple[dict, str]]:
-    return [
-        (fetch_medical_charge(), "medical_charge"),
-        (fetch_employee_salaries(), "employee_salaries"),
-    ]
-
-
-def get_dataset(info) -> Tuple[pd.DataFrame, pd.Series]:
-    df = pd.read_csv(info["path"], **info["read_csv_kwargs"])
-    y = df[info["y"]]
-    X = df.drop(info["y"], axis=1).astype(str)
-    return X, y
-
-
-def set_logging(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        logging_level = logging.DEBUG
-
-        logger = logging.getLogger()
-        logger.setLevel(logging_level)
-
-        formatter = logging.Formatter("%(asctime)s - [%(levelname)s] %(message)s")
-        formatter.datefmt = "%m/%d/%Y %H:%M:%S"
-
-        path = Path(__file__).parent / f"tuning_{str(datetime.now())[:10]}.log"
-
-        fh = logging.FileHandler(filename=path, mode="w")
-        fh.setLevel(logging_level)
-        fh.setFormatter(formatter)
-
-        # sh = logging.StreamHandler(sys.stdout)
-        # sh.setLevel(logging_level)
-        # sh.setFormatter(formatter)
-
-        logger.addHandler(fh)
-        # logger.addHandler(sh)
-
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-@set_logging
-def main():
-    logging.info("Launching !")
-
-    card_possibilities = [20, 30, 40, 50]
-    n_comp_possibilities = [10, 30, 50]
-
-    logging.debug("Creating pipelines")
-    regression_pipeline = Pipeline(
-        [
-            ("sv", SuperVectorizer()),
-            ("estimator", RandomForestRegressor()),
-        ]
-    )
-    classification_pipeline = Pipeline(
-        [
-            ("sv", SuperVectorizer()),
-            ("estimator", RandomForestClassifier()),
-        ]
-    )
-
-    logging.debug(
-        f"With cardinality possibilities: {card_possibilities} "
-        f"and n_components possibilities: {n_comp_possibilities}"
-    )
-    for pipeline, datasets in zip(
-        [
-            regression_pipeline,
-            classification_pipeline,
-        ],
-        [
-            get_regression_datasets(),
-            get_classification_datasets(),
-        ],
-    ):
-        for info, name in datasets:
-            X, y = get_dataset(info)
-            if name != "traffic_violations":
-                continue
-
-            csv_path = Path(".").resolve() / f"{name}_results.csv"
-            if csv_path.exists():
-                # If the results already exist, we'll skip to the next
-                logging.debug(f"Skipping {name} as {csv_path!s} was found")
-                continue
-
-            logging.debug(f"Running search on {name}")
-            grid = GridSearchCV(
-                estimator=pipeline,
-                param_grid={
-                    "sv__cardinality_threshold": card_possibilities,
-                    "sv__high_card_str_transformer__n_components": n_comp_possibilities,
-                },
-                n_jobs=30,
-            )
-            grid.fit(X, y)
-
-            df = pd.DataFrame(grid.cv_results_)
-            df.to_csv(csv_path)
-            logging.info(f"Saved search results in {csv_path!s}")
-
-
-if __name__ == "__main__":
-    main()
+"""
+Performs a GridSearch to find the best parameters for the TableVectorizer
+among a selection.
+"""
+
+import logging
+import pandas as pd
+
+from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
+from sklearn.model_selection import GridSearchCV
+from sklearn.pipeline import Pipeline
+
+from dirty_cat import TableVectorizer
+from dirty_cat.datasets import (
+    fetch_open_payments,
+    fetch_drug_directory,
+    fetch_road_safety,
+    fetch_midwest_survey,
+    fetch_medical_charge,
+    fetch_employee_salaries,
+    fetch_traffic_violations,
+)
+
+from pathlib import Path
+from functools import wraps
+from datetime import datetime
+from typing import List, Tuple
+
+
+def get_classification_datasets() -> List[Tuple[dict, str]]:
+    return [
+        (fetch_open_payments(), "open_payments"),
+        # (fetch_drug_directory(), 'drug_directory),
+        (fetch_road_safety(), "road_safety"),
+        (fetch_midwest_survey(), "midwest_survey"),
+        (fetch_traffic_violations(), "traffic_violations"),
+    ]
+
+
+def get_regression_datasets() -> List[Tuple[dict, str]]:
+    return [
+        (fetch_medical_charge(), "medical_charge"),
+        (fetch_employee_salaries(), "employee_salaries"),
+    ]
+
+
+def get_dataset(info) -> Tuple[pd.DataFrame, pd.Series]:
+    df = pd.read_csv(info["path"], **info["read_csv_kwargs"])
+    y = df[info["y"]]
+    X = df.drop(info["y"], axis=1).astype(str)
+    return X, y
+
+
+def set_logging(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        logging_level = logging.DEBUG
+
+        logger = logging.getLogger()
+        logger.setLevel(logging_level)
+
+        formatter = logging.Formatter("%(asctime)s - [%(levelname)s] %(message)s")
+        formatter.datefmt = "%m/%d/%Y %H:%M:%S"
+
+        path = Path(__file__).parent / f"tuning_{str(datetime.now())[:10]}.log"
+
+        fh = logging.FileHandler(filename=path, mode="w")
+        fh.setLevel(logging_level)
+        fh.setFormatter(formatter)
+
+        # sh = logging.StreamHandler(sys.stdout)
+        # sh.setLevel(logging_level)
+        # sh.setFormatter(formatter)
+
+        logger.addHandler(fh)
+        # logger.addHandler(sh)
+
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+@set_logging
+def main():
+    logging.info("Launching !")
+
+    card_possibilities = [20, 30, 40, 50]
+    n_comp_possibilities = [10, 30, 50]
+
+    logging.debug("Creating pipelines")
+    regression_pipeline = Pipeline(
+        [
+            ("tv", TableVectorizer()),
+            ("estimator", RandomForestRegressor()),
+        ]
+    )
+    classification_pipeline = Pipeline(
+        [
+            ("tv", TableVectorizer()),
+            ("estimator", RandomForestClassifier()),
+        ]
+    )
+
+    logging.debug(
+        f"With cardinality possibilities: {card_possibilities} "
+        f"and n_components possibilities: {n_comp_possibilities}"
+    )
+    for pipeline, datasets in zip(
+        [
+            regression_pipeline,
+            classification_pipeline,
+        ],
+        [
+            get_regression_datasets(),
+            get_classification_datasets(),
+        ],
+    ):
+        for info, name in datasets:
+            X, y = get_dataset(info)
+            if name != "traffic_violations":
+                continue
+
+            csv_path = Path(".").resolve() / f"{name}_results.csv"
+            if csv_path.exists():
+                # If the results already exist, we'll skip to the next
+                logging.debug(f"Skipping {name} as {csv_path!s} was found")
+                continue
+
+            logging.debug(f"Running search on {name}")
+            grid = GridSearchCV(
+                estimator=pipeline,
+                param_grid={
+                    "sv__cardinality_threshold": card_possibilities,
+                    "sv__high_card_str_transformer__n_components": n_comp_possibilities,
+                },
+                n_jobs=30,
+            )
+            grid.fit(X, y)
+
+            df = pd.DataFrame(grid.cv_results_)
+            df.to_csv(csv_path)
+            logging.info(f"Saved search results in {csv_path!s}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/utils/_argparser.py` & `dirty_cat-0.4.1/benchmarks/utils/_argparser.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from argparse import ArgumentParser
-
-# Inherit this parser in your file, like so:
-# >>> _parser = ArgumentParser(parents=[default_parser])
-
-default_parser = ArgumentParser(add_help=False)
-
-default_parser.add_argument(
-    "--run",
-    help="Runs the benchmark.",
-    action="store_true",
-)
-default_parser.add_argument(
-    "--plot",
-    help=(
-        "Plots the results. If '--run' is specified, plots those. "
-        "Otherwise, searches for result files in the results' directory. "
-        "If it finds none, exits. If it finds only one, displays it. "
-        "If it finds multiple, prompts the user to choose one. "
-    ),
-    action="store_true",
-)
+from argparse import ArgumentParser
+
+# Inherit this parser in your file, like so:
+# >>> _parser = ArgumentParser(parents=[default_parser])
+
+default_parser = ArgumentParser(add_help=False)
+
+default_parser.add_argument(
+    "--run",
+    help="Runs the benchmark.",
+    action="store_true",
+)
+default_parser.add_argument(
+    "--plot",
+    help=(
+        "Plots the results. If '--run' is specified, plots those. "
+        "Otherwise, searches for result files in the results' directory. "
+        "If it finds none, exits. If it finds only one, displays it. "
+        "If it finds multiple, prompts the user to choose one. "
+    ),
+    action="store_true",
+)
```

### Comparing `dirty_cat-0.4.0b2/benchmarks/utils/_various.py` & `dirty_cat-0.4.1/benchmarks/utils/_various.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-import pandas as pd
-
-from typing import List
-from pathlib import Path
-
-
-def find_result(bench_name: str) -> Path:
-    return choose_file(find_results(bench_name))
-
-
-def find_results(bench_name: str) -> List[Path]:
-    """
-    Returns the list of results in the results' directory.
-    """
-    results_dir = Path(__file__).parent.parent / "results"
-    return [
-        file
-        for file in results_dir.iterdir()
-        if file.stem.startswith(bench_name) and file.suffix == ".csv"
-    ]
-
-
-def choose_file(results: List[Path]) -> Path:
-    """
-    Given a list of files, chooses one based on these rules:
-    - If there are no files to choose from, exit the program
-    - If there's only one, return this one
-    - If there are multiple, prompt the user to choose one
-    """
-    if len(results) == 0:
-        print("No results file to choose from, exiting...")
-        exit()
-    elif len(results) == 1:
-        return results[0]
-    else:
-        for i, file in enumerate(results):
-            # Read the result file to get its dimensions
-            df = pd.read_csv(file)
-            # Try and get the number of repeats.
-            if "time" in df.columns:
-                repeat = len(eval(df["time"].iloc[0]))
-            elif "memory" in df.columns:
-                repeat = len(eval(df["memory"].iloc[0]))
-            else:
-                repeat = 1
-
-            bench_name, date = file.stem.split("-")
-            print(
-                f"{i + 1}) "
-                f"{date[:4]}-{date[4:6]}-{date[6:]} - "
-                f"{df.shape[0]}x{repeat} experiments "
-            )
-        choice = input("Choose the result to display: ")
-        if not choice.isnumeric() or (int(choice) - 1) not in range(len(results)):
-            print(f"Invalid choice {choice!r}, exiting.")
-            exit()
-        return results[int(choice) - 1]
+from pathlib import Path
+from typing import List
+
+import pandas as pd
+
+
+def find_result(bench_name: str) -> Path:
+    return choose_file(find_results(bench_name))
+
+
+def find_results(bench_name: str) -> List[Path]:
+    """
+    Returns the list of results in the results' directory.
+    """
+    results_dir = Path(__file__).parent.parent / "results"
+    return [
+        file
+        for file in results_dir.iterdir()
+        if file.stem.startswith(bench_name) and file.suffix == ".csv"
+    ]
+
+
+def choose_file(results: List[Path]) -> Path:
+    """
+    Given a list of files, chooses one based on these rules:
+    - If there are no files to choose from, exit the program
+    - If there's only one, return this one
+    - If there are multiple, prompt the user to choose one
+    """
+    if len(results) == 0:
+        print("No results file to choose from, exiting...")
+        exit()
+    elif len(results) == 1:
+        return results[0]
+    else:
+        for i, file in enumerate(results):
+            # Read the result file to get its dimensions
+            df = pd.read_csv(file)
+            if "iter" not in df.columns:
+                print(f"Invalid file {file.name!r}, skipping.")
+                continue
+            n_iter_per_xp = df["iter"].max() + 1
+            repeat = df.shape[0] // n_iter_per_xp
+
+            bench_name, date = file.stem.split("-")
+            print(
+                f"{i + 1}) "
+                f"{date[:4]}-{date[4:6]}-{date[6:]} - "
+                f"{df.shape[0]}x{repeat} experiments "
+            )
+        choice = input("Choose the result to display: ")
+        if not choice.isnumeric() or (int(choice) - 1) not in range(len(results)):
+            print(f"Invalid choice {choice!r}, exiting.")
+            exit()
+        return results[int(choice) - 1]
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/__init__.py` & `dirty_cat-0.4.1/dirty_cat/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-"""
-dirty_cat: Learning on dirty categories.
-"""
-from pathlib import Path as _Path
-
-try:
-    from ._check_dependencies import check_dependencies
-
-    check_dependencies()
-except ModuleNotFoundError:
-    import warnings
-
-    warnings.warn(
-        "pkg_resources is not available, dependencies versions will not be checked."
-    )
-
-from ._datetime_encoder import DatetimeEncoder
-from ._deduplicate import compute_ngram_distance, deduplicate
-from ._feature_augmenter import FeatureAugmenter
-from ._fuzzy_join import fuzzy_join
-from ._gap_encoder import GapEncoder
-from ._minhash_encoder import MinHashEncoder
-from ._similarity_encoder import SimilarityEncoder
-from ._super_vectorizer import SuperVectorizer
-from ._target_encoder import TargetEncoder
-
-with open(_Path(__file__).parent / "VERSION.txt") as _fh:
-    __version__ = _fh.read().strip()
-
-
-__all__ = [
-    "DatetimeEncoder",
-    "FeatureAugmenter",
-    "fuzzy_join",
-    "GapEncoder",
-    "MinHashEncoder",
-    "SimilarityEncoder",
-    "SuperVectorizer",
-    "TargetEncoder",
-    "deduplicate",
-    "compute_ngram_distance",
-]
+"""
+dirty_cat: Learning on dirty categories.
+"""
+from pathlib import Path as _Path
+
+try:
+    from ._check_dependencies import check_dependencies
+
+    check_dependencies()
+except ModuleNotFoundError:
+    import warnings
+
+    warnings.warn(
+        "pkg_resources is not available, dependencies versions will not be checked."
+    )
+
+from ._datetime_encoder import DatetimeEncoder
+from ._deduplicate import compute_ngram_distance, deduplicate
+from ._feature_augmenter import FeatureAugmenter
+from ._fuzzy_join import fuzzy_join
+from ._gap_encoder import GapEncoder
+from ._minhash_encoder import MinHashEncoder
+from ._similarity_encoder import SimilarityEncoder
+from ._table_vectorizer import SuperVectorizer, TableVectorizer
+from ._target_encoder import TargetEncoder
+
+with open(_Path(__file__).parent / "VERSION.txt") as _fh:
+    __version__ = _fh.read().strip()
+
+
+__all__ = [
+    "DatetimeEncoder",
+    "FeatureAugmenter",
+    "fuzzy_join",
+    "GapEncoder",
+    "MinHashEncoder",
+    "SimilarityEncoder",
+    "SuperVectorizer",
+    "TableVectorizer",
+    "TargetEncoder",
+    "deduplicate",
+    "compute_ngram_distance",
+]
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_check_dependencies.py` & `dirty_cat-0.4.1/dirty_cat/_check_dependencies.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import pkg_resources
-
-
-def check_dependencies():
-    package_name = "dirty-cat"
-    env = pkg_resources.Environment()
-    package = env[package_name][0]
-    requirements = package.requires()
-    for req in requirements:
-        try:
-            installed_dep = next(
-                iter(
-                    (
-                        installed_dep
-                        for installed_dep in env[req.name]
-                        if installed_dep.project_name == req.name
-                    )
-                )
-            )
-        except StopIteration:
-            raise ImportError(
-                f"{package_name} {package.version} requires {req}, "
-                "which you don't have."
-            )
-
-        if installed_dep not in req:
-            raise ImportError(
-                f"{package_name} {package.version} requires {req} "
-                f"but you have {installed_dep}, which is not compatible."
-            )
+import pkg_resources
+
+
+def check_dependencies():
+    package_name = "dirty-cat"
+    env = pkg_resources.Environment()
+    package = env[package_name][0]
+    requirements = package.requires()
+    for req in requirements:
+        try:
+            installed_dep = next(
+                iter(
+                    (
+                        installed_dep
+                        for installed_dep in env[req.name]
+                        if installed_dep.project_name == req.name
+                    )
+                )
+            )
+        except StopIteration:
+            raise ImportError(
+                f"{package_name} {package.version} requires {req}, "
+                "which you don't have."
+            )
+
+        if installed_dep not in req:
+            raise ImportError(
+                f"{package_name} {package.version} requires {req} "
+                f"but you have {installed_dep}, which is not compatible."
+            )
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_datetime_encoder.py` & `dirty_cat-0.4.1/dirty_cat/_datetime_encoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,275 +1,284 @@
-from typing import Dict, List, Literal, Optional
-from warnings import warn
-
-import numpy as np
-import pandas as pd
-from sklearn import __version__ as sklearn_version
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils.validation import check_is_fitted
-
-from dirty_cat._utils import check_input, parse_version
-
-# Required for ignoring lines too long in the docstrings
-# flake8: noqa: E501
-
-WORD_TO_ALIAS: Dict[str, str] = {
-    "year": "Y",
-    "month": "M",
-    "day": "D",
-    "hour": "H",
-    "minute": "min",
-    "second": "S",
-    "millisecond": "ms",
-    "microsecond": "us",
-    "nanosecond": "N",
-}
-TIME_LEVELS: List[str] = list(WORD_TO_ALIAS.keys())
-AcceptedTimeValues = Literal[
-    "year",
-    "month",
-    "day",
-    "hour",
-    "minute",
-    "second",
-    "millisecond",
-    "microsecond",
-    "nanosecond",
-]
-
-
-class DatetimeEncoder(BaseEstimator, TransformerMixin):
-    """
-    Transforms each datetime column into several numeric columns for temporal features (e.g year, month, day...).
-
-    Constant extracted features are dropped; for instance, if the year is
-    always the same in a feature, the extracted "year" column won't be added.
-    If the dates are timezone aware, all the features extracted will correspond
-    to the provided timezone.
-
-    Parameters
-    ----------
-    extract_until : AcceptedTimeValues, default="hour"
-        Extract up to this granularity.
-        If all features have not been extracted, add the "total_time" feature,
-        which contains the time to epoch (in seconds).
-        For instance, if you specify "day", only "year", "month", "day" and
-        "total_time" features will be created.
-    add_day_of_the_week : bool, default=False
-        Add day of the week feature (if day is extracted).
-        This is a numerical feature from 0 (Monday) to 6 (Sunday).
-
-    Attributes
-    ----------
-    n_features_in_: int
-        Number of features in the data seen during fit.
-    n_features_out_ : int
-        Number of features of the transformed data.
-    features_per_column_ : mapping of int to list of str
-        Dictionary mapping the index of the original columns
-        to the list of features extracted for each column.
-    col_names_ : None or list of str
-        List of the names of the features of the input data,
-        if input data was a pandas DataFrame, otherwise None.
-
-    Examples
-    --------
-    >>> enc = DatetimeEncoder()
-
-    Let's encode the following dates:
-
-    >>> X = [['2022-10-15'], ['2021-12-25'], ['2020-05-18'], ['2019-10-15 12:00:00']]
-
-    >>> enc.fit(X)
-    DatetimeEncoder()
-
-    The encoder will output a transformed array
-    with four columns (year, month, day and hour):
-
-    >>> enc.transform(X)
-    array([[2022.,   10.,   15.,    0.],
-           [2021.,   12.,   25.,    0.],
-           [2020.,    5.,   18.,    0.],
-           [2019.,   10.,   15.,   12.]])
-    """
-
-    n_features_in_: int
-    n_features_out_: int
-    features_per_column_: Dict[int, List[str]]
-    col_names_: Optional[List[str]]
-
-    def __init__(
-        self,
-        extract_until: AcceptedTimeValues = "hour",
-        add_day_of_the_week: bool = False,
-    ):
-        self.extract_until = extract_until
-        self.add_day_of_the_week = add_day_of_the_week
-
-    def _more_tags(self):
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def _validate_keywords(self):
-        if self.extract_until not in TIME_LEVELS:
-            raise ValueError(
-                f'"extract_until" should be one of {TIME_LEVELS}, '
-                f"got {self.extract_until}. "
-            )
-
-    @staticmethod
-    def _extract_from_date(date_series: pd.Series, feature: str):
-        if feature == "year":
-            return pd.DatetimeIndex(date_series).year.to_numpy()
-        elif feature == "month":
-            return pd.DatetimeIndex(date_series).month.to_numpy()
-        elif feature == "day":
-            return pd.DatetimeIndex(date_series).day.to_numpy()
-        elif feature == "hour":
-            return pd.DatetimeIndex(date_series).hour.to_numpy()
-        elif feature == "minute":
-            return pd.DatetimeIndex(date_series).minute.to_numpy()
-        elif feature == "second":
-            return pd.DatetimeIndex(date_series).second.to_numpy()
-        elif feature == "millisecond":
-            return pd.DatetimeIndex(date_series).millisecond.to_numpy()
-        elif feature == "microsecond":
-            return pd.DatetimeIndex(date_series).microsecond.to_numpy()
-        elif feature == "nanosecond":
-            return pd.DatetimeIndex(date_series).nanosecond.to_numpy()
-        elif feature == "dayofweek":
-            return pd.DatetimeIndex(date_series).dayofweek.to_numpy()
-        elif feature == "total_time":
-            tz = pd.DatetimeIndex(date_series).tz
-            # Compute the time in seconds from the epoch time UTC
-            if tz is None:
-                return (
-                    pd.to_datetime(date_series) - pd.Timestamp("1970-01-01")
-                ) // pd.Timedelta("1s")
-            else:
-                return (
-                    pd.DatetimeIndex(date_series).tz_convert("utc")
-                    - pd.Timestamp("1970-01-01", tz="utc")
-                ) // pd.Timedelta("1s")
-
-    def fit(self, X, y=None) -> "DatetimeEncoder":
-        """Fit the instance to X.
-
-        In practice, just stores which extracted features are not constant.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            Data where each column is a datetime feature.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        :class:`~dirty_cat.DatetimeEncoder`
-            Fitted :class:`~dirty_cat.DatetimeEncoder` instance (self).
-        """
-        self._validate_keywords()
-        # Columns to extract for each column,
-        # before taking into account constant columns
-        self._to_extract = TIME_LEVELS[: TIME_LEVELS.index(self.extract_until) + 1]
-        if self.add_day_of_the_week:
-            self._to_extract.append("dayofweek")
-        if isinstance(X, pd.DataFrame):
-            self.col_names_ = X.columns.to_list()
-        else:
-            self.col_names_ = None
-        X = check_input(X)
-        # Features to extract for each column, after removing constant features
-        self.features_per_column_ = {}
-        for i in range(X.shape[1]):
-            self.features_per_column_[i] = []
-        # Check which columns are constant
-        for i in range(X.shape[1]):
-            for feature in self._to_extract:
-                if np.nanstd(self._extract_from_date(X[:, i], feature)) > 0:
-                    self.features_per_column_[i].append(feature)
-            # If some date features have not been extracted, then add the
-            # "total_time" feature, which contains the full time to epoch
-            remainder = (
-                pd.to_datetime(X[:, i])
-                - pd.to_datetime(
-                    pd.DatetimeIndex(X[:, i]).floor(WORD_TO_ALIAS[self.extract_until])
-                )
-            ).seconds.to_numpy()
-            if np.nanstd(remainder) > 0:
-                self.features_per_column_[i].append("total_time")
-
-        self.n_features_in_ = X.shape[1]
-        self.n_features_out_ = len(
-            np.concatenate(list(self.features_per_column_.values()))
-        )
-
-        return self
-
-    def transform(self, X, y=None) -> np.ndarray:
-        """Transform X by replacing each datetime column with corresponding numerical features.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            The data to transform, where each column is a datetime feature.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        :obj:`~numpy.ndarray`, shape (n_samples, n_features_out_)
-            Transformed input.
-        """
-        check_is_fitted(
-            self,
-            attributes=["n_features_in_", "n_features_out_", "features_per_column_"],
-        )
-        X = check_input(X)
-        if X.shape[1] != self.n_features_in_:
-            raise ValueError(
-                f"The number of features in the input data ({X.shape[1]}) "
-                "does not match the number of features "
-                f"seen during fit ({self.n_features_in_}). "
-            )
-        # Create a new array with the extracted features,
-        # choosing only features that weren't constant during fit
-        X_ = np.empty((X.shape[0], self.n_features_out_), dtype=np.float64)
-        idx = 0
-        for i in range(X.shape[1]):
-            for j, feature in enumerate(self.features_per_column_[i]):
-                X_[:, idx + j] = self._extract_from_date(X[:, i], feature)
-            idx += len(self.features_per_column_[i])
-        return X_
-
-    def get_feature_names_out(self, input_features=None) -> List[str]:
-        """
-        Returns clean feature names with format "<column_name>_<new_feature>"
-        if the original data has column names, otherwise with format
-        "<column_index>_<new_feature>" where `<new_feature>` is one of
-        ["year", "month", "day", "hour", "minute", "second", "millisecond",
-        "microsecond", "nanosecond", "dayofweek"].
-        """
-        feature_names = []
-        for i in self.features_per_column_.keys():
-            prefix = str(i) if self.col_names_ is None else self.col_names_[i]
-            for feature in self.features_per_column_[i]:
-                feature_names.append(f"{prefix}_{feature}")
-        return feature_names
-
-    def get_feature_names(self, input_features=None) -> List[str]:
-        """
-        Ensures compatibility with sklearn < 1.0, and returns the output of
-        get_feature_names_out.
-        """
-        if parse_version(sklearn_version) >= parse_version("1.0"):
-            warn(
-                "Following the changes in scikit-learn 1.0, "
-                "get_feature_names is deprecated. "
-                "Use get_feature_names_out instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        return self.get_feature_names_out()
+from typing import Dict, List, Literal, Optional
+from warnings import warn
+
+import numpy as np
+import pandas as pd
+from sklearn import __version__ as sklearn_version
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils.validation import check_is_fitted
+
+from dirty_cat._utils import check_input, parse_version
+
+# Required for ignoring lines too long in the docstrings
+# flake8: noqa: E501
+
+WORD_TO_ALIAS: Dict[str, str] = {
+    "year": "Y",
+    "month": "M",
+    "day": "D",
+    "hour": "H",
+    "minute": "min",
+    "second": "S",
+    "millisecond": "ms",
+    "microsecond": "us",
+    "nanosecond": "N",
+}
+TIME_LEVELS: List[str] = list(WORD_TO_ALIAS.keys())
+AcceptedTimeValues = Literal[
+    "year",
+    "month",
+    "day",
+    "hour",
+    "minute",
+    "second",
+    "millisecond",
+    "microsecond",
+    "nanosecond",
+]
+
+
+class DatetimeEncoder(BaseEstimator, TransformerMixin):
+    """
+    Transforms each datetime column into several numeric columns for temporal features (e.g year, month, day...).
+
+    Constant extracted features are dropped; for instance, if the year is
+    always the same in a feature, the extracted "year" column won't be added.
+    If the dates are timezone aware, all the features extracted will correspond
+    to the provided timezone.
+
+    Parameters
+    ----------
+    extract_until : AcceptedTimeValues, default="hour"
+        Extract up to this granularity.
+        If all features have not been extracted, add the "total_time" feature,
+        which contains the time to epoch (in seconds).
+        For instance, if you specify "day", only "year", "month", "day" and
+        "total_time" features will be created.
+    add_day_of_the_week : bool, default=False
+        Add day of the week feature (if day is extracted).
+        This is a numerical feature from 0 (Monday) to 6 (Sunday).
+
+    Attributes
+    ----------
+    n_features_in_: int
+        Number of features in the data seen during fit.
+    n_features_out_ : int
+        Number of features of the transformed data.
+    features_per_column_ : mapping of int to list of str
+        Dictionary mapping the index of the original columns
+        to the list of features extracted for each column.
+    col_names_ : None or list of str
+        List of the names of the features of the input data,
+        if input data was a pandas DataFrame, otherwise None.
+
+    See Also
+    --------
+    :class:`~dirty_cat.GapEncoder` :
+        Encodes dirty categories (strings) by constructing latent topics with continuous encoding.
+    :class:`~dirty_cat.MinHashEncoder` :
+        Encode string columns as a numeric array with the minhash method.
+    :class:`~dirty_cat.SimilarityEncoder` :
+        Encode string columns as a numeric array with n-gram string similarity.
+
+    Examples
+    --------
+    >>> enc = DatetimeEncoder()
+
+    Let's encode the following dates:
+
+    >>> X = [['2022-10-15'], ['2021-12-25'], ['2020-05-18'], ['2019-10-15 12:00:00']]
+
+    >>> enc.fit(X)
+    DatetimeEncoder()
+
+    The encoder will output a transformed array
+    with four columns (year, month, day and hour):
+
+    >>> enc.transform(X)
+    array([[2022.,   10.,   15.,    0.],
+           [2021.,   12.,   25.,    0.],
+           [2020.,    5.,   18.,    0.],
+           [2019.,   10.,   15.,   12.]])
+    """
+
+    n_features_in_: int
+    n_features_out_: int
+    features_per_column_: Dict[int, List[str]]
+    col_names_: Optional[List[str]]
+
+    def __init__(
+        self,
+        extract_until: AcceptedTimeValues = "hour",
+        add_day_of_the_week: bool = False,
+    ):
+        self.extract_until = extract_until
+        self.add_day_of_the_week = add_day_of_the_week
+
+    def _more_tags(self):
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {"X_types": ["categorical"]}
+
+    def _validate_keywords(self):
+        if self.extract_until not in TIME_LEVELS:
+            raise ValueError(
+                f'"extract_until" should be one of {TIME_LEVELS}, '
+                f"got {self.extract_until}. "
+            )
+
+    @staticmethod
+    def _extract_from_date(date_series: pd.Series, feature: str):
+        if feature == "year":
+            return pd.DatetimeIndex(date_series).year.to_numpy()
+        elif feature == "month":
+            return pd.DatetimeIndex(date_series).month.to_numpy()
+        elif feature == "day":
+            return pd.DatetimeIndex(date_series).day.to_numpy()
+        elif feature == "hour":
+            return pd.DatetimeIndex(date_series).hour.to_numpy()
+        elif feature == "minute":
+            return pd.DatetimeIndex(date_series).minute.to_numpy()
+        elif feature == "second":
+            return pd.DatetimeIndex(date_series).second.to_numpy()
+        elif feature == "millisecond":
+            return pd.DatetimeIndex(date_series).millisecond.to_numpy()
+        elif feature == "microsecond":
+            return pd.DatetimeIndex(date_series).microsecond.to_numpy()
+        elif feature == "nanosecond":
+            return pd.DatetimeIndex(date_series).nanosecond.to_numpy()
+        elif feature == "dayofweek":
+            return pd.DatetimeIndex(date_series).dayofweek.to_numpy()
+        elif feature == "total_time":
+            tz = pd.DatetimeIndex(date_series).tz
+            # Compute the time in seconds from the epoch time UTC
+            if tz is None:
+                return (
+                    pd.to_datetime(date_series) - pd.Timestamp("1970-01-01")
+                ) // pd.Timedelta("1s")
+            else:
+                return (
+                    pd.DatetimeIndex(date_series).tz_convert("utc")
+                    - pd.Timestamp("1970-01-01", tz="utc")
+                ) // pd.Timedelta("1s")
+
+    def fit(self, X, y=None) -> "DatetimeEncoder":
+        """Fit the instance to X.
+
+        In practice, just stores which extracted features are not constant.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Data where each column is a datetime feature.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        :class:`~dirty_cat.DatetimeEncoder`
+            Fitted :class:`~dirty_cat.DatetimeEncoder` instance (self).
+        """
+        self._validate_keywords()
+        # Columns to extract for each column,
+        # before taking into account constant columns
+        self._to_extract = TIME_LEVELS[: TIME_LEVELS.index(self.extract_until) + 1]
+        if self.add_day_of_the_week:
+            self._to_extract.append("dayofweek")
+        if isinstance(X, pd.DataFrame):
+            self.col_names_ = X.columns.to_list()
+        else:
+            self.col_names_ = None
+        X = check_input(X)
+        # Features to extract for each column, after removing constant features
+        self.features_per_column_ = {}
+        for i in range(X.shape[1]):
+            self.features_per_column_[i] = []
+        # Check which columns are constant
+        for i in range(X.shape[1]):
+            for feature in self._to_extract:
+                if np.nanstd(self._extract_from_date(X[:, i], feature)) > 0:
+                    self.features_per_column_[i].append(feature)
+            # If some date features have not been extracted, then add the
+            # "total_time" feature, which contains the full time to epoch
+            remainder = (
+                pd.to_datetime(X[:, i])
+                - pd.to_datetime(
+                    pd.DatetimeIndex(X[:, i]).floor(WORD_TO_ALIAS[self.extract_until])
+                )
+            ).seconds.to_numpy()
+            if np.nanstd(remainder) > 0:
+                self.features_per_column_[i].append("total_time")
+
+        self.n_features_in_ = X.shape[1]
+        self.n_features_out_ = len(
+            np.concatenate(list(self.features_per_column_.values()))
+        )
+
+        return self
+
+    def transform(self, X, y=None) -> np.ndarray:
+        """Transform X by replacing each datetime column with corresponding numerical features.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            The data to transform, where each column is a datetime feature.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray`, shape (n_samples, n_features_out_)
+            Transformed input.
+        """
+        check_is_fitted(
+            self,
+            attributes=["n_features_in_", "n_features_out_", "features_per_column_"],
+        )
+        X = check_input(X)
+        if X.shape[1] != self.n_features_in_:
+            raise ValueError(
+                f"The number of features in the input data ({X.shape[1]}) "
+                "does not match the number of features "
+                f"seen during fit ({self.n_features_in_}). "
+            )
+        # Create a new array with the extracted features,
+        # choosing only features that weren't constant during fit
+        X_ = np.empty((X.shape[0], self.n_features_out_), dtype=np.float64)
+        idx = 0
+        for i in range(X.shape[1]):
+            for j, feature in enumerate(self.features_per_column_[i]):
+                X_[:, idx + j] = self._extract_from_date(X[:, i], feature)
+            idx += len(self.features_per_column_[i])
+        return X_
+
+    def get_feature_names_out(self, input_features=None) -> List[str]:
+        """
+        Returns clean feature names with format "<column_name>_<new_feature>"
+        if the original data has column names, otherwise with format
+        "<column_index>_<new_feature>" where `<new_feature>` is one of
+        ["year", "month", "day", "hour", "minute", "second", "millisecond",
+        "microsecond", "nanosecond", "dayofweek"].
+        """
+        feature_names = []
+        for i in self.features_per_column_.keys():
+            prefix = str(i) if self.col_names_ is None else self.col_names_[i]
+            for feature in self.features_per_column_[i]:
+                feature_names.append(f"{prefix}_{feature}")
+        return feature_names
+
+    def get_feature_names(self, input_features=None) -> List[str]:
+        """
+        Ensures compatibility with sklearn < 1.0, and returns the output of
+        get_feature_names_out.
+        """
+        if parse_version(sklearn_version) >= parse_version("1.0"):
+            warn(
+                "Following the changes in scikit-learn 1.0, "
+                "get_feature_names is deprecated. "
+                "Use get_feature_names_out instead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        return self.get_feature_names_out()
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_deduplicate.py` & `dirty_cat-0.4.1/dirty_cat/_deduplicate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,219 +1,230 @@
-"""
-Implements deduplication based on clustering string distance matrices.
-This works best if there is a number of underlying categories that
-sometimes appear in the data with small variations and/or misspellings.
-"""
-from typing import List, Literal, Optional, Sequence, Tuple, Union
-
-import numpy as np
-import pandas as pd
-from scipy.cluster.hierarchy import fcluster, linkage
-from scipy.spatial.distance import pdist, squareform
-from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.metrics import silhouette_score
-
-
-def compute_ngram_distance(
-    unique_words: Union[Sequence[str], np.ndarray],
-    ngram_range: Tuple[int, int] = (2, 4),
-    analyzer: str = "char_wb",
-) -> np.ndarray:
-    """Compute the condensed pair-wise n-gram distance between `unique_words`.
-
-    Parameters
-    ----------
-    unique_words : Union[Sequence[str], np.ndarray]
-        Sequence or array of unique words from the original data.
-    ngram_range : Tuple[int, int], optional, default=(2,4)
-        The n-gram range to compute the distance in.
-    analyzer : str, optional, default=`char_wb`
-        Analyzer to extract n-grams.
-
-    Returns
-    -------
-    np.ndarray
-        An n-times-(n-1)/2 array of n-gram tf-idf distances between `unique_words`.
-
-    Notes
-    -----
-    Extracts n-grams of all elements in `unique_words`, calculates the
-    term frequency-inverse document frequency (tf-idf) for each n-gram, then
-    computes the pair-wise euclidean distance between elements based on their n-gram
-    tf-idf representation.
-    """
-    encoded = TfidfVectorizer(ngram_range=ngram_range, analyzer=analyzer).fit_transform(
-        unique_words
-    )
-
-    distance_mat = pdist(encoded.todense(), metric="euclidean")
-    return distance_mat
-
-
-def _guess_clusters(Z: np.ndarray, distance_mat: np.ndarray) -> int:
-    """Finds the number of clusters that maximize the silhouette score
-    when clustering `distance_mat`.
-
-    Parameters
-    ----------
-    Z : np.ndarray
-        hierarchical linkage matrix, specifies which clusters to merge.
-    distance_mat : np.ndarray
-        distance matrix either in square or condensed form.
-
-    Returns
-    -------
-    int
-        number of clusters that maximize the silhouette score.
-    """
-    max_clusters = distance_mat.shape[0]
-    n_clusters = np.arange(2, max_clusters)
-    # silhouette score needs a redundant distance matrix
-    redundant_dist = squareform(distance_mat)
-    silhouette_scores = []
-    for n_clust in n_clusters:
-        labels = fcluster(Z, n_clust, criterion="maxclust")
-        silhouette_avg = silhouette_score(redundant_dist, labels, metric="precomputed")
-        silhouette_scores.append(silhouette_avg)
-    return n_clusters[np.argmax(silhouette_scores)]
-
-
-def _create_spelling_correction(
-    unique_words: Union[Sequence[str], np.ndarray],
-    counts: Union[Sequence[int], np.ndarray],
-    clusters: Sequence[int],
-) -> pd.Series:
-    """Creates a pandas Series that map each cluster member to the most
-    frequent cluster member. The assumption is that the most common spelling
-    is the correct one.
-
-    Parameters
-    ----------
-    unique_words : Union[Sequence[str], np.ndarray]
-        A sequence or array of unique words in the original data.
-    counts : Union[Sequence[int], np.ndarray]
-        A sequence or array of counts of how often each unique word appears in
-        the original data.
-    clusters : Sequence[int]
-        A sequence of ints, indicating cluster membership of each unique word
-        in `count_series`.
-
-    Returns
-    -------
-    pd.Series
-        Series with unique (original) words as indices and (estimated)
-        corrected spelling of each word as values.
-    """
-    count_series = pd.Series(counts, index=unique_words)
-    original_spelling: List[str] = []
-    corrected_spelling: List[str] = []
-    for cluster in np.unique(clusters):
-        sorted_spellings = (
-            count_series.loc[clusters == cluster]
-            .sort_values(ascending=False)
-            .index.tolist()
-        )
-        original_spelling.extend(sorted_spellings)
-        # assumes spelling that occurs most frequently in cluster is correct
-        corrected_spelling.extend(sorted_spellings[:1] * len(sorted_spellings))
-    pd_spell_correct = pd.Series(corrected_spelling, index=original_spelling)
-    return pd_spell_correct
-
-
-def deduplicate(
-    data: Sequence[str],
-    n_clusters: Optional[int] = None,
-    ngram_range: Tuple[int, int] = (2, 4),
-    analyzer: Literal["word", "char", "char_wb"] = "char_wb",
-    method: Literal[
-        "single", "complete", "average", "centroid", "median", "ward"
-    ] = "average",
-) -> List[str]:
-    """Deduplicate data by hierarchically clustering similar strings.
-
-    Parameters
-    ----------
-    data : Sequence[str]
-        The data to be deduplicated.
-    n_clusters : Optional[int], optional, default=None
-        Number of clusters to use for hierarchical clustering, if None use the
-        number of clusters that lead to the lowest silhouette score.
-    ngram_range : Tuple[int, int], optional, default=(2, 4)
-        Range to use for computing n-gram distance.
-    analyzer : typing.Literal["word", "char", "char_wb"], optional, default=`char_wb`
-        Analyzer parameter for the CountVectorizer used for the string
-        similarities.
-        Options: {`word`, `char`, `char_wb`}, describing whether the matrix V
-        to factorize should be made of word counts or character n-gram counts.
-        Option `char_wb` creates character n-grams only from text inside word
-        boundaries; n-grams at the edges of words are padded with space.
-    method : str, optional, default=`average`
-        Linkage method parameter to use for merging clusters via scipy's
-        `linkage` method.
-        Options: {`single`, `complete`, `average`, `centroid`, `median`, `ward`},
-        describing different methods to calculate the distance between two clusters.
-        Option `average` calculates the distance between two clusters as the average
-        distance between data points in the first and second cluster.
-
-    Returns
-    -------
-    List[str]
-       The deduplicated data.
-
-    Notes
-    -----
-    Deduplication is done by first computing the n-gram distance between unique
-    categories in data, then performing hierarchical clustering on this distance
-    matrix, and choosing the most frequent element in each cluster as the
-    'correct' spelling. This method works best if the true number of
-    categories is significantly smaller than the number of observed spellings.
-
-    Examples
-    --------
-    >>> from dirty_cat.datasets import make_deduplication_data
-    >>> duplicated = make_deduplication_data(examples=['black', 'white'],
-                                             entries_per_example=[5, 5],
-                                             prob_mistake_per_letter=0.3,
-                                             random_state=42)
-
-    >>> duplicated
-    ['blacn', 'black', 'black', 'black', 'black',
-     'hvite', 'white', 'white', 'white', 'white']
-
-    To deduplicate the data, we can build a correspondance matrix:
-
-    >>> deduplicate_correspondence = deduplicate(duplicated)
-    >>> deduplicate_correspondence
-    blacn    black
-    black    black
-    black    black
-    black    black
-    black    black
-    hvite    white
-    white    white
-    white    white
-    white    white
-    white    white
-    dtype: object
-
-    The translation table above is actually a series, giving the deduplicated values, and indexed by the original values. A deduplicated version of the initial list can easily be created:
-
-    >>> deduplicated = list(deduplicate_correspondence)
-    >>> deduplicated
-    ['black', 'black', 'black', 'black', 'black',
-    'white', 'white', 'white', 'white', 'white']
-
-    We have our dirty categories deduplicated.
-    """
-    unique_words, counts = np.unique(data, return_counts=True)
-    distance_mat = compute_ngram_distance(
-        unique_words, ngram_range=ngram_range, analyzer=analyzer
-    )
-
-    Z = linkage(distance_mat, method=method, optimal_ordering=True)
-    if n_clusters is None:
-        n_clusters = _guess_clusters(Z, distance_mat)
-    clusters = fcluster(Z, n_clusters, criterion="maxclust")
-
-    translation_table = _create_spelling_correction(unique_words, counts, clusters)
-    unrolled_corrections = translation_table[data]
-    return unrolled_corrections
+"""
+Implements deduplication based on clustering string distance matrices.
+This works best if there is a number of underlying categories that
+sometimes appear in the data with small variations and/or misspellings.
+"""
+from typing import List, Literal, Optional, Sequence, Tuple, Union
+
+import numpy as np
+import pandas as pd
+from scipy.cluster.hierarchy import fcluster, linkage
+from scipy.spatial.distance import pdist, squareform
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.metrics import silhouette_score
+
+
+def compute_ngram_distance(
+    unique_words: Union[Sequence[str], np.ndarray],
+    ngram_range: Tuple[int, int] = (2, 4),
+    analyzer: str = "char_wb",
+) -> np.ndarray:
+    """Compute the condensed pair-wise n-gram distance between `unique_words`.
+
+    Parameters
+    ----------
+    unique_words : Union[Sequence[str], np.ndarray]
+        Sequence or array of unique words from the original data.
+    ngram_range : Tuple[int, int], optional, default=(2,4)
+        The n-gram range to compute the distance in.
+    analyzer : str, optional, default=`char_wb`
+        Analyzer to extract n-grams.
+
+    Returns
+    -------
+    np.ndarray
+        An n-times-(n-1)/2 array of n-gram tf-idf distances between `unique_words`.
+
+    Notes
+    -----
+    Extracts n-grams of all elements in `unique_words`, calculates the
+    term frequency-inverse document frequency (tf-idf) for each n-gram, then
+    computes the pair-wise euclidean distance between elements based on their n-gram
+    tf-idf representation.
+    """
+    encoded = TfidfVectorizer(ngram_range=ngram_range, analyzer=analyzer).fit_transform(
+        unique_words
+    )
+
+    distance_mat = pdist(encoded.todense(), metric="euclidean")
+    return distance_mat
+
+
+def _guess_clusters(Z: np.ndarray, distance_mat: np.ndarray) -> int:
+    """Finds the number of clusters that maximize the silhouette score
+    when clustering `distance_mat`.
+
+    Parameters
+    ----------
+    Z : np.ndarray
+        hierarchical linkage matrix, specifies which clusters to merge.
+    distance_mat : np.ndarray
+        distance matrix either in square or condensed form.
+
+    Returns
+    -------
+    int
+        number of clusters that maximize the silhouette score.
+    """
+    max_clusters = distance_mat.shape[0]
+    n_clusters = np.arange(2, max_clusters)
+    # silhouette score needs a redundant distance matrix
+    redundant_dist = squareform(distance_mat)
+    silhouette_scores = []
+    for n_clust in n_clusters:
+        labels = fcluster(Z, n_clust, criterion="maxclust")
+        silhouette_avg = silhouette_score(redundant_dist, labels, metric="precomputed")
+        silhouette_scores.append(silhouette_avg)
+    return n_clusters[np.argmax(silhouette_scores)]
+
+
+def _create_spelling_correction(
+    unique_words: Union[Sequence[str], np.ndarray],
+    counts: Union[Sequence[int], np.ndarray],
+    clusters: Sequence[int],
+) -> pd.Series:
+    """Creates a pandas Series that map each cluster member to the most
+    frequent cluster member. The assumption is that the most common spelling
+    is the correct one.
+
+    Parameters
+    ----------
+    unique_words : Union[Sequence[str], np.ndarray]
+        A sequence or array of unique words in the original data.
+    counts : Union[Sequence[int], np.ndarray]
+        A sequence or array of counts of how often each unique word appears in
+        the original data.
+    clusters : Sequence[int]
+        A sequence of ints, indicating cluster membership of each unique word
+        in `count_series`.
+
+    Returns
+    -------
+    pd.Series
+        Series with unique (original) words as indices and (estimated)
+        corrected spelling of each word as values.
+    """
+    count_series = pd.Series(counts, index=unique_words)
+    original_spelling: List[str] = []
+    corrected_spelling: List[str] = []
+    for cluster in np.unique(clusters):
+        sorted_spellings = (
+            count_series.loc[clusters == cluster]
+            .sort_values(ascending=False)
+            .index.tolist()
+        )
+        original_spelling.extend(sorted_spellings)
+        # assumes spelling that occurs most frequently in cluster is correct
+        corrected_spelling.extend(sorted_spellings[:1] * len(sorted_spellings))
+    pd_spell_correct = pd.Series(corrected_spelling, index=original_spelling)
+    return pd_spell_correct
+
+
+def deduplicate(
+    data: Sequence[str],
+    n_clusters: Optional[int] = None,
+    ngram_range: Tuple[int, int] = (2, 4),
+    analyzer: Literal["word", "char", "char_wb"] = "char_wb",
+    method: Literal[
+        "single", "complete", "average", "centroid", "median", "ward"
+    ] = "average",
+) -> List[str]:
+    """Deduplicate data by hierarchically clustering similar strings.
+
+    Parameters
+    ----------
+    data : Sequence[str]
+        The data to be deduplicated.
+    n_clusters : Optional[int], optional, default=None
+        Number of clusters to use for hierarchical clustering, if None use the
+        number of clusters that lead to the lowest silhouette score.
+    ngram_range : Tuple[int, int], optional, default=(2, 4)
+        Range to use for computing n-gram distance.
+    analyzer : typing.Literal["word", "char", "char_wb"], optional, default=`char_wb`
+        Analyzer parameter for the CountVectorizer used for the string
+        similarities.
+        Options: {`word`, `char`, `char_wb`}, describing whether the matrix V
+        to factorize should be made of word counts or character n-gram counts.
+        Option `char_wb` creates character n-grams only from text inside word
+        boundaries; n-grams at the edges of words are padded with space.
+    method : str, optional, default=`average`
+        Linkage method parameter to use for merging clusters via scipy's
+        `linkage` method.
+        Options: {`single`, `complete`, `average`, `centroid`, `median`, `ward`},
+        describing different methods to calculate the distance between two clusters.
+        Option `average` calculates the distance between two clusters as the average
+        distance between data points in the first and second cluster.
+
+    Returns
+    -------
+    List[str]
+       The deduplicated data.
+
+    See Also
+    --------
+    :class:`~dirty_cat.GapEncoder` :
+        Encodes dirty categories (strings) by constructing latent topics with continuous encoding.
+    :class:`~dirty_cat.MinHashEncoder` :
+        Encode string columns as a numeric array with the minhash method.
+    :class:`~dirty_cat.SimilarityEncoder` :
+        Encode string columns as a numeric array with n-gram string similarity.
+
+    Notes
+    -----
+    Deduplication is done by first computing the n-gram distance between unique
+    categories in data, then performing hierarchical clustering on this distance
+    matrix, and choosing the most frequent element in each cluster as the
+    'correct' spelling. This method works best if the true number of
+    categories is significantly smaller than the number of observed spellings.
+
+    Examples
+    --------
+    >>> from dirty_cat.datasets import make_deduplication_data
+    >>> duplicated = make_deduplication_data(examples=['black', 'white'],
+                                             entries_per_example=[5, 5],
+                                             prob_mistake_per_letter=0.3,
+                                             random_state=42)
+
+    >>> duplicated
+    ['blacn', 'black', 'black', 'black', 'black',
+     'hvite', 'white', 'white', 'white', 'white']
+
+    To deduplicate the data, we can build a correspondance matrix:
+
+    >>> deduplicate_correspondence = deduplicate(duplicated)
+    >>> deduplicate_correspondence
+    blacn    black
+    black    black
+    black    black
+    black    black
+    black    black
+    hvite    white
+    white    white
+    white    white
+    white    white
+    white    white
+    dtype: object
+
+    The translation table above is actually a series, giving the deduplicated values,
+    and indexed by the original values.
+    A deduplicated version of the initial list can easily be created:
+
+    >>> deduplicated = list(deduplicate_correspondence)
+    >>> deduplicated
+    ['black', 'black', 'black', 'black', 'black',
+    'white', 'white', 'white', 'white', 'white']
+
+    We have our dirty categories deduplicated.
+    """
+    unique_words, counts = np.unique(data, return_counts=True)
+    distance_mat = compute_ngram_distance(
+        unique_words, ngram_range=ngram_range, analyzer=analyzer
+    )
+
+    Z = linkage(distance_mat, method=method, optimal_ordering=True)
+    if n_clusters is None:
+        n_clusters = _guess_clusters(Z, distance_mat)
+    clusters = fcluster(Z, n_clusters, criterion="maxclust")
+
+    translation_table = _create_spelling_correction(unique_words, counts, clusters)
+    unrolled_corrections = translation_table[data]
+    return unrolled_corrections
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_fast_hash.py` & `dirty_cat-0.4.1/dirty_cat/_fast_hash.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""
-n-gram hashing by simple dot products
-
-The principle is as follows:
-  1. A string is viewed as a succession of numbers (the ASCII or UTF8
-     representation of its elements).
-  2. Each n-gram is then an n-dimensional vector of integers "g". A simple
-     hash function is then computed by taking the dot product with a
-     given random vector "atom", modulo max-int (integers larger than
-     max-int overflow). The corresponding operation defines a random
-     order in the interval [-maxint, maxint]
-  3. Computing this dot product over a sliding window (to compute it for
-     every n-gram is a convolution)
-  4. We can then take the min (or the max) of the resulting sliding window
-"""
-
-import functools
-
-import numpy as np
-
-# Precompute to avoid the cost and
-# cast to int32 to speed up the min
-MININT32 = np.int32(-(2 ** (32 - 1)))
-MAXINT32 = np.int32(2 ** (32 - 1) - 1)
-
-
-@functools.lru_cache(maxsize=1024)
-def gen_atom(atom_len, seed=0):
-    """
-    Generate a random integer array (atom).
-
-    Parameters
-    ----------
-    atom_len : int
-        The length of the atom.
-    seed : int, default=0
-        The seed of the random_number generator.
-
-    Returns
-    -------
-    array, shape (atom_len, )
-        An array of random integers of length atom_len and dtype int32
-        (assuming dtype_size=32).
-    """
-    rng = np.random.RandomState(seed)
-    atom = rng.randint(-MAXINT32, MAXINT32, size=atom_len, dtype=np.dtype("int32"))
-    return atom
-
-
-def ngram_min_hash(string, ngram_range=(2, 4), seed=0, return_minmax=False):
-    """
-    Compute the min/max hash of the ngrams of the string.
-
-    Parameters
-    ----------
-    string : str
-        String to encode.
-    ngram_range : tuple (min_n, max_n), default=(2, 4)
-        The lower and upper boundary of the range of n-values
-        for different n-grams to be extracted.
-    seed : int, default=0
-        Integer used to seed the hashing function.
-    return_minmax : bool, default=False
-        If True, returns both the minhash and maxhash of the string.
-        Else, only returns the minhash.
-
-    Returns
-    -------
-    int or tuple
-        The min_hash or (min_hash, max_hash) of the n-grams of the string.
-    """
-    # Create a numerical 1D array from the string
-    array = np.frombuffer(string.encode(), dtype="int8", count=len(string))
-
-    max_hash = MININT32
-    min_hash = MAXINT32
-    for atom_len in range(ngram_range[0], ngram_range[1]):
-        atom = gen_atom(atom_len, seed=seed)
-        # np.correlate is faster than np.convolve
-        # the convolution gives a hash for each ngram
-        hashes = np.correlate(array, atom)
-        min_hash = min(min_hash, hashes.min())
-        if return_minmax:
-            max_hash = max(max_hash, hashes.max())
-
-    # We should check that longer windows do not have different
-    # statistics from shorter ones
-    if return_minmax:
-        return min_hash, max_hash
-    return min_hash
+"""
+n-gram hashing by simple dot products
+
+The principle is as follows:
+  1. A string is viewed as a succession of numbers (the ASCII or UTF8
+     representation of its elements).
+  2. Each n-gram is then an n-dimensional vector of integers "g". A simple
+     hash function is then computed by taking the dot product with a
+     given random vector "atom", modulo max-int (integers larger than
+     max-int overflow). The corresponding operation defines a random
+     order in the interval [-maxint, maxint]
+  3. Computing this dot product over a sliding window (to compute it for
+     every n-gram is a convolution)
+  4. We can then take the min (or the max) of the resulting sliding window
+"""
+
+import functools
+
+import numpy as np
+
+# Precompute to avoid the cost and
+# cast to int32 to speed up the min
+MININT32 = np.int32(-(2 ** (32 - 1)))
+MAXINT32 = np.int32(2 ** (32 - 1) - 1)
+
+
+@functools.lru_cache(maxsize=1024)
+def gen_atom(atom_len, seed=0):
+    """
+    Generate a random integer array (atom).
+
+    Parameters
+    ----------
+    atom_len : int
+        The length of the atom.
+    seed : int, default=0
+        The seed of the random_number generator.
+
+    Returns
+    -------
+    array, shape (atom_len, )
+        An array of random integers of length atom_len and dtype int32
+        (assuming dtype_size=32).
+    """
+    rng = np.random.RandomState(seed)
+    atom = rng.randint(-MAXINT32, MAXINT32, size=atom_len, dtype=np.dtype("int32"))
+    return atom
+
+
+def ngram_min_hash(string, ngram_range=(2, 4), seed=0, return_minmax=False):
+    """
+    Compute the min/max hash of the ngrams of the string.
+
+    Parameters
+    ----------
+    string : str
+        String to encode.
+    ngram_range : tuple (min_n, max_n), default=(2, 4)
+        The lower and upper boundary of the range of n-values
+        for different n-grams to be extracted.
+    seed : int, default=0
+        Integer used to seed the hashing function.
+    return_minmax : bool, default=False
+        If True, returns both the minhash and maxhash of the string.
+        Else, only returns the minhash.
+
+    Returns
+    -------
+    int or tuple
+        The min_hash or (min_hash, max_hash) of the n-grams of the string.
+    """
+    # Create a numerical 1D array from the string
+    array = np.frombuffer(string.encode(), dtype="int8", count=len(string))
+
+    max_hash = MININT32
+    min_hash = MAXINT32
+    for atom_len in range(ngram_range[0], ngram_range[1]):
+        atom = gen_atom(atom_len, seed=seed)
+        # np.correlate is faster than np.convolve
+        # the convolution gives a hash for each ngram
+        hashes = np.correlate(array, atom)
+        min_hash = min(min_hash, hashes.min())
+        if return_minmax:
+            max_hash = max(max_hash, hashes.max())
+
+    # We should check that longer windows do not have different
+    # statistics from shorter ones
+    if return_minmax:
+        return min_hash, max_hash
+    return min_hash
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_gap_encoder.py` & `dirty_cat-0.4.1/dirty_cat/_gap_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1077 +1,1089 @@
-"""
-Online Gamma-Poisson factorization of string arrays.
-The principle is as follows:
-    1. Given an input string array X, we build its bag-of-n-grams
-       representation V (n_samples, vocab_size).
-    2. Instead of using the n-grams counts as encodings, we look for low-
-       dimensional representations by modeling n-grams counts as linear
-       combinations of topics V = HW, with W (n_topics, vocab_size) the topics
-       and H (n_samples, n_topics) the associated activations.
-    3. Assuming that n-grams counts follow a Poisson law, we fit H and W to
-       maximize the likelihood of the data, with a Gamma prior for the
-       activations H to induce sparsity.
-    4. In practice, this is equivalent to a non-negative matrix factorization
-       with the Kullback-Leibler divergence as loss, and a Gamma prior on H.
-       We thus optimize H and W with the multiplicative update method.
-"""
-
-import warnings
-from typing import Dict, Generator, List, Literal, Optional, Tuple, Union
-
-import numpy as np
-import pandas as pd
-from numpy.random import RandomState
-from scipy import sparse
-from sklearn import __version__ as sklearn_version
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.cluster import KMeans
-from sklearn.feature_extraction.text import CountVectorizer, HashingVectorizer
-from sklearn.neighbors import NearestNeighbors
-from sklearn.utils import check_random_state, gen_batches
-from sklearn.utils.extmath import row_norms, safe_sparse_dot
-from sklearn.utils.fixes import _object_dtype_isnan
-from sklearn.utils.validation import check_is_fitted
-
-from ._utils import check_input, parse_version
-
-if parse_version(sklearn_version) < parse_version("0.24"):
-    from sklearn.cluster._kmeans import _k_init
-else:
-    from sklearn.cluster import kmeans_plusplus
-
-from sklearn.decomposition._nmf import _beta_divergence
-
-# Ignore lines too long, as some things in the docstring cannot be cut.
-# flake8: noqa: E501
-
-
-class GapEncoderColumn(BaseEstimator, TransformerMixin):
-
-    """See GapEncoder's docstring."""
-
-    rho_: float
-    H_dict_: Dict[np.ndarray, np.ndarray]
-
-    def __init__(
-        self,
-        n_components: int = 10,
-        batch_size: int = 128,
-        gamma_shape_prior: float = 1.1,
-        gamma_scale_prior: float = 1.0,
-        rho: float = 0.95,
-        rescale_rho: bool = False,
-        hashing: bool = False,
-        hashing_n_features: int = 2**12,
-        init: Literal["k-means++", "random", "k-means"] = "k-means++",
-        tol: float = 1e-4,
-        min_iter: int = 2,
-        max_iter: int = 5,
-        ngram_range: Tuple[int, int] = (2, 4),
-        analyzer: Literal["word", "char", "char_wb"] = "char",
-        add_words: bool = False,
-        random_state: Optional[Union[int, RandomState]] = None,
-        rescale_W: bool = True,
-        max_iter_e_step: int = 20,
-    ):
-        self.ngram_range = ngram_range
-        self.n_components = n_components
-        self.gamma_shape_prior = gamma_shape_prior  # 'a' parameter
-        self.gamma_scale_prior = gamma_scale_prior  # 'b' parameter
-        self.rho = rho
-        self.rescale_rho = rescale_rho
-        self.batch_size = batch_size
-        self.tol = tol
-        self.hashing = hashing
-        self.hashing_n_features = hashing_n_features
-        self.max_iter = max_iter
-        self.min_iter = min_iter
-        self.init = init
-        self.analyzer = analyzer
-        self.add_words = add_words
-        self.random_state = check_random_state(random_state)
-        self.rescale_W = rescale_W
-        self.max_iter_e_step = max_iter_e_step
-
-    def _init_vars(self, X) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """
-        Build the bag-of-n-grams representation V of X and initialize
-        the topics W.
-        """
-        # Init n-grams counts vectorizer
-        if self.hashing:
-            self.ngrams_count_ = HashingVectorizer(
-                analyzer=self.analyzer,
-                ngram_range=self.ngram_range,
-                n_features=self.hashing_n_features,
-                norm=None,
-                alternate_sign=False,
-            )
-            if self.add_words:  # Init a word counts vectorizer if needed
-                self.word_count_ = HashingVectorizer(
-                    analyzer="word",
-                    n_features=self.hashing_n_features,
-                    norm=None,
-                    alternate_sign=False,
-                )
-        else:
-            self.ngrams_count_ = CountVectorizer(
-                analyzer=self.analyzer, ngram_range=self.ngram_range, dtype=np.float64
-            )
-            if self.add_words:
-                self.word_count_ = CountVectorizer(dtype=np.float64)
-
-        # Init H_dict_ with empty dict to train from scratch
-        self.H_dict_ = dict()
-        # Build the n-grams counts matrix unq_V on unique elements of X
-        unq_X, lookup = np.unique(X, return_inverse=True)
-        unq_V = self.ngrams_count_.fit_transform(unq_X)
-        if self.add_words:  # Add word counts to unq_V
-            unq_V2 = self.word_count_.fit_transform(unq_X)
-            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
-
-        if not self.hashing:  # Build n-grams/word vocabulary
-            if parse_version(sklearn_version) < parse_version("1.0"):
-                self.vocabulary = self.ngrams_count_.get_feature_names()
-            else:
-                self.vocabulary = self.ngrams_count_.get_feature_names_out()
-            if self.add_words:
-                if parse_version(sklearn_version) < parse_version("1.0"):
-                    self.vocabulary = np.concatenate(
-                        (self.vocabulary, self.word_count_.get_feature_names())
-                    )
-                else:
-                    self.vocabulary = np.concatenate(
-                        (self.vocabulary, self.word_count_.get_feature_names_out())
-                    )
-        _, self.n_vocab = unq_V.shape
-        # Init the topics W given the n-grams counts V
-        self.W_, self.A_, self.B_ = self._init_w(unq_V[lookup], X)
-        # Init the activations unq_H of each unique input string
-        unq_H = _rescale_h(unq_V, np.ones((len(unq_X), self.n_components)))
-        # Update self.H_dict_ with unique input strings and their activations
-        self.H_dict_.update(zip(unq_X, unq_H))
-        if self.rescale_rho:
-            # Make update rate per iteration independent of the batch_size
-            self.rho_ = self.rho ** (self.batch_size / len(X))
-        return unq_X, unq_V, lookup
-
-    def _get_H(self, X: np.array) -> np.array:
-        """
-        Return the bag-of-n-grams representation of X.
-        """
-        H_out = np.empty((len(X), self.n_components))
-        for x, h_out in zip(X, H_out):
-            h_out[:] = self.H_dict_[x]
-        return H_out
-
-    def _init_w(self, V: np.array, X) -> Tuple[np.array, np.array, np.array]:
-        """
-        Initialize the topics W.
-        If self.init='k-means++', we use the init method of
-        sklearn.cluster.KMeans.
-        If self.init='random', topics are initialized with a Gamma
-        distribution.
-        If self.init='k-means', topics are initialized with a KMeans on the
-        n-grams counts.
-        """
-        if self.init == "k-means++":
-            if parse_version(sklearn_version) < parse_version("0.24"):
-                W = (
-                    _k_init(
-                        V,
-                        self.n_components,
-                        x_squared_norms=row_norms(V, squared=True),
-                        random_state=self.random_state,
-                        n_local_trials=None,
-                    )
-                    + 0.1
-                )
-            else:
-                W, _ = kmeans_plusplus(
-                    V,
-                    self.n_components,
-                    x_squared_norms=row_norms(V, squared=True),
-                    random_state=self.random_state,
-                    n_local_trials=None,
-                )
-                W = W + 0.1  # To avoid restricting topics to a few n-grams only
-        elif self.init == "random":
-            W = self.random_state.gamma(
-                shape=self.gamma_shape_prior,
-                scale=self.gamma_scale_prior,
-                size=(self.n_components, self.n_vocab),
-            )
-        elif self.init == "k-means":
-            prototypes = get_kmeans_prototypes(
-                X,
-                self.n_components,
-                analyzer=self.analyzer,
-                random_state=self.random_state,
-            )
-            W = self.ngrams_count_.transform(prototypes).A + 0.1
-            if self.add_words:
-                W2 = self.word_count_.transform(prototypes).A + 0.1
-                W = np.hstack((W, W2))
-            # if k-means doesn't find the exact number of prototypes
-            if W.shape[0] < self.n_components:
-                if parse_version(sklearn_version) < parse_version("0.24"):
-                    W2 = (
-                        _k_init(
-                            V,
-                            self.n_components - W.shape[0],
-                            x_squared_norms=row_norms(V, squared=True),
-                            random_state=self.random_state,
-                            n_local_trials=None,
-                        )
-                        + 0.1
-                    )
-                else:
-                    W2, _ = kmeans_plusplus(
-                        V,
-                        self.n_components - W.shape[0],
-                        x_squared_norms=row_norms(V, squared=True),
-                        random_state=self.random_state,
-                        n_local_trials=None,
-                    )
-                    W2 = W2 + 0.1
-                W = np.concatenate((W, W2), axis=0)
-        else:
-            raise ValueError(f"Initialization method {self.init!r} does not exist. ")
-        W /= W.sum(axis=1, keepdims=True)
-        A = np.ones((self.n_components, self.n_vocab)) * 1e-10
-        B = A.copy()
-        return W, A, B
-
-    def fit(self, X, y=None) -> "GapEncoderColumn":
-        """
-        Fit the GapEncoder on batches of X.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, )
-            The string data to fit the model on.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        self
-            Fitting GapEncoderColumn instance.
-        """
-        # Copy parameter rho
-        self.rho_ = self.rho
-        # Check if first item has str or np.str_ type
-        assert isinstance(X[0], str), "Input data is not string. "
-        # Make n-grams counts matrix unq_V
-        unq_X, unq_V, lookup = self._init_vars(X)
-        n_batch = (len(X) - 1) // self.batch_size + 1
-        del X
-        # Get activations unq_H
-        unq_H = self._get_H(unq_X)
-
-        for n_iter_ in range(self.max_iter):
-            # Loop over batches
-            for i, (unq_idx, idx) in enumerate(batch_lookup(lookup, n=self.batch_size)):
-                if i == n_batch - 1:
-                    W_last = self.W_.copy()
-                # Update activations unq_H
-                unq_H[unq_idx] = _multiplicative_update_h(
-                    unq_V[unq_idx],
-                    self.W_,
-                    unq_H[unq_idx],
-                    epsilon=1e-3,
-                    max_iter=self.max_iter_e_step,
-                    rescale_W=self.rescale_W,
-                    gamma_shape_prior=self.gamma_shape_prior,
-                    gamma_scale_prior=self.gamma_scale_prior,
-                )
-                # Update the topics self.W_
-                _multiplicative_update_w(
-                    unq_V[idx],
-                    self.W_,
-                    self.A_,
-                    self.B_,
-                    unq_H[idx],
-                    self.rescale_W,
-                    self.rho_,
-                )
-
-                if i == n_batch - 1:
-                    # Compute the norm of the update of W in the last batch
-                    W_change = np.linalg.norm(self.W_ - W_last) / np.linalg.norm(W_last)
-
-            if (W_change < self.tol) and (n_iter_ >= self.min_iter - 1):
-                break  # Stop if the change in W is smaller than the tolerance
-
-        # Update self.H_dict_ with the learned encoded vectors (activations)
-        self.H_dict_.update(zip(unq_X, unq_H))
-        return self
-
-    def get_feature_names(self, n_labels=3, prefix=""):
-        """
-        Ensures compatibility with sklearn < 1.0.
-        Use `get_feature_names_out` instead.
-        """
-        warnings.warn(
-            "Following the changes in scikit-learn 1.0, "
-            "get_feature_names is deprecated. "
-            "Use get_feature_names_out instead. ",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.get_feature_names_out(n_labels=n_labels, prefix=prefix)
-
-    def get_feature_names_out(
-        self,
-        n_labels: int = 3,
-        prefix: str = "",
-    ) -> List[str]:
-        """
-        Returns the labels that best summarize the learned components/topics.
-        For each topic, labels with the highest activations are selected.
-
-        Parameters
-        ----------
-        n_labels : int, default=3
-            The number of labels used to describe each topic.
-        prefix : str, default=""
-            Used as a prefix for the categories.
-
-        Returns
-        -------
-        topic_labels : typing.List[str]
-            The labels that best describe each topic.
-        """
-
-        vectorizer = CountVectorizer()
-        vectorizer.fit(list(self.H_dict_.keys()))
-        if parse_version(sklearn_version) < parse_version("1.0"):
-            vocabulary = np.array(vectorizer.get_feature_names())
-        else:
-            vocabulary = np.array(vectorizer.get_feature_names_out())
-        encoding = self.transform(np.array(vocabulary).reshape(-1))
-        encoding = abs(encoding)
-        encoding = encoding / np.sum(encoding, axis=1, keepdims=True)
-        n_components = encoding.shape[1]
-        topic_labels = []
-        for i in range(n_components):
-            x = encoding[:, i]
-            labels = vocabulary[np.argsort(-x)[:n_labels]]
-            topic_labels.append(labels)
-        topic_labels = [prefix + ", ".join(label) for label in topic_labels]
-        return topic_labels
-
-    def score(self, X) -> float:
-        """
-        Returns the Kullback-Leibler divergence between the n-grams counts
-        matrix V of X, and its non-negative factorization HW.
-
-        Parameters
-        ----------
-        X : array-like (str), shape (n_samples, )
-            The data to encode.
-
-        Returns
-        -------
-        float.
-            The Kullback-Leibler divergence.
-        """
-
-        # Build n-grams/word counts matrix
-        unq_X, lookup = np.unique(X, return_inverse=True)
-        unq_V = self.ngrams_count_.transform(unq_X)
-        if self.add_words:
-            unq_V2 = self.word_count_.transform(unq_X)
-            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
-
-        self._add_unseen_keys_to_H_dict(unq_X)
-        unq_H = self._get_H(unq_X)
-        # Given the learnt topics W, optimize the activations H to fit V = HW
-        for slice in gen_batches(n=unq_H.shape[0], batch_size=self.batch_size):
-            unq_H[slice] = _multiplicative_update_h(
-                unq_V[slice],
-                self.W_,
-                unq_H[slice],
-                epsilon=1e-3,
-                max_iter=self.max_iter_e_step,
-                rescale_W=self.rescale_W,
-                gamma_shape_prior=self.gamma_shape_prior,
-                gamma_scale_prior=self.gamma_scale_prior,
-            )
-        # Compute the KL divergence between V and HW
-        kl_divergence = _beta_divergence(
-            unq_V[lookup], unq_H[lookup], self.W_, "kullback-leibler", square_root=False
-        )
-        return kl_divergence
-
-    def partial_fit(self, X, y=None) -> "GapEncoderColumn":
-        """
-        Partial fit of the GapEncoder on X.
-        To be used in an online learning procedure where batches of data are
-        coming one by one.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, )
-            The string data to fit the model on.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        GapEncoderColumn
-            The fitted GapEncoderColumn instance.
-        """
-
-        # Init H_dict_ with empty dict if it's the first call of partial_fit
-        if not hasattr(self, "H_dict_"):
-            self.H_dict_ = dict()
-        # Same thing for the rho_ parameter
-        if not hasattr(self, "rho_"):
-            self.rho_ = self.rho
-        # Check if first item has str or np.str_ type
-        assert isinstance(X[0], str), "Input data is not string. "
-        # Check if it is not the first batch
-        if hasattr(self, "vocabulary"):  # Update unq_X, unq_V with new batch
-            unq_X, lookup = np.unique(X, return_inverse=True)
-            unq_V = self.ngrams_count_.transform(unq_X)
-            if self.add_words:
-                unq_V2 = self.word_count_.transform(unq_X)
-                unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
-
-            unseen_X = np.setdiff1d(unq_X, np.array([*self.H_dict_]))
-            unseen_V = self.ngrams_count_.transform(unseen_X)
-            if self.add_words:
-                unseen_V2 = self.word_count_.transform(unseen_X)
-                unseen_V = sparse.hstack((unseen_V, unseen_V2), format="csr")
-
-            if unseen_V.shape[0] != 0:
-                unseen_H = _rescale_h(
-                    unseen_V, np.ones((len(unseen_X), self.n_components))
-                )
-                for x, h in zip(unseen_X, unseen_H):
-                    self.H_dict_[x] = h
-                del unseen_H
-            del unseen_X, unseen_V
-        else:  # If it is the first batch, call _init_vars to init unq_X, unq_V
-            unq_X, unq_V, lookup = self._init_vars(X)
-
-        unq_H = self._get_H(unq_X)
-        # Update unq_H, the activations
-        unq_H = _multiplicative_update_h(
-            unq_V,
-            self.W_,
-            unq_H,
-            epsilon=1e-3,
-            max_iter=self.max_iter_e_step,
-            rescale_W=self.rescale_W,
-            gamma_shape_prior=self.gamma_shape_prior,
-            gamma_scale_prior=self.gamma_scale_prior,
-        )
-        # Update the topics self.W_
-        _multiplicative_update_w(
-            unq_V[lookup],
-            self.W_,
-            self.A_,
-            self.B_,
-            unq_H[lookup],
-            self.rescale_W,
-            self.rho_,
-        )
-        # Update self.H_dict_ with the learned encoded vectors (activations)
-        self.H_dict_.update(zip(unq_X, unq_H))
-        return self
-
-    def _add_unseen_keys_to_H_dict(self, X) -> None:
-        """
-        Add activations of unseen string categories from X to H_dict.
-        """
-        unseen_X = np.setdiff1d(X, np.array([*self.H_dict_]))
-        if unseen_X.size > 0:
-            unseen_V = self.ngrams_count_.transform(unseen_X)
-            if self.add_words:
-                unseen_V2 = self.word_count_.transform(unseen_X)
-                unseen_V = sparse.hstack((unseen_V, unseen_V2), format="csr")
-
-            unseen_H = _rescale_h(
-                unseen_V, np.ones((unseen_V.shape[0], self.n_components))
-            )
-            self.H_dict_.update(zip(unseen_X, unseen_H))
-
-    def transform(self, X) -> np.array:
-        """
-        Return the encoded vectors (activations) H of input strings in X.
-        Given the learnt topics W, the activations H are tuned to fit V = HW.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples)
-            The string data to encode.
-
-        Returns
-        -------
-        H : 2-d array, shape (n_samples, n_topics)
-            Transformed input.
-        """
-        check_is_fitted(self, "H_dict_")
-        # Check if first item has str or np.str_ type
-        assert isinstance(X[0], str), "Input data is not string. "
-        unq_X = np.unique(X)
-        # Build the n-grams counts matrix V for the string data to encode
-        unq_V = self.ngrams_count_.transform(unq_X)
-        if self.add_words:  # Add words counts
-            unq_V2 = self.word_count_.transform(unq_X)
-            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
-        # Add unseen strings in X to H_dict
-        self._add_unseen_keys_to_H_dict(unq_X)
-        unq_H = self._get_H(unq_X)
-        # Loop over batches
-        for slc in gen_batches(n=unq_H.shape[0], batch_size=self.batch_size):
-            # Given the learnt topics W, optimize H to fit V = HW
-            unq_H[slc] = _multiplicative_update_h(
-                unq_V[slc],
-                self.W_,
-                unq_H[slc],
-                epsilon=1e-3,
-                max_iter=100,
-                rescale_W=self.rescale_W,
-                gamma_shape_prior=self.gamma_shape_prior,
-                gamma_scale_prior=self.gamma_scale_prior,
-            )
-        # Store and return the encoded vectors of X
-        self.H_dict_.update(zip(unq_X, unq_H))
-        return self._get_H(X)
-
-
-class GapEncoder(BaseEstimator, TransformerMixin):
-    """Constructs latent topics with continuous encoding.
-
-    This encoder can be understood as a continuous encoding on a set of latent
-    categories estimated from the data. The latent categories are built by
-    capturing combinations of substrings that frequently co-occur.
-
-    The :class:`~dirty_cat.GapEncoder` supports online learning on batches of
-    data for scalability through the :func:`~dirty_cat.GapEncoder.partial_fit`
-    method.
-
-    Parameters
-    ----------
-    n_components : int, optional, default=10
-        Number of latent categories used to model string data.
-    batch_size : int, optional, default=128
-        Number of samples per batch.
-    gamma_shape_prior : float, optional, default=1.1
-        Shape parameter for the Gamma prior distribution.
-    gamma_scale_prior : float, optional, default=1.0
-        Scale parameter for the Gamma prior distribution.
-    rho : float, optional, default=0.95
-        Weight parameter for the update of the *W* matrix.
-    rescale_rho : bool, optional, default=False
-        If true, use ``rho ** (batch_size / len(X))`` instead of rho to obtain an
-        update rate per iteration that is independent of the batch size.
-    hashing : bool, optional, default=False
-        If true, :class:`~sklearn.feature_extraction.text.HashingVectorizer`
-        is used instead of :class:`~sklearn.feature_extraction.text.CountVectorizer`.
-        It has the advantage of being very low memory, scalable to large
-        datasets as there is no need to store a vocabulary dictionary in
-        memory.
-    hashing_n_features : int, optional, default=2**12
-        Number of features for the :class:`~sklearn.feature_extraction.text.HashingVectorizer`.
-        Only relevant if `hashing=True`.
-    init : {"k-means++", "random", "k-means"}, optional, default='k-means++'
-        Initialization method of the W matrix.
-        If `init='k-means++'`, we use the init method of :class:`~sklearn.cluster.KMeans`.
-        If `init='random'`, topics are initialized with a Gamma distribution.
-        If `init='k-means'`, topics are initialized with a KMeans on the n-grams
-        counts. This usually makes convergence faster but is a bit slower.
-    tol : float, default=1e-4
-        Tolerance for the convergence of the matrix *W*.
-    min_iter : int, optional, default=2
-        Minimum number of iterations on the input data.
-    max_iter : int, optional, default=5
-        Maximum number of iterations on the input data.
-    ngram_range : int 2-tuple, optional, default=(2, 4)
-        The range of ngram length that will be used to build the
-        bag-of-n-grams representation of the input data.
-    analyzer : {"word", "char", "char_wb"}, optional, default='char'
-        Analyzer parameter for the :class:`~sklearn.feature_extraction.text.HashingVectorizer`
-        / :class:`~sklearn.feature_extraction.text.CountVectorizer`.
-        Describes whether the matrix *V* to factorize should be made of word counts
-        or character n-gram counts.
-        Option ‘char_wb’ creates character n-grams only from text inside word
-        boundaries; n-grams at the edges of words are padded with space.
-    add_words : bool, optional, default=False
-        If true, add the words counts to the bag-of-n-grams representation
-        of the input data.
-    random_state : int, :class:`numpy.random.RandomState` or None, optional, default=None
-        RNG seed for reproducible output across multiple function calls.
-    rescale_W : bool, optional, default=True
-        If true, the weight matrix *W* is rescaled at each iteration
-        to have a l1 norm equal to 1 for each row.
-    max_iter_e_step : int, default=20
-        Maximum number of iterations to adjust the activations h at each step.
-    handle_missing : {"error", "empty_impute"}, optional, default='empty_impute'
-        Whether to raise an error or impute with empty string ``''`` if missing
-        values (NaN) are present during fit (default is to impute).
-        In the inverse transform, the missing category will be denoted as None.
-
-    Attributes
-    ----------
-    rho_: float
-        Effective update rate for the W matrix
-    fitted_models_: list of GapEncoderColumn
-        Column-wise fitted GapEncoders
-    column_names_: list of str
-        Column names of the data the Gap was fitted on
-
-    References
-    ----------
-    For a detailed description of the method, see
-    `Encoding high-cardinality string categorical variables
-    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
-
-    Examples
-    --------
-    >>> enc = GapEncoder(n_components=2)
-
-    Let's encode the following non-normalized data:
-
-    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['Paris, France'],
-             ['london'], ['London, England'], ['London'], ['Pqris']]
-
-    >>> enc.fit(X)
-    GapEncoder(n_components=2)
-
-    The :class:`~dirty_cat.GapEncoder` has found the following two topics:
-
-    >>> enc.get_feature_names()
-    ['england, london, uk', 'france, paris, pqris']
-
-    It got it right, reccuring topics are "London" and "England" on the
-    one side and "Paris" and "France" on the other.
-
-    As this is a continuous encoding, we can look at the level of
-    activation of each topic for each category:
-
-    >>> enc.transform(X)
-    array([[ 0.05202843, 10.54797156],
-          [ 0.05000118,  4.54999882],
-          [12.04734788,  0.05265212],
-          [ 0.05263068, 16.54736932],
-          [ 6.04999624,  0.05000376],
-          [19.546716  ,  0.053284  ],
-          [ 6.04999623,  0.05000376],
-          [ 0.05002016,  4.54997983]])
-
-    The higher the value, the bigger the correspondance with the topic.
-    """
-
-    rho_: float
-    fitted_models_: List[GapEncoderColumn]
-    column_names_: List[str]
-
-    def __init__(
-        self,
-        n_components: int = 10,
-        batch_size: int = 128,
-        gamma_shape_prior: float = 1.1,
-        gamma_scale_prior: float = 1.0,
-        rho: float = 0.95,
-        rescale_rho: bool = False,
-        hashing: bool = False,
-        hashing_n_features: int = 2**12,
-        init: Literal["k-means++", "random", "k-means"] = "k-means++",
-        tol: float = 1e-4,
-        min_iter: int = 2,
-        max_iter: int = 5,
-        ngram_range: Tuple[int, int] = (2, 4),
-        analyzer: Literal["word", "char", "char_wb"] = "char",
-        add_words: bool = False,
-        random_state: Optional[Union[int, RandomState]] = None,
-        rescale_W: bool = True,
-        max_iter_e_step: int = 20,
-        handle_missing: Literal["error", "empty_impute"] = "zero_impute",
-    ):
-        self.ngram_range = ngram_range
-        self.n_components = n_components
-        self.gamma_shape_prior = gamma_shape_prior  # 'a' parameter
-        self.gamma_scale_prior = gamma_scale_prior  # 'b' parameter
-        self.rho = rho
-        self.rescale_rho = rescale_rho
-        self.batch_size = batch_size
-        self.tol = tol
-        self.hashing = hashing
-        self.hashing_n_features = hashing_n_features
-        self.max_iter = max_iter
-        self.min_iter = min_iter
-        self.init = init
-        self.analyzer = analyzer
-        self.add_words = add_words
-        self.random_state = random_state
-        self.rescale_W = rescale_W
-        self.max_iter_e_step = max_iter_e_step
-        self.handle_missing = handle_missing
-
-    def _more_tags(self) -> Dict[str, List[str]]:
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def _create_column_gap_encoder(self) -> GapEncoderColumn:
-        return GapEncoderColumn(
-            ngram_range=self.ngram_range,
-            n_components=self.n_components,
-            analyzer=self.analyzer,
-            gamma_shape_prior=self.gamma_shape_prior,
-            gamma_scale_prior=self.gamma_scale_prior,
-            rho=self.rho,
-            rescale_rho=self.rescale_rho,
-            batch_size=self.batch_size,
-            tol=self.tol,
-            hashing=self.hashing,
-            hashing_n_features=self.hashing_n_features,
-            max_iter=self.max_iter,
-            init=self.init,
-            add_words=self.add_words,
-            random_state=self.random_state,
-            rescale_W=self.rescale_W,
-            max_iter_e_step=self.max_iter_e_step,
-        )
-
-    def _handle_missing(self, X):
-        """
-        Imputes missing values with `` or raises an error
-        Note: modifies the array in-place.
-        """
-        if self.handle_missing not in ["error", "zero_impute"]:
-            raise ValueError(
-                "handle_missing should be either 'error' or "
-                f"'zero_impute', got {self.handle_missing!r}. "
-            )
-
-        missing_mask = _object_dtype_isnan(X)
-
-        if missing_mask.any():
-            if self.handle_missing == "error":
-                raise ValueError("Input data contains missing values. ")
-            elif self.handle_missing == "zero_impute":
-                X[missing_mask] = ""
-
-        return X
-
-    def fit(self, X, y=None) -> "GapEncoder":
-        """
-        Fit the instance on batches of X.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            The string data to fit the model on.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        :class:`~dirty_cat.GapEncoder`
-            Fitted :class:`~dirty_cat.GapEncoder` instance (self).
-        """
-
-        # Check that n_samples >= n_components
-        if len(X) < self.n_components:
-            raise ValueError(
-                f"n_samples={len(X)} should be >= n_components={self.n_components}. "
-            )
-        # Copy parameter rho
-        self.rho_ = self.rho
-        # If X is a dataframe, store its column names
-        if isinstance(X, pd.DataFrame):
-            self.column_names_ = list(X.columns)
-        # Check input data shape
-        X = check_input(X)
-        X = self._handle_missing(X)
-        self.fitted_models_ = []
-        for k in range(X.shape[1]):
-            col_enc = self._create_column_gap_encoder()
-            self.fitted_models_.append(col_enc.fit(X[:, k]))
-        return self
-
-    def transform(self, X) -> np.array:
-        """
-        Return the encoded vectors (activations) H of input strings in X.
-        Given the learnt topics W, the activations H are tuned to fit V = HW.
-        When X has several columns, they are encoded separately and
-        then concatenated.
-
-        Remark: calling transform multiple times in a row on the same
-        input X can give slightly different encodings. This is expected
-        due to a caching mechanism to speed things up.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            The string data to encode.
-
-        Returns
-        -------
-        H : 2-d array, shape (n_samples, n_topics * n_features)
-            Transformed input.
-        """
-        check_is_fitted(self, "fitted_models_")
-        # Check input data shape
-        X = check_input(X)
-        X = self._handle_missing(X)
-        X_enc = []
-        for k in range(X.shape[1]):
-            X_enc.append(self.fitted_models_[k].transform(X[:, k]))
-        X_enc = np.hstack(X_enc)
-        return X_enc
-
-    def partial_fit(self, X, y=None) -> "GapEncoder":
-        """
-        Partial fit of the GapEncoder on X.
-        To be used in an online learning procedure where batches of data are
-        coming one by one.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            The string data to fit the model on.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        GapEncoder
-            Fitted GapEncoder instance.
-        """
-
-        # If X is a dataframe, store its column names
-        if isinstance(X, pd.DataFrame):
-            self.column_names_ = list(X.columns)
-        # Check input data shape
-        X = check_input(X)
-        X = self._handle_missing(X)
-        # Init the `GapEncoderColumn` instances if the model was
-        # not fitted already.
-        if not hasattr(self, "fitted_models_"):
-            self.fitted_models_ = [
-                self._create_column_gap_encoder() for _ in range(X.shape[1])
-            ]
-        for k in range(X.shape[1]):
-            self.fitted_models_[k].partial_fit(X[:, k])
-        return self
-
-    def get_feature_names_out(
-        self,
-        col_names: Optional[Union[Literal["auto"], List[str]]] = None,
-        n_labels: int = 3,
-    ):
-        """
-        Returns the labels that best summarize the learned components/topics.
-        For each topic, labels with the highest activations are selected.
-
-        Parameters
-        ----------
-        col_names : typing.Optional[typing.Union[typing.Literal["auto"], typing.List[str]]], default=None  # noqa
-            The column names to be added as prefixes before the labels.
-            If col_names == None, no prefixes are used.
-            If col_names == 'auto', column names are automatically defined:
-
-                - if the input data was a dataframe, its column names are used,
-                - otherwise, 'col1', ..., 'colN' are used as prefixes.
-
-            Prefixes can be manually set by passing a list for col_names.
-        n_labels : int, default=3
-            The number of labels used to describe each topic.
-
-        Returns
-        -------
-        topic_labels : list of strings
-            The labels that best describe each topic.
-        """
-        assert hasattr(
-            self, "fitted_models_"
-        ), "ERROR: GapEncoder must be fitted first."
-        # Generate prefixes
-        if isinstance(col_names, str) and col_names == "auto":
-            if hasattr(self, "column_names_"):  # Use column names
-                prefixes = ["%s: " % col for col in self.column_names_]
-            else:  # Use 'col1: ', ... 'colN: ' as prefixes
-                prefixes = ["col%d: " % i for i in range(len(self.fitted_models_))]
-        elif col_names is None:  # Empty prefixes
-            prefixes = [""] * len(self.fitted_models_)
-        else:
-            prefixes = ["%s: " % col for col in col_names]
-        labels = list()
-        for k, enc in enumerate(self.fitted_models_):
-            col_labels = enc.get_feature_names_out(n_labels, prefixes[k])
-            labels.extend(col_labels)
-        return labels
-
-    def get_feature_names(
-        self, input_features=None, col_names: List[str] = None, n_labels: int = 3
-    ) -> List[str]:
-        """
-        Ensures compatibility with sklearn < 1.0.
-        Use `get_feature_names_out` instead.
-        """
-        if parse_version(sklearn_version) >= parse_version("1.0"):
-            warnings.warn(
-                "Following the changes in scikit-learn 1.0, "
-                "get_feature_names is deprecated. "
-                "Use get_feature_names_out instead. ",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        return self.get_feature_names_out(col_names, n_labels)
-
-    def score(self, X) -> float:
-        """
-        Returns the sum over the columns of X of the Kullback-Leibler
-        divergence between the n-grams counts matrix V of X, and its
-        non-negative factorization HW.
-
-        Parameters
-        ----------
-        X : array-like (str), shape (n_samples, n_features)
-            The data to encode.
-
-        Returns
-        -------
-        float.
-            The Kullback-Leibler divergence.
-        """
-        X = check_input(X)
-        kl_divergence = 0
-        for k in range(X.shape[1]):
-            kl_divergence += self.fitted_models_[k].score(X[:, k])
-        return kl_divergence
-
-
-def _rescale_W(W: np.array, A: np.array) -> None:
-    """
-    Rescale the topics W to have a L1-norm equal to 1.
-    Note that they are modified in-place.
-    """
-    s = W.sum(axis=1, keepdims=True)
-    W /= s
-    A /= s
-
-
-def _multiplicative_update_w(
-    Vt: np.array,
-    W: np.array,
-    A: np.array,
-    B: np.array,
-    Ht: np.array,
-    rescale_W: bool,
-    rho: float,
-) -> Tuple[np.array, np.array, np.array]:
-    """
-    Multiplicative update step for the topics W.
-    """
-    A *= rho
-    A += W * safe_sparse_dot(Ht.T, Vt.multiply(1 / (np.dot(Ht, W) + 1e-10)))
-    B *= rho
-    B += Ht.sum(axis=0).reshape(-1, 1)
-    np.divide(A, B, out=W)
-    if rescale_W:
-        _rescale_W(W, A)
-    return W, A, B
-
-
-def _rescale_h(V: np.array, H: np.array) -> np.array:
-    """
-    Rescale the activations H.
-    """
-    epsilon = 1e-10  # in case of a document having length=0
-    H *= np.maximum(epsilon, V.sum(axis=1).A)
-    H /= H.sum(axis=1, keepdims=True)
-    return H
-
-
-def _multiplicative_update_h(
-    Vt: np.array,
-    W: np.array,
-    Ht: np.array,
-    epsilon: float = 1e-3,
-    max_iter: int = 10,
-    rescale_W: bool = False,
-    gamma_shape_prior: float = 1.1,
-    gamma_scale_prior: float = 1.0,
-):
-    """
-    Multiplicative update step for the activations H.
-    """
-    if rescale_W:
-        WT1 = 1 + 1 / gamma_scale_prior
-        W_WT1 = W / WT1
-    else:
-        WT1 = np.sum(W, axis=1) + 1 / gamma_scale_prior
-        W_WT1 = W / WT1.reshape(-1, 1)
-    const = (gamma_shape_prior - 1) / WT1
-    squared_epsilon = epsilon**2
-    for vt, ht in zip(Vt, Ht):
-        vt_ = vt.data
-        idx = vt.indices
-        W_WT1_ = W_WT1[:, idx]
-        W_ = W[:, idx]
-        squared_norm = 1
-        for n_iter_ in range(max_iter):
-            if squared_norm <= squared_epsilon:
-                break
-            aux = np.dot(W_WT1_, vt_ / (np.dot(ht, W_) + 1e-10))
-            ht_out = ht * aux + const
-            squared_norm = np.dot(ht_out - ht, ht_out - ht) / np.dot(ht, ht)
-            ht[:] = ht_out
-    return Ht
-
-
-def batch_lookup(
-    lookup: np.array,
-    n: int = 1,
-) -> Generator[Tuple[np.array, np.array], None, None]:
-    """
-    Make batches of the lookup array.
-    """
-    len_iter = len(lookup)
-    for idx in range(0, len_iter, n):
-        indices = lookup[slice(idx, min(idx + n, len_iter))]
-        unq_indices = np.unique(indices)
-        yield unq_indices, indices
-
-
-def get_kmeans_prototypes(
-    X,
-    n_prototypes: int,
-    analyzer: Literal["word", "char", "char_wb"] = "char",
-    hashing_dim: int = 128,
-    ngram_range: Tuple[int, int] = (2, 4),
-    sparse: bool = False,
-    sample_weight=None,
-    random_state: Optional[Union[int, RandomState]] = None,
-):
-    """
-    Computes prototypes based on:
-      - dimensionality reduction (via hashing n-grams)
-      - k-means clustering
-      - nearest neighbor
-    """
-    vectorizer = HashingVectorizer(
-        analyzer=analyzer,
-        norm=None,
-        alternate_sign=False,
-        ngram_range=ngram_range,
-        n_features=hashing_dim,
-    )
-    projected = vectorizer.transform(X)
-    if not sparse:
-        projected = projected.toarray()
-    kmeans = KMeans(n_clusters=n_prototypes, random_state=random_state)
-    kmeans.fit(projected, sample_weight=sample_weight)
-    centers = kmeans.cluster_centers_
-    neighbors = NearestNeighbors()
-    neighbors.fit(projected)
-    indexes_prototypes = np.unique(neighbors.kneighbors(centers, 1)[-1])
-    return np.sort(X[indexes_prototypes])
+"""
+Online Gamma-Poisson factorization of string arrays.
+The principle is as follows:
+    1. Given an input string array X, we build its bag-of-n-grams
+       representation V (n_samples, vocab_size).
+    2. Instead of using the n-grams counts as encodings, we look for low-
+       dimensional representations by modeling n-grams counts as linear
+       combinations of topics V = HW, with W (n_topics, vocab_size) the topics
+       and H (n_samples, n_topics) the associated activations.
+    3. Assuming that n-grams counts follow a Poisson law, we fit H and W to
+       maximize the likelihood of the data, with a Gamma prior for the
+       activations H to induce sparsity.
+    4. In practice, this is equivalent to a non-negative matrix factorization
+       with the Kullback-Leibler divergence as loss, and a Gamma prior on H.
+       We thus optimize H and W with the multiplicative update method.
+"""
+
+import warnings
+from copy import deepcopy
+from typing import Dict, Generator, List, Literal, Optional, Tuple, Union
+
+import numpy as np
+import pandas as pd
+from numpy.random import RandomState
+from scipy import sparse
+from sklearn import __version__ as sklearn_version
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.cluster import KMeans
+from sklearn.feature_extraction.text import CountVectorizer, HashingVectorizer
+from sklearn.neighbors import NearestNeighbors
+from sklearn.utils import check_random_state, gen_batches
+from sklearn.utils.extmath import row_norms, safe_sparse_dot
+from sklearn.utils.fixes import _object_dtype_isnan
+from sklearn.utils.validation import check_is_fitted
+
+from ._utils import check_input, parse_version
+
+if parse_version(sklearn_version) < parse_version("0.24"):
+    from sklearn.cluster._kmeans import _k_init
+else:
+    from sklearn.cluster import kmeans_plusplus
+
+from sklearn.decomposition._nmf import _beta_divergence
+
+# Ignore lines too long, as some things in the docstring cannot be cut.
+# flake8: noqa: E501
+
+
+class GapEncoderColumn(BaseEstimator, TransformerMixin):
+
+    """See GapEncoder's docstring."""
+
+    rho_: float
+    H_dict_: Dict[np.ndarray, np.ndarray]
+
+    def __init__(
+        self,
+        n_components: int = 10,
+        batch_size: int = 128,
+        gamma_shape_prior: float = 1.1,
+        gamma_scale_prior: float = 1.0,
+        rho: float = 0.95,
+        rescale_rho: bool = False,
+        hashing: bool = False,
+        hashing_n_features: int = 2**12,
+        init: Literal["k-means++", "random", "k-means"] = "k-means++",
+        tol: float = 1e-4,
+        min_iter: int = 2,
+        max_iter: int = 5,
+        ngram_range: Tuple[int, int] = (2, 4),
+        analyzer: Literal["word", "char", "char_wb"] = "char",
+        add_words: bool = False,
+        random_state: Optional[Union[int, RandomState]] = None,
+        rescale_W: bool = True,
+        max_iter_e_step: int = 20,
+    ):
+        self.ngram_range = ngram_range
+        self.n_components = n_components
+        self.gamma_shape_prior = gamma_shape_prior  # 'a' parameter
+        self.gamma_scale_prior = gamma_scale_prior  # 'b' parameter
+        self.rho = rho
+        self.rescale_rho = rescale_rho
+        self.batch_size = batch_size
+        self.tol = tol
+        self.hashing = hashing
+        self.hashing_n_features = hashing_n_features
+        self.max_iter = max_iter
+        self.min_iter = min_iter
+        self.init = init
+        self.analyzer = analyzer
+        self.add_words = add_words
+        self.random_state = check_random_state(random_state)
+        self.rescale_W = rescale_W
+        self.max_iter_e_step = max_iter_e_step
+
+    def _init_vars(self, X) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Build the bag-of-n-grams representation V of X and initialize
+        the topics W.
+        """
+        # Init n-grams counts vectorizer
+        if self.hashing:
+            self.ngrams_count_ = HashingVectorizer(
+                analyzer=self.analyzer,
+                ngram_range=self.ngram_range,
+                n_features=self.hashing_n_features,
+                norm=None,
+                alternate_sign=False,
+            )
+            if self.add_words:  # Init a word counts vectorizer if needed
+                self.word_count_ = HashingVectorizer(
+                    analyzer="word",
+                    n_features=self.hashing_n_features,
+                    norm=None,
+                    alternate_sign=False,
+                )
+        else:
+            self.ngrams_count_ = CountVectorizer(
+                analyzer=self.analyzer, ngram_range=self.ngram_range, dtype=np.float64
+            )
+            if self.add_words:
+                self.word_count_ = CountVectorizer(dtype=np.float64)
+
+        # Init H_dict_ with empty dict to train from scratch
+        self.H_dict_ = dict()
+        # Build the n-grams counts matrix unq_V on unique elements of X
+        unq_X, lookup = np.unique(X, return_inverse=True)
+        unq_V = self.ngrams_count_.fit_transform(unq_X)
+        if self.add_words:  # Add word counts to unq_V
+            unq_V2 = self.word_count_.fit_transform(unq_X)
+            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
+
+        if not self.hashing:  # Build n-grams/word vocabulary
+            if parse_version(sklearn_version) < parse_version("1.0"):
+                self.vocabulary = self.ngrams_count_.get_feature_names()
+            else:
+                self.vocabulary = self.ngrams_count_.get_feature_names_out()
+            if self.add_words:
+                if parse_version(sklearn_version) < parse_version("1.0"):
+                    self.vocabulary = np.concatenate(
+                        (self.vocabulary, self.word_count_.get_feature_names())
+                    )
+                else:
+                    self.vocabulary = np.concatenate(
+                        (self.vocabulary, self.word_count_.get_feature_names_out())
+                    )
+        _, self.n_vocab = unq_V.shape
+        # Init the topics W given the n-grams counts V
+        self.W_, self.A_, self.B_ = self._init_w(unq_V[lookup], X)
+        # Init the activations unq_H of each unique input string
+        unq_H = _rescale_h(unq_V, np.ones((len(unq_X), self.n_components)))
+        # Update self.H_dict_ with unique input strings and their activations
+        self.H_dict_.update(zip(unq_X, unq_H))
+        if self.rescale_rho:
+            # Make update rate per iteration independent of the batch_size
+            self.rho_ = self.rho ** (self.batch_size / len(X))
+        return unq_X, unq_V, lookup
+
+    def _get_H(self, X: np.array) -> np.array:
+        """
+        Return the bag-of-n-grams representation of X.
+        """
+        H_out = np.empty((len(X), self.n_components))
+        for x, h_out in zip(X, H_out):
+            h_out[:] = self.H_dict_[x]
+        return H_out
+
+    def _init_w(self, V: np.array, X) -> Tuple[np.array, np.array, np.array]:
+        """
+        Initialize the topics W.
+        If self.init='k-means++', we use the init method of
+        sklearn.cluster.KMeans.
+        If self.init='random', topics are initialized with a Gamma
+        distribution.
+        If self.init='k-means', topics are initialized with a KMeans on the
+        n-grams counts.
+        """
+        if self.init == "k-means++":
+            if parse_version(sklearn_version) < parse_version("0.24"):
+                W = (
+                    _k_init(
+                        V,
+                        self.n_components,
+                        x_squared_norms=row_norms(V, squared=True),
+                        random_state=self.random_state,
+                        n_local_trials=None,
+                    )
+                    + 0.1
+                )
+            else:
+                W, _ = kmeans_plusplus(
+                    V,
+                    self.n_components,
+                    x_squared_norms=row_norms(V, squared=True),
+                    random_state=self.random_state,
+                    n_local_trials=None,
+                )
+                W = W + 0.1  # To avoid restricting topics to a few n-grams only
+        elif self.init == "random":
+            W = self.random_state.gamma(
+                shape=self.gamma_shape_prior,
+                scale=self.gamma_scale_prior,
+                size=(self.n_components, self.n_vocab),
+            )
+        elif self.init == "k-means":
+            prototypes = get_kmeans_prototypes(
+                X,
+                self.n_components,
+                analyzer=self.analyzer,
+                random_state=self.random_state,
+            )
+            W = self.ngrams_count_.transform(prototypes).A + 0.1
+            if self.add_words:
+                W2 = self.word_count_.transform(prototypes).A + 0.1
+                W = np.hstack((W, W2))
+            # if k-means doesn't find the exact number of prototypes
+            if W.shape[0] < self.n_components:
+                if parse_version(sklearn_version) < parse_version("0.24"):
+                    W2 = (
+                        _k_init(
+                            V,
+                            self.n_components - W.shape[0],
+                            x_squared_norms=row_norms(V, squared=True),
+                            random_state=self.random_state,
+                            n_local_trials=None,
+                        )
+                        + 0.1
+                    )
+                else:
+                    W2, _ = kmeans_plusplus(
+                        V,
+                        self.n_components - W.shape[0],
+                        x_squared_norms=row_norms(V, squared=True),
+                        random_state=self.random_state,
+                        n_local_trials=None,
+                    )
+                    W2 = W2 + 0.1
+                W = np.concatenate((W, W2), axis=0)
+        else:
+            raise ValueError(f"Initialization method {self.init!r} does not exist. ")
+        W /= W.sum(axis=1, keepdims=True)
+        A = np.ones((self.n_components, self.n_vocab)) * 1e-10
+        B = A.copy()
+        return W, A, B
+
+    def fit(self, X, y=None) -> "GapEncoderColumn":
+        """
+        Fit the GapEncoder on batches of X.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, )
+            The string data to fit the model on.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        self
+            Fitting GapEncoderColumn instance.
+        """
+        # Copy parameter rho
+        self.rho_ = self.rho
+        # Check if first item has str or np.str_ type
+        assert isinstance(X[0], str), "Input data is not string. "
+        # Make n-grams counts matrix unq_V
+        unq_X, unq_V, lookup = self._init_vars(X)
+        n_batch = (len(X) - 1) // self.batch_size + 1
+        del X
+        # Get activations unq_H
+        unq_H = self._get_H(unq_X)
+
+        for n_iter_ in range(self.max_iter):
+            # Loop over batches
+            for i, (unq_idx, idx) in enumerate(batch_lookup(lookup, n=self.batch_size)):
+                if i == n_batch - 1:
+                    W_last = self.W_.copy()
+                # Update activations unq_H
+                unq_H[unq_idx] = _multiplicative_update_h(
+                    unq_V[unq_idx],
+                    self.W_,
+                    unq_H[unq_idx],
+                    epsilon=1e-3,
+                    max_iter=self.max_iter_e_step,
+                    rescale_W=self.rescale_W,
+                    gamma_shape_prior=self.gamma_shape_prior,
+                    gamma_scale_prior=self.gamma_scale_prior,
+                )
+                # Update the topics self.W_
+                _multiplicative_update_w(
+                    unq_V[idx],
+                    self.W_,
+                    self.A_,
+                    self.B_,
+                    unq_H[idx],
+                    self.rescale_W,
+                    self.rho_,
+                )
+
+                if i == n_batch - 1:
+                    # Compute the norm of the update of W in the last batch
+                    W_change = np.linalg.norm(self.W_ - W_last) / np.linalg.norm(W_last)
+
+            if (W_change < self.tol) and (n_iter_ >= self.min_iter - 1):
+                break  # Stop if the change in W is smaller than the tolerance
+
+        # Update self.H_dict_ with the learned encoded vectors (activations)
+        self.H_dict_.update(zip(unq_X, unq_H))
+        return self
+
+    def get_feature_names(self, n_labels=3, prefix=""):
+        """
+        Ensures compatibility with sklearn < 1.0.
+        Use `get_feature_names_out` instead.
+        """
+        warnings.warn(
+            "Following the changes in scikit-learn 1.0, "
+            "get_feature_names is deprecated. "
+            "Use get_feature_names_out instead. ",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.get_feature_names_out(n_labels=n_labels, prefix=prefix)
+
+    def get_feature_names_out(
+        self,
+        n_labels: int = 3,
+        prefix: str = "",
+    ) -> List[str]:
+        """
+        Returns the labels that best summarize the learned components/topics.
+        For each topic, labels with the highest activations are selected.
+
+        Parameters
+        ----------
+        n_labels : int, default=3
+            The number of labels used to describe each topic.
+        prefix : str, default=""
+            Used as a prefix for the categories.
+
+        Returns
+        -------
+        topic_labels : typing.List[str]
+            The labels that best describe each topic.
+        """
+
+        vectorizer = CountVectorizer()
+        vectorizer.fit(list(self.H_dict_.keys()))
+        if parse_version(sklearn_version) < parse_version("1.0"):
+            vocabulary = np.array(vectorizer.get_feature_names())
+        else:
+            vocabulary = np.array(vectorizer.get_feature_names_out())
+        encoding = self.transform(np.array(vocabulary).reshape(-1))
+        encoding = abs(encoding)
+        encoding = encoding / np.sum(encoding, axis=1, keepdims=True)
+        n_components = encoding.shape[1]
+        topic_labels = []
+        for i in range(n_components):
+            x = encoding[:, i]
+            labels = vocabulary[np.argsort(-x)[:n_labels]]
+            topic_labels.append(labels)
+        topic_labels = [prefix + ", ".join(label) for label in topic_labels]
+        return topic_labels
+
+    def score(self, X) -> float:
+        """
+        Returns the Kullback-Leibler divergence between the n-grams counts
+        matrix V of X, and its non-negative factorization HW.
+
+        Parameters
+        ----------
+        X : array-like (str), shape (n_samples, )
+            The data to encode.
+
+        Returns
+        -------
+        float.
+            The Kullback-Leibler divergence.
+        """
+
+        # Build n-grams/word counts matrix
+        unq_X, lookup = np.unique(X, return_inverse=True)
+        unq_V = self.ngrams_count_.transform(unq_X)
+        if self.add_words:
+            unq_V2 = self.word_count_.transform(unq_X)
+            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
+
+        self._add_unseen_keys_to_H_dict(unq_X)
+        unq_H = self._get_H(unq_X)
+        # Given the learnt topics W, optimize the activations H to fit V = HW
+        for slice in gen_batches(n=unq_H.shape[0], batch_size=self.batch_size):
+            unq_H[slice] = _multiplicative_update_h(
+                unq_V[slice],
+                self.W_,
+                unq_H[slice],
+                epsilon=1e-3,
+                max_iter=self.max_iter_e_step,
+                rescale_W=self.rescale_W,
+                gamma_shape_prior=self.gamma_shape_prior,
+                gamma_scale_prior=self.gamma_scale_prior,
+            )
+        # Compute the KL divergence between V and HW
+        kl_divergence = _beta_divergence(
+            unq_V[lookup], unq_H[lookup], self.W_, "kullback-leibler", square_root=False
+        )
+        return kl_divergence
+
+    def partial_fit(self, X, y=None) -> "GapEncoderColumn":
+        """
+        Partial fit of the GapEncoder on X.
+        To be used in an online learning procedure where batches of data are
+        coming one by one.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, )
+            The string data to fit the model on.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        GapEncoderColumn
+            The fitted GapEncoderColumn instance.
+        """
+
+        # Init H_dict_ with empty dict if it's the first call of partial_fit
+        if not hasattr(self, "H_dict_"):
+            self.H_dict_ = dict()
+        # Same thing for the rho_ parameter
+        if not hasattr(self, "rho_"):
+            self.rho_ = self.rho
+        # Check if first item has str or np.str_ type
+        assert isinstance(X[0], str), "Input data is not string. "
+        # Check if it is not the first batch
+        if hasattr(self, "vocabulary"):  # Update unq_X, unq_V with new batch
+            unq_X, lookup = np.unique(X, return_inverse=True)
+            unq_V = self.ngrams_count_.transform(unq_X)
+            if self.add_words:
+                unq_V2 = self.word_count_.transform(unq_X)
+                unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
+
+            unseen_X = np.setdiff1d(unq_X, np.array([*self.H_dict_]))
+            unseen_V = self.ngrams_count_.transform(unseen_X)
+            if self.add_words:
+                unseen_V2 = self.word_count_.transform(unseen_X)
+                unseen_V = sparse.hstack((unseen_V, unseen_V2), format="csr")
+
+            if unseen_V.shape[0] != 0:
+                unseen_H = _rescale_h(
+                    unseen_V, np.ones((len(unseen_X), self.n_components))
+                )
+                for x, h in zip(unseen_X, unseen_H):
+                    self.H_dict_[x] = h
+                del unseen_H
+            del unseen_X, unseen_V
+        else:  # If it is the first batch, call _init_vars to init unq_X, unq_V
+            unq_X, unq_V, lookup = self._init_vars(X)
+
+        unq_H = self._get_H(unq_X)
+        # Update unq_H, the activations
+        unq_H = _multiplicative_update_h(
+            unq_V,
+            self.W_,
+            unq_H,
+            epsilon=1e-3,
+            max_iter=self.max_iter_e_step,
+            rescale_W=self.rescale_W,
+            gamma_shape_prior=self.gamma_shape_prior,
+            gamma_scale_prior=self.gamma_scale_prior,
+        )
+        # Update the topics self.W_
+        _multiplicative_update_w(
+            unq_V[lookup],
+            self.W_,
+            self.A_,
+            self.B_,
+            unq_H[lookup],
+            self.rescale_W,
+            self.rho_,
+        )
+        # Update self.H_dict_ with the learned encoded vectors (activations)
+        self.H_dict_.update(zip(unq_X, unq_H))
+        return self
+
+    def _add_unseen_keys_to_H_dict(self, X) -> None:
+        """
+        Add activations of unseen string categories from X to H_dict.
+        """
+        unseen_X = np.setdiff1d(X, np.array([*self.H_dict_]))
+        if unseen_X.size > 0:
+            unseen_V = self.ngrams_count_.transform(unseen_X)
+            if self.add_words:
+                unseen_V2 = self.word_count_.transform(unseen_X)
+                unseen_V = sparse.hstack((unseen_V, unseen_V2), format="csr")
+
+            unseen_H = _rescale_h(
+                unseen_V, np.ones((unseen_V.shape[0], self.n_components))
+            )
+            self.H_dict_.update(zip(unseen_X, unseen_H))
+
+    def transform(self, X) -> np.array:
+        """
+        Return the encoded vectors (activations) H of input strings in X.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples)
+            The string data to encode.
+
+        Returns
+        -------
+        2-d array, shape (n_samples, n_topics)
+            Transformed input.
+        """
+        check_is_fitted(self, "H_dict_")
+        # Copy the state of H before continuing fitting it
+        pre_trans_H_dict_ = deepcopy(self.H_dict_)
+        # Check if the first item has str or np.str_ type
+        assert isinstance(X[0], str), "Input data is not string. "
+        unq_X = np.unique(X)
+        # Build the n-grams counts matrix V for the string data to encode
+        unq_V = self.ngrams_count_.transform(unq_X)
+        if self.add_words:  # Add words counts
+            unq_V2 = self.word_count_.transform(unq_X)
+            unq_V = sparse.hstack((unq_V, unq_V2), format="csr")
+        # Add unseen strings in X to H_dict
+        self._add_unseen_keys_to_H_dict(unq_X)
+        unq_H = self._get_H(unq_X)
+        # Loop over batches
+        for slc in gen_batches(n=unq_H.shape[0], batch_size=self.batch_size):
+            # Given the learnt topics W, optimize H to fit V = HW
+            unq_H[slc] = _multiplicative_update_h(
+                unq_V[slc],
+                self.W_,
+                unq_H[slc],
+                epsilon=1e-3,
+                max_iter=100,
+                rescale_W=self.rescale_W,
+                gamma_shape_prior=self.gamma_shape_prior,
+                gamma_scale_prior=self.gamma_scale_prior,
+            )
+        # Store and return the encoded vectors of X
+        self.H_dict_.update(zip(unq_X, unq_H))
+        feature_names_out = self._get_H(X)
+        # Restore H
+        self.H_dict_ = pre_trans_H_dict_
+        return feature_names_out
+
+
+class GapEncoder(BaseEstimator, TransformerMixin):
+    """Constructs latent topics with continuous encoding.
+
+    This encoder can be understood as a continuous encoding on a set of latent
+    categories estimated from the data. The latent categories are built by
+    capturing combinations of substrings that frequently co-occur.
+
+    The :class:`~dirty_cat.GapEncoder` supports online learning on batches of
+    data for scalability through the :func:`~dirty_cat.GapEncoder.partial_fit`
+    method.
+
+    Parameters
+    ----------
+    n_components : int, optional, default=10
+        Number of latent categories used to model string data.
+    batch_size : int, optional, default=128
+        Number of samples per batch.
+    gamma_shape_prior : float, optional, default=1.1
+        Shape parameter for the Gamma prior distribution.
+    gamma_scale_prior : float, optional, default=1.0
+        Scale parameter for the Gamma prior distribution.
+    rho : float, optional, default=0.95
+        Weight parameter for the update of the *W* matrix.
+    rescale_rho : bool, optional, default=False
+        If true, use ``rho ** (batch_size / len(X))`` instead of rho to obtain an
+        update rate per iteration that is independent of the batch size.
+    hashing : bool, optional, default=False
+        If true, :class:`~sklearn.feature_extraction.text.HashingVectorizer`
+        is used instead of :class:`~sklearn.feature_extraction.text.CountVectorizer`.
+        It has the advantage of being very low memory, scalable to large
+        datasets as there is no need to store a vocabulary dictionary in
+        memory.
+    hashing_n_features : int, optional, default=2**12
+        Number of features for the :class:`~sklearn.feature_extraction.text.HashingVectorizer`.
+        Only relevant if `hashing=True`.
+    init : {"k-means++", "random", "k-means"}, optional, default='k-means++'
+        Initialization method of the W matrix.
+        If `init='k-means++'`, we use the init method of :class:`~sklearn.cluster.KMeans`.
+        If `init='random'`, topics are initialized with a Gamma distribution.
+        If `init='k-means'`, topics are initialized with a KMeans on the n-grams
+        counts. This usually makes convergence faster but is a bit slower.
+    tol : float, default=1e-4
+        Tolerance for the convergence of the matrix *W*.
+    min_iter : int, optional, default=2
+        Minimum number of iterations on the input data.
+    max_iter : int, optional, default=5
+        Maximum number of iterations on the input data.
+    ngram_range : int 2-tuple, optional, default=(2, 4)
+        The range of ngram length that will be used to build the
+        bag-of-n-grams representation of the input data.
+    analyzer : {"word", "char", "char_wb"}, optional, default='char'
+        Analyzer parameter for the :class:`~sklearn.feature_extraction.text.HashingVectorizer`
+        / :class:`~sklearn.feature_extraction.text.CountVectorizer`.
+        Describes whether the matrix *V* to factorize should be made of word counts
+        or character n-gram counts.
+        Option ‘char_wb’ creates character n-grams only from text inside word
+        boundaries; n-grams at the edges of words are padded with space.
+    add_words : bool, optional, default=False
+        If true, add the words counts to the bag-of-n-grams representation
+        of the input data.
+    random_state : int, :class:`numpy.random.RandomState` or None, optional, default=None
+        RNG seed for reproducible output across multiple function calls.
+    rescale_W : bool, optional, default=True
+        If true, the weight matrix *W* is rescaled at each iteration
+        to have a l1 norm equal to 1 for each row.
+    max_iter_e_step : int, default=20
+        Maximum number of iterations to adjust the activations h at each step.
+    handle_missing : {"error", "empty_impute"}, optional, default='empty_impute'
+        Whether to raise an error or impute with empty string ``''`` if missing
+        values (NaN) are present during fit (default is to impute).
+        In the inverse transform, the missing category will be denoted as None.
+
+    Attributes
+    ----------
+    rho_: float
+        Effective update rate for the W matrix
+    fitted_models_: list of GapEncoderColumn
+        Column-wise fitted GapEncoders
+    column_names_: list of str
+        Column names of the data the Gap was fitted on
+
+    See Also
+    --------
+    :class:`~dirty_cat.MinHashEncoder` :
+        Encode string columns as a numeric array with the minhash method.
+    :class:`~dirty_cat.SimilarityEncoder` :
+        Encode string columns as a numeric array with n-gram string similarity.
+    :class:`~dirty_cat.deduplicate` :
+        Deduplicate data by hierarchically clustering similar strings.
+
+    References
+    ----------
+    For a detailed description of the method, see
+    `Encoding high-cardinality string categorical variables
+    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
+
+    Examples
+    --------
+    >>> enc = GapEncoder(n_components=2)
+
+    Let's encode the following non-normalized data:
+
+    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['Paris, France'],
+             ['london'], ['London, England'], ['London'], ['Pqris']]
+
+    >>> enc.fit(X)
+    GapEncoder(n_components=2)
+
+    The :class:`~dirty_cat.GapEncoder` has found the following two topics:
+
+    >>> enc.get_feature_names_out()
+    ['england, london, uk', 'france, paris, pqris']
+
+    It got it right, reccuring topics are "London" and "England" on the
+    one side and "Paris" and "France" on the other.
+
+    As this is a continuous encoding, we can look at the level of
+    activation of each topic for each category:
+
+    >>> enc.transform(X)
+    array([[ 0.05202843, 10.54797156],
+          [ 0.05000118,  4.54999882],
+          [12.04734788,  0.05265212],
+          [ 0.05263068, 16.54736932],
+          [ 6.04999624,  0.05000376],
+          [19.546716  ,  0.053284  ],
+          [ 6.04999623,  0.05000376],
+          [ 0.05002016,  4.54997983]])
+
+    The higher the value, the bigger the correspondance with the topic.
+    """
+
+    rho_: float
+    fitted_models_: List[GapEncoderColumn]
+    column_names_: List[str]
+
+    def __init__(
+        self,
+        n_components: int = 10,
+        batch_size: int = 128,
+        gamma_shape_prior: float = 1.1,
+        gamma_scale_prior: float = 1.0,
+        rho: float = 0.95,
+        rescale_rho: bool = False,
+        hashing: bool = False,
+        hashing_n_features: int = 2**12,
+        init: Literal["k-means++", "random", "k-means"] = "k-means++",
+        tol: float = 1e-4,
+        min_iter: int = 2,
+        max_iter: int = 5,
+        ngram_range: Tuple[int, int] = (2, 4),
+        analyzer: Literal["word", "char", "char_wb"] = "char",
+        add_words: bool = False,
+        random_state: Optional[Union[int, RandomState]] = None,
+        rescale_W: bool = True,
+        max_iter_e_step: int = 20,
+        handle_missing: Literal["error", "empty_impute"] = "zero_impute",
+    ):
+        self.ngram_range = ngram_range
+        self.n_components = n_components
+        self.gamma_shape_prior = gamma_shape_prior  # 'a' parameter
+        self.gamma_scale_prior = gamma_scale_prior  # 'b' parameter
+        self.rho = rho
+        self.rescale_rho = rescale_rho
+        self.batch_size = batch_size
+        self.tol = tol
+        self.hashing = hashing
+        self.hashing_n_features = hashing_n_features
+        self.max_iter = max_iter
+        self.min_iter = min_iter
+        self.init = init
+        self.analyzer = analyzer
+        self.add_words = add_words
+        self.random_state = random_state
+        self.rescale_W = rescale_W
+        self.max_iter_e_step = max_iter_e_step
+        self.handle_missing = handle_missing
+
+    def _more_tags(self) -> Dict[str, List[str]]:
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {"X_types": ["categorical"]}
+
+    def _create_column_gap_encoder(self) -> GapEncoderColumn:
+        return GapEncoderColumn(
+            ngram_range=self.ngram_range,
+            n_components=self.n_components,
+            analyzer=self.analyzer,
+            gamma_shape_prior=self.gamma_shape_prior,
+            gamma_scale_prior=self.gamma_scale_prior,
+            rho=self.rho,
+            rescale_rho=self.rescale_rho,
+            batch_size=self.batch_size,
+            tol=self.tol,
+            hashing=self.hashing,
+            hashing_n_features=self.hashing_n_features,
+            max_iter=self.max_iter,
+            init=self.init,
+            add_words=self.add_words,
+            random_state=self.random_state,
+            rescale_W=self.rescale_W,
+            max_iter_e_step=self.max_iter_e_step,
+        )
+
+    def _handle_missing(self, X):
+        """
+        Imputes missing values with `` or raises an error
+        Note: modifies the array in-place.
+        """
+        if self.handle_missing not in ["error", "zero_impute"]:
+            raise ValueError(
+                "handle_missing should be either 'error' or "
+                f"'zero_impute', got {self.handle_missing!r}. "
+            )
+
+        missing_mask = _object_dtype_isnan(X)
+
+        if missing_mask.any():
+            if self.handle_missing == "error":
+                raise ValueError("Input data contains missing values. ")
+            elif self.handle_missing == "zero_impute":
+                X[missing_mask] = ""
+
+        return X
+
+    def fit(self, X, y=None) -> "GapEncoder":
+        """
+        Fit the instance on batches of X.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            The string data to fit the model on.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        :class:`~dirty_cat.GapEncoder`
+            Fitted :class:`~dirty_cat.GapEncoder` instance (self).
+        """
+
+        # Check that n_samples >= n_components
+        if len(X) < self.n_components:
+            raise ValueError(
+                f"n_samples={len(X)} should be >= n_components={self.n_components}. "
+            )
+        # Copy parameter rho
+        self.rho_ = self.rho
+        # If X is a dataframe, store its column names
+        if isinstance(X, pd.DataFrame):
+            self.column_names_ = list(X.columns)
+        # Check input data shape
+        X = check_input(X)
+        X = self._handle_missing(X)
+        self.fitted_models_ = []
+        for k in range(X.shape[1]):
+            col_enc = self._create_column_gap_encoder()
+            self.fitted_models_.append(col_enc.fit(X[:, k]))
+        return self
+
+    def transform(self, X) -> np.array:
+        """
+        Return the encoded vectors (activations) H of input strings in X.
+        Given the learnt topics W, the activations H are tuned to fit V = HW.
+        When X has several columns, they are encoded separately and
+        then concatenated.
+
+        Remark: calling transform multiple times in a row on the same
+        input X can give slightly different encodings. This is expected
+        due to a caching mechanism to speed things up.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            The string data to encode.
+
+        Returns
+        -------
+        H : 2-d array, shape (n_samples, n_topics * n_features)
+            Transformed input.
+        """
+        check_is_fitted(self, "fitted_models_")
+        # Check input data shape
+        X = check_input(X)
+        X = self._handle_missing(X)
+        X_enc = []
+        for k in range(X.shape[1]):
+            X_enc.append(self.fitted_models_[k].transform(X[:, k]))
+        X_enc = np.hstack(X_enc)
+        return X_enc
+
+    def partial_fit(self, X, y=None) -> "GapEncoder":
+        """
+        Partial fit of the GapEncoder on X.
+        To be used in an online learning procedure where batches of data are
+        coming one by one.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            The string data to fit the model on.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        GapEncoder
+            Fitted GapEncoder instance.
+        """
+
+        # If X is a dataframe, store its column names
+        if isinstance(X, pd.DataFrame):
+            self.column_names_ = list(X.columns)
+        # Check input data shape
+        X = check_input(X)
+        X = self._handle_missing(X)
+        # Init the `GapEncoderColumn` instances if the model was
+        # not fitted already.
+        if not hasattr(self, "fitted_models_"):
+            self.fitted_models_ = [
+                self._create_column_gap_encoder() for _ in range(X.shape[1])
+            ]
+        for k in range(X.shape[1]):
+            self.fitted_models_[k].partial_fit(X[:, k])
+        return self
+
+    def get_feature_names_out(
+        self,
+        col_names: Optional[Union[Literal["auto"], List[str]]] = None,
+        n_labels: int = 3,
+    ):
+        """
+        Returns the labels that best summarize the learned components/topics.
+        For each topic, labels with the highest activations are selected.
+
+        Parameters
+        ----------
+        col_names : "auto" or list of strings, optional
+            The column names to be added as prefixes before the labels.
+            If col_names == None, no prefixes are used.
+            If col_names == 'auto', column names are automatically defined:
+
+                - if the input data was a dataframe, its column names are used,
+                - otherwise, 'col1', ..., 'colN' are used as prefixes.
+
+            Prefixes can be manually set by passing a list for col_names.
+        n_labels : int, default=3
+            The number of labels used to describe each topic.
+
+        Returns
+        -------
+        list of strings
+            The labels that best describe each topic.
+        """
+        check_is_fitted(self, "fitted_models_")
+        # Generate prefixes
+        if isinstance(col_names, str) and col_names == "auto":
+            if hasattr(self, "column_names_"):  # Use column names
+                prefixes = ["%s: " % col for col in self.column_names_]
+            else:  # Use 'col1: ', ... 'colN: ' as prefixes
+                prefixes = ["col%d: " % i for i in range(len(self.fitted_models_))]
+        elif col_names is None:  # Empty prefixes
+            prefixes = [""] * len(self.fitted_models_)
+        else:
+            prefixes = ["%s: " % col for col in col_names]
+        labels = list()
+        for k, enc in enumerate(self.fitted_models_):
+            col_labels = enc.get_feature_names_out(n_labels, prefixes[k])
+            labels.extend(col_labels)
+        return labels
+
+    def get_feature_names(
+        self, input_features=None, col_names: List[str] = None, n_labels: int = 3
+    ) -> List[str]:
+        """
+        Ensures compatibility with sklearn < 1.0.
+        Use `get_feature_names_out` instead.
+        """
+        if parse_version(sklearn_version) >= parse_version("1.0"):
+            warnings.warn(
+                "Following the changes in scikit-learn 1.0, "
+                "get_feature_names is deprecated. "
+                "Use get_feature_names_out instead. ",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        return self.get_feature_names_out(col_names, n_labels)
+
+    def score(self, X) -> float:
+        """
+        Returns the sum over the columns of X of the Kullback-Leibler
+        divergence between the n-grams counts matrix V of X, and its
+        non-negative factorization HW.
+
+        Parameters
+        ----------
+        X : array-like (str), shape (n_samples, n_features)
+            The data to encode.
+
+        Returns
+        -------
+        float.
+            The Kullback-Leibler divergence.
+        """
+        X = check_input(X)
+        kl_divergence = 0
+        for k in range(X.shape[1]):
+            kl_divergence += self.fitted_models_[k].score(X[:, k])
+        return kl_divergence
+
+
+def _rescale_W(W: np.array, A: np.array) -> None:
+    """
+    Rescale the topics W to have a L1-norm equal to 1.
+    Note that they are modified in-place.
+    """
+    s = W.sum(axis=1, keepdims=True)
+    W /= s
+    A /= s
+
+
+def _multiplicative_update_w(
+    Vt: np.array,
+    W: np.array,
+    A: np.array,
+    B: np.array,
+    Ht: np.array,
+    rescale_W: bool,
+    rho: float,
+) -> Tuple[np.array, np.array, np.array]:
+    """
+    Multiplicative update step for the topics W.
+    """
+    A *= rho
+    A += W * safe_sparse_dot(Ht.T, Vt.multiply(1 / (np.dot(Ht, W) + 1e-10)))
+    B *= rho
+    B += Ht.sum(axis=0).reshape(-1, 1)
+    np.divide(A, B, out=W)
+    if rescale_W:
+        _rescale_W(W, A)
+    return W, A, B
+
+
+def _rescale_h(V: np.array, H: np.array) -> np.array:
+    """
+    Rescale the activations H.
+    """
+    epsilon = 1e-10  # in case of a document having length=0
+    H *= np.maximum(epsilon, V.sum(axis=1).A)
+    H /= H.sum(axis=1, keepdims=True)
+    return H
+
+
+def _multiplicative_update_h(
+    Vt: np.array,
+    W: np.array,
+    Ht: np.array,
+    epsilon: float = 1e-3,
+    max_iter: int = 10,
+    rescale_W: bool = False,
+    gamma_shape_prior: float = 1.1,
+    gamma_scale_prior: float = 1.0,
+):
+    """
+    Multiplicative update step for the activations H.
+    """
+    if rescale_W:
+        WT1 = 1 + 1 / gamma_scale_prior
+        W_WT1 = W / WT1
+    else:
+        WT1 = np.sum(W, axis=1) + 1 / gamma_scale_prior
+        W_WT1 = W / WT1.reshape(-1, 1)
+    const = (gamma_shape_prior - 1) / WT1
+    squared_epsilon = epsilon**2
+    for vt, ht in zip(Vt, Ht):
+        vt_ = vt.data
+        idx = vt.indices
+        W_WT1_ = W_WT1[:, idx]
+        W_ = W[:, idx]
+        squared_norm = 1
+        for n_iter_ in range(max_iter):
+            if squared_norm <= squared_epsilon:
+                break
+            aux = np.dot(W_WT1_, vt_ / (np.dot(ht, W_) + 1e-10))
+            ht_out = ht * aux + const
+            squared_norm = np.dot(ht_out - ht, ht_out - ht) / np.dot(ht, ht)
+            ht[:] = ht_out
+    return Ht
+
+
+def batch_lookup(
+    lookup: np.array,
+    n: int = 1,
+) -> Generator[Tuple[np.array, np.array], None, None]:
+    """
+    Make batches of the lookup array.
+    """
+    len_iter = len(lookup)
+    for idx in range(0, len_iter, n):
+        indices = lookup[slice(idx, min(idx + n, len_iter))]
+        unq_indices = np.unique(indices)
+        yield unq_indices, indices
+
+
+def get_kmeans_prototypes(
+    X,
+    n_prototypes: int,
+    analyzer: Literal["word", "char", "char_wb"] = "char",
+    hashing_dim: int = 128,
+    ngram_range: Tuple[int, int] = (2, 4),
+    sparse: bool = False,
+    sample_weight=None,
+    random_state: Optional[Union[int, RandomState]] = None,
+):
+    """
+    Computes prototypes based on:
+      - dimensionality reduction (via hashing n-grams)
+      - k-means clustering
+      - nearest neighbor
+    """
+    vectorizer = HashingVectorizer(
+        analyzer=analyzer,
+        norm=None,
+        alternate_sign=False,
+        ngram_range=ngram_range,
+        n_features=hashing_dim,
+    )
+    projected = vectorizer.transform(X)
+    if not sparse:
+        projected = projected.toarray()
+    kmeans = KMeans(n_clusters=n_prototypes, random_state=random_state)
+    kmeans.fit(projected, sample_weight=sample_weight)
+    centers = kmeans.cluster_centers_
+    neighbors = NearestNeighbors()
+    neighbors.fit(projected)
+    indexes_prototypes = np.unique(neighbors.kneighbors(centers, 1)[-1])
+    return np.sort(X[indexes_prototypes])
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_minhash_encoder.py` & `dirty_cat-0.4.1/dirty_cat/_minhash_encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,330 +1,338 @@
-"""
-Minhash encoding of string arrays.
-The principle is as follows:
-  1. A string is viewed as a succession of numbers (the ASCII or UTF8
-     representation of its elements).
-  2. The string is then decomposed into a set of n-grams, i.e.
-     n-dimensional vectors of integers.
-  3. A hashing function is used to assign an integer to each n-gram.
-     The minimum of the hashes over all n-grams is used in the encoding.
-  4. This process is repeated with N hashing functions are used to
-     form N-dimensional encodings.
-Maxhash encodings can be computed similarly by taking the hashes maximum
-instead.
-With this procedure, strings that share many n-grams have greater
-probability of having same encoding values. These encodings thus capture
-morphological similarities between strings.
-"""
-
-from typing import Callable, Collection, Dict, List, Literal, Tuple
-
-import numpy as np
-from joblib import Parallel, delayed, effective_n_jobs
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils import gen_even_slices, murmurhash3_32
-from sklearn.utils.validation import check_is_fitted
-
-from ._fast_hash import ngram_min_hash
-from ._string_distances import get_unique_ngrams
-from ._utils import LRUDict, check_input
-
-NoneType = type(None)
-
-
-# Ignore lines too long, as links in the docstring cannot be cut.
-# flake8: noqa: E501
-
-
-class MinHashEncoder(BaseEstimator, TransformerMixin):
-    """
-    Encode string categorical features as a numeric array, minhash method
-    applied to ngram decomposition of strings based on ngram decomposition
-    of the string.
-
-    Parameters
-    ----------
-    n_components : int, default=30
-        The number of dimension of encoded strings. Numbers around 300 tend to
-        lead to good prediction performance, but with more computational cost.
-    ngram_range : typing.Tuple[int, int], default=(2, 4)
-        The lower and upper boundary of the range of n-values for different
-        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
-        will be used.
-    hashing : typing.Literal["fast", "murmur"], default=fast
-        Hashing function. fast is faster but
-        might have some concern with its entropy.
-    minmax_hash : bool, default=False
-        if True, return min hash and max hash concatenated.
-    handle_missing : typing.Literal["error", "zero_impute"], default=zero_impute
-        Whether to raise an error or encode missing values (NaN) with
-        vectors filled with zeros.
-    n_jobs : int, default=None
-        The number of jobs to run in parallel.
-        The hash computations for all unique elements are parallelized.
-        None means 1 unless in a
-        `joblib.parallel_backend context <https://joblib.readthedocs.io/en/latest/parallel.html>`_.
-        -1 means using all processors.
-        See `Scikit-learn Glossary <https://scikit-learn.org/stable/glossary.html#term-n_jobs>`_
-        for more details.
-
-    Attributes
-    ----------
-    hash_dict_ : LRUDict
-        Computed hashes.
-
-    Examples
-    --------
-    >>> enc = MinHashEncoder(n_components=5)
-
-    Let's encode the following non-normalized data:
-
-    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['London']]
-
-    >>> enc.fit(X)
-    MinHashEncoder()
-
-    The encoded data with 5 components are:
-
-    >>> enc.transform(X)
-    array([[-1.78337518e+09, -1.58827021e+09, -1.66359234e+09,
-            -1.81988679e+09, -1.96259387e+09],
-           [-8.48046971e+08, -1.76657887e+09, -1.55891205e+09,
-            -1.48574446e+09, -1.68729890e+09],
-           [-1.97582893e+09, -2.09500033e+09, -1.59652117e+09,
-            -1.81759383e+09, -2.09569333e+09],
-           [-1.97582893e+09, -2.09500033e+09, -1.53072052e+09,
-            -1.45918266e+09, -1.58098831e+09]])
-
-    References
-    ----------
-    For a detailed description of the method, see
-    `Encoding high-cardinality string categorical variables
-    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
-
-    """
-
-    hash_dict_: LRUDict
-
-    _capacity: int = 2**10
-
-    def __init__(
-        self,
-        n_components: int = 30,
-        ngram_range: Tuple[int, int] = (2, 4),
-        hashing: Literal["fast", "murmur"] = "fast",
-        minmax_hash: bool = False,
-        handle_missing: Literal["error", "zero_impute"] = "zero_impute",
-        n_jobs: int = None,
-    ):
-        self.ngram_range = ngram_range
-        self.n_components = n_components
-        self.hashing = hashing
-        self.minmax_hash = minmax_hash
-        self.handle_missing = handle_missing
-        self.n_jobs = n_jobs
-
-    def _more_tags(self) -> Dict[str, List[str]]:
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def _get_murmur_hash(self, string: str) -> np.array:
-        """
-        Encode a string using murmur hashing function.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-
-        Returns
-        -------
-        :obj:`~numpy.ndarray` of shape (n_components, )
-            The encoded string.
-        """
-        min_hashes = np.ones(self.n_components) * np.infty
-        grams = get_unique_ngrams(string, self.ngram_range)
-        if len(grams) == 0:
-            grams = get_unique_ngrams(" Na ", self.ngram_range)
-        for gram in grams:
-            hash_array = np.array(
-                [
-                    murmurhash3_32("".join(gram), seed=d, positive=True)
-                    for d in range(self.n_components)
-                ]
-            )
-            min_hashes = np.minimum(min_hashes, hash_array)
-        return min_hashes / (2**32 - 1)
-
-    def _get_fast_hash(self, string: str) -> np.array:
-        """
-        Encode a string with fast hashing function.
-        fast hashing supports both min_hash and minmax_hash encoding.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-
-        Returns
-        -------
-        :obj:`~numpy.ndarray` of shape (n_components, )
-            The encoded string, using specified encoding scheme.
-        """
-        if self.minmax_hash:
-            return np.concatenate(
-                [
-                    ngram_min_hash(string, self.ngram_range, seed, return_minmax=True)
-                    for seed in range(self.n_components // 2)
-                ]
-            )
-        else:
-            return np.array(
-                [
-                    ngram_min_hash(string, self.ngram_range, seed)
-                    for seed in range(self.n_components)
-                ]
-            )
-
-    def _compute_hash_batched(
-        self, batch: Collection[str], hash_func: Callable[[str], np.ndarray]
-    ):
-        """
-        Function called to compute the hashes of a batch of strings.
-
-        Check if the string is in the hash dictionary, if not, compute the hash
-        using the specified hashing function and add it to the dictionary.
-
-        Parameters
-        ----------
-        batch : collection of str
-            The batch of strings to encode.
-        hash_func : callable
-            Hashing function to use on the string.
-
-        Returns
-        -------
-        :obj:`~numpy.ndarray` of shape (n_samples, n_components)
-            The encoded strings, using specified encoding scheme.
-        """
-        res = np.zeros((len(batch), self.n_components))
-        for i, string in enumerate(batch):
-            if string not in self.hash_dict_:
-                if string == "NAN":  # true if x is a missing value
-                    self.hash_dict_[string] = np.zeros(self.n_components)
-                else:
-                    self.hash_dict_[string] = hash_func(string)
-            res[i] = self.hash_dict_[string]
-        return res
-
-    def fit(self, X, y=None) -> "MinHashEncoder":
-        """
-        Fit the MinHashEncoder to X. In practice, just initializes a dictionary
-        to store encodings to speed up computation.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
-            The string data to encode. Only here for compatibility.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        MinHashEncoder
-            The fitted MinHashEncoder instance.
-        """
-        if self.hashing not in ["fast", "murmur"]:
-            raise ValueError(
-                f"Got hashing={self.hashing!r}, "
-                'but expected any of {"fast", "murmur"}. '
-            )
-        if self.handle_missing not in ["error", "zero_impute"]:
-            raise ValueError(
-                f"Got handle_missing={self.handle_missing!r}, but expected "
-                'any of {"error", "zero_impute"}. '
-            )
-        self.hash_dict_ = LRUDict(capacity=self._capacity)
-        return self
-
-    def transform(self, X) -> np.array:
-        """
-        Transform X using specified encoding scheme.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
-            The string data to encode.
-
-        Returns
-        -------
-        :obj:`~numpy.ndarray` of shape (n_samples, n_components)
-            Transformed input.
-        """
-        check_is_fitted(self, "hash_dict_")
-        X = check_input(X)
-        if self.minmax_hash:
-            if self.n_components % 2 != 0:
-                raise ValueError(
-                    "n_components should be even when using"
-                    f"minmax_hash encoding, got {self.n_components}"
-                )
-        if self.hashing == "murmur":
-            if self.minmax_hash:
-                raise ValueError(
-                    "minmax_hash encoding is not supported"
-                    "with the murmur hashing function"
-                )
-        if self.handle_missing not in ["error", "zero_impute"]:
-            raise ValueError(
-                "handle_missing should be either "
-                f"'error' or 'zero_impute', got {self.handle_missing!r}"
-            )
-
-        # Handle missing values
-        missing_mask = (
-            ~(X == X)  # Find np.nan
-            | (X == None)  # Find None. Note: `X is None` doesn't work.
-            | (X == "")  # Find empty strings
-        )
-
-        if missing_mask.any():  # contains at least one missing value
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='zero_impute' to encode with missing values"
-                )
-            elif self.handle_missing == "zero_impute":
-                # NANs will be replaced by zeroes in _compute_hash
-                X[missing_mask] = "NAN"
-
-        if self.hashing == "fast":
-            hash_func = self._get_fast_hash
-        elif self.hashing == "murmur":
-            hash_func = self._get_murmur_hash
-        else:
-            raise ValueError(
-                "Hashing function should be either 'fast' or 'murmur', "
-                f"got {self.hashing!r}"
-            )
-
-        # Compute the hashes for unique values
-        unique_x, indices_x = np.unique(X, return_inverse=True)
-        n_jobs = effective_n_jobs(self.n_jobs)
-
-        # Compute the hashes in parallel on n_jobs batches
-        unique_x_trans = Parallel(n_jobs=n_jobs)(
-            delayed(self._compute_hash_batched)(
-                unique_x[idx_slice],
-                hash_func,
-            )
-            for idx_slice in gen_even_slices(len(unique_x), n_jobs)
-        )
-
-        # Match the hashes of the unique value to the original values
-        X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
-            len(X), X.shape[1] * self.n_components
-        )
-
-        return X_out.astype(np.float64)  # The output is an int32 before conversion
+"""
+Minhash encoding of string arrays.
+The principle is as follows:
+  1. A string is viewed as a succession of numbers (the ASCII or UTF8
+     representation of its elements).
+  2. The string is then decomposed into a set of n-grams, i.e.
+     n-dimensional vectors of integers.
+  3. A hashing function is used to assign an integer to each n-gram.
+     The minimum of the hashes over all n-grams is used in the encoding.
+  4. This process is repeated with N hashing functions are used to
+     form N-dimensional encodings.
+Maxhash encodings can be computed similarly by taking the hashes maximum
+instead.
+With this procedure, strings that share many n-grams have greater
+probability of having same encoding values. These encodings thus capture
+morphological similarities between strings.
+"""
+
+from typing import Callable, Collection, Dict, List, Literal, Tuple
+
+import numpy as np
+from joblib import Parallel, delayed, effective_n_jobs
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils import gen_even_slices, murmurhash3_32
+from sklearn.utils.validation import check_is_fitted
+
+from ._fast_hash import ngram_min_hash
+from ._string_distances import get_unique_ngrams
+from ._utils import LRUDict, check_input
+
+NoneType = type(None)
+
+
+# Ignore lines too long, as links in the docstring cannot be cut.
+# flake8: noqa: E501
+
+
+class MinHashEncoder(BaseEstimator, TransformerMixin):
+    """
+    Encode string categorical features as a numeric array, minhash method
+    applied to ngram decomposition of strings based on ngram decomposition
+    of the string.
+
+    Parameters
+    ----------
+    n_components : int, default=30
+        The number of dimension of encoded strings. Numbers around 300 tend to
+        lead to good prediction performance, but with more computational cost.
+    ngram_range : typing.Tuple[int, int], default=(2, 4)
+        The lower and upper boundary of the range of n-values for different
+        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
+        will be used.
+    hashing : typing.Literal["fast", "murmur"], default=fast
+        Hashing function. fast is faster but
+        might have some concern with its entropy.
+    minmax_hash : bool, default=False
+        if True, return min hash and max hash concatenated.
+    handle_missing : typing.Literal["error", "zero_impute"], default=zero_impute
+        Whether to raise an error or encode missing values (NaN) with
+        vectors filled with zeros.
+    n_jobs : int, default=None
+        The number of jobs to run in parallel.
+        The hash computations for all unique elements are parallelized.
+        None means 1 unless in a
+        `joblib.parallel_backend context <https://joblib.readthedocs.io/en/latest/parallel.html>`_.
+        -1 means using all processors.
+        See `Scikit-learn Glossary <https://scikit-learn.org/stable/glossary.html#term-n_jobs>`_
+        for more details.
+
+    Attributes
+    ----------
+    hash_dict_ : LRUDict
+        Computed hashes.
+
+    See Also
+    --------
+    :class:`~dirty_cat.GapEncoder` :
+        Encodes dirty categories (strings) by constructing latent topics with continuous encoding.
+    :class:`~dirty_cat.SimilarityEncoder` :
+        Encode string columns as a numeric array with n-gram string similarity.
+    :class:`~dirty_cat.deduplicate` :
+        Deduplicate data by hierarchically clustering similar strings.
+
+    References
+    ----------
+    For a detailed description of the method, see
+    `Encoding high-cardinality string categorical variables
+    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
+
+    Examples
+    --------
+    >>> enc = MinHashEncoder(n_components=5)
+
+    Let's encode the following non-normalized data:
+
+    >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['London']]
+
+    >>> enc.fit(X)
+    MinHashEncoder()
+
+    The encoded data with 5 components are:
+
+    >>> enc.transform(X)
+    array([[-1.78337518e+09, -1.58827021e+09, -1.66359234e+09,
+            -1.81988679e+09, -1.96259387e+09],
+           [-8.48046971e+08, -1.76657887e+09, -1.55891205e+09,
+            -1.48574446e+09, -1.68729890e+09],
+           [-1.97582893e+09, -2.09500033e+09, -1.59652117e+09,
+            -1.81759383e+09, -2.09569333e+09],
+           [-1.97582893e+09, -2.09500033e+09, -1.53072052e+09,
+            -1.45918266e+09, -1.58098831e+09]])
+    """
+
+    hash_dict_: LRUDict
+
+    _capacity: int = 2**10
+
+    def __init__(
+        self,
+        n_components: int = 30,
+        ngram_range: Tuple[int, int] = (2, 4),
+        hashing: Literal["fast", "murmur"] = "fast",
+        minmax_hash: bool = False,
+        handle_missing: Literal["error", "zero_impute"] = "zero_impute",
+        n_jobs: int = None,
+    ):
+        self.ngram_range = ngram_range
+        self.n_components = n_components
+        self.hashing = hashing
+        self.minmax_hash = minmax_hash
+        self.handle_missing = handle_missing
+        self.n_jobs = n_jobs
+
+    def _more_tags(self) -> Dict[str, List[str]]:
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {"X_types": ["categorical"]}
+
+    def _get_murmur_hash(self, string: str) -> np.array:
+        """
+        Encode a string using murmur hashing function.
+
+        Parameters
+        ----------
+        string : str
+            The string to encode.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray` of shape (n_components, )
+            The encoded string.
+        """
+        min_hashes = np.ones(self.n_components) * np.infty
+        grams = get_unique_ngrams(string, self.ngram_range)
+        if len(grams) == 0:
+            grams = get_unique_ngrams(" Na ", self.ngram_range)
+        for gram in grams:
+            hash_array = np.array(
+                [
+                    murmurhash3_32("".join(gram), seed=d, positive=True)
+                    for d in range(self.n_components)
+                ]
+            )
+            min_hashes = np.minimum(min_hashes, hash_array)
+        return min_hashes / (2**32 - 1)
+
+    def _get_fast_hash(self, string: str) -> np.array:
+        """
+        Encode a string with fast hashing function.
+        fast hashing supports both min_hash and minmax_hash encoding.
+
+        Parameters
+        ----------
+        string : str
+            The string to encode.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray` of shape (n_components, )
+            The encoded string, using specified encoding scheme.
+        """
+        if self.minmax_hash:
+            return np.concatenate(
+                [
+                    ngram_min_hash(string, self.ngram_range, seed, return_minmax=True)
+                    for seed in range(self.n_components // 2)
+                ]
+            )
+        else:
+            return np.array(
+                [
+                    ngram_min_hash(string, self.ngram_range, seed)
+                    for seed in range(self.n_components)
+                ]
+            )
+
+    def _compute_hash_batched(
+        self, batch: Collection[str], hash_func: Callable[[str], np.ndarray]
+    ):
+        """
+        Function called to compute the hashes of a batch of strings.
+
+        Check if the string is in the hash dictionary, if not, compute the hash
+        using the specified hashing function and add it to the dictionary.
+
+        Parameters
+        ----------
+        batch : collection of str
+            The batch of strings to encode.
+        hash_func : callable
+            Hashing function to use on the string.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray` of shape (n_samples, n_components)
+            The encoded strings, using specified encoding scheme.
+        """
+        res = np.zeros((len(batch), self.n_components))
+        for i, string in enumerate(batch):
+            if string not in self.hash_dict_:
+                if string == "NAN":  # true if x is a missing value
+                    self.hash_dict_[string] = np.zeros(self.n_components)
+                else:
+                    self.hash_dict_[string] = hash_func(string)
+            res[i] = self.hash_dict_[string]
+        return res
+
+    def fit(self, X, y=None) -> "MinHashEncoder":
+        """
+        Fit the MinHashEncoder to X. In practice, just initializes a dictionary
+        to store encodings to speed up computation.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, ) or (n_samples, 1)
+            The string data to encode. Only here for compatibility.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        MinHashEncoder
+            The fitted MinHashEncoder instance.
+        """
+        if self.hashing not in ["fast", "murmur"]:
+            raise ValueError(
+                f"Got hashing={self.hashing!r}, "
+                'but expected any of {"fast", "murmur"}. '
+            )
+        if self.handle_missing not in ["error", "zero_impute"]:
+            raise ValueError(
+                f"Got handle_missing={self.handle_missing!r}, but expected "
+                'any of {"error", "zero_impute"}. '
+            )
+        self.hash_dict_ = LRUDict(capacity=self._capacity)
+        return self
+
+    def transform(self, X) -> np.array:
+        """
+        Transform X using specified encoding scheme.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, ) or (n_samples, 1)
+            The string data to encode.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray` of shape (n_samples, n_components)
+            Transformed input.
+        """
+        check_is_fitted(self, "hash_dict_")
+        X = check_input(X)
+        if self.minmax_hash:
+            if self.n_components % 2 != 0:
+                raise ValueError(
+                    "n_components should be even when using"
+                    f"minmax_hash encoding, got {self.n_components}"
+                )
+        if self.hashing == "murmur":
+            if self.minmax_hash:
+                raise ValueError(
+                    "minmax_hash encoding is not supported"
+                    "with the murmur hashing function"
+                )
+        if self.handle_missing not in ["error", "zero_impute"]:
+            raise ValueError(
+                "handle_missing should be either "
+                f"'error' or 'zero_impute', got {self.handle_missing!r}"
+            )
+
+        # Handle missing values
+        missing_mask = (
+            ~(X == X)  # Find np.nan
+            | (X == None)  # Find None. Note: `X is None` doesn't work.
+            | (X == "")  # Find empty strings
+        )
+
+        if missing_mask.any():  # contains at least one missing value
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='zero_impute' to encode with missing values"
+                )
+            elif self.handle_missing == "zero_impute":
+                # NANs will be replaced by zeroes in _compute_hash
+                X[missing_mask] = "NAN"
+
+        if self.hashing == "fast":
+            hash_func = self._get_fast_hash
+        elif self.hashing == "murmur":
+            hash_func = self._get_murmur_hash
+        else:
+            raise ValueError(
+                "Hashing function should be either 'fast' or 'murmur', "
+                f"got {self.hashing!r}"
+            )
+
+        # Compute the hashes for unique values
+        unique_x, indices_x = np.unique(X, return_inverse=True)
+        n_jobs = effective_n_jobs(self.n_jobs)
+
+        # Compute the hashes in parallel on n_jobs batches
+        unique_x_trans = Parallel(n_jobs=n_jobs)(
+            delayed(self._compute_hash_batched)(
+                unique_x[idx_slice],
+                hash_func,
+            )
+            for idx_slice in gen_even_slices(len(unique_x), n_jobs)
+        )
+
+        # Match the hashes of the unique value to the original values
+        X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
+            len(X), X.shape[1] * self.n_components
+        )
+
+        return X_out.astype(np.float64)  # The output is an int32 before conversion
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_similarity_encoder.py` & `dirty_cat-0.4.1/dirty_cat/_similarity_encoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,670 +1,692 @@
-"""
-Similarity encoding of string arrays.
-The principle is as follows:
-    1. Given an input string array X = [x1, ..., xn] with k unique categories
-       [c1, ..., ck] and a similarity measure sim(s1, s2) between strings,
-       we define the encoded vector of xi as [sim(xi, c1), ... , sim(xi, ck)].
-       Similarity encoding of X results in a matrix with shape (n, k) that
-       captures morphological similarities between string entries.
-    2. To avoid dealing with high-dimensional encodings when k is high, we can
-       use d << k prototypes [p1, ..., pd] with which similarities will be
-       computed:  xi -> [sim(xi, p1), ..., sim(xi, pd)]. These prototypes can
-       be automatically sampled from the input data (most frequent categories,
-       KMeans) or provided by the user.
-"""
-
-import warnings
-from typing import List, Literal, Optional, Tuple, Union
-
-import numpy as np
-import sklearn
-from joblib import Parallel, delayed
-from numpy.random import RandomState
-from scipy import sparse
-from sklearn.cluster import KMeans
-from sklearn.feature_extraction.text import CountVectorizer, HashingVectorizer
-from sklearn.neighbors import NearestNeighbors
-from sklearn.preprocessing import OneHotEncoder
-from sklearn.utils import check_random_state
-from sklearn.utils.fixes import _object_dtype_isnan
-from sklearn.utils.validation import check_is_fitted
-
-from ._string_distances import get_ngram_count, preprocess
-from ._utils import parse_version
-
-
-def _ngram_similarity_one_sample_inplace(
-    x_count_vector: np.ndarray,
-    vocabulary_count_matrix: np.ndarray,
-    str_x: str,
-    vocabulary_ngram_counts: np.ndarray,
-    se_dict: dict,
-    unq_X: np.ndarray,
-    i: int,
-    ngram_range: Tuple[int, int],
-) -> None:
-    """
-    Update inplace a dict of similarities between a string and a vocabulary
-
-    Parameters
-    ----------
-    x_count_vector : np.ndarray
-        Count vector of the sample based on the ngrams of the vocabulary
-    vocabulary_count_matrix : np.ndarray
-        Count vector of the vocabulary based on its ngrams
-    str_x: str
-        The actual sample string
-    vocabulary_ngram_counts : np.ndarray
-        Number of ngrams for each unique element of the vocabulary
-    se_dict : dict
-        Dictionary containing the similarities for each x in unq_X
-    unq_X : np.ndarray
-        The arrays of all unique samples
-    i : str
-        The index of x_count_vector in the csr count matrix
-    ngram_range : tuple
-        n-grams to use for the decomposition, where ``n_min <= n <= n_max``.
-    """
-    nonzero_idx = x_count_vector.indices
-    nonzero_vals = x_count_vector.data
-
-    same_grams = np.asarray(
-        (vocabulary_count_matrix[:, nonzero_idx].minimum(nonzero_vals)).sum(axis=1)
-    )
-
-    all_grams = (
-        get_ngram_count(str_x, ngram_range) + vocabulary_ngram_counts - same_grams
-    )
-    similarity = np.divide(
-        same_grams, all_grams, out=np.zeros_like(same_grams), where=all_grams != 0
-    )
-    se_dict[unq_X[i]] = similarity.reshape(-1)
-
-
-def ngram_similarity_matrix(
-    X,
-    cats: List[str],
-    ngram_range: Tuple[int, int],
-    hashing_dim: int,
-    dtype: type = np.float64,
-) -> np.ndarray:
-    """
-    Similarity encoding for dirty categorical variables:
-    Given two arrays of strings, returns the similarity encoding matrix
-    of size len(X) x len(cats)
-
-    ngram_sim(s_i, s_j) =
-        ||min(ci, cj)||_1 / (||ci||_1 + ||cj||_1 - ||min(ci, cj)||_1)
-    """
-    min_n, max_n = ngram_range
-    unq_X = np.unique(X)
-    cats = np.array([" %s " % cat for cat in cats])
-    unq_X_ = np.array([" %s " % x for x in unq_X])
-    if not hashing_dim:
-        vectorizer = CountVectorizer(
-            analyzer="char", ngram_range=(min_n, max_n), dtype=dtype
-        )
-        vectorizer.fit(np.concatenate((cats, unq_X_)))
-    else:
-        vectorizer = HashingVectorizer(
-            analyzer="char",
-            ngram_range=(min_n, max_n),
-            n_features=hashing_dim,
-            norm=None,
-            alternate_sign=False,
-            dtype=dtype,
-        )
-        vectorizer.fit(X)
-    count_cats = vectorizer.transform(cats)
-    count_X = vectorizer.transform(unq_X_)
-    # We don't need the vectorizer anymore, delete it to save memory
-    del vectorizer
-    sum_cats = np.asarray(count_cats.sum(axis=1))
-    SE_dict = {}
-
-    for i, x in enumerate(count_X):
-        _, nonzero_idx, nonzero_vals = sparse.find(x)
-        same_grams = np.asarray(
-            (count_cats[:, nonzero_idx].minimum(nonzero_vals)).sum(axis=1)
-        )
-        all_grams = x.sum() + sum_cats - same_grams
-        similarity = np.divide(same_grams, all_grams)
-        SE_dict[unq_X[i]] = similarity.reshape(-1)
-    # We don't need the counts anymore, delete them to save memory
-    del count_cats, count_X
-
-    out = np.empty((len(X), similarity.size), dtype=dtype)
-    for x, out_row in zip(X, out):
-        out_row[:] = SE_dict[x]
-
-    return np.nan_to_num(out, copy=False)
-
-
-def get_prototype_frequencies(prototypes: np.ndarray) -> np.array:
-    """
-    Computes the frequencies of the values contained in prototypes
-    Reverse sorts the array by the frequency
-    Returns a numpy array of the values without their frequencies
-    """
-    uniques, counts = np.unique(prototypes, return_counts=True)
-    sorted_indexes = np.argsort(counts)[::-1]
-    return uniques[sorted_indexes], counts[sorted_indexes]
-
-
-def get_kmeans_prototypes(
-    X,
-    n_prototypes: int,
-    hashing_dim: int = 128,
-    ngram_range: Tuple[int, int] = (3, 3),
-    sparse: bool = False,
-    sample_weight=None,
-    random_state: Optional[Union[int, RandomState]] = None,
-) -> np.array:
-    """
-    Computes prototypes based on:
-      - dimensionality reduction (via hashing n-grams)
-      - k-means clustering
-      - nearest neighbor
-    """
-    vectorizer = HashingVectorizer(
-        analyzer="char",
-        norm=None,
-        alternate_sign=False,
-        ngram_range=ngram_range,
-        n_features=hashing_dim,
-    )
-    projected = vectorizer.transform(X)
-    if not sparse:
-        projected = projected.toarray()
-    kmeans = KMeans(n_clusters=n_prototypes, random_state=random_state)
-    kmeans.fit(projected, sample_weight=sample_weight)
-    centers = kmeans.cluster_centers_
-    neighbors = NearestNeighbors()
-    neighbors.fit(projected)
-    indexes_prototypes = np.unique(neighbors.kneighbors(centers, 1)[-1])
-    if indexes_prototypes.shape[0] < n_prototypes:
-        warnings.warn(
-            "Final number of unique prototypes is lower than "
-            + "n_prototypes (expected). "
-        )
-    return np.sort(X[indexes_prototypes])
-
-
-class SimilarityEncoder(OneHotEncoder):
-    """
-    Encode string categorical features as a numeric array.
-
-    The input to this transformer should be an array-like of
-    strings.
-    The method is based on calculating the morphological similarities
-    between the categories.
-    This encoding is an alternative to OneHotEncoder in the case of
-    dirty categorical variables.
-
-    Parameters
-    ----------
-    similarity : None
-        Deprecated in dirty_cat 0.3, will be removed in 0.5.
-        Was used to specify the type of pairwise string similarity to use.
-        Since 0.3, only the ngram similarity is supported.
-    ngram_range : tuple (min_n, max_n), default=(2, 4)
-        The range of values for the n_gram similarity.
-    categories : typing.Union[typing.Literal["auto", "k-means", "most_frequent"], typing.List[typing.List[str]]]  # noqa
-        Categories (unique values) per feature:
-
-        - 'auto' : Determine categories automatically from the training data.
-        - list : ``categories[i]`` holds the categories expected in the i-th
-          column. The passed categories must be sorted and should not mix
-          strings and numeric values.
-        - 'most_frequent' : Computes the most frequent values for every
-           categorical variable
-        - 'k-means' : Computes the K nearest neighbors of K-mean centroids
-           in order to choose the prototype categories
-
-        The categories used can be found in the ``categories_`` attribute.
-    dtype : number type, default np.float64
-        Desired dtype of output.
-    handle_unknown : 'error' or 'ignore' (default)
-        Whether to raise an error or ignore if an unknown categorical feature
-        is present during transform (default is to ignore). When this parameter
-        is set to 'ignore' and an unknown category is encountered during
-        transform, the resulting encoded columns for this feature
-        will be all zeros. In the inverse transform, an unknown category
-        will be denoted as None.
-    handle_missing : 'error' or '' (default)
-        Whether to raise an error or impute with blank string '' if missing
-        values (NaN) are present during fit (default is to impute).
-        When this parameter is set to '', and a missing value is encountered
-        during fit_transform, the resulting encoded columns for this feature
-        will be all zeros. In the inverse transform, the missing category
-        will be denoted as None.
-    hashing_dim : int type or None.
-        If None, the base vectorizer is CountVectorizer, else it's set to
-        HashingVectorizer with a number of features equal to `hashing_dim`.
-    n_prototypes : number of prototype we want to use.
-        Useful when `most_frequent` or `k-means` is used.
-        Must be a positive non-null integer.
-    random_state : either an int used as a seed, a RandomState instance or None.
-        Useful when `k-means` strategy is used.
-    n_jobs : int, optional
-        maximum number of processes used to compute similarity matrices. Used
-        only if ``fast=True`` in ``SimilarityEncoder.transform``
-
-    Examples
-    --------
-    >>> enc = SimilarityEncoder()
-    >>> X = [['Male', 1], ['Female', 3], ['Female', 2]]
-    >>> enc.fit(X)
-    SimilarityEncoder()
-
-    It inherits the same methods as sklearn's :class:`~sklearn.preprocessing.OneHotEncoder`:
-
-    >>> enc.categories_
-    [array(['Female', 'Male'], dtype=object), array([1, 2, 3], dtype=object)]
-
-    But it provides a continuous encoding based on similarity
-    instead of a discrete one based on exact matches:
-
-    >>> enc.transform([['Female', 1], ['Male', 4]])
-    array([[1., 0.42857143, 1., 0., 0.],
-           [0.42857143, 1., 0. , 0. , 0.]])
-
-    >>> enc.inverse_transform([[1., 0.42857143, 1., 0., 0.], [0.42857143, 1., 0. , 0. , 0.]])
-    array([['Female', 1],
-           ['Male', None]], dtype=object)
-
-    >>> enc.get_feature_names_out(['gender', 'group'])
-    array(['gender_Female', 'gender_Male', 'group_1', 'group_2', 'group_3'], ...)
-
-    Attributes
-    ----------
-    categories_ : typing.List[np.array]
-        The categories of each feature determined during fitting
-        (in order corresponding with output of ``transform``).
-    _infrequent_enabled : bool, default=False
-        Avoid taking into account the existence of infrequent categories.
-
-    References
-    ----------
-
-    For a detailed description of the method, see
-    `Similarity encoding for learning with dirty categorical variables
-    <https://hal.inria.fr/hal-01806175>`_ by Cerda, Varoquaux, Kegl. 2018
-    (accepted for publication at: Machine Learning journal, Springer).
-
-    """
-
-    categories_: List[np.array]
-    n_features_in_: int
-    random_state_: Union[int, RandomState]
-    drop_idx_: np.array
-    vectorizers_: List[CountVectorizer]
-    vocabulary_count_matrices_: List[np.array]
-    vocabulary_ngram_counts_: List[List[int]]
-    _infrequent_enabled: bool
-
-    def __init__(
-        self,
-        similarity: str = "ngram",
-        ngram_range: Tuple[int, int] = (2, 4),
-        categories: Union[
-            Literal["auto", "k-means", "most_frequent"], List[List[str]]
-        ] = "auto",
-        dtype: type = np.float64,
-        handle_unknown: Literal["error", "ignore"] = "ignore",
-        handle_missing: Literal["error", ""] = "",
-        hashing_dim: Optional[int] = None,
-        n_prototypes: Optional[int] = None,
-        random_state: Optional[Union[int, RandomState]] = None,
-        n_jobs: Optional[int] = None,
-    ):
-        super().__init__()
-        self.categories = categories
-        self.dtype = dtype
-        self.handle_unknown = handle_unknown
-        self.handle_missing = handle_missing
-        self.ngram_range = ngram_range
-        self.hashing_dim = hashing_dim
-        self.n_prototypes = n_prototypes
-        self.random_state = random_state
-        self.n_jobs = n_jobs
-
-        if similarity is not None:
-            warnings.warn(
-                'The "similarity" argument is deprecated since dirty_cat 0.3, '
-                "and will be removed in 0.5."
-                "The n-gram similarity is the only one currently supported. ",
-                category=UserWarning,
-                stacklevel=2,
-            )
-        self.similarity = None
-
-        if not isinstance(categories, list):
-            if categories not in ["auto", "k-means", "most_frequent"]:
-                raise ValueError(
-                    f"Got categories={self.categories}, but expected "
-                    "any of {'auto', 'k-means', 'most_frequent'}. "
-                )
-        if categories in ["k-means", "most_frequent"] and (
-            n_prototypes is None or n_prototypes == 0
-        ):
-            raise ValueError(
-                "n_prototypes expected None or a positive non null integer. "
-            )
-        if categories == "auto" and n_prototypes is not None:
-            warnings.warn('n_prototypes parameter ignored with category type "auto". ')
-
-    def get_most_frequent(self, prototypes: List[str]) -> np.array:
-        """
-        Get the most frequent category prototypes.
-
-        Parameters
-        ----------
-        prototypes : list of str
-            The list of values for a category variable.
-
-        Returns
-        -------
-        np.array
-            The n_prototypes most frequent values for a category variable.
-        """
-        values, _ = get_prototype_frequencies(prototypes)
-        return values[: self.n_prototypes]
-
-    def fit(self, X, y=None) -> "SimilarityEncoder":
-        """
-        Fit the instance to X.
-
-        Parameters
-        ----------
-        X : array-like, shape [n_samples, n_features]
-            The data to determine the categories of each feature.
-        y : None
-            Unused, only here for compatibility.
-
-        Returns
-        -------
-        :class:`~dirty_cat.SimilarityEncoder`
-            The fitted :class:`~dirty_cat.SimilarityEncoder` instance (self).
-        """
-
-        if self.handle_missing not in ["error", ""]:
-            raise ValueError(
-                f"Got handle_missing={self.handle_missing}, but expected "
-                "any of {'error', ''}. "
-            )
-        if hasattr(X, "iloc") and X.isna().values.any():
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='' to encode with missing values. "
-                )
-            else:
-                X = X.fillna(self.handle_missing)
-        elif not hasattr(X, "dtype") and isinstance(X, list):
-            X = np.asarray(X, dtype=object)
-
-        if hasattr(X, "dtype"):
-            mask = _object_dtype_isnan(X)
-            if X.dtype.kind == "O" and mask.any():
-                if self.handle_missing == "error":
-                    raise ValueError(
-                        "Found missing values in input data; set "
-                        "handle_missing='' to encode with missing values. "
-                    )
-                else:
-                    X[mask] = self.handle_missing
-
-        Xlist, n_samples, n_features = self._check_X(X)
-        self.n_features_in_ = n_features
-
-        if self.handle_unknown not in ["error", "ignore"]:
-            raise ValueError(
-                f"Got handle_unknown={self.handle_unknown!r}, but expected "
-                "any of {'error', 'ignore'}. "
-            )
-
-        if (self.hashing_dim is not None) and (not isinstance(self.hashing_dim, int)):
-            raise ValueError(
-                f"Got hashing_dim={self.hashing_dim!r}, which has an invalid "
-                f"type ({type(self.hashing_dim)}), expected None or int. "
-            )
-
-        if self.categories not in ["auto", "most_frequent", "k-means"]:
-            for cats in self.categories:
-                if not np.all(np.sort(cats) == np.array(cats)):
-                    raise ValueError("Unsorted categories are not yet supported. ")
-
-        self.categories_ = list()
-        self.random_state_ = check_random_state(self.random_state)
-
-        for i in range(n_features):
-            Xi = Xlist[i]
-            if self.categories == "auto":
-                self.categories_.append(np.unique(Xi))
-            elif self.categories == "most_frequent":
-                self.categories_.append(self.get_most_frequent(Xi))
-            elif self.categories == "k-means":
-                uniques, count = np.unique(Xi, return_counts=True)
-                self.categories_.append(
-                    get_kmeans_prototypes(
-                        uniques,
-                        self.n_prototypes,
-                        sample_weight=count,
-                        random_state=self.random_state_,
-                    )
-                )
-            else:
-                if self.handle_unknown == "error":
-                    valid_mask = np.in1d(Xi, self.categories[i])
-                    if not np.all(valid_mask):
-                        diff = np.unique(Xi[~valid_mask])
-                        raise ValueError(
-                            f"Found unknown categories {diff} in column {i} "
-                            "during fit. "
-                        )
-                self.categories_.append(np.array(self.categories[i], dtype=object))
-
-        self.vectorizers_ = []
-        self.vocabulary_count_matrices_ = []
-        self.vocabulary_ngram_counts_ = []
-
-        for i in range(n_features):
-            vectorizer = CountVectorizer(
-                analyzer="char",
-                ngram_range=self.ngram_range,
-                dtype=self.dtype,
-                strip_accents=None,
-            )
-
-            # Store the raw-categories (and not the preprocessed
-            # categories) but use the preprocessed categories to compute
-            # the stored count_matrices. This done to preserve the
-            # equivalency between the user input and the categories_
-            # attribute of the SimilarityEncoder, while being compliant
-            # with the CountVectorizer preprocessing steps.
-            categories = self.categories_[i]
-
-            self.vectorizers_.append(vectorizer)
-
-            self.vocabulary_count_matrices_.append(
-                vectorizer.fit_transform(
-                    [preprocess(category) for category in categories]
-                )
-            )
-
-            self.vocabulary_ngram_counts_.append(
-                [
-                    get_ngram_count(preprocess(category), self.ngram_range)
-                    for category in categories
-                ]
-            )
-
-        self.drop_idx_ = self._compute_drop_idx()
-        if parse_version(sklearn.__version__) >= parse_version("1.1.0"):
-            self._infrequent_enabled = False
-
-        return self
-
-    def transform(self, X, fast: bool = True) -> np.array:
-        """
-        Transform X using specified encoding scheme.
-
-        Parameters
-        ----------
-        X : array-like, shape [n_samples, n_features]
-            The data to encode.
-        fast : bool
-            Whether to use the fast computation of ngrams.
-
-        Returns
-        -------
-        X_new : 2-d array, shape [n_samples, n_features_new]
-            Transformed input.
-        """
-        check_is_fitted(self, "categories_")
-        if hasattr(X, "iloc") and X.isna().values.any():
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='' to encode with missing values. "
-                )
-            else:
-                X = X.fillna(self.handle_missing)
-        elif not hasattr(X, "dtype") and isinstance(X, list):
-            X = np.asarray(X, dtype=object)
-
-        if hasattr(X, "dtype"):
-            mask = _object_dtype_isnan(X)
-            if X.dtype.kind == "O" and mask.any():
-                if self.handle_missing == "error":
-                    raise ValueError(
-                        "Found missing values in input data; set "
-                        "handle_missing='' to encode with missing values. "
-                    )
-                else:
-                    X[mask] = self.handle_missing
-
-        Xlist, n_samples, n_features = self._check_X(X)
-
-        for i in range(n_features):
-            Xi = Xlist[i]
-            valid_mask = np.in1d(Xi, self.categories_[i])
-
-            if not np.all(valid_mask):
-                if self.handle_unknown == "error":
-                    diff = np.unique(X[~valid_mask, i])
-                    raise ValueError(
-                        f"Found unknown categories {diff} in column {i} during fit. "
-                    )
-
-        min_n, max_n = self.ngram_range
-
-        total_length = sum(len(x) for x in self.categories_)
-        out = np.empty((len(X), total_length), dtype=self.dtype)
-        last = 0
-        for j, categories in enumerate(self.categories_):
-            if fast:
-                encoded_Xj = self._ngram_similarity_fast(Xlist[j], j)
-            else:
-                encoded_Xj = ngram_similarity_matrix(
-                    Xlist[j],
-                    categories,
-                    ngram_range=(min_n, max_n),
-                    hashing_dim=self.hashing_dim,
-                    dtype=np.float32,
-                )
-
-            out[:, last : last + len(categories)] = encoded_Xj
-            last += len(categories)
-        return out
-
-    def _ngram_similarity_fast(
-        self,
-        X: Union[list, np.array],
-        col_idx: int,
-    ) -> np.array:
-        """
-        Fast computation of ngram similarity.
-
-        :func:`~dirty_cat.SimilarityEncoder.transform` uses the count vectors
-        of the vocabulary in its computations.
-        In `ngram_similarity`, these count vectors have to be
-        re-computed each time, which can slow down the execution. In this
-        method, the count vectors are recovered from
-        :attr:`~dirty_cat.SimilarityEncoder.vocabulary_count_matrices`,
-        speeding up the execution.
-
-        Parameters
-        ----------
-        X : list or :obj:`numpy.ndarray`
-            Observations being transformed.
-        col_idx : int
-            The column index of X in the original feature matrix.
-        """
-        vectorizer = self.vectorizers_[col_idx]
-
-        unq_X = np.unique(X)
-        unq_X_ = np.array([preprocess(x) for x in unq_X])
-
-        X_count_matrix = vectorizer.transform(unq_X_)
-        vocabulary_count_matrix = self.vocabulary_count_matrices_[col_idx]
-        vocabulary_ngram_count = np.array(
-            self.vocabulary_ngram_counts_[col_idx]
-        ).reshape(-1, 1)
-
-        se_dict = {}
-
-        Parallel(n_jobs=self.n_jobs, backend="threading")(
-            delayed(_ngram_similarity_one_sample_inplace)(
-                X_count_vector,
-                vocabulary_count_matrix,
-                x_str,
-                vocabulary_ngram_count,
-                se_dict,
-                unq_X,
-                i,
-                self.ngram_range,
-            )
-            for X_count_vector, x_str, i in zip(
-                X_count_matrix, unq_X_, range(len(unq_X))
-            )
-        )
-
-        out = np.empty(
-            (len(X), vocabulary_count_matrix.shape[0]),
-            dtype=self.dtype,
-        )
-
-        for x, out_row in zip(X, out):
-            out_row[:] = se_dict[x]
-
-        return np.nan_to_num(out, copy=False)
-
-    def fit_transform(self, X, y=None, **fit_params) -> np.array:
-        """
-        Fit SimilarityEncoder to data, then transform it.
-        Fits transformer to `X` and `y` with optional parameters
-        `fit_params` and returns a transformed version of `X`.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            Target values (None for unsupervised transformations).
-        **fit_params
-            Additional fit parameters.
-
-        Returns
-        -------
-        array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        if y is None:
-            # fit method of arity 1 (unsupervised transformation)
-            return self.fit(X, **fit_params).transform(X)
-        else:
-            # fit method of arity 2 (supervised transformation)
-            return self.fit(X, y, **fit_params).transform(X)
+"""
+Similarity encoding of string arrays.
+The principle is as follows:
+    1. Given an input string array X = [x1, ..., xn] with k unique categories
+       [c1, ..., ck] and a similarity measure sim(s1, s2) between strings,
+       we define the encoded vector of xi as [sim(xi, c1), ... , sim(xi, ck)].
+       Similarity encoding of X results in a matrix with shape (n, k) that
+       captures morphological similarities between string entries.
+    2. To avoid dealing with high-dimensional encodings when k is high, we can
+       use d << k prototypes [p1, ..., pd] with which similarities will be
+       computed:  xi -> [sim(xi, p1), ..., sim(xi, pd)]. These prototypes can
+       be automatically sampled from the input data (most frequent categories,
+       KMeans) or provided by the user.
+"""
+
+import warnings
+from typing import List, Literal, Optional, Tuple, Union
+
+import numpy as np
+import sklearn
+from joblib import Parallel, delayed
+from numpy.random import RandomState
+from scipy import sparse
+from sklearn.cluster import KMeans
+from sklearn.feature_extraction.text import CountVectorizer, HashingVectorizer
+from sklearn.neighbors import NearestNeighbors
+from sklearn.preprocessing import OneHotEncoder
+from sklearn.utils import check_random_state
+from sklearn.utils.fixes import _object_dtype_isnan
+from sklearn.utils.validation import check_is_fitted
+
+from ._string_distances import get_ngram_count, preprocess
+from ._utils import parse_version
+
+
+def _ngram_similarity_one_sample_inplace(
+    x_count_vector: np.ndarray,
+    vocabulary_count_matrix: np.ndarray,
+    str_x: str,
+    vocabulary_ngram_counts: np.ndarray,
+    se_dict: dict,
+    unq_X: np.ndarray,
+    i: int,
+    ngram_range: Tuple[int, int],
+) -> None:
+    """
+    Update inplace a dict of similarities between a string and a vocabulary
+
+    Parameters
+    ----------
+    x_count_vector : np.ndarray
+        Count vector of the sample based on the ngrams of the vocabulary
+    vocabulary_count_matrix : np.ndarray
+        Count vector of the vocabulary based on its ngrams
+    str_x: str
+        The actual sample string
+    vocabulary_ngram_counts : np.ndarray
+        Number of ngrams for each unique element of the vocabulary
+    se_dict : dict
+        Dictionary containing the similarities for each x in unq_X
+    unq_X : np.ndarray
+        The arrays of all unique samples
+    i : str
+        The index of x_count_vector in the csr count matrix
+    ngram_range : tuple
+        n-grams to use for the decomposition, where ``n_min <= n <= n_max``.
+    """
+    nonzero_idx = x_count_vector.indices
+    nonzero_vals = x_count_vector.data
+
+    same_grams = np.asarray(
+        (vocabulary_count_matrix[:, nonzero_idx].minimum(nonzero_vals)).sum(axis=1)
+    )
+
+    all_grams = (
+        get_ngram_count(str_x, ngram_range) + vocabulary_ngram_counts - same_grams
+    )
+    similarity = np.divide(
+        same_grams, all_grams, out=np.zeros_like(same_grams), where=all_grams != 0
+    )
+    se_dict[unq_X[i]] = similarity.reshape(-1)
+
+
+def ngram_similarity_matrix(
+    X,
+    cats: List[str],
+    ngram_range: Tuple[int, int],
+    hashing_dim: int,
+    dtype: type = np.float64,
+) -> np.ndarray:
+    """
+    Similarity encoding for dirty categorical variables:
+    Given two arrays of strings, returns the similarity encoding matrix
+    of size len(X) x len(cats)
+
+    ngram_sim(s_i, s_j) =
+        ||min(ci, cj)||_1 / (||ci||_1 + ||cj||_1 - ||min(ci, cj)||_1)
+    """
+    min_n, max_n = ngram_range
+    unq_X = np.unique(X)
+    cats = np.array([" %s " % cat for cat in cats])
+    unq_X_ = np.array([" %s " % x for x in unq_X])
+    if not hashing_dim:
+        vectorizer = CountVectorizer(
+            analyzer="char", ngram_range=(min_n, max_n), dtype=dtype
+        )
+        vectorizer.fit(np.concatenate((cats, unq_X_)))
+    else:
+        vectorizer = HashingVectorizer(
+            analyzer="char",
+            ngram_range=(min_n, max_n),
+            n_features=hashing_dim,
+            norm=None,
+            alternate_sign=False,
+            dtype=dtype,
+        )
+        vectorizer.fit(X)
+    count_cats = vectorizer.transform(cats)
+    count_X = vectorizer.transform(unq_X_)
+    # We don't need the vectorizer anymore, delete it to save memory
+    del vectorizer
+    sum_cats = np.asarray(count_cats.sum(axis=1))
+    SE_dict = {}
+
+    for i, x in enumerate(count_X):
+        _, nonzero_idx, nonzero_vals = sparse.find(x)
+        same_grams = np.asarray(
+            (count_cats[:, nonzero_idx].minimum(nonzero_vals)).sum(axis=1)
+        )
+        all_grams = x.sum() + sum_cats - same_grams
+        similarity = np.divide(same_grams, all_grams)
+        SE_dict[unq_X[i]] = similarity.reshape(-1)
+    # We don't need the counts anymore, delete them to save memory
+    del count_cats, count_X
+
+    out = np.empty((len(X), similarity.size), dtype=dtype)
+    for x, out_row in zip(X, out):
+        out_row[:] = SE_dict[x]
+
+    return np.nan_to_num(out, copy=False)
+
+
+def get_prototype_frequencies(prototypes: np.ndarray) -> np.ndarray:
+    """
+    Computes the frequencies of the values contained in prototypes
+    Reverse sorts the array by the frequency
+    Returns a numpy array of the values without their frequencies
+    """
+    uniques, counts = np.unique(prototypes, return_counts=True)
+    sorted_indexes = np.argsort(counts)[::-1]
+    return uniques[sorted_indexes], counts[sorted_indexes]
+
+
+def get_kmeans_prototypes(
+    X,
+    n_prototypes: int,
+    hashing_dim: int = 128,
+    ngram_range: Tuple[int, int] = (3, 3),
+    sparse: bool = False,
+    sample_weight=None,
+    random_state: Optional[Union[int, RandomState]] = None,
+) -> np.ndarray:
+    """
+    Computes prototypes based on:
+      - dimensionality reduction (via hashing n-grams)
+      - k-means clustering
+      - nearest neighbor
+    """
+    vectorizer = HashingVectorizer(
+        analyzer="char",
+        norm=None,
+        alternate_sign=False,
+        ngram_range=ngram_range,
+        n_features=hashing_dim,
+    )
+    projected = vectorizer.transform(X)
+    if not sparse:
+        projected = projected.toarray()
+    kmeans = KMeans(n_clusters=n_prototypes, random_state=random_state)
+    kmeans.fit(projected, sample_weight=sample_weight)
+    centers = kmeans.cluster_centers_
+    neighbors = NearestNeighbors()
+    neighbors.fit(projected)
+    indexes_prototypes = np.unique(neighbors.kneighbors(centers, 1)[-1])
+    if indexes_prototypes.shape[0] < n_prototypes:
+        warnings.warn(
+            "Final number of unique prototypes is lower than "
+            + "n_prototypes (expected). "
+        )
+    return np.sort(X[indexes_prototypes])
+
+
+class SimilarityEncoder(OneHotEncoder):
+    """
+    Encode string categorical features as a numeric array.
+
+    The input to this transformer should be an array-like of strings.
+    The method is based on calculating the morphological similarities
+    between the categories.
+    This encoding is an alternative to
+    :class:`~sklearn.preprocessing.OneHotEncoder` for dirty categorical variables.
+
+    Parameters
+    ----------
+    similarity : None
+        Deprecated in dirty_cat 0.3, will be removed in 0.5.
+        Was used to specify the type of pairwise string similarity to use.
+        Since 0.3, only the ngram similarity is supported.
+    ngram_range : int 2-tuple (min_n, max_n), default=(2, 4)
+        The range of values for the n_gram similarity.
+    categories : {"auto", "k-means", "most_frequent"} or list of list of str
+        Categories (unique values) per feature:
+
+        - 'auto' : Determine categories automatically from the training data.
+        - list : ``categories[i]`` holds the categories expected in the i-th
+          column. The passed categories must be sorted and should not mix
+          strings and numeric values.
+        - 'most_frequent' : Computes the most frequent values for every
+           categorical variable
+        - 'k-means' : Computes the K nearest neighbors of K-mean centroids
+           in order to choose the prototype categories
+
+        The categories used can be found in the
+        :attr:`~SimilarityEncoder.categories_` attribute.
+    dtype : number type, default :obj:`~numpy.float64`, optional
+        Desired dtype of output.
+    handle_unknown : 'error' or 'ignore', default='', optional
+        Whether to raise an error or ignore if an unknown categorical feature
+        is present during transform (default is to ignore). When this parameter
+        is set to 'ignore' and an unknown category is encountered during
+        transform, the resulting encoded columns for this feature
+        will be all zeros. In the inverse transform, an unknown category
+        will be denoted as None.
+    handle_missing : 'error' or '', default='', optional
+        Whether to raise an error or impute with blank string '' if missing
+        values (NaN) are present during fit (default is to impute).
+        When this parameter is set to '', and a missing value is encountered
+        during fit_transform, the resulting encoded columns for this feature
+        will be all zeros. In the inverse transform, the missing category
+        will be denoted as None.
+    hashing_dim : int or None, optional
+        If None, the base vectorizer is
+        :class:`~sklearn.feature_extraction.text.CountVectorizer`,
+        else it's set to
+        :class:`~sklearn.feature_extraction.text.HashingVectorizer`
+        with a number of features equal to `hashing_dim`.
+    n_prototypes : int, optional
+        Useful when `most_frequent` or `k-means` is used.
+        Must be a positive non-null integer.
+    random_state : int, RandomState or None, optional
+        Useful when `k-means` strategy is used.
+    n_jobs : int, optional
+        Maximum number of processes used to compute similarity matrices. Used
+        only if `fast=True` in :func:`~SimilarityEncoder.transform`.
+
+    Attributes
+    ----------
+    categories_ : list of :obj:`~numpy.ndarray`
+        The categories of each feature determined during fitting
+        (in the same order as the output of :func:`~SimilarityEncoder.transform`).
+
+    See Also
+    --------
+    :class:`~dirty_cat.MinHashEncoder` :
+        Encode string columns as a numeric array with the minhash method.
+    :class:`~dirty_cat.GapEncoder` :
+        Encodes dirty categories (strings) by constructing latent topics
+        with continuous encoding.
+    :class:`~dirty_cat.deduplicate` :
+        Deduplicate data by hierarchically clustering similar strings.
+
+    Notes
+    -----
+    The functionality of :class:`~SimilarityEncoder` is easy to explain
+    and understand, but it is not scalable.
+    Instead, the :class:`~dirty_cat.GapEncoder` is usually recommended.
+
+    References
+    ----------
+
+    For a detailed description of the method, see
+    `Similarity encoding for learning with dirty categorical variables
+    <https://hal.inria.fr/hal-01806175>`_ by Cerda, Varoquaux, Kegl. 2018
+    (Machine Learning journal, Springer).
+
+    Examples
+    --------
+    >>> enc = SimilarityEncoder()
+    >>> X = [['Male', 1], ['Female', 3], ['Female', 2]]
+    >>> enc.fit(X)
+    SimilarityEncoder()
+
+    It inherits the same methods as the
+    :class:`~sklearn.preprocessing.OneHotEncoder`:
+
+    >>> enc.categories_
+    [array(['Female', 'Male'], dtype=object), array([1, 2, 3], dtype=object)]
+
+    But it provides a continuous encoding based on similarity
+    instead of a discrete one based on exact matches:
+
+    >>> enc.transform([['Female', 1], ['Male', 4]])
+    array([[1., 0.42857143, 1., 0., 0.],
+           [0.42857143, 1., 0. , 0. , 0.]])
+
+    >>> enc.inverse_transform(
+    >>>     [[1., 0.42857143, 1., 0., 0.], [0.42857143, 1., 0. , 0. , 0.]]
+    >>> )
+    array([['Female', 1],
+           ['Male', None]], dtype=object)
+
+    >>> enc.get_feature_names_out(['gender', 'group'])
+    array(['gender_Female', 'gender_Male', 'group_1', 'group_2', 'group_3'], ...)
+    """
+
+    categories_: List[np.ndarray]
+    n_features_in_: int
+    random_state_: Union[int, RandomState]
+    drop_idx_: np.ndarray
+    vectorizers_: List[CountVectorizer]
+    vocabulary_count_matrices_: List[np.ndarray]
+    vocabulary_ngram_counts_: List[List[int]]
+    _infrequent_enabled: bool
+
+    def __init__(
+        self,
+        similarity: str = None,
+        ngram_range: Tuple[int, int] = (2, 4),
+        categories: Union[
+            Literal["auto", "k-means", "most_frequent"], List[List[str]]
+        ] = "auto",
+        dtype: type = np.float64,
+        handle_unknown: Literal["error", "ignore"] = "ignore",
+        handle_missing: Literal["error", ""] = "",
+        hashing_dim: Optional[int] = None,
+        n_prototypes: Optional[int] = None,
+        random_state: Optional[Union[int, RandomState]] = None,
+        n_jobs: Optional[int] = None,
+    ):
+        super().__init__()
+        self.categories = categories
+        self.dtype = dtype
+        self.handle_unknown = handle_unknown
+        self.handle_missing = handle_missing
+        self.ngram_range = ngram_range
+        self.hashing_dim = hashing_dim
+        self.n_prototypes = n_prototypes
+        self.random_state = random_state
+        self.n_jobs = n_jobs
+
+        if similarity is not None:
+            warnings.warn(
+                'The "similarity" argument is deprecated since dirty_cat 0.3, '
+                "and will be removed in 0.5."
+                "The n-gram similarity is the only one currently supported. ",
+                category=UserWarning,
+                stacklevel=2,
+            )
+        self.similarity = None
+
+        if not isinstance(categories, list):
+            if categories not in ["auto", "k-means", "most_frequent"]:
+                raise ValueError(
+                    f"Got categories={self.categories}, but expected "
+                    "any of {'auto', 'k-means', 'most_frequent'}. "
+                )
+        if categories in ["k-means", "most_frequent"] and (
+            n_prototypes is None or n_prototypes == 0
+        ):
+            raise ValueError(
+                "n_prototypes expected None or a positive non null integer. "
+            )
+        if categories == "auto" and n_prototypes is not None:
+            warnings.warn('n_prototypes parameter ignored with category type "auto". ')
+
+    def get_most_frequent(self, prototypes: List[str]) -> np.ndarray:
+        """
+        Get the most frequent category prototypes.
+
+        Parameters
+        ----------
+        prototypes : list of str
+            The list of values for a category variable.
+
+        Returns
+        -------
+        :obj:`~numpy.ndarray`
+            The n_prototypes most frequent values for a category variable.
+        """
+        values, _ = get_prototype_frequencies(prototypes)
+        return values[: self.n_prototypes]
+
+    def fit(self, X, y=None) -> "SimilarityEncoder":
+        """
+        Fit the instance to X.
+
+        Parameters
+        ----------
+        X : array-like, shape [n_samples, n_features]
+            The data to determine the categories of each feature.
+        y : None
+            Unused, only here for compatibility.
+
+        Returns
+        -------
+        :class:`~dirty_cat.SimilarityEncoder`
+            The fitted :class:`~dirty_cat.SimilarityEncoder` instance (self).
+        """
+
+        if self.handle_missing not in ["error", ""]:
+            raise ValueError(
+                f"Got handle_missing={self.handle_missing}, but expected "
+                "any of {'error', ''}. "
+            )
+        if hasattr(X, "iloc") and X.isna().values.any():
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='' to encode with missing values. "
+                )
+            else:
+                X = X.fillna(self.handle_missing)
+        elif not hasattr(X, "dtype") and isinstance(X, list):
+            X = np.asarray(X, dtype=object)
+
+        if hasattr(X, "dtype"):
+            mask = _object_dtype_isnan(X)
+            if X.dtype.kind == "O" and mask.any():
+                if self.handle_missing == "error":
+                    raise ValueError(
+                        "Found missing values in input data; set "
+                        "handle_missing='' to encode with missing values. "
+                    )
+                else:
+                    X[mask] = self.handle_missing
+
+        Xlist, n_samples, n_features = self._check_X(X)
+        self.n_features_in_ = n_features
+
+        if self.handle_unknown not in ["error", "ignore"]:
+            raise ValueError(
+                f"Got handle_unknown={self.handle_unknown!r}, but expected "
+                "any of {'error', 'ignore'}. "
+            )
+
+        if (self.hashing_dim is not None) and (not isinstance(self.hashing_dim, int)):
+            raise ValueError(
+                f"Got hashing_dim={self.hashing_dim!r}, which has an invalid "
+                f"type ({type(self.hashing_dim)}), expected None or int. "
+            )
+
+        if self.categories not in ["auto", "most_frequent", "k-means"]:
+            for cats in self.categories:
+                if not np.all(np.sort(cats) == np.array(cats)):
+                    raise ValueError("Unsorted categories are not yet supported. ")
+
+        self.categories_ = list()
+        self.random_state_ = check_random_state(self.random_state)
+
+        for i in range(n_features):
+            Xi = Xlist[i]
+            if self.categories == "auto":
+                self.categories_.append(np.unique(Xi))
+            elif self.categories == "most_frequent":
+                self.categories_.append(self.get_most_frequent(Xi))
+            elif self.categories == "k-means":
+                uniques, count = np.unique(Xi, return_counts=True)
+                self.categories_.append(
+                    get_kmeans_prototypes(
+                        uniques,
+                        self.n_prototypes,
+                        sample_weight=count,
+                        random_state=self.random_state_,
+                    )
+                )
+            else:
+                if self.handle_unknown == "error":
+                    valid_mask = np.in1d(Xi, self.categories[i])
+                    if not np.all(valid_mask):
+                        diff = np.unique(Xi[~valid_mask])
+                        raise ValueError(
+                            f"Found unknown categories {diff} in column {i} "
+                            "during fit. "
+                        )
+                self.categories_.append(np.array(self.categories[i], dtype=object))
+
+        self.vectorizers_ = []
+        self.vocabulary_count_matrices_ = []
+        self.vocabulary_ngram_counts_ = []
+
+        for i in range(n_features):
+            vectorizer = CountVectorizer(
+                analyzer="char",
+                ngram_range=self.ngram_range,
+                dtype=self.dtype,
+                strip_accents=None,
+            )
+
+            # Store the raw-categories (and not the preprocessed
+            # categories) but use the preprocessed categories to compute
+            # the stored count_matrices. This done to preserve the
+            # equivalency between the user input and the categories_
+            # attribute of the SimilarityEncoder, while being compliant
+            # with the CountVectorizer preprocessing steps.
+            categories = self.categories_[i]
+
+            self.vectorizers_.append(vectorizer)
+
+            self.vocabulary_count_matrices_.append(
+                vectorizer.fit_transform(
+                    [preprocess(category) for category in categories]
+                )
+            )
+
+            self.vocabulary_ngram_counts_.append(
+                [
+                    get_ngram_count(preprocess(category), self.ngram_range)
+                    for category in categories
+                ]
+            )
+
+        if parse_version(sklearn.__version__) >= parse_version("1.1.0"):
+            self._infrequent_enabled = False
+        if parse_version(sklearn.__version__) >= parse_version("1.2.2"):
+            self.drop_idx_ = self._set_drop_idx()
+        else:
+            self.drop_idx_ = self._compute_drop_idx()
+
+        return self
+
+    def transform(self, X, fast: bool = True) -> np.ndarray:
+        """
+        Transform X using specified encoding scheme.
+
+        Parameters
+        ----------
+        X : array-like, shape [n_samples, n_features]
+            The data to encode.
+        fast : bool
+            Whether to use the fast computation of ngrams.
+
+        Returns
+        -------
+        2-d :obj:`~numpy.ndarray`, shape [n_samples, n_features_new]
+            Transformed input.
+        """
+        check_is_fitted(self, "categories_")
+        if hasattr(X, "iloc") and X.isna().values.any():
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='' to encode with missing values. "
+                )
+            else:
+                X = X.fillna(self.handle_missing)
+        elif not hasattr(X, "dtype") and isinstance(X, list):
+            X = np.asarray(X, dtype=object)
+
+        if hasattr(X, "dtype"):
+            mask = _object_dtype_isnan(X)
+            if X.dtype.kind == "O" and mask.any():
+                if self.handle_missing == "error":
+                    raise ValueError(
+                        "Found missing values in input data; set "
+                        "handle_missing='' to encode with missing values. "
+                    )
+                else:
+                    X[mask] = self.handle_missing
+
+        Xlist, n_samples, n_features = self._check_X(X)
+
+        for i in range(n_features):
+            Xi = Xlist[i]
+            valid_mask = np.in1d(Xi, self.categories_[i])
+
+            if not np.all(valid_mask):
+                if self.handle_unknown == "error":
+                    diff = np.unique(X[~valid_mask, i])
+                    raise ValueError(
+                        f"Found unknown categories {diff} in column {i} during fit. "
+                    )
+
+        min_n, max_n = self.ngram_range
+
+        total_length = sum(len(x) for x in self.categories_)
+        out = np.empty((len(X), total_length), dtype=self.dtype)
+        last = 0
+        for j, categories in enumerate(self.categories_):
+            if fast:
+                encoded_Xj = self._ngram_similarity_fast(Xlist[j], j)
+            else:
+                encoded_Xj = ngram_similarity_matrix(
+                    Xlist[j],
+                    categories,
+                    ngram_range=(min_n, max_n),
+                    hashing_dim=self.hashing_dim,
+                    dtype=np.float32,
+                )
+
+            out[:, last : last + len(categories)] = encoded_Xj
+            last += len(categories)
+        return out
+
+    def _ngram_similarity_fast(
+        self,
+        X: Union[list, np.ndarray],
+        col_idx: int,
+    ) -> np.ndarray:
+        """
+        Fast computation of ngram similarity.
+
+        :func:`~dirty_cat.SimilarityEncoder.transform` uses the count vectors
+        of the vocabulary in its computations.
+        In `ngram_similarity`, these count vectors have to be
+        re-computed each time, which can slow down the execution. In this
+        method, the count vectors are recovered from
+        :attr:`~dirty_cat.SimilarityEncoder.vocabulary_count_matrices`,
+        speeding up the execution.
+
+        Parameters
+        ----------
+        X : list or :obj:`numpy.ndarray`
+            Observations being transformed.
+        col_idx : int
+            The column index of X in the original feature matrix.
+        """
+        vectorizer = self.vectorizers_[col_idx]
+
+        unq_X = np.unique(X)
+        unq_X_ = np.array([preprocess(x) for x in unq_X])
+
+        X_count_matrix = vectorizer.transform(unq_X_)
+        vocabulary_count_matrix = self.vocabulary_count_matrices_[col_idx]
+        vocabulary_ngram_count = np.array(
+            self.vocabulary_ngram_counts_[col_idx]
+        ).reshape(-1, 1)
+
+        se_dict = {}
+
+        Parallel(n_jobs=self.n_jobs, backend="threading")(
+            delayed(_ngram_similarity_one_sample_inplace)(
+                X_count_vector,
+                vocabulary_count_matrix,
+                x_str,
+                vocabulary_ngram_count,
+                se_dict,
+                unq_X,
+                i,
+                self.ngram_range,
+            )
+            for X_count_vector, x_str, i in zip(
+                X_count_matrix, unq_X_, range(len(unq_X))
+            )
+        )
+
+        out = np.empty(
+            (len(X), vocabulary_count_matrix.shape[0]),
+            dtype=self.dtype,
+        )
+
+        for x, out_row in zip(X, out):
+            out_row[:] = se_dict[x]
+
+        return np.nan_to_num(out, copy=False)
+
+    def fit_transform(self, X, y=None, **fit_params) -> np.ndarray:
+        """
+        Fit SimilarityEncoder to data, then transform it.
+        Fits transformer to `X` and `y` with optional parameters
+        `fit_params` and returns a transformed version of `X`.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            Target values (None for unsupervised transformations).
+        **fit_params
+            Additional fit parameters.
+
+        Returns
+        -------
+        array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        if y is None:
+            # fit method of arity 1 (unsupervised transformation)
+            return self.fit(X, **fit_params).transform(X)
+        else:
+            # fit method of arity 2 (supervised transformation)
+            return self.fit(X, y, **fit_params).transform(X)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_string_distances.py` & `dirty_cat-0.4.1/dirty_cat/_string_distances.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-"""
-Some string distances
-"""
-
-import re
-from collections import Counter
-from typing import Tuple
-
-# TODO vectorize these functions (accept arrays)
-
-
-def get_ngram_count(string: str, ngram_range: Tuple[int, int]) -> int:
-    """
-    Compute the number of ngrams in a string.
-
-    Here is where the formula comes from:
-
-    * the number of 3-grams in a string is the number of sliding windows of
-      size 3 in the string: len(string) - 3 + 1
-    * this can be generalized to n-grams by changing 3 by n.
-    * when given a ngram_range, we can sum this formula over all possible
-      ngrams
-
-    """
-    min_n, max_n = ngram_range
-    ngram_count = 0
-
-    for i in range(min_n, max_n + 1):
-        ngram_count += len(string) - i + 1
-
-    return ngram_count
-
-
-def preprocess(x: str) -> str:
-    """
-    Combine preprocessing done by CountVectorizer and the SimilarityEncoder.
-
-    Different methods exist to compute the number of ngrams in a string:
-
-    - Simply sum the values of a count vector, which is the output of a
-      CountVectorizer with analyzer="char", and a specific ngram_range
-    - Compute the number of ngrams using a formula (see ``get_ngram_count``)
-
-    However, in the first case, some preprocessing is done by the
-    CountVectorizer that may change the length of the string (in particular,
-    stripping sequences of 2 or more whitespaces into 1). In order for the two
-    methods to output similar results, this pre-processing is done upstream,
-    prior to the CountVectorizer.
-    """
-
-    # Preprocessing step done in ngram_similarity
-    x = f" {x} "
-
-    # Preprocessing step done in the CountVectorizer
-    _white_spaces = re.compile(r"\s\s+")
-
-    return _white_spaces.sub(" ", x)
-
-
-def get_unique_ngrams(string: str, ngram_range: Tuple[int, int]):
-    """
-    Return the set of unique n-grams of a string.
-
-    Parameters
-    ----------
-    string : str
-        The string to split in n-grams.
-    ngram_range : tuple (min_n, max_n)
-        The lower and upper boundary of the range of n-values for different
-        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
-
-    Returns
-    -------
-    set
-        The set of unique n-grams of the string.
-    """
-    spaces = " "  # * (n // 2 + n % 2)
-    string = spaces + " ".join(string.lower().split()) + spaces
-    ngram_set = set()
-    for n in range(ngram_range[0], ngram_range[1] + 1):
-        string_list = [string[i:] for i in range(n)]
-        ngram_set |= set(zip(*string_list))
-    return ngram_set
-
-
-def get_ngrams(string, n):
-    """Return the set of different tri-grams in a string"""
-    # Pure Python implementation: no numpy
-    spaces = " "  # * (n // 2 + n % 2)
-    string = spaces + " ".join(string.lower().split()) + spaces
-    string_list = [string[i:] for i in range(n)]
-    return list(zip(*string_list))
-
-
-def ngram_similarity(string1, string2, n, preprocess_strings=True):
-    """n-gram similarity between two strings"""
-    if preprocess_strings:
-        string1, string2 = preprocess(string1), preprocess(string2)
-
-    ngrams1 = get_ngrams(string1, n)
-    count1 = Counter(ngrams1)
-
-    ngrams2 = get_ngrams(string2, n)
-    count2 = Counter(ngrams2)
-
-    samegrams = sum((count1 & count2).values())
-    allgrams = len(ngrams1) + len(ngrams2)
-    similarity = samegrams / (allgrams - samegrams)
-    return similarity
-
-
-if __name__ == "__main__":
-    s1 = "aa"
-    s2 = "aaab"
-    print("3-gram similarity: %.3f" % ngram_similarity(s1, s2, 3))
+"""
+Some string distances
+"""
+
+import re
+from collections import Counter
+from typing import Tuple
+
+# TODO vectorize these functions (accept arrays)
+
+
+def get_ngram_count(string: str, ngram_range: Tuple[int, int]) -> int:
+    """
+    Compute the number of ngrams in a string.
+
+    Here is where the formula comes from:
+
+    * the number of 3-grams in a string is the number of sliding windows of
+      size 3 in the string: len(string) - 3 + 1
+    * this can be generalized to n-grams by changing 3 by n.
+    * when given a ngram_range, we can sum this formula over all possible
+      ngrams
+
+    """
+    min_n, max_n = ngram_range
+    ngram_count = 0
+
+    for i in range(min_n, max_n + 1):
+        ngram_count += len(string) - i + 1
+
+    return ngram_count
+
+
+def preprocess(x: str) -> str:
+    """
+    Combine preprocessing done by CountVectorizer and the SimilarityEncoder.
+
+    Different methods exist to compute the number of ngrams in a string:
+
+    - Simply sum the values of a count vector, which is the output of a
+      CountVectorizer with analyzer="char", and a specific ngram_range
+    - Compute the number of ngrams using a formula (see ``get_ngram_count``)
+
+    However, in the first case, some preprocessing is done by the
+    CountVectorizer that may change the length of the string (in particular,
+    stripping sequences of 2 or more whitespaces into 1). In order for the two
+    methods to output similar results, this pre-processing is done upstream,
+    prior to the CountVectorizer.
+    """
+
+    # Preprocessing step done in ngram_similarity
+    x = f" {x} "
+
+    # Preprocessing step done in the CountVectorizer
+    _white_spaces = re.compile(r"\s\s+")
+
+    return _white_spaces.sub(" ", x)
+
+
+def get_unique_ngrams(string: str, ngram_range: Tuple[int, int]):
+    """
+    Return the set of unique n-grams of a string.
+
+    Parameters
+    ----------
+    string : str
+        The string to split in n-grams.
+    ngram_range : tuple (min_n, max_n)
+        The lower and upper boundary of the range of n-values for different
+        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
+
+    Returns
+    -------
+    set
+        The set of unique n-grams of the string.
+    """
+    spaces = " "  # * (n // 2 + n % 2)
+    string = spaces + " ".join(string.lower().split()) + spaces
+    ngram_set = set()
+    for n in range(ngram_range[0], ngram_range[1] + 1):
+        string_list = [string[i:] for i in range(n)]
+        ngram_set |= set(zip(*string_list))
+    return ngram_set
+
+
+def get_ngrams(string, n):
+    """Return the set of different tri-grams in a string"""
+    # Pure Python implementation: no numpy
+    spaces = " "  # * (n // 2 + n % 2)
+    string = spaces + " ".join(string.lower().split()) + spaces
+    string_list = [string[i:] for i in range(n)]
+    return list(zip(*string_list))
+
+
+def ngram_similarity(string1, string2, n, preprocess_strings=True):
+    """n-gram similarity between two strings"""
+    if preprocess_strings:
+        string1, string2 = preprocess(string1), preprocess(string2)
+
+    ngrams1 = get_ngrams(string1, n)
+    count1 = Counter(ngrams1)
+
+    ngrams2 = get_ngrams(string2, n)
+    count2 = Counter(ngrams2)
+
+    samegrams = sum((count1 & count2).values())
+    allgrams = len(ngrams1) + len(ngrams2)
+    similarity = samegrams / (allgrams - samegrams)
+    return similarity
+
+
+if __name__ == "__main__":
+    s1 = "aa"
+    s2 = "aaab"
+    print("3-gram similarity: %.3f" % ngram_similarity(s1, s2, 3))
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_target_encoder.py` & `dirty_cat-0.4.1/dirty_cat/_target_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,311 +1,320 @@
-import collections
-from typing import Dict, List, Literal, Union
-
-import numpy as np
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.preprocessing import LabelEncoder
-from sklearn.utils import check_array
-from sklearn.utils.fixes import _object_dtype_isnan
-from sklearn.utils.validation import check_is_fitted
-
-from dirty_cat._utils import check_input
-
-
-def lambda_(x, n):
-    return x / (x + n)
-
-
-class TargetEncoder(BaseEstimator, TransformerMixin):
-    """Encode categorical features as a numeric array given a target vector.
-
-    Each category is encoded given the effect that it has in the
-    target variable y. The method considers that categorical
-    variables can present rare categories. It represents each category by the
-    probability of y conditional on this category.
-    In addition, it takes an empirical Bayes approach to shrink the estimate.
-
-
-    Parameters
-    ----------
-    categories : typing.Union[typing.Literal["auto"], typing.List[typing.List[typing.Union[str, int]]]  # noqa
-        Categories (unique values) per feature:
-
-        - 'auto' : Determine categories automatically from the training data.
-        - list : ``categories[i]`` holds the categories expected in the i-th
-          column. The passed categories must be sorted and should not mix
-          strings and numeric values.
-
-        The categories used can be found in the ``categories_`` attribute.
-    clf_type : typing.Literal["regression", "binary-clf", "multiclass-clf"]
-        The type of classification/regression problem.
-    dtype : type, default=np.float64
-        Desired dtype of output.
-    handle_unknown : typing.Literal["error", "ignore"], default="error"
-        Whether to raise an error or ignore if a unknown categorical feature is
-        present during transform (default is to raise). When this parameter
-        is set to 'ignore' and an unknown category is encountered during
-        transform, the encoded columns for this feature
-        will be assigned the prior mean of the target variable.
-    handle_missing : typing.Literal["error", ""], default=""
-        Whether to raise an error or impute with blank string '' if missing
-        values (NaN) are present during fit (default is to impute).
-        When this parameter is set to '', and a missing value is encountered
-        during fit_transform, the resulting encoded columns for this feature
-        will be all zeros.
-
-    Attributes
-    ----------
-    n_features_in_: int
-        Number of features in the data seen during fit.
-    categories_ : typing.List[np.ndarray]
-        The categories of each feature determined during fitting
-        (in order corresponding with output of ``transform``).
-
-    References
-    ----------
-    For more details, see Micci-Barreca, 2001: A preprocessing scheme for
-    high-cardinality categorical attributes in classification and prediction
-    problems.
-
-    Examples
-    --------
-    >>> enc = TargetEncoder(handle_unknown='ignore')
-    >>> X = [['male'], ['Male'], ['Female'], ['male'], ['Female']]
-    >>> y = np.array([1, 2, 3, 4, 5])
-
-    >>> enc.fit(X, y)
-    TargetEncoder(handle_unknown='ignore')
-
-    The encoder has found the following categories:
-
-    >>> enc.categories_
-    [array(['Female', 'Male', 'male'], dtype='<U6')]
-
-    We will encode the following categories, of which the first two are unknown :
-
-    >>> X2 = [['MALE'], ['FEMALE'], ['Female'], ['male'], ['Female']]
-
-    >>> enc.transform(X2)
-    array([[3.        ],
-        [3.        ],
-        [3.54545455],
-        [2.72727273],
-        [3.54545455]])
-
-    As expected, they were encoded according to their influence on y.
-    The unknown categories were assigned the mean of the target variable.
-
-    """
-
-    n_features_in_: int
-    _label_encoders_: List[LabelEncoder]
-    categories_: List[np.ndarray]
-    n_: int
-
-    def __init__(
-        self,
-        categories: Union[Literal["auto"], List[Union[List[str], np.ndarray]]] = "auto",
-        clf_type: Literal["regression", "binary-clf", "multiclass-clf"] = "binary-clf",
-        dtype: type = np.float64,
-        handle_unknown: Literal["error", "ignore"] = "error",
-        handle_missing: Literal["error", ""] = "",
-    ):
-        self.categories = categories
-        self.dtype = dtype
-        self.clf_type = clf_type
-        self.handle_unknown = handle_unknown
-        self.handle_missing = handle_missing
-
-    def _more_tags(self) -> Dict[str, List[str]]:
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def fit(self, X, y) -> "TargetEncoder":
-        """
-        Fit the instance to X.
-
-        Parameters
-        ----------
-        X : array-like, shape [n_samples, n_features]
-            The data to determine the categories of each feature.
-        y : array
-            The associated target vector.
-
-        Returns
-        -------
-        :class:`~dirty_cat.TargetEncoder`
-            Fitted :class:`~dirty_cat.TargetEncoder` instance (self).
-        """
-        X = check_input(X)
-        self.n_features_in_ = X.shape[1]
-        if self.handle_missing not in ["error", ""]:
-            raise ValueError(
-                f"Got handle_missing={self.handle_missing!r}, but expected "
-                "any of {'error', ''}. "
-            )
-
-        mask = _object_dtype_isnan(X)
-        if mask.any():
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='' to encode with missing values. "
-                )
-            else:
-                X[mask] = self.handle_missing
-
-        if self.handle_unknown not in ["error", "ignore"]:
-            raise ValueError(
-                f"Got handle_unknown={self.handle_unknown!r}, but expected "
-                'any of {"error", "ignore"}. '
-            )
-
-        if self.categories != "auto":
-            for cats in self.categories:
-                if not np.all(np.sort(cats) == np.array(cats)):
-                    raise ValueError("Unsorted categories are not yet supported. ")
-
-        X_temp = check_array(X, dtype=None)
-        X = X_temp
-
-        n_samples, n_features = X.shape
-
-        self._label_encoders_ = [LabelEncoder() for _ in range(n_features)]
-
-        for j in range(n_features):
-            le = self._label_encoders_[j]
-            Xj = X[:, j]
-            if self.categories == "auto":
-                le.fit(Xj)
-            else:
-                if self.handle_unknown == "error":
-                    valid_mask = np.in1d(Xj, self.categories[j])
-                    if not np.all(valid_mask):
-                        diff = np.unique(Xj[~valid_mask])
-                        raise ValueError(
-                            f"Found unknown categories {diff} in column {j} during fit"
-                        )
-                le.classes_ = np.array(self.categories[j])
-
-        self.categories_ = [le.classes_ for le in self._label_encoders_]
-        self.n_ = len(y)
-        if self.clf_type in ["binary-clf", "regression"]:
-            self.Eyx_ = [
-                {cat: np.mean(y[X[:, j] == cat]) for cat in self.categories_[j]}
-                for j in range(len(self.categories_))
-            ]
-            self.Ey_ = np.mean(y)
-            self.counter_ = {j: collections.Counter(X[:, j]) for j in range(n_features)}
-        if self.clf_type in ["multiclass-clf"]:
-            self.classes_ = np.unique(y)
-
-            self.Eyx_ = {
-                c: [
-                    {
-                        cat: np.mean((y == c)[X[:, j] == cat])
-                        for cat in self.categories_[j]
-                    }
-                    for j in range(len(self.categories_))
-                ]
-                for c in self.classes_
-            }
-            self.Ey_ = {c: np.mean(y == c) for c in self.classes_}
-            self.counter_ = {j: collections.Counter(X[:, j]) for j in range(n_features)}
-        self.k_ = {j: len(self.counter_[j]) for j in self.counter_}
-        return self
-
-    def transform(self, X) -> np.ndarray:
-        """
-        Transform X using the specified encoding scheme.
-
-        Parameters
-        ----------
-        X : array-like, shape [n_samples, n_features_new]
-            The data to encode.
-
-        Returns
-        -------
-        2-d :class:`~numpy.ndarray`
-            Transformed input.
-        """
-        check_is_fitted(self, attributes=["n_features_in_"])
-        X = check_input(X)
-        if X.shape[1] != self.n_features_in_:
-            raise ValueError(
-                f"The number of features in the input data ({X.shape[1]}) "
-                "does not match the number of features "
-                f"seen during fit ({self.n_features_in_})."
-            )
-        mask = _object_dtype_isnan(X)
-        if mask.any():
-            if self.handle_missing == "error":
-                raise ValueError(
-                    "Found missing values in input data; set "
-                    "handle_missing='' to encode with missing values. "
-                )
-            else:
-                X[mask] = self.handle_missing
-
-        X_temp = check_array(X, dtype=None)
-        X = X_temp
-
-        n_samples, n_features = X.shape
-        X_int = np.zeros_like(X, dtype=int)
-        X_mask = np.ones_like(X, dtype=bool)
-
-        for i in range(n_features):
-            Xi = X[:, i]
-            valid_mask = np.in1d(Xi, self.categories_[i])
-
-            if not np.all(valid_mask):
-                if self.handle_unknown == "error":
-                    diff = np.unique(X[~valid_mask, i])
-                    raise ValueError(
-                        f"Found unknown categories {diff} in column {i} "
-                        "during transform."
-                    )
-                else:
-                    # Set the problematic rows to an acceptable value and
-                    # continue `The rows are marked `X_mask` and will be
-                    # removed later.
-                    X_mask[:, i] = valid_mask
-                    Xi = Xi.copy()
-                    Xi[~valid_mask] = self.categories_[i][0]
-            X_int[:, i] = self._label_encoders_[i].transform(Xi)
-
-        out = []
-
-        for j, cats in enumerate(self.categories_):
-            unqX = np.unique(X[:, j])
-            encoder = {x: 0 for x in unqX}
-            if self.clf_type in ["binary-clf", "regression"]:
-                for x in unqX:
-                    if x not in cats:
-                        Eyx = 0
-                    else:
-                        Eyx = self.Eyx_[j][x]
-                    lambda_n = lambda_(self.counter_[j][x], self.n_ / self.k_[j])
-                    encoder[x] = lambda_n * Eyx + (1 - lambda_n) * self.Ey_
-                x_out = np.zeros((len(X[:, j]), 1))
-                for i, x in enumerate(X[:, j]):
-                    x_out[i, 0] = encoder[x]
-                out.append(x_out.reshape(-1, 1))
-            if self.clf_type == "multiclass-clf":
-                x_out = np.zeros((len(X[:, j]), len(self.classes_)))
-                lambda_n = {x: 0 for x in unqX}
-                for x in unqX:
-                    lambda_n[x] = lambda_(self.counter_[j][x], self.n_ / self.k_[j])
-                for k, c in enumerate(np.unique(self.classes_)):
-                    for x in unqX:
-                        if x not in cats:
-                            Eyx = 0
-                        else:
-                            Eyx = self.Eyx_[c][j][x]
-                        encoder[x] = lambda_n[x] * Eyx + (1 - lambda_n[x]) * self.Ey_[c]
-                    for i, x in enumerate(X[:, j]):
-                        x_out[i, k] = encoder[x]
-                out.append(x_out)
-        out = np.hstack(out)
-        return out
+import collections
+from typing import Dict, List, Literal, Union
+
+import numpy as np
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.preprocessing import LabelEncoder
+from sklearn.utils import check_array
+from sklearn.utils.fixes import _object_dtype_isnan
+from sklearn.utils.validation import check_is_fitted
+
+from dirty_cat._utils import check_input
+
+
+def lambda_(x, n):
+    return x / (x + n)
+
+
+class TargetEncoder(BaseEstimator, TransformerMixin):
+    """Encode categorical features as a numeric array given a target vector.
+
+    Each category is encoded given the effect that it has in the
+    target variable y. The method considers that categorical
+    variables can present rare categories. It represents each category by the
+    probability of y conditional on this category.
+    In addition, it takes an empirical Bayes approach to shrink the estimate.
+
+
+    Parameters
+    ----------
+    categories : typing.Union[typing.Literal["auto"], typing.List[typing.List[typing.Union[str, int]]]  # noqa
+        Categories (unique values) per feature:
+
+        - 'auto' : Determine categories automatically from the training data.
+        - list : ``categories[i]`` holds the categories expected in the i-th
+          column. The passed categories must be sorted and should not mix
+          strings and numeric values.
+
+        The categories used can be found in the ``categories_`` attribute.
+    clf_type : typing.Literal["regression", "binary-clf", "multiclass-clf"]
+        The type of classification/regression problem.
+    dtype : type, default=np.float64
+        Desired dtype of output.
+    handle_unknown : typing.Literal["error", "ignore"], default="error"
+        Whether to raise an error or ignore if a unknown categorical feature is
+        present during transform (default is to raise). When this parameter
+        is set to 'ignore' and an unknown category is encountered during
+        transform, the encoded columns for this feature
+        will be assigned the prior mean of the target variable.
+    handle_missing : typing.Literal["error", ""], default=""
+        Whether to raise an error or impute with blank string '' if missing
+        values (NaN) are present during fit (default is to impute).
+        When this parameter is set to '', and a missing value is encountered
+        during fit_transform, the resulting encoded columns for this feature
+        will be all zeros.
+
+    Attributes
+    ----------
+    n_features_in_: int
+        Number of features in the data seen during fit.
+    categories_ : typing.List[np.ndarray]
+        The categories of each feature determined during fitting
+        (in order corresponding with output of ``transform``).
+
+    See Also
+    --------
+    :class:`~dirty_cat.GapEncoder` :
+        Encodes dirty categories (strings) by constructing latent topics with continuous encoding.
+    :class:`~dirty_cat.MinHashEncoder` :
+        Encode string columns as a numeric array with the minhash method.
+    :class:`~dirty_cat.SimilarityEncoder` :
+        Encode string columns as a numeric array with n-gram string similarity.
+
+    References
+    ----------
+    For more details, see Micci-Barreca, 2001: A preprocessing scheme for
+    high-cardinality categorical attributes in classification and prediction
+    problems.
+
+    Examples
+    --------
+    >>> enc = TargetEncoder(handle_unknown='ignore')
+    >>> X = [['male'], ['Male'], ['Female'], ['male'], ['Female']]
+    >>> y = np.array([1, 2, 3, 4, 5])
+
+    >>> enc.fit(X, y)
+    TargetEncoder(handle_unknown='ignore')
+
+    The encoder has found the following categories:
+
+    >>> enc.categories_
+    [array(['Female', 'Male', 'male'], dtype='<U6')]
+
+    We will encode the following categories, of which the first two are unknown :
+
+    >>> X2 = [['MALE'], ['FEMALE'], ['Female'], ['male'], ['Female']]
+
+    >>> enc.transform(X2)
+    array([[3.        ],
+        [3.        ],
+        [3.54545455],
+        [2.72727273],
+        [3.54545455]])
+
+    As expected, they were encoded according to their influence on y.
+    The unknown categories were assigned the mean of the target variable.
+
+    """
+
+    n_features_in_: int
+    _label_encoders_: List[LabelEncoder]
+    categories_: List[np.ndarray]
+    n_: int
+
+    def __init__(
+        self,
+        categories: Union[Literal["auto"], List[Union[List[str], np.ndarray]]] = "auto",
+        clf_type: Literal["regression", "binary-clf", "multiclass-clf"] = "binary-clf",
+        dtype: type = np.float64,
+        handle_unknown: Literal["error", "ignore"] = "error",
+        handle_missing: Literal["error", ""] = "",
+    ):
+        self.categories = categories
+        self.dtype = dtype
+        self.clf_type = clf_type
+        self.handle_unknown = handle_unknown
+        self.handle_missing = handle_missing
+
+    def _more_tags(self) -> Dict[str, List[str]]:
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {"X_types": ["categorical"]}
+
+    def fit(self, X, y) -> "TargetEncoder":
+        """
+        Fit the instance to X.
+
+        Parameters
+        ----------
+        X : array-like, shape [n_samples, n_features]
+            The data to determine the categories of each feature.
+        y : array
+            The associated target vector.
+
+        Returns
+        -------
+        :class:`~dirty_cat.TargetEncoder`
+            Fitted :class:`~dirty_cat.TargetEncoder` instance (self).
+        """
+        X = check_input(X)
+        self.n_features_in_ = X.shape[1]
+        if self.handle_missing not in ["error", ""]:
+            raise ValueError(
+                f"Got handle_missing={self.handle_missing!r}, but expected "
+                "any of {'error', ''}. "
+            )
+
+        mask = _object_dtype_isnan(X)
+        if mask.any():
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='' to encode with missing values. "
+                )
+            else:
+                X[mask] = self.handle_missing
+
+        if self.handle_unknown not in ["error", "ignore"]:
+            raise ValueError(
+                f"Got handle_unknown={self.handle_unknown!r}, but expected "
+                'any of {"error", "ignore"}. '
+            )
+
+        if self.categories != "auto":
+            for cats in self.categories:
+                if not np.all(np.sort(cats) == np.array(cats)):
+                    raise ValueError("Unsorted categories are not yet supported. ")
+
+        X_temp = check_array(X, dtype=None)
+        X = X_temp
+
+        n_samples, n_features = X.shape
+
+        self._label_encoders_ = [LabelEncoder() for _ in range(n_features)]
+
+        for j in range(n_features):
+            le = self._label_encoders_[j]
+            Xj = X[:, j]
+            if self.categories == "auto":
+                le.fit(Xj)
+            else:
+                if self.handle_unknown == "error":
+                    valid_mask = np.in1d(Xj, self.categories[j])
+                    if not np.all(valid_mask):
+                        diff = np.unique(Xj[~valid_mask])
+                        raise ValueError(
+                            f"Found unknown categories {diff} in column {j} during fit"
+                        )
+                le.classes_ = np.array(self.categories[j])
+
+        self.categories_ = [le.classes_ for le in self._label_encoders_]
+        self.n_ = len(y)
+        if self.clf_type in ["binary-clf", "regression"]:
+            self.Eyx_ = [
+                {cat: np.mean(y[X[:, j] == cat]) for cat in self.categories_[j]}
+                for j in range(len(self.categories_))
+            ]
+            self.Ey_ = np.mean(y)
+            self.counter_ = {j: collections.Counter(X[:, j]) for j in range(n_features)}
+        if self.clf_type in ["multiclass-clf"]:
+            self.classes_ = np.unique(y)
+
+            self.Eyx_ = {
+                c: [
+                    {
+                        cat: np.mean((y == c)[X[:, j] == cat])
+                        for cat in self.categories_[j]
+                    }
+                    for j in range(len(self.categories_))
+                ]
+                for c in self.classes_
+            }
+            self.Ey_ = {c: np.mean(y == c) for c in self.classes_}
+            self.counter_ = {j: collections.Counter(X[:, j]) for j in range(n_features)}
+        self.k_ = {j: len(self.counter_[j]) for j in self.counter_}
+        return self
+
+    def transform(self, X) -> np.ndarray:
+        """
+        Transform X using the specified encoding scheme.
+
+        Parameters
+        ----------
+        X : array-like, shape [n_samples, n_features_new]
+            The data to encode.
+
+        Returns
+        -------
+        2-d :class:`~numpy.ndarray`
+            Transformed input.
+        """
+        check_is_fitted(self, attributes=["n_features_in_"])
+        X = check_input(X)
+        if X.shape[1] != self.n_features_in_:
+            raise ValueError(
+                f"The number of features in the input data ({X.shape[1]}) "
+                "does not match the number of features "
+                f"seen during fit ({self.n_features_in_})."
+            )
+        mask = _object_dtype_isnan(X)
+        if mask.any():
+            if self.handle_missing == "error":
+                raise ValueError(
+                    "Found missing values in input data; set "
+                    "handle_missing='' to encode with missing values. "
+                )
+            else:
+                X[mask] = self.handle_missing
+
+        X_temp = check_array(X, dtype=None)
+        X = X_temp
+
+        n_samples, n_features = X.shape
+        X_int = np.zeros_like(X, dtype=int)
+        X_mask = np.ones_like(X, dtype=bool)
+
+        for i in range(n_features):
+            Xi = X[:, i]
+            valid_mask = np.in1d(Xi, self.categories_[i])
+
+            if not np.all(valid_mask):
+                if self.handle_unknown == "error":
+                    diff = np.unique(X[~valid_mask, i])
+                    raise ValueError(
+                        f"Found unknown categories {diff} in column {i} "
+                        "during transform."
+                    )
+                else:
+                    # Set the problematic rows to an acceptable value and
+                    # continue `The rows are marked `X_mask` and will be
+                    # removed later.
+                    X_mask[:, i] = valid_mask
+                    Xi = Xi.copy()
+                    Xi[~valid_mask] = self.categories_[i][0]
+            X_int[:, i] = self._label_encoders_[i].transform(Xi)
+
+        out = []
+
+        for j, cats in enumerate(self.categories_):
+            unqX = np.unique(X[:, j])
+            encoder = {x: 0 for x in unqX}
+            if self.clf_type in ["binary-clf", "regression"]:
+                for x in unqX:
+                    if x not in cats:
+                        Eyx = 0
+                    else:
+                        Eyx = self.Eyx_[j][x]
+                    lambda_n = lambda_(self.counter_[j][x], self.n_ / self.k_[j])
+                    encoder[x] = lambda_n * Eyx + (1 - lambda_n) * self.Ey_
+                x_out = np.zeros((len(X[:, j]), 1))
+                for i, x in enumerate(X[:, j]):
+                    x_out[i, 0] = encoder[x]
+                out.append(x_out.reshape(-1, 1))
+            if self.clf_type == "multiclass-clf":
+                x_out = np.zeros((len(X[:, j]), len(self.classes_)))
+                lambda_n = {x: 0 for x in unqX}
+                for x in unqX:
+                    lambda_n[x] = lambda_(self.counter_[j][x], self.n_ / self.k_[j])
+                for k, c in enumerate(np.unique(self.classes_)):
+                    for x in unqX:
+                        if x not in cats:
+                            Eyx = 0
+                        else:
+                            Eyx = self.Eyx_[c][j][x]
+                        encoder[x] = lambda_n[x] * Eyx + (1 - lambda_n[x]) * self.Ey_[c]
+                    for i, x in enumerate(X[:, j]):
+                        x_out[i, k] = encoder[x]
+                out.append(x_out)
+        out = np.hstack(out)
+        return out
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/_utils.py` & `dirty_cat-0.4.1/dirty_cat/_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import collections
-from typing import Any, Hashable
-
-import numpy as np
-from sklearn.utils import check_array
-
-try:
-    # Works for sklearn >= 1.0
-    from sklearn.utils import parse_version  # noqa
-except ImportError:
-    # Works for sklearn < 1.0
-    from sklearn.utils.fixes import _parse_version as parse_version  # noqa
-
-
-class LRUDict:
-    """dict with limited capacity
-
-    Using LRU eviction avoids memorizing a full dataset"""
-
-    def __init__(self, capacity: int):
-        self.capacity = capacity
-        self.cache = collections.OrderedDict()
-
-    def __getitem__(self, key: Hashable):
-        try:
-            value = self.cache.pop(key)
-            self.cache[key] = value
-            return value
-        except KeyError:
-            return -1
-
-    def __setitem__(self, key: Hashable, value: Any):
-        try:
-            self.cache.pop(key)
-        except KeyError:
-            if len(self.cache) >= self.capacity:
-                self.cache.popitem(last=False)
-        self.cache[key] = value
-
-    def __contains__(self, key: Hashable):
-        return key in self.cache
-
-
-def check_input(X) -> np.ndarray:
-    """
-    Check input with sklearn standards.
-    Also converts X to a numpy array if not already.
-    """
-    # TODO check for weird type of input to pass scikit learn tests
-    #  without messing with the original type too much
-
-    X_ = check_array(
-        X,
-        dtype=None,
-        ensure_2d=True,
-        force_all_finite=False,
-    )
-    # If the array contains both NaNs and strings, convert to object type
-    if X_.dtype.kind in {"U", "S"}:  # contains strings
-        if np.any(X_ == "nan"):  # missing value converted to string
-            return check_array(
-                np.array(X, dtype=object),
-                dtype=None,
-                ensure_2d=True,
-                force_all_finite=False,
-            )
-
-    return X_
+import collections
+from typing import Any, Hashable
+
+import numpy as np
+from sklearn.utils import check_array
+
+try:
+    # Works for sklearn >= 1.0
+    from sklearn.utils import parse_version  # noqa
+except ImportError:
+    # Works for sklearn < 1.0
+    from sklearn.utils.fixes import _parse_version as parse_version  # noqa
+
+
+class LRUDict:
+    """dict with limited capacity
+
+    Using LRU eviction avoids memorizing a full dataset"""
+
+    def __init__(self, capacity: int):
+        self.capacity = capacity
+        self.cache = collections.OrderedDict()
+
+    def __getitem__(self, key: Hashable):
+        try:
+            value = self.cache.pop(key)
+            self.cache[key] = value
+            return value
+        except KeyError:
+            return -1
+
+    def __setitem__(self, key: Hashable, value: Any):
+        try:
+            self.cache.pop(key)
+        except KeyError:
+            if len(self.cache) >= self.capacity:
+                self.cache.popitem(last=False)
+        self.cache[key] = value
+
+    def __contains__(self, key: Hashable):
+        return key in self.cache
+
+
+def check_input(X) -> np.ndarray:
+    """
+    Check input with sklearn standards.
+    Also converts X to a numpy array if not already.
+    """
+    # TODO check for weird type of input to pass scikit learn tests
+    #  without messing with the original type too much
+
+    X_ = check_array(
+        X,
+        dtype=None,
+        ensure_2d=True,
+        force_all_finite=False,
+    )
+    # If the array contains both NaNs and strings, convert to object type
+    if X_.dtype.kind in {"U", "S"}:  # contains strings
+        if np.any(X_ == "nan"):  # missing value converted to string
+            return check_array(
+                np.array(X, dtype=object),
+                dtype=None,
+                ensure_2d=True,
+                force_all_finite=False,
+            )
+
+    return X_
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/datasets/_generating.py` & `dirty_cat-0.4.1/dirty_cat/datasets/_generating.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-"""
-Functions that generate example data.
-
-"""
-from __future__ import annotations
-
-from typing import List, Optional, Union
-import string
-
-import numpy as np
-
-from sklearn.utils import check_random_state
-
-def make_deduplication_data(
-    examples: List[str],
-    entries_per_example: List[int],
-    prob_mistake_per_letter: float,
-    random_state: Optional[Union[int, np.random.RandomState]] = None,
-) -> List[str]:
-    """Duplicates examples with spelling mistakes.
-    Characters are misspelled with probability `prob_mistake_per_letter`.
-
-    Parameters
-    ----------
-    examples : List[str]
-        examples to duplicate
-    entries_per_example : List[int]
-        number of duplications per example
-    prob_mistake_per_letter : float in [0, 1]
-        probability of misspelling a character in duplications
-    random_state : int, RandomState instance or None, default=None
-        Determines random number generation for dataset noise. Pass an int
-        for reproducible output across multiple function calls.
-
-    Returns
-    -------
-    List[str]
-        list of duplicated examples with spelling mistakes
-    """
-    rng = check_random_state(random_state)
-
-    data = []
-    for example, n_ex in zip(examples, entries_per_example):
-        len_ex = len(example)
-        # generate a 2D array of chars of size (n_ex, len_ex)
-        str_as_list = np.array([list(example)] * n_ex)
-        # randomly choose which characters are misspelled
-        idxes = np.where(
-            rng.random(len(example[0]) * n_ex) < prob_mistake_per_letter
-        )[0]
-        # and randomly pick with which character to replace
-        replacements = [
-            string.ascii_lowercase[i]
-            for i in np.random.choice(np.arange(26), len(idxes)).astype(int)
-        ]
-        # introduce spelling mistakes at right examples and char locations per example
-        str_as_list[idxes // len_ex, idxes % len_ex] = replacements
-        # go back to 1d array of strings
-        data.append(np.ascontiguousarray(str_as_list).view(f"U{len_ex}").ravel())
-    return np.concatenate(data).tolist()
+"""
+Functions that generate example data.
+
+"""
+from __future__ import annotations
+
+from typing import List, Optional, Union
+import string
+
+import numpy as np
+
+from sklearn.utils import check_random_state
+
+def make_deduplication_data(
+    examples: List[str],
+    entries_per_example: List[int],
+    prob_mistake_per_letter: float,
+    random_state: Optional[Union[int, np.random.RandomState]] = None,
+) -> List[str]:
+    """Duplicates examples with spelling mistakes.
+    Characters are misspelled with probability `prob_mistake_per_letter`.
+
+    Parameters
+    ----------
+    examples : List[str]
+        examples to duplicate
+    entries_per_example : List[int]
+        number of duplications per example
+    prob_mistake_per_letter : float in [0, 1]
+        probability of misspelling a character in duplications
+    random_state : int, RandomState instance or None, default=None
+        Determines random number generation for dataset noise. Pass an int
+        for reproducible output across multiple function calls.
+
+    Returns
+    -------
+    List[str]
+        list of duplicated examples with spelling mistakes
+    """
+    rng = check_random_state(random_state)
+
+    data = []
+    for example, n_ex in zip(examples, entries_per_example):
+        len_ex = len(example)
+        # generate a 2D array of chars of size (n_ex, len_ex)
+        str_as_list = np.array([list(example)] * n_ex)
+        # randomly choose which characters are misspelled
+        idxes = np.where(
+            rng.random(len(example[0]) * n_ex) < prob_mistake_per_letter
+        )[0]
+        # and randomly pick with which character to replace
+        replacements = [
+            string.ascii_lowercase[i]
+            for i in np.random.choice(np.arange(26), len(idxes)).astype(int)
+        ]
+        # introduce spelling mistakes at right examples and char locations per example
+        str_as_list[idxes // len_ex, idxes % len_ex] = replacements
+        # go back to 1d array of strings
+        data.append(np.ascontiguousarray(str_as_list).view(f"U{len_ex}").ravel())
+    return np.concatenate(data).tolist()
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/datasets/tests/test_utils.py` & `dirty_cat-0.4.1/dirty_cat/datasets/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from pathlib import Path
-from unittest import mock
-
-
-@mock.patch("os.path.dirname")
-def test_get_data_dir(mock_os_path_dirname):
-    """
-    Tests function ``get_data_dir()``.
-    """
-    from dirty_cat.datasets._utils import get_data_dir
-
-    expected_return_value_default = Path("/user/directory/data")
-
-    mock_os_path_dirname.return_value = "/user/directory/"
-    assert get_data_dir() == expected_return_value_default
-
-    expected_return_value_custom = expected_return_value_default / "tests"
-    assert get_data_dir("tests") == expected_return_value_custom
+from pathlib import Path
+from unittest import mock
+
+
+@mock.patch("os.path.dirname")
+def test_get_data_dir(mock_os_path_dirname):
+    """
+    Tests function ``get_data_dir()``.
+    """
+    from dirty_cat.datasets._utils import get_data_dir
+
+    expected_return_value_default = Path("/user/directory/data")
+
+    mock_os_path_dirname.return_value = "/user/directory/"
+    assert get_data_dir() == expected_return_value_default
+
+    expected_return_value_custom = expected_return_value_default / "tests"
+    assert get_data_dir("tests") == expected_return_value_custom
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_datetime_encoder.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_datetime_encoder.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,355 +1,355 @@
-import pytest
-import numpy as np
-import pandas as pd
-from sklearn.exceptions import NotFittedError
-
-from dirty_cat._datetime_encoder import DatetimeEncoder
-
-
-def get_date_array() -> np.array:
-    return np.array(
-        [
-            pd.to_datetime(["2020-01-01", "2020-01-02", "2020-01-03"]),
-            pd.to_datetime(["2021-02-03", "2020-02-04", "2021-02-05"]),
-            pd.to_datetime(["2022-01-01", "2020-12-25", "2022-01-03"]),
-            pd.to_datetime(["2023-02-03", "2020-02-04", "2023-02-05"]),
-        ]
-    )
-
-
-def get_constant_date_array() -> np.array:
-    return np.array(
-        [
-            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
-            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
-            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
-            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
-        ]
-    )
-
-
-def get_datetime_array() -> np.array:
-    return np.array(
-        [
-            pd.to_datetime(
-                ["2020-01-01 10:12:01", "2020-01-02 10:23:00", "2020-01-03 10:00:00"]
-            ),
-            pd.to_datetime(
-                ["2021-02-03 12:45:23", "2020-02-04 22:12:00", "2021-02-05 12:00:00"]
-            ),
-            pd.to_datetime(
-                ["2022-01-01 23:23:43", "2020-12-25 11:12:00", "2022-01-03 11:00:00"]
-            ),
-            pd.to_datetime(
-                ["2023-02-03 11:12:12", "2020-02-04 08:32:00", "2023-02-05 23:00:00"]
-            ),
-        ]
-    )
-
-
-def get_dirty_datetime_array() -> np.array:
-    return np.array(
-        [
-            np.array(
-                pd.to_datetime(
-                    [
-                        "2020-01-01 10:12:01",
-                        "2020-01-02 10:23:00",
-                        "2020-01-03 10:00:00",
-                    ]
-                )
-            ),
-            np.array(
-                pd.to_datetime([np.nan, "2020-02-04 22:12:00", "2021-02-05 12:00:00"])
-            ),
-            np.array(
-                pd.to_datetime(["2022-01-01 23:23:43", "2020-12-25 11:12:00", pd.NaT])
-            ),
-            np.array(
-                pd.to_datetime(
-                    [
-                        "2023-02-03 11:12:12",
-                        "2020-02-04 08:32:00",
-                        "2023-02-05 23:00:00",
-                    ]
-                )
-            ),
-        ]
-    )
-
-
-def get_datetime_with_TZ_array() -> pd.DataFrame:
-    res = pd.DataFrame(
-        [
-            pd.to_datetime(["2020-01-01 10:12:01"]),
-            pd.to_datetime(["2021-02-03 12:45:23"]),
-            pd.to_datetime(["2022-01-01 23:23:43"]),
-            pd.to_datetime(["2023-02-03 11:12:12"]),
-        ]
-    )
-    for col in res.columns:
-        res[col] = pd.DatetimeIndex(res[col]).tz_localize("Asia/Kolkata")
-    return res
-
-
-def test_fit() -> None:
-    # Dates
-    X = get_date_array()
-    enc = DatetimeEncoder()
-    expected_to_extract = ["year", "month", "day", "hour"]
-    expected_features_per_column_ = {
-        0: ["year", "month", "day"],
-        1: ["month", "day"],
-        2: ["year", "month", "day"],
-    }
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    X = get_date_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_to_extract = ["year", "month", "day", "hour", "dayofweek"]
-    expected_features_per_column_ = {
-        0: ["year", "month", "day", "dayofweek"],
-        1: ["month", "day", "dayofweek"],
-        2: ["year", "month", "day", "dayofweek"],
-    }
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    # Datetimes
-    X = get_datetime_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_to_extract = ["year", "month", "day", "hour", "dayofweek"]
-    expected_features_per_column_ = {
-        0: ["year", "month", "day", "hour", "dayofweek", "total_time"],
-        1: ["month", "day", "hour", "dayofweek", "total_time"],
-        2: ["year", "month", "day", "hour", "dayofweek"],
-    }
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    X = get_datetime_array()
-    enc = DatetimeEncoder(extract_until="minute")
-    expected_to_extract = ["year", "month", "day", "hour", "minute"]
-    expected_features_per_column_ = {
-        0: ["year", "month", "day", "hour", "minute", "total_time"],
-        1: ["month", "day", "hour", "minute"],
-        2: ["year", "month", "day", "hour"],
-    }
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    # Dirty Datetimes
-    X = get_dirty_datetime_array()
-    enc = DatetimeEncoder()
-    expected_to_extract = ["year", "month", "day", "hour"]
-    expected_features_per_column_ = {
-        0: ["year", "month", "day", "hour", "total_time"],
-        1: ["month", "day", "hour", "total_time"],
-        2: ["year", "month", "day", "hour"],
-    }
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    # Datetimes with TZ
-    X = get_datetime_with_TZ_array()
-    enc = DatetimeEncoder()
-    expected_to_extract = ["year", "month", "day", "hour"]
-    expected_features_per_column_ = {0: ["year", "month", "day", "hour", "total_time"]}
-    enc.fit(X)
-    assert enc._to_extract == expected_to_extract
-    assert enc.features_per_column_ == expected_features_per_column_
-
-    # Feature names
-    # Without column names
-    X = get_datetime_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_feature_names = [
-        "0_year",
-        "0_month",
-        "0_day",
-        "0_hour",
-        "0_dayofweek",
-        "0_total_time",
-        "1_month",
-        "1_day",
-        "1_hour",
-        "1_dayofweek",
-        "1_total_time",
-        "2_year",
-        "2_month",
-        "2_day",
-        "2_hour",
-        "2_dayofweek",
-    ]
-    enc.fit(X)
-    assert enc.get_feature_names_out() == expected_feature_names
-
-    # With column names
-    X = get_datetime_array()
-    X = pd.DataFrame(X)
-    X.columns = ["col1", "col2", "col3"]
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_feature_names = [
-        "col1_year",
-        "col1_month",
-        "col1_day",
-        "col1_hour",
-        "col1_dayofweek",
-        "col1_total_time",
-        "col2_month",
-        "col2_day",
-        "col2_hour",
-        "col2_dayofweek",
-        "col2_total_time",
-        "col3_year",
-        "col3_month",
-        "col3_day",
-        "col3_hour",
-        "col3_dayofweek",
-    ]
-    enc.fit(X)
-    assert enc.get_feature_names_out() == expected_feature_names
-
-
-def test_transform():
-    # Dates
-    X = get_date_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 2, 1, 2, 3, 2020, 1, 3, 4],
-            [2021, 2, 3, 2, 2, 4, 1, 2021, 2, 5, 4],
-            [2022, 1, 1, 5, 12, 25, 4, 2022, 1, 3, 0],
-            [2023, 2, 3, 4, 2, 4, 1, 2023, 2, 5, 6],
-        ]
-    )
-    enc.fit(X)
-    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
-
-    enc = DatetimeEncoder(add_day_of_the_week=False)
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 1, 2, 2020, 1, 3],
-            [2021, 2, 3, 2, 4, 2021, 2, 5],
-            [2022, 1, 1, 12, 25, 2022, 1, 3],
-            [2023, 2, 3, 2, 4, 2023, 2, 5],
-        ]
-    )
-    enc.fit(X)
-    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
-
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 2, 1, 2, 3, 2020, 1, 3, 4],
-            [2021, 2, 3, 2, 2, 4, 1, 2021, 2, 5, 4],
-            [2022, 1, 1, 5, 12, 25, 4, 2022, 1, 3, 0],
-            [2023, 2, 3, 4, 2, 4, 1, 2023, 2, 5, 6],
-        ]
-    )
-    enc.fit(X)
-    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
-
-    # Datetimes
-    X = get_datetime_array()[:, 0].reshape(-1, 1)
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    # Check that the "total_time" feature is working
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 10, 2, 0],
-            [2021, 2, 3, 12, 2, 0],
-            [2022, 1, 1, 23, 5, 0],
-            [2023, 2, 3, 11, 4, 0],
-        ]
-    ).astype(np.float64)
-    # Time from epochs in seconds
-    expected_result[:, 5] = (X.astype("int64") // 1e9).astype(np.float64).reshape(-1)
-
-    enc.fit(X)
-    X_trans = enc.transform(X)
-    assert np.allclose(X_trans, expected_result, equal_nan=True)
-
-    # Check if we find back the date from the time to epoch
-    assert (
-        (
-            pd.to_datetime(X_trans[:, 5], unit="s") - pd.to_datetime(X.reshape(-1))
-        ).total_seconds()
-        == 0
-    ).all()
-
-    # Dirty datetimes
-    X = get_dirty_datetime_array()[:, 0].reshape(-1, 1)
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 10, 2, 0],
-            [np.nan] * 6,
-            [2022, 1, 1, 23, 5, 0],
-            [2023, 2, 3, 11, 4, 0],
-        ]
-    )
-    # Time from epochs in seconds
-    expected_result[:, 5] = (X.astype("int64") // 1e9).astype(np.float64).reshape(-1)
-    expected_result[1, 5] = np.nan
-    enc.fit(X)
-    X_trans = enc.transform(X)
-    assert np.allclose(X_trans, expected_result, equal_nan=True)
-
-    # Datetimes with TZ
-    # If the dates are timezone-aware, all the feature extractions should
-    # be done in the provided timezone.
-    # But the full time to epoch should correspond to the true number of
-    # seconds between epoch time and the time of the date.
-    X = get_datetime_with_TZ_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    expected_result = np.array(
-        [
-            [2020, 1, 1, 10, 2, 0],
-            [2021, 2, 3, 12, 2, 0],
-            [2022, 1, 1, 23, 5, 0],
-            [2023, 2, 3, 11, 4, 0],
-        ]
-    ).astype(np.float64)
-    # Time from epochs in seconds
-    expected_result[:, 5] = (
-        (X.iloc[:, 0].view(dtype="int64") // 1e9)
-        .astype(np.float64)
-        .to_numpy()
-        .reshape(-1)
-    )
-    enc.fit(X)
-    X_trans = enc.transform(X)
-    assert np.allclose(X_trans, expected_result, equal_nan=True)
-
-    # Check if we find back the date from the time to epoch
-    assert (
-        (
-            pd.to_datetime(X_trans[:, 5], unit="s")
-            .tz_localize("utc")
-            .tz_convert(X.iloc[:, 0][0].tz)
-            - pd.DatetimeIndex(X.iloc[:, 0])
-        ).total_seconds()
-        == 0
-    ).all()
-
-    # Check if it's working when the date is constant
-    X = get_constant_date_array()
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    assert enc.fit_transform(X).shape[1] == 0
-
-def test_check_fitted_datetime_encoder():
-    """Test that calling transform before fit raises an error"""
-    X = get_datetime_array()[:, 0].reshape(-1, 1)
-    enc = DatetimeEncoder(add_day_of_the_week=True)
-    with pytest.raises(NotFittedError):
-        enc.transform(X)
-    
-    # Check that it works after fit
-    enc.fit(X)
-    enc.transform(X)
+import pytest
+import numpy as np
+import pandas as pd
+from sklearn.exceptions import NotFittedError
+
+from dirty_cat._datetime_encoder import DatetimeEncoder
+
+
+def get_date_array() -> np.array:
+    return np.array(
+        [
+            pd.to_datetime(["2020-01-01", "2020-01-02", "2020-01-03"]),
+            pd.to_datetime(["2021-02-03", "2020-02-04", "2021-02-05"]),
+            pd.to_datetime(["2022-01-01", "2020-12-25", "2022-01-03"]),
+            pd.to_datetime(["2023-02-03", "2020-02-04", "2023-02-05"]),
+        ]
+    )
+
+
+def get_constant_date_array() -> np.array:
+    return np.array(
+        [
+            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
+            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
+            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
+            pd.to_datetime(["2020-01-01", "2020-02-04", "2021-02-05"]),
+        ]
+    )
+
+
+def get_datetime_array() -> np.array:
+    return np.array(
+        [
+            pd.to_datetime(
+                ["2020-01-01 10:12:01", "2020-01-02 10:23:00", "2020-01-03 10:00:00"]
+            ),
+            pd.to_datetime(
+                ["2021-02-03 12:45:23", "2020-02-04 22:12:00", "2021-02-05 12:00:00"]
+            ),
+            pd.to_datetime(
+                ["2022-01-01 23:23:43", "2020-12-25 11:12:00", "2022-01-03 11:00:00"]
+            ),
+            pd.to_datetime(
+                ["2023-02-03 11:12:12", "2020-02-04 08:32:00", "2023-02-05 23:00:00"]
+            ),
+        ]
+    )
+
+
+def get_dirty_datetime_array() -> np.array:
+    return np.array(
+        [
+            np.array(
+                pd.to_datetime(
+                    [
+                        "2020-01-01 10:12:01",
+                        "2020-01-02 10:23:00",
+                        "2020-01-03 10:00:00",
+                    ]
+                )
+            ),
+            np.array(
+                pd.to_datetime([np.nan, "2020-02-04 22:12:00", "2021-02-05 12:00:00"])
+            ),
+            np.array(
+                pd.to_datetime(["2022-01-01 23:23:43", "2020-12-25 11:12:00", pd.NaT])
+            ),
+            np.array(
+                pd.to_datetime(
+                    [
+                        "2023-02-03 11:12:12",
+                        "2020-02-04 08:32:00",
+                        "2023-02-05 23:00:00",
+                    ]
+                )
+            ),
+        ]
+    )
+
+
+def get_datetime_with_TZ_array() -> pd.DataFrame:
+    res = pd.DataFrame(
+        [
+            pd.to_datetime(["2020-01-01 10:12:01"]),
+            pd.to_datetime(["2021-02-03 12:45:23"]),
+            pd.to_datetime(["2022-01-01 23:23:43"]),
+            pd.to_datetime(["2023-02-03 11:12:12"]),
+        ]
+    )
+    for col in res.columns:
+        res[col] = pd.DatetimeIndex(res[col]).tz_localize("Asia/Kolkata")
+    return res
+
+
+def test_fit() -> None:
+    # Dates
+    X = get_date_array()
+    enc = DatetimeEncoder()
+    expected_to_extract = ["year", "month", "day", "hour"]
+    expected_features_per_column_ = {
+        0: ["year", "month", "day"],
+        1: ["month", "day"],
+        2: ["year", "month", "day"],
+    }
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    X = get_date_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_to_extract = ["year", "month", "day", "hour", "dayofweek"]
+    expected_features_per_column_ = {
+        0: ["year", "month", "day", "dayofweek"],
+        1: ["month", "day", "dayofweek"],
+        2: ["year", "month", "day", "dayofweek"],
+    }
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    # Datetimes
+    X = get_datetime_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_to_extract = ["year", "month", "day", "hour", "dayofweek"]
+    expected_features_per_column_ = {
+        0: ["year", "month", "day", "hour", "dayofweek", "total_time"],
+        1: ["month", "day", "hour", "dayofweek", "total_time"],
+        2: ["year", "month", "day", "hour", "dayofweek"],
+    }
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    X = get_datetime_array()
+    enc = DatetimeEncoder(extract_until="minute")
+    expected_to_extract = ["year", "month", "day", "hour", "minute"]
+    expected_features_per_column_ = {
+        0: ["year", "month", "day", "hour", "minute", "total_time"],
+        1: ["month", "day", "hour", "minute"],
+        2: ["year", "month", "day", "hour"],
+    }
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    # Dirty Datetimes
+    X = get_dirty_datetime_array()
+    enc = DatetimeEncoder()
+    expected_to_extract = ["year", "month", "day", "hour"]
+    expected_features_per_column_ = {
+        0: ["year", "month", "day", "hour", "total_time"],
+        1: ["month", "day", "hour", "total_time"],
+        2: ["year", "month", "day", "hour"],
+    }
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    # Datetimes with TZ
+    X = get_datetime_with_TZ_array()
+    enc = DatetimeEncoder()
+    expected_to_extract = ["year", "month", "day", "hour"]
+    expected_features_per_column_ = {0: ["year", "month", "day", "hour", "total_time"]}
+    enc.fit(X)
+    assert enc._to_extract == expected_to_extract
+    assert enc.features_per_column_ == expected_features_per_column_
+
+    # Feature names
+    # Without column names
+    X = get_datetime_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_feature_names = [
+        "0_year",
+        "0_month",
+        "0_day",
+        "0_hour",
+        "0_dayofweek",
+        "0_total_time",
+        "1_month",
+        "1_day",
+        "1_hour",
+        "1_dayofweek",
+        "1_total_time",
+        "2_year",
+        "2_month",
+        "2_day",
+        "2_hour",
+        "2_dayofweek",
+    ]
+    enc.fit(X)
+    assert enc.get_feature_names_out() == expected_feature_names
+
+    # With column names
+    X = get_datetime_array()
+    X = pd.DataFrame(X)
+    X.columns = ["col1", "col2", "col3"]
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_feature_names = [
+        "col1_year",
+        "col1_month",
+        "col1_day",
+        "col1_hour",
+        "col1_dayofweek",
+        "col1_total_time",
+        "col2_month",
+        "col2_day",
+        "col2_hour",
+        "col2_dayofweek",
+        "col2_total_time",
+        "col3_year",
+        "col3_month",
+        "col3_day",
+        "col3_hour",
+        "col3_dayofweek",
+    ]
+    enc.fit(X)
+    assert enc.get_feature_names_out() == expected_feature_names
+
+
+def test_transform():
+    # Dates
+    X = get_date_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 2, 1, 2, 3, 2020, 1, 3, 4],
+            [2021, 2, 3, 2, 2, 4, 1, 2021, 2, 5, 4],
+            [2022, 1, 1, 5, 12, 25, 4, 2022, 1, 3, 0],
+            [2023, 2, 3, 4, 2, 4, 1, 2023, 2, 5, 6],
+        ]
+    )
+    enc.fit(X)
+    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
+
+    enc = DatetimeEncoder(add_day_of_the_week=False)
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 1, 2, 2020, 1, 3],
+            [2021, 2, 3, 2, 4, 2021, 2, 5],
+            [2022, 1, 1, 12, 25, 2022, 1, 3],
+            [2023, 2, 3, 2, 4, 2023, 2, 5],
+        ]
+    )
+    enc.fit(X)
+    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
+
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 2, 1, 2, 3, 2020, 1, 3, 4],
+            [2021, 2, 3, 2, 2, 4, 1, 2021, 2, 5, 4],
+            [2022, 1, 1, 5, 12, 25, 4, 2022, 1, 3, 0],
+            [2023, 2, 3, 4, 2, 4, 1, 2023, 2, 5, 6],
+        ]
+    )
+    enc.fit(X)
+    assert np.allclose(enc.transform(X), expected_result, equal_nan=True)
+
+    # Datetimes
+    X = get_datetime_array()[:, 0].reshape(-1, 1)
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    # Check that the "total_time" feature is working
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 10, 2, 0],
+            [2021, 2, 3, 12, 2, 0],
+            [2022, 1, 1, 23, 5, 0],
+            [2023, 2, 3, 11, 4, 0],
+        ]
+    ).astype(np.float64)
+    # Time from epochs in seconds
+    expected_result[:, 5] = (X.astype("int64") // 1e9).astype(np.float64).reshape(-1)
+
+    enc.fit(X)
+    X_trans = enc.transform(X)
+    assert np.allclose(X_trans, expected_result, equal_nan=True)
+
+    # Check if we find back the date from the time to epoch
+    assert (
+        (
+            pd.to_datetime(X_trans[:, 5], unit="s") - pd.to_datetime(X.reshape(-1))
+        ).total_seconds()
+        == 0
+    ).all()
+
+    # Dirty datetimes
+    X = get_dirty_datetime_array()[:, 0].reshape(-1, 1)
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 10, 2, 0],
+            [np.nan] * 6,
+            [2022, 1, 1, 23, 5, 0],
+            [2023, 2, 3, 11, 4, 0],
+        ]
+    )
+    # Time from epochs in seconds
+    expected_result[:, 5] = (X.astype("int64") // 1e9).astype(np.float64).reshape(-1)
+    expected_result[1, 5] = np.nan
+    enc.fit(X)
+    X_trans = enc.transform(X)
+    assert np.allclose(X_trans, expected_result, equal_nan=True)
+
+    # Datetimes with TZ
+    # If the dates are timezone-aware, all the feature extractions should
+    # be done in the provided timezone.
+    # But the full time to epoch should correspond to the true number of
+    # seconds between epoch time and the time of the date.
+    X = get_datetime_with_TZ_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    expected_result = np.array(
+        [
+            [2020, 1, 1, 10, 2, 0],
+            [2021, 2, 3, 12, 2, 0],
+            [2022, 1, 1, 23, 5, 0],
+            [2023, 2, 3, 11, 4, 0],
+        ]
+    ).astype(np.float64)
+    # Time from epochs in seconds
+    expected_result[:, 5] = (
+        (X.iloc[:, 0].view(dtype="int64") // 1e9)
+        .astype(np.float64)
+        .to_numpy()
+        .reshape(-1)
+    )
+    enc.fit(X)
+    X_trans = enc.transform(X)
+    assert np.allclose(X_trans, expected_result, equal_nan=True)
+
+    # Check if we find back the date from the time to epoch
+    assert (
+        (
+            pd.to_datetime(X_trans[:, 5], unit="s")
+            .tz_localize("utc")
+            .tz_convert(X.iloc[:, 0][0].tz)
+            - pd.DatetimeIndex(X.iloc[:, 0])
+        ).total_seconds()
+        == 0
+    ).all()
+
+    # Check if it's working when the date is constant
+    X = get_constant_date_array()
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    assert enc.fit_transform(X).shape[1] == 0
+
+def test_check_fitted_datetime_encoder():
+    """Test that calling transform before fit raises an error"""
+    X = get_datetime_array()[:, 0].reshape(-1, 1)
+    enc = DatetimeEncoder(add_day_of_the_week=True)
+    with pytest.raises(NotFittedError):
+        enc.transform(X)
+    
+    # Check that it works after fit
+    enc.fit(X)
+    enc.transform(X)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_deduplicate.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_deduplicate.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import string
-from typing import List
-
-import numpy as np
-import pandas as pd
-import pytest
-from scipy.cluster.hierarchy import linkage
-from scipy.spatial.distance import squareform
-
-from dirty_cat._deduplicate import (
-    _create_spelling_correction,
-    _guess_clusters,
-    compute_ngram_distance,
-    deduplicate,
-)
-
-
-def generate_example_data(examples, entries_per_example, prob_mistake_per_letter, rng):
-    """Helper function to generate data consisting of multiple entries per example.
-    Characters are misspelled with probability `prob_mistake_per_letter`"""
-
-    data = []
-    for example, n_ex in zip(examples, entries_per_example):
-        len_ex = len(example)
-        # generate a 2D array of chars of size (n_ex, len_ex)
-        str_as_list = np.array([list(example)] * n_ex)
-        # randomly choose which characters are misspelled
-        idxes = np.where(
-            rng.random_sample(len(example[0]) * n_ex) < prob_mistake_per_letter
-        )[0]
-        # and randomly pick with which character to replace
-        replacements = [
-            string.ascii_lowercase[i]
-            for i in rng.choice(np.arange(26), len(idxes)).astype(int)
-        ]
-        # introduce spelling mistakes at right examples and char locations per example
-        str_as_list[idxes // len_ex, idxes % len_ex] = replacements
-        # go back to 1d array of strings
-        data.append(np.ascontiguousarray(str_as_list).view(f"U{len_ex}").ravel())
-    return np.concatenate(data)
-
-
-@pytest.mark.parametrize(
-    "entries_per_category, prob_mistake_per_letter",
-    [[[500, 100, 1500], 0.05], [[100, 100], 0.02], [[200, 50, 30, 200, 800], 0.01]],
-)
-def test_deduplicate(
-    entries_per_category: List[int],
-    prob_mistake_per_letter: float,
-    seed: int = 123,
-) -> None:
-    rng = np.random.RandomState(seed)
-
-    # hard coded to fix ground truth string similarities
-    clean_categories = [
-        "Example Category",
-        "Generic",
-        "Random Word",
-        "Pretty similar category",
-        "Final cluster",
-    ]
-    n_clusters = len(entries_per_category)
-    clean_categories = clean_categories[:n_clusters]
-    data = generate_example_data(
-        clean_categories, entries_per_category, prob_mistake_per_letter, rng
-    )
-    deduplicated_data = np.array(deduplicate(data, n_clusters=None))
-    assert deduplicated_data.shape[0] == data.shape[0]
-    recovered_categories = np.unique(deduplicated_data)
-    assert recovered_categories.shape[0] == n_clusters
-    assert np.isin(clean_categories, recovered_categories).all()
-    deduplicated_data = deduplicate(data, n_clusters=n_clusters)
-    translation_table = pd.Series(deduplicated_data, index=data)
-    translation_table = translation_table[
-        ~translation_table.index.duplicated(keep="first")
-    ]
-    assert np.isin(np.unique(deduplicated_data), recovered_categories).all()
-    assert np.alltrue(translation_table[data] == np.array(deduplicated_data))
-    deduplicated_other_analyzer = np.array(
-        deduplicate(data, n_clusters=n_clusters, analyzer="char")
-    )
-    unique_other_analyzer = np.unique(deduplicated_other_analyzer)
-    assert np.isin(unique_other_analyzer, recovered_categories).all()
-
-
-def test_compute_ngram_distance() -> None:
-    words = np.array(["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"])
-    distance = compute_ngram_distance(words)
-    distance = squareform(distance)
-    assert distance.shape[0] == words.shape[0]
-    assert np.allclose(np.diag(distance), 0)
-    for un_word in np.unique(words):
-        assert np.allclose(distance[words == un_word][:, words == un_word], 0)
-
-
-def test__guess_clusters() -> None:
-    words = np.array(["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"])
-    distance = compute_ngram_distance(words)
-    Z = linkage(distance, method="average")
-    n_clusters = _guess_clusters(Z, distance)
-    assert n_clusters == len(np.unique(words))
-
-
-def test__create_spelling_correction(seed: int = 123) -> None:
-    rng = np.random.RandomState(seed)
-    n_clusters = 3
-    samples_per_cluster = 10
-    counts = np.concatenate(
-        [rng.randint(0, 100, samples_per_cluster) for _ in range(n_clusters)]
-    )
-    clusters = (
-        np.repeat(np.arange(n_clusters), samples_per_cluster).astype("int").tolist()
-    )
-    spelling_correction = _create_spelling_correction(
-        counts.astype("str"),
-        counts,
-        clusters,
-    )
-    # check that the most common sample per cluster is chosen as the 'correct' spelling
-    for n in np.arange(n_clusters):
-        assert (
-            spelling_correction.values[clusters == n].astype("int")
-            == counts[clusters == n].max()
-        ).all()
+import string
+from typing import List
+
+import numpy as np
+import pandas as pd
+import pytest
+from scipy.cluster.hierarchy import linkage
+from scipy.spatial.distance import squareform
+
+from dirty_cat._deduplicate import (
+    _create_spelling_correction,
+    _guess_clusters,
+    compute_ngram_distance,
+    deduplicate,
+)
+
+
+def generate_example_data(examples, entries_per_example, prob_mistake_per_letter, rng):
+    """Helper function to generate data consisting of multiple entries per example.
+    Characters are misspelled with probability `prob_mistake_per_letter`"""
+
+    data = []
+    for example, n_ex in zip(examples, entries_per_example):
+        len_ex = len(example)
+        # generate a 2D array of chars of size (n_ex, len_ex)
+        str_as_list = np.array([list(example)] * n_ex)
+        # randomly choose which characters are misspelled
+        idxes = np.where(
+            rng.random_sample(len(example[0]) * n_ex) < prob_mistake_per_letter
+        )[0]
+        # and randomly pick with which character to replace
+        replacements = [
+            string.ascii_lowercase[i]
+            for i in rng.choice(np.arange(26), len(idxes)).astype(int)
+        ]
+        # introduce spelling mistakes at right examples and char locations per example
+        str_as_list[idxes // len_ex, idxes % len_ex] = replacements
+        # go back to 1d array of strings
+        data.append(np.ascontiguousarray(str_as_list).view(f"U{len_ex}").ravel())
+    return np.concatenate(data)
+
+
+@pytest.mark.parametrize(
+    "entries_per_category, prob_mistake_per_letter",
+    [[[500, 100, 1500], 0.05], [[100, 100], 0.02], [[200, 50, 30, 200, 800], 0.01]],
+)
+def test_deduplicate(
+    entries_per_category: List[int],
+    prob_mistake_per_letter: float,
+    seed: int = 123,
+) -> None:
+    rng = np.random.RandomState(seed)
+
+    # hard coded to fix ground truth string similarities
+    clean_categories = [
+        "Example Category",
+        "Generic",
+        "Random Word",
+        "Pretty similar category",
+        "Final cluster",
+    ]
+    n_clusters = len(entries_per_category)
+    clean_categories = clean_categories[:n_clusters]
+    data = generate_example_data(
+        clean_categories, entries_per_category, prob_mistake_per_letter, rng
+    )
+    deduplicated_data = np.array(deduplicate(data, n_clusters=None))
+    assert deduplicated_data.shape[0] == data.shape[0]
+    recovered_categories = np.unique(deduplicated_data)
+    assert recovered_categories.shape[0] == n_clusters
+    assert np.isin(clean_categories, recovered_categories).all()
+    deduplicated_data = deduplicate(data, n_clusters=n_clusters)
+    translation_table = pd.Series(deduplicated_data, index=data)
+    translation_table = translation_table[
+        ~translation_table.index.duplicated(keep="first")
+    ]
+    assert np.isin(np.unique(deduplicated_data), recovered_categories).all()
+    assert np.alltrue(translation_table[data] == np.array(deduplicated_data))
+    deduplicated_other_analyzer = np.array(
+        deduplicate(data, n_clusters=n_clusters, analyzer="char")
+    )
+    unique_other_analyzer = np.unique(deduplicated_other_analyzer)
+    assert np.isin(unique_other_analyzer, recovered_categories).all()
+
+
+def test_compute_ngram_distance() -> None:
+    words = np.array(["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"])
+    distance = compute_ngram_distance(words)
+    distance = squareform(distance)
+    assert distance.shape[0] == words.shape[0]
+    assert np.allclose(np.diag(distance), 0)
+    for un_word in np.unique(words):
+        assert np.allclose(distance[words == un_word][:, words == un_word], 0)
+
+
+def test__guess_clusters() -> None:
+    words = np.array(["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"])
+    distance = compute_ngram_distance(words)
+    Z = linkage(distance, method="average")
+    n_clusters = _guess_clusters(Z, distance)
+    assert n_clusters == len(np.unique(words))
+
+
+def test__create_spelling_correction(seed: int = 123) -> None:
+    rng = np.random.RandomState(seed)
+    n_clusters = 3
+    samples_per_cluster = 10
+    counts = np.concatenate(
+        [rng.randint(0, 100, samples_per_cluster) for _ in range(n_clusters)]
+    )
+    clusters = (
+        np.repeat(np.arange(n_clusters), samples_per_cluster).astype("int").tolist()
+    )
+    spelling_correction = _create_spelling_correction(
+        counts.astype("str"),
+        counts,
+        clusters,
+    )
+    # check that the most common sample per cluster is chosen as the 'correct' spelling
+    for n in np.arange(n_clusters):
+        assert (
+            spelling_correction.values[clusters == n].astype("int")
+            == counts[clusters == n].max()
+        ).all()
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_feature_augmenter.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_feature_augmenter.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import pandas as pd
-import pytest
-
-from dirty_cat import FeatureAugmenter
-
-
-def test_feature_augmenter():
-    main_table = pd.DataFrame(
-        [
-            "France",
-            "Germany",
-            "Italy",
-        ],
-        columns=["Country"],
-    )
-
-    aux_table_1 = pd.DataFrame(
-        [
-            ["Germany", 84_000_000],
-            ["French Republic", 68_000_000],
-            ["Italia", 59_000_000],
-        ],
-        columns=["Country", "Population"],
-    )
-
-    aux_table_2 = pd.DataFrame(
-        [
-            ["France", 2937],
-            ["Italy", 2099],
-            ["Germany", 4223],
-            ["UK", 3186],
-        ],
-        columns=["Country name", "GDP (billion)"],
-    )
-
-    aux_table_3 = pd.DataFrame(
-        [
-            ["La France", "Paris"],
-            ["Italy", "Rome"],
-            ["Germany", "Berlin"],
-        ],
-        columns=["Countries", "Capital"],
-    )
-
-    aux_tables = [
-        (aux_table_1, "Country"),
-        (aux_table_2, "Country name"),
-        (aux_table_3, "Countries"),
-    ]
-
-    fa = FeatureAugmenter(tables=aux_tables, main_key="Country")
-
-    fa.fit(main_table)
-
-    number_of_cols = tuple(
-        map(
-            sum,
-            zip(
-                main_table.shape,
-                aux_table_1.shape,
-                aux_table_2.shape,
-                aux_table_3.shape,
-            ),
-        )
-    )[1]
-
-    big_table = fa.transform(main_table)
-    assert big_table.shape == (main_table.shape[0], number_of_cols)
-
-    big_table = fa.fit_transform(main_table)
-    assert big_table.shape == (main_table.shape[0], number_of_cols)
-
-    false_fa = FeatureAugmenter(tables=aux_tables, main_key="Countryy")
-
-    with pytest.raises(
-        ValueError,
-        match=r"Got main_key",
-    ):
-        false_fa.fit(main_table)
-
-    false_aux_tables = [
-        (aux_table_1, "Countrys"),
-        (aux_table_2, "Country name"),
-        (aux_table_3, "Countries"),
-    ]
-
-    false_fa2 = FeatureAugmenter(tables=false_aux_tables, main_key="Country")
-    with pytest.raises(
-        ValueError,
-        match=r"Got column key",
-    ):
-        false_fa2.fit(main_table)
+import pandas as pd
+import pytest
+
+from dirty_cat import FeatureAugmenter
+
+
+def test_feature_augmenter():
+    main_table = pd.DataFrame(
+        [
+            "France",
+            "Germany",
+            "Italy",
+        ],
+        columns=["Country"],
+    )
+
+    aux_table_1 = pd.DataFrame(
+        [
+            ["Germany", 84_000_000],
+            ["French Republic", 68_000_000],
+            ["Italia", 59_000_000],
+        ],
+        columns=["Country", "Population"],
+    )
+
+    aux_table_2 = pd.DataFrame(
+        [
+            ["France", 2937],
+            ["Italy", 2099],
+            ["Germany", 4223],
+            ["UK", 3186],
+        ],
+        columns=["Country name", "GDP (billion)"],
+    )
+
+    aux_table_3 = pd.DataFrame(
+        [
+            ["La France", "Paris"],
+            ["Italy", "Rome"],
+            ["Germany", "Berlin"],
+        ],
+        columns=["Countries", "Capital"],
+    )
+
+    aux_tables = [
+        (aux_table_1, "Country"),
+        (aux_table_2, "Country name"),
+        (aux_table_3, "Countries"),
+    ]
+
+    fa = FeatureAugmenter(tables=aux_tables, main_key="Country")
+
+    fa.fit(main_table)
+
+    number_of_cols = tuple(
+        map(
+            sum,
+            zip(
+                main_table.shape,
+                aux_table_1.shape,
+                aux_table_2.shape,
+                aux_table_3.shape,
+            ),
+        )
+    )[1]
+
+    big_table = fa.transform(main_table)
+    assert big_table.shape == (main_table.shape[0], number_of_cols)
+
+    big_table = fa.fit_transform(main_table)
+    assert big_table.shape == (main_table.shape[0], number_of_cols)
+
+    false_fa = FeatureAugmenter(tables=aux_tables, main_key="Countryy")
+
+    with pytest.raises(
+        ValueError,
+        match=r"Got main_key",
+    ):
+        false_fa.fit(main_table)
+
+    false_aux_tables = [
+        (aux_table_1, "Countrys"),
+        (aux_table_2, "Country name"),
+        (aux_table_3, "Countries"),
+    ]
+
+    false_fa2 = FeatureAugmenter(tables=false_aux_tables, main_key="Country")
+    with pytest.raises(
+        ValueError,
+        match=r"Got column key",
+    ):
+        false_fa2.fit(main_table)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_minhash_encoder.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_minhash_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,253 @@
-import random
-from string import ascii_lowercase
-
-import joblib
-import numpy as np
-import pandas as pd
-import pytest
-from sklearn.utils._testing import assert_array_equal, skip_if_no_parallel
-from sklearn.exceptions import NotFittedError
-
-from dirty_cat import MinHashEncoder
-
-from .utils import generate_data
-
-
-@pytest.mark.parametrize(
-    "hashing, minmax_hash", [("fast", True), ("fast", False), ("murmur", False)]
-)
-def test_minhash_encoder(hashing, minmax_hash) -> None:
-    X = np.array(["al ice", "b ob", "bob and alice", "alice and bob"])[:, None]
-    # Test output shape
-    encoder = MinHashEncoder(n_components=2, hashing=hashing)
-    encoder.fit(X)
-    y = encoder.transform(X)
-    assert y.shape == (4, 2), str(y.shape)
-    assert len(set(y[0])) == 2
-
-    # Test that using the same seed returns the same output
-    encoder2 = MinHashEncoder(2, hashing=hashing)
-    encoder2.fit(X)
-    y2 = encoder2.transform(X)
-    np.testing.assert_array_equal(y, y2)
-
-    # Test min property
-    if not minmax_hash:
-        X_substring = [x[: x.find(" ")] for x in X[:, 0]]
-        X_substring = np.array(X_substring)[:, None]
-        encoder3 = MinHashEncoder(2, hashing=hashing)
-        encoder3.fit(X_substring)
-        y_substring = encoder3.transform(X_substring)
-        np.testing.assert_array_less(y - y_substring, 0.001)
-
-
-def test_multiple_columns() -> None:
-    """
-    This test aims at verifying that fitting multiple columns
-    with the MinHashEncoder will not produce an error, and will
-    encode the column independently.
-    """
-    X = pd.DataFrame(
-        [
-            ("bird", "parrot"),
-            ("bird", "nightingale"),
-            ("mammal", "monkey"),
-            ("mammal", np.nan),
-        ],
-        columns=("class", "type"),
-    )
-    X1 = X[["class"]]
-    X2 = X[["type"]]
-    fit1 = MinHashEncoder(n_components=30).fit_transform(X1)
-    fit2 = MinHashEncoder(n_components=30).fit_transform(X2)
-    fit = MinHashEncoder(n_components=30).fit_transform(X)
-    assert np.array_equal(
-        np.array([fit[:, :30], fit[:, 30:60]]), np.array([fit1, fit2])
-    )
-
-
-def test_input_type() -> None:
-    # Numpy array
-    X = np.array(["alice", "bob"])[:, None]
-    enc = MinHashEncoder(n_components=2)
-    enc.fit_transform(X)
-    # List
-    X = [["alice"], ["bob"]]
-    enc = MinHashEncoder(n_components=2)
-    enc.fit_transform(X)
-
-
-@pytest.mark.parametrize(
-    "hashing, minmax_hash", [("fast", True), ("fast", False), ("murmur", False)]
-)
-def test_encoder_params(hashing, minmax_hash) -> None:
-    X = generate_data(n_samples=20)
-    enc = MinHashEncoder(
-        n_components=50, hashing=hashing, minmax_hash=minmax_hash, ngram_range=(3, 3)
-    )
-    enc.fit(X)
-    y = enc.transform(X)
-    assert y.shape == (len(X), 50)
-    X2 = np.array([["a", "", "c"]]).T
-    y2 = enc.transform(X2)
-    assert y2.shape == (len(X2), 50)
-
-
-input_types = ["numpy", "pandas"]
-missings = ["error", "zero_impute", "aaa"]
-hashings = ["fast", "murmur", "aaa"]
-
-
-@pytest.mark.parametrize("input_type", input_types)
-@pytest.mark.parametrize("missing", missings)
-@pytest.mark.parametrize("hashing", hashings)
-def test_missing_values(input_type: str, missing: str, hashing: str) -> None:
-    X = ["Red", np.nan, "green", "blue", "green", "green", "blue", float("nan")]
-    n = 3
-    z = np.zeros(n)
-
-    if input_type == "numpy":
-        X = np.array(X, dtype=object)[:, None]
-    elif input_type == "pandas":
-        X = pd.DataFrame(X)
-
-    encoder = MinHashEncoder(
-        n_components=n, hashing=hashing, minmax_hash=False, handle_missing=missing
-    )
-
-    if hashing == "aaa":
-        with pytest.raises(ValueError, match=r"Got hashing="):
-            encoder.fit_transform(X)
-    else:
-        if missing == "error":
-            if input_type in ["numpy", "pandas"]:
-                with pytest.raises(
-                    ValueError, match=r"Found missing values in input data; set"
-                ):
-                    encoder.fit_transform(X)
-        elif missing == "zero_impute":
-            y = encoder.fit_transform(X)
-            assert np.array_equal(y[1], z)
-            assert np.array_equal(y[-1], z)
-        else:
-            with pytest.raises(ValueError, match=r"Got handle_missing="):
-                encoder.fit_transform(X)
-    return
-
-
-def test_missing_values_none():
-    # Test that "None" is also understood as a missing value
-    a = np.array([["a", "b", None, "c"]], dtype=object).T
-
-    enc = MinHashEncoder()
-    d = enc.fit_transform(a)
-    np.testing.assert_array_equal(d[2], 0)
-
-    e = np.array([["a", "b", "", "c"]], dtype=object).T
-    f = enc.fit_transform(e)
-    np.testing.assert_array_equal(f[2], 0)
-
-
-def test_cache_overflow() -> None:
-    # Regression test for cache overflow resulting in -1s in encoding
-    def get_random_string(length):
-        letters = ascii_lowercase
-        result_str = "".join(random.choice(letters) for _ in range(length))
-        return result_str
-
-    encoder = MinHashEncoder(n_components=3)
-    capacity = encoder._capacity
-    raw_data = [get_random_string(10) for _ in range(capacity + 1)]
-    raw_data = np.array(raw_data)[:, None]
-    y = encoder.fit_transform(raw_data)
-
-    assert len(y[y == -1.0]) == 0
-
-
-@skip_if_no_parallel
-def test_parallelism():
-    # Test that parallelism works
-    encoder = MinHashEncoder(n_components=3, n_jobs=1)
-    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
-    y = encoder.fit_transform(X)
-    for n_jobs in [None, 2, -1]:
-        encoder = MinHashEncoder(n_components=3, n_jobs=n_jobs)
-        y_parallel = encoder.fit_transform(X)
-        assert_array_equal(y, y_parallel)
-
-    # Test with threading backend
-    encoder = MinHashEncoder(n_components=3, n_jobs=2)
-    with joblib.parallel_backend("threading"):
-        y_threading = encoder.fit_transform(X)
-    assert_array_equal(y, y_threading)
-    assert encoder.n_jobs == 2
-
-
-DEFAULT_JOBLIB_BACKEND = joblib.parallel.get_active_backend()[0].__class__
-
-
-class DummyBackend(DEFAULT_JOBLIB_BACKEND):  # type: ignore
-    """
-    A dummy backend used to check that specifying a backend works
-    in MinHashEncoder.
-    The `count` attribute is used to check that the backend is used.
-    Copied from https://github.com/scikit-learn/scikit-learn/blob/36958fb240fbe435673a9e3c52e769f01f36bec0/sklearn/ensemble/tests/test_forest.py  # noqa
-    """
-
-    def __init__(self, *args, **kwargs):
-        self.count = 0
-        super().__init__(*args, **kwargs)
-
-    def start_call(self):
-        self.count += 1
-        return super().start_call()
-
-
-joblib.register_parallel_backend("testing", DummyBackend)
-
-
-@skip_if_no_parallel
-def test_backend_respected():
-    """
-    Test that the joblib backend is used.
-    Copied from https://github.com/scikit-learn/scikit-learn/blob/36958fb240fbe435673a9e3c52e769f01f36bec0/sklearn/ensemble/tests/test_forest.py  # noqa
-    """
-    # Test that parallelism works
-    encoder = MinHashEncoder(n_components=3, n_jobs=2)
-    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
-
-    with joblib.parallel_backend("testing") as (ba, n_jobs):
-        encoder.fit_transform(X)
-
-    assert ba.count > 0
-
-
-def test_correct_arguments():
-    # Test that the correct arguments are passed to the hashing function
-    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
-    # Write an incorrect value for the `hashing` argument
-    with pytest.raises(ValueError, match=r"expected any of"):
-        encoder = MinHashEncoder(n_components=3, hashing="incorrect")
-        encoder.fit_transform(X)
-
-    # Write an incorrect value for the `handle_missing` argument
-    with pytest.raises(ValueError, match=r"expected any of"):
-        encoder = MinHashEncoder(n_components=3, handle_missing="incorrect")
-        encoder.fit_transform(X)
-
-    # Use minmax_hash with murmur hashing
-    with pytest.raises(ValueError, match=r"minmax_hash encoding is not supported"):
-        encoder = MinHashEncoder(n_components=2, minmax_hash=True, hashing="murmur")
-        encoder.fit_transform(X)
-
-    # Use minmax_hash with an odd number of components
-    with pytest.raises(ValueError, match=r"n_components should be even"):
-        encoder = MinHashEncoder(n_components=3, minmax_hash=True)
-        encoder.fit_transform(X)
-
-def test_check_fitted_minhash_encoder():
-    """Test that calling transform before fit raises an error"""
-    encoder = MinHashEncoder(n_components=3)
-    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
-    with pytest.raises(NotFittedError):
-        encoder.transform(X)
-    
-    # Check that it works after fitting
-    encoder.fit(X)
-    encoder.transform(X)
-
+import random
+from string import ascii_lowercase
+
+import joblib
+import numpy as np
+import pandas as pd
+import pytest
+from sklearn.exceptions import NotFittedError
+from sklearn.utils._testing import assert_array_equal, skip_if_no_parallel
+
+from dirty_cat import MinHashEncoder
+
+from .utils import generate_data
+
+
+@pytest.mark.parametrize(
+    "hashing, minmax_hash", [("fast", True), ("fast", False), ("murmur", False)]
+)
+def test_minhash_encoder(hashing, minmax_hash) -> None:
+    X = np.array(["al ice", "b ob", "bob and alice", "alice and bob"])[:, None]
+    # Test output shape
+    encoder = MinHashEncoder(n_components=2, hashing=hashing)
+    encoder.fit(X)
+    y = encoder.transform(X)
+    assert y.shape == (4, 2), str(y.shape)
+    assert len(set(y[0])) == 2
+
+    # Test that using the same seed returns the same output
+    encoder2 = MinHashEncoder(2, hashing=hashing)
+    encoder2.fit(X)
+    y2 = encoder2.transform(X)
+    np.testing.assert_array_equal(y, y2)
+
+    # Test min property
+    if not minmax_hash:
+        X_substring = [x[: x.find(" ")] for x in X[:, 0]]
+        X_substring = np.array(X_substring)[:, None]
+        encoder3 = MinHashEncoder(2, hashing=hashing)
+        encoder3.fit(X_substring)
+        y_substring = encoder3.transform(X_substring)
+        np.testing.assert_array_less(y - y_substring, 0.001)
+
+
+def test_multiple_columns() -> None:
+    """
+    This test aims at verifying that fitting multiple columns
+    with the MinHashEncoder will not produce an error, and will
+    encode the column independently.
+    """
+    X = pd.DataFrame(
+        [
+            ("bird", "parrot"),
+            ("bird", "nightingale"),
+            ("mammal", "monkey"),
+            ("mammal", np.nan),
+        ],
+        columns=("class", "type"),
+    )
+    X1 = X[["class"]]
+    X2 = X[["type"]]
+    fit1 = MinHashEncoder(n_components=30).fit_transform(X1)
+    fit2 = MinHashEncoder(n_components=30).fit_transform(X2)
+    fit = MinHashEncoder(n_components=30).fit_transform(X)
+    assert np.array_equal(
+        np.array([fit[:, :30], fit[:, 30:60]]), np.array([fit1, fit2])
+    )
+
+
+def test_input_type() -> None:
+    # Numpy array
+    X = np.array(["alice", "bob"])[:, None]
+    enc = MinHashEncoder(n_components=2)
+    enc.fit_transform(X)
+    # List
+    X = [["alice"], ["bob"]]
+    enc = MinHashEncoder(n_components=2)
+    enc.fit_transform(X)
+
+
+@pytest.mark.parametrize(
+    "hashing, minmax_hash", [("fast", True), ("fast", False), ("murmur", False)]
+)
+def test_encoder_params(hashing, minmax_hash) -> None:
+    X = generate_data(n_samples=20)
+    enc = MinHashEncoder(
+        n_components=50, hashing=hashing, minmax_hash=minmax_hash, ngram_range=(3, 3)
+    )
+    enc.fit(X)
+    y = enc.transform(X)
+    assert y.shape == (len(X), 50)
+    X2 = np.array([["a", "", "c"]]).T
+    y2 = enc.transform(X2)
+    assert y2.shape == (len(X2), 50)
+
+
+@pytest.mark.parametrize("input_type", ["numpy", "pandas"])
+@pytest.mark.parametrize("missing", ["error", "zero_impute", "aaa"])
+@pytest.mark.parametrize("hashing", ["fast", "murmur", "aaa"])
+def test_missing_values(input_type: str, missing: str, hashing: str) -> None:
+    X = ["Red", np.nan, "green", "blue", "green", "green", "blue", float("nan")]
+    n = 3
+    z = np.zeros(n)
+
+    if input_type == "numpy":
+        X = np.array(X, dtype=object)[:, None]
+    elif input_type == "pandas":
+        X = pd.DataFrame(X)
+
+    encoder = MinHashEncoder(
+        n_components=n, hashing=hashing, minmax_hash=False, handle_missing=missing
+    )
+
+    if hashing == "aaa":
+        with pytest.raises(ValueError, match=r"Got hashing="):
+            encoder.fit_transform(X)
+    else:
+        if missing == "error":
+            if input_type in ["numpy", "pandas"]:
+                with pytest.raises(
+                    ValueError, match=r"Found missing values in input data; set"
+                ):
+                    encoder.fit_transform(X)
+        elif missing == "zero_impute":
+            y = encoder.fit_transform(X)
+            assert np.array_equal(y[1], z)
+            assert np.array_equal(y[-1], z)
+        else:
+            with pytest.raises(ValueError, match=r"Got handle_missing="):
+                encoder.fit_transform(X)
+    return
+
+
+def test_missing_values_none():
+    # Test that "None" is also understood as a missing value
+    a = np.array([["a", "b", None, "c"]], dtype=object).T
+
+    enc = MinHashEncoder()
+    d = enc.fit_transform(a)
+    np.testing.assert_array_equal(d[2], 0)
+
+    e = np.array([["a", "b", "", "c"]], dtype=object).T
+    f = enc.fit_transform(e)
+    np.testing.assert_array_equal(f[2], 0)
+
+
+def test_cache_overflow() -> None:
+    # Regression test for cache overflow resulting in -1s in encoding
+    def get_random_string(length):
+        letters = ascii_lowercase
+        result_str = "".join(random.choice(letters) for _ in range(length))
+        return result_str
+
+    encoder = MinHashEncoder(n_components=3)
+    capacity = encoder._capacity
+    raw_data = [get_random_string(10) for _ in range(capacity + 1)]
+    raw_data = np.array(raw_data)[:, None]
+    y = encoder.fit_transform(raw_data)
+
+    assert len(y[y == -1.0]) == 0
+
+
+@skip_if_no_parallel
+def test_parallelism():
+    # Test that parallelism works
+    encoder = MinHashEncoder(n_components=3, n_jobs=1)
+    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
+    y = encoder.fit_transform(X)
+    for n_jobs in [None, 2, -1]:
+        encoder = MinHashEncoder(n_components=3, n_jobs=n_jobs)
+        y_parallel = encoder.fit_transform(X)
+        assert_array_equal(y, y_parallel)
+
+    # Test with threading backend
+    encoder = MinHashEncoder(n_components=3, n_jobs=2)
+    with joblib.parallel_backend("threading"):
+        y_threading = encoder.fit_transform(X)
+    assert_array_equal(y, y_threading)
+    assert encoder.n_jobs == 2
+
+
+DEFAULT_JOBLIB_BACKEND = joblib.parallel.get_active_backend()[0].__class__
+
+
+class DummyBackend(DEFAULT_JOBLIB_BACKEND):  # type: ignore
+    """
+    A dummy backend used to check that specifying a backend works
+    in MinHashEncoder.
+    The `count` attribute is used to check that the backend is used.
+    Copied from https://github.com/scikit-learn/scikit-learn/blob/36958fb240fbe435673a9e3c52e769f01f36bec0/sklearn/ensemble/tests/test_forest.py  # noqa
+    """
+
+    def __init__(self, *args, **kwargs):
+        self.count = 0
+        super().__init__(*args, **kwargs)
+
+    def start_call(self):
+        self.count += 1
+        return super().start_call()
+
+
+joblib.register_parallel_backend("testing", DummyBackend)
+
+
+@skip_if_no_parallel
+def test_backend_respected():
+    """
+    Test that the joblib backend is used.
+    Copied from https://github.com/scikit-learn/scikit-learn/blob/36958fb240fbe435673a9e3c52e769f01f36bec0/sklearn/ensemble/tests/test_forest.py  # noqa
+    """
+    # Test that parallelism works
+    encoder = MinHashEncoder(n_components=3, n_jobs=2)
+    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
+
+    with joblib.parallel_backend("testing") as (ba, n_jobs):
+        encoder.fit_transform(X)
+
+    assert ba.count > 0
+
+
+def test_correct_arguments():
+    # Test that the correct arguments are passed to the hashing function
+    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
+    # Write an incorrect value for the `hashing` argument
+    with pytest.raises(ValueError, match=r"expected any of"):
+        encoder = MinHashEncoder(n_components=3, hashing="incorrect")
+        encoder.fit_transform(X)
+
+    # Write an incorrect value for the `handle_missing` argument
+    with pytest.raises(ValueError, match=r"expected any of"):
+        encoder = MinHashEncoder(n_components=3, handle_missing="incorrect")
+        encoder.fit_transform(X)
+
+    # Use minmax_hash with murmur hashing
+    with pytest.raises(ValueError, match=r"minmax_hash encoding is not supported"):
+        encoder = MinHashEncoder(n_components=2, minmax_hash=True, hashing="murmur")
+        encoder.fit_transform(X)
+
+    # Use minmax_hash with an odd number of components
+    with pytest.raises(ValueError, match=r"n_components should be even"):
+        encoder = MinHashEncoder(n_components=3, minmax_hash=True)
+        encoder.fit_transform(X)
+
+
+def test_check_fitted_minhash_encoder():
+    """Test that calling transform before fit raises an error"""
+    encoder = MinHashEncoder(n_components=3)
+    X = np.array(["a", "b", "c", "d", "e", "f", "g", "h"])[:, None]
+    with pytest.raises(NotFittedError):
+        encoder.transform(X)
+
+    # Check that it works after fitting
+    encoder.fit(X)
+    encoder.transform(X)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_similarity_encoder.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_similarity_encoder.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-from typing import Callable, Optional
-
-import numpy as np
-import numpy.testing
-import pytest
-from sklearn import __version__ as sklearn_version
-from sklearn.exceptions import NotFittedError
-
-from dirty_cat import SimilarityEncoder
-from dirty_cat._similarity_encoder import get_kmeans_prototypes, ngram_similarity_matrix
-from dirty_cat._string_distances import ngram_similarity
-from dirty_cat._utils import parse_version
-
-
-def test_specifying_categories() -> None:
-    # When creating a new SimilarityEncoder:
-    # - if categories = 'auto', the categories are the sorted, unique training
-    # set observations (for each column)
-    # - if categories is a list (of lists), the categories for each column are
-    # each item in the list
-
-    # In this test, we first find the sorted, unique categories in the training
-    # set, and create a SimilarityEncoder by giving it explicitly the computed
-    # categories. The test consists in making sure the transformed observations
-    # given by this encoder are equal to the transformed observations in the
-    # case of a SimilarityEncoder created with categories = 'auto'
-
-    observations = [["bar"], ["foo"]]
-    categories = [["bar", "foo"]]
-
-    sim_enc_with_cat = SimilarityEncoder(categories=categories, ngram_range=(2, 3))
-    sim_enc_auto_cat = SimilarityEncoder(ngram_range=(2, 3))
-
-    feature_matrix_with_cat = sim_enc_with_cat.fit_transform(observations)
-    feature_matrix_auto_cat = sim_enc_auto_cat.fit_transform(observations)
-
-    assert np.allclose(feature_matrix_auto_cat, feature_matrix_with_cat)
-
-
-def test_fast_ngram_similarity() -> None:
-    vocabulary = [["bar", "foo"]]
-    observations = [["foo"], ["baz"]]
-
-    sim_enc = SimilarityEncoder(ngram_range=(2, 2), categories=vocabulary)
-
-    sim_enc.fit(observations)
-    feature_matrix = sim_enc.transform(observations, fast=False)
-    feature_matrix_fast = sim_enc.transform(observations, fast=True)
-
-    assert np.allclose(feature_matrix, feature_matrix_fast)
-
-
-def test_parameters():
-    X = [["foo"], ["baz"]]
-    X2 = [["foo"], ["bar"]]
-    with pytest.raises(ValueError, match=r"Got handle_unknown="):
-        SimilarityEncoder(handle_unknown="bb").fit(X)
-    with pytest.raises(ValueError, match=r"Got hashing_dim="):
-        SimilarityEncoder(hashing_dim="bb").fit(X)
-    with pytest.raises(ValueError, match=r"Got categories="):
-        SimilarityEncoder(categories="bb")
-    with pytest.raises(ValueError, match=r"Unsorted categories "):
-        SimilarityEncoder(categories=[["cat2", "cat1"], ["cat3", "cat4"]]).fit(X)
-    with pytest.raises(ValueError, match=r"Found unknown categories "):
-        SimilarityEncoder(categories=[["fooo", "loo"]], handle_unknown="error").fit(X)
-    with pytest.raises(ValueError, match=r"Found unknown categories "):
-        sim = SimilarityEncoder(categories=[["baz", "foo"]], handle_unknown="error")
-        sim.fit(X)
-        sim.transform(X2)
-
-
-def _test_missing_values(input_type, missing):
-    observations = [["a", "b"], ["b", "a"], ["b", np.nan], ["a", "c"], [np.nan, "a"]]
-    encoded = np.array(
-        [
-            [0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
-            [0.0, 0.0, 1.0, 0.0, 1.0, 0.0, 0.0],
-            [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
-            [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 1.0],
-            [0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
-        ]
-    )
-
-    if input_type == "numpy":
-        observations = np.array(observations, dtype=object)
-    elif input_type == "pandas":
-        pd = pytest.importorskip("pandas")
-        observations = pd.DataFrame(observations)
-
-    sim_enc = SimilarityEncoder(handle_missing=missing)
-    if missing == "error":
-        with pytest.raises(ValueError, match=r"Found missing values in input"):
-            sim_enc.fit_transform(observations)
-    elif missing == "":
-        ans = sim_enc.fit_transform(observations)
-        assert np.allclose(encoded, ans)
-    else:
-        with pytest.raises(ValueError, match=r"expected any of"):
-            sim_enc.fit_transform(observations)
-        return
-
-
-def _test_missing_values_transform(input_type: str, missing: str) -> None:
-    observations = [["a", "b"], ["b", "a"], ["b", "b"], ["a", "c"], ["c", "a"]]
-    test_observations = [
-        ["a", "b"],
-        ["b", "a"],
-        ["b", np.nan],
-        ["a", "c"],
-        [np.nan, "a"],
-    ]
-    encoded = np.array(
-        [
-            [1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
-            [0.0, 1.0, 0.0, 1.0, 0.0, 0.0],
-            [0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
-            [1.0, 0.0, 0.0, 0.0, 0.0, 1.0],
-            [0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
-        ]
-    )
-
-    if input_type == "numpy":
-        test_observations = np.array(test_observations, dtype=object)
-    elif input_type == "pandas":
-        pd = pytest.importorskip("pandas")
-        test_observations = pd.DataFrame(test_observations)
-
-    sim_enc = SimilarityEncoder(handle_missing=missing)
-    if missing == "error":
-        sim_enc.fit_transform(observations)
-        with pytest.raises(ValueError, match=r"Found missing values in input"):
-            sim_enc.transform(test_observations)
-    elif missing == "":
-        sim_enc.fit_transform(observations)
-        ans = sim_enc.transform(test_observations)
-        assert np.allclose(encoded, ans)
-
-
-def _test_similarity(
-    similarity_f: Callable,
-    hashing_dim: Optional[int] = None,
-    categories: str = "auto",
-    n_prototypes: int = None,
-) -> None:
-    if n_prototypes is None:
-        X = np.array(["aa", "aaa", "aaab"]).reshape(-1, 1)
-        X_test = np.array([["Aa", "aAa", "aaa", "aaab", " aaa  c"]]).reshape(-1, 1)
-
-        model = SimilarityEncoder(
-            hashing_dim=hashing_dim,
-            categories=categories,
-            n_prototypes=n_prototypes,
-            ngram_range=(3, 3),
-        )
-
-        encoder = model.fit(X).transform(X_test)
-
-        ans = np.zeros((len(X_test), len(X)))
-        for i, x_t in enumerate(X_test.reshape(-1)):
-            for j, x in enumerate(X.reshape(-1)):
-                ans[i, j] = similarity_f(x_t, x, 3)
-        numpy.testing.assert_almost_equal(encoder, ans)
-    else:
-        X = np.array(
-            ["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"]
-        ).reshape(-1, 1)
-        X_test = np.array([["Aa", "aAa", "aaa", "aaab", " aaa  c"]]).reshape(-1, 1)
-
-        if categories == "auto":
-            with pytest.warns(UserWarning, match=r"n_prototypes parameter ignored"):
-                SimilarityEncoder(
-                    categories=categories,
-                    n_prototypes=n_prototypes,
-                )
-        try:
-            model = SimilarityEncoder(
-                hashing_dim=hashing_dim,
-                categories=categories,
-                n_prototypes=n_prototypes,
-                random_state=42,
-                ngram_range=(3, 3),
-            )
-        except ValueError as e:
-            assert (
-                e.__str__()
-                == "n_prototypes expected None or a positive non null integer. "
-            )
-            return
-
-        encoder = model.fit(X).transform(X_test)
-        if n_prototypes == 1:
-            assert model.categories_ == ["aaa"]
-        elif n_prototypes == 2:
-            a = [np.array(["aaa", "aaab"], dtype="<U4")]
-            assert np.array_equal(a, model.categories_)
-        elif n_prototypes == 3:
-            a = [np.array(["aaa", "aaab", "aac"], dtype="<U4")]
-            assert np.array_equal(a, model.categories_)
-
-        ans = np.zeros((len(X_test), len(np.array(model.categories_).reshape(-1))))
-        for i, x_t in enumerate(X_test.reshape(-1)):
-            for j, x in enumerate(np.array(model.categories_).reshape(-1)):
-                ans[i, j] = similarity_f(x_t, x, 3)
-
-        numpy.testing.assert_almost_equal(encoder, ans)
-
-
-def test_similarity_encoder() -> None:
-    categories = ["auto", "most_frequent", "k-means"]
-    for category in categories:
-        if category == "auto":
-            _test_similarity(
-                ngram_similarity,
-                categories=category,
-                n_prototypes=None,
-            )
-            _test_similarity(
-                ngram_similarity,
-                hashing_dim=2**16,
-                categories=category,
-            )
-            _test_similarity(ngram_similarity, categories=category, n_prototypes=4)
-        else:
-            for i in range(0, 4):
-                _test_similarity(
-                    ngram_similarity,
-                    categories=category,
-                    n_prototypes=i,
-                )
-                _test_similarity(
-                    ngram_similarity,
-                    hashing_dim=2**16,
-                    categories=category,
-                    n_prototypes=i,
-                )
-
-    input_types = ["list", "numpy", "pandas"]
-    handle_missing = ["aaa", "error", ""]
-    for input_type in input_types:
-        for missing in handle_missing:
-            _test_missing_values(input_type, missing)
-            _test_missing_values_transform(input_type, missing)
-
-
-def test_kmeans_protoypes() -> None:
-    X_test = np.array(["cbbba", "baaac", "accc"])
-    proto = get_kmeans_prototypes(X_test, 3, sparse=True)
-    assert np.array_equal(np.sort(proto), np.sort(X_test))
-    X_test_2 = np.array(["aa", "bb", "cc", "bbb"])
-    with pytest.warns(UserWarning, match=r"number of unique prototypes is lower "):
-        get_kmeans_prototypes(X_test_2, 4)
-
-
-def test_ngram_similarity_matrix() -> None:
-    X1 = np.array(["cat1", "cat2", "cat3"])
-    X2 = np.array(["cata1", "caat2", "ccat3"])
-    sim = ngram_similarity_matrix(X1, X2, ngram_range=(2, 2), hashing_dim=5)
-    assert sim.shape == (len(X1), len(X2))
-
-
-def test_reproducibility() -> None:
-    sim_enc = SimilarityEncoder(
-        categories="k-means",
-        n_prototypes=10,
-        random_state=435,
-    )
-    X = np.array([" %s " % chr(i) for i in range(32, 127)]).reshape((-1, 1))
-    prototypes = sim_enc.fit(X).categories_[0]
-    for i in range(10):
-        assert np.array_equal(prototypes, sim_enc.fit(X).categories_[0])
-
-
-def test_fit_transform():
-    X = [["foo"], ["baz"]]
-    y = ["foo", "bar"]
-    tr1 = SimilarityEncoder().fit_transform(X, y)
-    sim = SimilarityEncoder()
-    sim.fit(X, y)
-    tr2 = sim.transform(X, y)
-    assert np.array_equal(tr1, tr2)
-
-
-def test_get_features() -> None:
-    # See https://github.com/dirty-cat/dirty_cat/issues/168
-    sim_enc = SimilarityEncoder(random_state=435)
-    X = np.array(["%s" % chr(i) for i in range(32, 127)]).reshape((-1, 1))
-    sim_enc.fit(X)
-    if parse_version(sklearn_version) < parse_version("1.0"):
-        feature_names = sim_enc.get_feature_names()
-    else:
-        feature_names = sim_enc.get_feature_names_out()
-    assert feature_names.tolist() == [
-        "x0_ ",
-        "x0_!",
-        'x0_"',
-        "x0_#",
-        "x0_$",
-        "x0_%",
-        "x0_&",
-        "x0_'",
-        "x0_(",
-        "x0_)",
-        "x0_*",
-        "x0_+",
-        "x0_,",
-        "x0_-",
-        "x0_.",
-        "x0_/",
-        "x0_0",
-        "x0_1",
-        "x0_2",
-        "x0_3",
-        "x0_4",
-        "x0_5",
-        "x0_6",
-        "x0_7",
-        "x0_8",
-        "x0_9",
-        "x0_:",
-        "x0_;",
-        "x0_<",
-        "x0_=",
-        "x0_>",
-        "x0_?",
-        "x0_@",
-        "x0_A",
-        "x0_B",
-        "x0_C",
-        "x0_D",
-        "x0_E",
-        "x0_F",
-        "x0_G",
-        "x0_H",
-        "x0_I",
-        "x0_J",
-        "x0_K",
-        "x0_L",
-        "x0_M",
-        "x0_N",
-        "x0_O",
-        "x0_P",
-        "x0_Q",
-        "x0_R",
-        "x0_S",
-        "x0_T",
-        "x0_U",
-        "x0_V",
-        "x0_W",
-        "x0_X",
-        "x0_Y",
-        "x0_Z",
-        "x0_[",
-        "x0_\\",
-        "x0_]",
-        "x0_^",
-        "x0__",
-        "x0_`",
-        "x0_a",
-        "x0_b",
-        "x0_c",
-        "x0_d",
-        "x0_e",
-        "x0_f",
-        "x0_g",
-        "x0_h",
-        "x0_i",
-        "x0_j",
-        "x0_k",
-        "x0_l",
-        "x0_m",
-        "x0_n",
-        "x0_o",
-        "x0_p",
-        "x0_q",
-        "x0_r",
-        "x0_s",
-        "x0_t",
-        "x0_u",
-        "x0_v",
-        "x0_w",
-        "x0_x",
-        "x0_y",
-        "x0_z",
-        "x0_{",
-        "x0_|",
-        "x0_}",
-        "x0_~",
-    ]
-
-def test_check_fitted_super_vectorizer():
-    """Test that calling transform before fit raises an error"""
-    sim_enc = SimilarityEncoder()
-    X = np.array(["%s" % chr(i) for i in range(32, 127)]).reshape((-1, 1))
-    with pytest.raises(NotFittedError):
-        sim_enc.transform(X)
-    sim_enc.fit(X)
-    sim_enc.transform(X)
+from typing import Callable, Optional
+
+import numpy as np
+import numpy.testing
+import pytest
+from sklearn import __version__ as sklearn_version
+from sklearn.exceptions import NotFittedError
+
+from dirty_cat import SimilarityEncoder
+from dirty_cat._similarity_encoder import get_kmeans_prototypes, ngram_similarity_matrix
+from dirty_cat._string_distances import ngram_similarity
+from dirty_cat._utils import parse_version
+
+
+def test_specifying_categories() -> None:
+    # When creating a new SimilarityEncoder:
+    # - if categories = 'auto', the categories are the sorted, unique training
+    # set observations (for each column)
+    # - if categories is a list (of lists), the categories for each column are
+    # each item in the list
+
+    # In this test, we first find the sorted, unique categories in the training
+    # set, and create a SimilarityEncoder by giving it explicitly the computed
+    # categories. The test consists in making sure the transformed observations
+    # given by this encoder are equal to the transformed observations in the
+    # case of a SimilarityEncoder created with categories = 'auto'
+
+    observations = [["bar"], ["foo"]]
+    categories = [["bar", "foo"]]
+
+    sim_enc_with_cat = SimilarityEncoder(categories=categories, ngram_range=(2, 3))
+    sim_enc_auto_cat = SimilarityEncoder(ngram_range=(2, 3))
+
+    feature_matrix_with_cat = sim_enc_with_cat.fit_transform(observations)
+    feature_matrix_auto_cat = sim_enc_auto_cat.fit_transform(observations)
+
+    assert np.allclose(feature_matrix_auto_cat, feature_matrix_with_cat)
+
+
+def test_fast_ngram_similarity() -> None:
+    vocabulary = [["bar", "foo"]]
+    observations = [["foo"], ["baz"]]
+
+    sim_enc = SimilarityEncoder(ngram_range=(2, 2), categories=vocabulary)
+
+    sim_enc.fit(observations)
+    feature_matrix = sim_enc.transform(observations, fast=False)
+    feature_matrix_fast = sim_enc.transform(observations, fast=True)
+
+    assert np.allclose(feature_matrix, feature_matrix_fast)
+
+
+def test_parameters():
+    X = [["foo"], ["baz"]]
+    X2 = [["foo"], ["bar"]]
+    with pytest.raises(ValueError, match=r"Got handle_unknown="):
+        SimilarityEncoder(handle_unknown="bb").fit(X)
+    with pytest.raises(ValueError, match=r"Got hashing_dim="):
+        SimilarityEncoder(hashing_dim="bb").fit(X)
+    with pytest.raises(ValueError, match=r"Got categories="):
+        SimilarityEncoder(categories="bb")
+    with pytest.raises(ValueError, match=r"Unsorted categories "):
+        SimilarityEncoder(categories=[["cat2", "cat1"], ["cat3", "cat4"]]).fit(X)
+    with pytest.raises(ValueError, match=r"Found unknown categories "):
+        SimilarityEncoder(categories=[["fooo", "loo"]], handle_unknown="error").fit(X)
+    with pytest.raises(ValueError, match=r"Found unknown categories "):
+        sim = SimilarityEncoder(categories=[["baz", "foo"]], handle_unknown="error")
+        sim.fit(X)
+        sim.transform(X2)
+
+
+def _test_missing_values(input_type, missing):
+    observations = [["a", "b"], ["b", "a"], ["b", np.nan], ["a", "c"], [np.nan, "a"]]
+    encoded = np.array(
+        [
+            [0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+            [0.0, 0.0, 1.0, 0.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 1.0],
+            [0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
+        ]
+    )
+
+    if input_type == "numpy":
+        observations = np.array(observations, dtype=object)
+    elif input_type == "pandas":
+        pd = pytest.importorskip("pandas")
+        observations = pd.DataFrame(observations)
+
+    sim_enc = SimilarityEncoder(handle_missing=missing)
+    if missing == "error":
+        with pytest.raises(ValueError, match=r"Found missing values in input"):
+            sim_enc.fit_transform(observations)
+    elif missing == "":
+        ans = sim_enc.fit_transform(observations)
+        assert np.allclose(encoded, ans)
+    else:
+        with pytest.raises(ValueError, match=r"expected any of"):
+            sim_enc.fit_transform(observations)
+        return
+
+
+def _test_missing_values_transform(input_type: str, missing: str) -> None:
+    observations = [["a", "b"], ["b", "a"], ["b", "b"], ["a", "c"], ["c", "a"]]
+    test_observations = [
+        ["a", "b"],
+        ["b", "a"],
+        ["b", np.nan],
+        ["a", "c"],
+        [np.nan, "a"],
+    ]
+    encoded = np.array(
+        [
+            [1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+            [0.0, 1.0, 0.0, 1.0, 0.0, 0.0],
+            [0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
+            [1.0, 0.0, 0.0, 0.0, 0.0, 1.0],
+            [0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
+        ]
+    )
+
+    if input_type == "numpy":
+        test_observations = np.array(test_observations, dtype=object)
+    elif input_type == "pandas":
+        pd = pytest.importorskip("pandas")
+        test_observations = pd.DataFrame(test_observations)
+
+    sim_enc = SimilarityEncoder(handle_missing=missing)
+    if missing == "error":
+        sim_enc.fit_transform(observations)
+        with pytest.raises(ValueError, match=r"Found missing values in input"):
+            sim_enc.transform(test_observations)
+    elif missing == "":
+        sim_enc.fit_transform(observations)
+        ans = sim_enc.transform(test_observations)
+        assert np.allclose(encoded, ans)
+
+
+def _test_similarity(
+    similarity_f: Callable,
+    hashing_dim: Optional[int] = None,
+    categories: str = "auto",
+    n_prototypes: int = None,
+) -> None:
+    if n_prototypes is None:
+        X = np.array(["aa", "aaa", "aaab"]).reshape(-1, 1)
+        X_test = np.array([["Aa", "aAa", "aaa", "aaab", " aaa  c"]]).reshape(-1, 1)
+
+        model = SimilarityEncoder(
+            hashing_dim=hashing_dim,
+            categories=categories,
+            n_prototypes=n_prototypes,
+            ngram_range=(3, 3),
+        )
+
+        encoder = model.fit(X).transform(X_test)
+
+        ans = np.zeros((len(X_test), len(X)))
+        for i, x_t in enumerate(X_test.reshape(-1)):
+            for j, x in enumerate(X.reshape(-1)):
+                ans[i, j] = similarity_f(x_t, x, 3)
+        numpy.testing.assert_almost_equal(encoder, ans)
+    else:
+        X = np.array(
+            ["aac", "aaa", "aaab", "aaa", "aaab", "aaa", "aaab", "aaa"]
+        ).reshape(-1, 1)
+        X_test = np.array([["Aa", "aAa", "aaa", "aaab", " aaa  c"]]).reshape(-1, 1)
+
+        if categories == "auto":
+            with pytest.warns(UserWarning, match=r"n_prototypes parameter ignored"):
+                SimilarityEncoder(
+                    categories=categories,
+                    n_prototypes=n_prototypes,
+                )
+        try:
+            model = SimilarityEncoder(
+                hashing_dim=hashing_dim,
+                categories=categories,
+                n_prototypes=n_prototypes,
+                random_state=42,
+                ngram_range=(3, 3),
+            )
+        except ValueError as e:
+            assert (
+                e.__str__()
+                == "n_prototypes expected None or a positive non null integer. "
+            )
+            return
+
+        encoder = model.fit(X).transform(X_test)
+        if n_prototypes == 1:
+            assert model.categories_ == ["aaa"]
+        elif n_prototypes == 2:
+            a = [np.array(["aaa", "aaab"], dtype="<U4")]
+            assert np.array_equal(a, model.categories_)
+        elif n_prototypes == 3:
+            a = [np.array(["aaa", "aaab", "aac"], dtype="<U4")]
+            assert np.array_equal(a, model.categories_)
+
+        ans = np.zeros((len(X_test), len(np.array(model.categories_).reshape(-1))))
+        for i, x_t in enumerate(X_test.reshape(-1)):
+            for j, x in enumerate(np.array(model.categories_).reshape(-1)):
+                ans[i, j] = similarity_f(x_t, x, 3)
+
+        numpy.testing.assert_almost_equal(encoder, ans)
+
+
+def test_similarity_encoder() -> None:
+    categories = ["auto", "most_frequent", "k-means"]
+    for category in categories:
+        if category == "auto":
+            _test_similarity(
+                ngram_similarity,
+                categories=category,
+                n_prototypes=None,
+            )
+            _test_similarity(
+                ngram_similarity,
+                hashing_dim=2**16,
+                categories=category,
+            )
+            _test_similarity(ngram_similarity, categories=category, n_prototypes=4)
+        else:
+            for i in range(0, 4):
+                _test_similarity(
+                    ngram_similarity,
+                    categories=category,
+                    n_prototypes=i,
+                )
+                _test_similarity(
+                    ngram_similarity,
+                    hashing_dim=2**16,
+                    categories=category,
+                    n_prototypes=i,
+                )
+
+    input_types = ["list", "numpy", "pandas"]
+    handle_missing = ["aaa", "error", ""]
+    for input_type in input_types:
+        for missing in handle_missing:
+            _test_missing_values(input_type, missing)
+            _test_missing_values_transform(input_type, missing)
+
+
+def test_kmeans_protoypes() -> None:
+    X_test = np.array(["cbbba", "baaac", "accc"])
+    proto = get_kmeans_prototypes(X_test, 3, sparse=True)
+    assert np.array_equal(np.sort(proto), np.sort(X_test))
+    X_test_2 = np.array(["aa", "bb", "cc", "bbb"])
+    with pytest.warns(UserWarning, match=r"number of unique prototypes is lower "):
+        get_kmeans_prototypes(X_test_2, 4)
+
+
+def test_ngram_similarity_matrix() -> None:
+    X1 = np.array(["cat1", "cat2", "cat3"])
+    X2 = np.array(["cata1", "caat2", "ccat3"])
+    sim = ngram_similarity_matrix(X1, X2, ngram_range=(2, 2), hashing_dim=5)
+    assert sim.shape == (len(X1), len(X2))
+
+
+def test_reproducibility() -> None:
+    sim_enc = SimilarityEncoder(
+        categories="k-means",
+        n_prototypes=10,
+        random_state=435,
+    )
+    X = np.array([" %s " % chr(i) for i in range(32, 127)]).reshape((-1, 1))
+    prototypes = sim_enc.fit(X).categories_[0]
+    for i in range(10):
+        assert np.array_equal(prototypes, sim_enc.fit(X).categories_[0])
+
+
+def test_fit_transform():
+    X = [["foo"], ["baz"]]
+    y = ["foo", "bar"]
+    tr1 = SimilarityEncoder().fit_transform(X, y)
+    sim = SimilarityEncoder()
+    sim.fit(X, y)
+    tr2 = sim.transform(X, y)
+    assert np.array_equal(tr1, tr2)
+
+
+def test_get_features() -> None:
+    # See https://github.com/dirty-cat/dirty_cat/issues/168
+    sim_enc = SimilarityEncoder(random_state=435)
+    X = np.array(["%s" % chr(i) for i in range(32, 127)]).reshape((-1, 1))
+    sim_enc.fit(X)
+    if parse_version(sklearn_version) < parse_version("1.0"):
+        feature_names = sim_enc.get_feature_names()
+    else:
+        feature_names = sim_enc.get_feature_names_out()
+    assert feature_names.tolist() == [
+        "x0_ ",
+        "x0_!",
+        'x0_"',
+        "x0_#",
+        "x0_$",
+        "x0_%",
+        "x0_&",
+        "x0_'",
+        "x0_(",
+        "x0_)",
+        "x0_*",
+        "x0_+",
+        "x0_,",
+        "x0_-",
+        "x0_.",
+        "x0_/",
+        "x0_0",
+        "x0_1",
+        "x0_2",
+        "x0_3",
+        "x0_4",
+        "x0_5",
+        "x0_6",
+        "x0_7",
+        "x0_8",
+        "x0_9",
+        "x0_:",
+        "x0_;",
+        "x0_<",
+        "x0_=",
+        "x0_>",
+        "x0_?",
+        "x0_@",
+        "x0_A",
+        "x0_B",
+        "x0_C",
+        "x0_D",
+        "x0_E",
+        "x0_F",
+        "x0_G",
+        "x0_H",
+        "x0_I",
+        "x0_J",
+        "x0_K",
+        "x0_L",
+        "x0_M",
+        "x0_N",
+        "x0_O",
+        "x0_P",
+        "x0_Q",
+        "x0_R",
+        "x0_S",
+        "x0_T",
+        "x0_U",
+        "x0_V",
+        "x0_W",
+        "x0_X",
+        "x0_Y",
+        "x0_Z",
+        "x0_[",
+        "x0_\\",
+        "x0_]",
+        "x0_^",
+        "x0__",
+        "x0_`",
+        "x0_a",
+        "x0_b",
+        "x0_c",
+        "x0_d",
+        "x0_e",
+        "x0_f",
+        "x0_g",
+        "x0_h",
+        "x0_i",
+        "x0_j",
+        "x0_k",
+        "x0_l",
+        "x0_m",
+        "x0_n",
+        "x0_o",
+        "x0_p",
+        "x0_q",
+        "x0_r",
+        "x0_s",
+        "x0_t",
+        "x0_u",
+        "x0_v",
+        "x0_w",
+        "x0_x",
+        "x0_y",
+        "x0_z",
+        "x0_{",
+        "x0_|",
+        "x0_}",
+        "x0_~",
+    ]
+
+def test_check_fitted_super_vectorizer():
+    """Test that calling transform before fit raises an error"""
+    sim_enc = SimilarityEncoder()
+    X = np.array(["%s" % chr(i) for i in range(32, 127)]).reshape((-1, 1))
+    with pytest.raises(NotFittedError):
+        sim_enc.transform(X)
+    sim_enc.fit(X)
+    sim_enc.transform(X)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_sklearn.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_sklearn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from sklearn.utils.estimator_checks import check_estimator
-
-from dirty_cat import (
-    DatetimeEncoder,
-    GapEncoder,
-    MinHashEncoder,
-    SimilarityEncoder,
-    TargetEncoder,
-)
-
-
-def test_sklearn_compatible_DatetimeEncoder():
-    check_estimator(DatetimeEncoder())
-
-
-def test_sklearn_compatible_GapEncoder():
-    check_estimator(GapEncoder())
-
-
-def test_sklearn_compatible_MinHashEncoder():
-    check_estimator(MinHashEncoder())
-
-
-def test_sklearn_compatible_SimilarityEncoder():
-    check_estimator(SimilarityEncoder())
-
-
-# def test_sklearn_compatible_SuperVectorizer():
-#    check_estimator(SuperVectorizer())
-
-
-def test_sklearn_compatible_TargetEncoder():
-    check_estimator(TargetEncoder())
+from sklearn.utils.estimator_checks import check_estimator
+
+from dirty_cat import (
+    DatetimeEncoder,
+    GapEncoder,
+    MinHashEncoder,
+    SimilarityEncoder,
+    TargetEncoder,
+)
+
+
+def test_sklearn_compatible_DatetimeEncoder():
+    check_estimator(DatetimeEncoder())
+
+
+def test_sklearn_compatible_GapEncoder():
+    check_estimator(GapEncoder())
+
+
+def test_sklearn_compatible_MinHashEncoder():
+    check_estimator(MinHashEncoder())
+
+
+def test_sklearn_compatible_SimilarityEncoder():
+    check_estimator(SimilarityEncoder())
+
+
+# def test_sklearn_compatible_TableVectorizer():
+#    check_estimator(TableVectorizer())
+
+
+def test_sklearn_compatible_TargetEncoder():
+    check_estimator(TargetEncoder())
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_string_distances.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_string_distances.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import List, Tuple
-
-import numpy as np
-
-from dirty_cat import _string_distances
-
-
-def test_get_unique_ngrams() -> None:
-    string = "test"
-    true_ngrams = {
-        (" ", "t"),
-        ("t", "e"),
-        ("e", "s"),
-        ("s", "t"),
-        ("t", " "),
-        (" ", "t", "e"),
-        ("t", "e", "s"),
-        ("e", "s", "t"),
-        ("s", "t", " "),
-        (" ", "t", "e", "s"),
-        ("t", "e", "s", "t"),
-        ("e", "s", "t", " "),
-    }
-    ngram_range = (2, 4)
-    ngrams = _string_distances.get_unique_ngrams(string, ngram_range)
-    assert ngrams == true_ngrams
-
-
-def _random_string_pairs(n_pairs=50, seed=1) -> List[Tuple[str, str]]:
-    rng = np.random.RandomState(seed)
-    characters = list(map(chr, range(10000)))
-    pairs = []
-    for n in range(n_pairs):
-        s1_len = rng.randint(50)
-        s2_len = rng.randint(50)
-        s1 = "".join(rng.choice(characters, s1_len))
-        s2 = "".join(rng.choice(characters, s2_len))
-        pairs.append((s1, s2))
-    return pairs
-
-
-def _check_symmetry(dist_func, *args, **kwargs) -> None:
-    for a, b in _random_string_pairs():
-        assert dist_func(a, b, *args, **kwargs) == dist_func(b, a, *args, **kwargs)
-
-
-def test_ngram_similarity() -> None:
-    # TODO
-    # assert ...
-    for n in range(1, 4):
-        _check_symmetry(_string_distances.ngram_similarity, n)
+from typing import List, Tuple
+
+import numpy as np
+
+from dirty_cat import _string_distances
+
+
+def test_get_unique_ngrams() -> None:
+    string = "test"
+    true_ngrams = {
+        (" ", "t"),
+        ("t", "e"),
+        ("e", "s"),
+        ("s", "t"),
+        ("t", " "),
+        (" ", "t", "e"),
+        ("t", "e", "s"),
+        ("e", "s", "t"),
+        ("s", "t", " "),
+        (" ", "t", "e", "s"),
+        ("t", "e", "s", "t"),
+        ("e", "s", "t", " "),
+    }
+    ngram_range = (2, 4)
+    ngrams = _string_distances.get_unique_ngrams(string, ngram_range)
+    assert ngrams == true_ngrams
+
+
+def _random_string_pairs(n_pairs=50, seed=1) -> List[Tuple[str, str]]:
+    rng = np.random.RandomState(seed)
+    characters = list(map(chr, range(10000)))
+    pairs = []
+    for n in range(n_pairs):
+        s1_len = rng.randint(50)
+        s2_len = rng.randint(50)
+        s1 = "".join(rng.choice(characters, s1_len))
+        s2 = "".join(rng.choice(characters, s2_len))
+        pairs.append((s1, s2))
+    return pairs
+
+
+def _check_symmetry(dist_func, *args, **kwargs) -> None:
+    for a, b in _random_string_pairs():
+        assert dist_func(a, b, *args, **kwargs) == dist_func(b, a, *args, **kwargs)
+
+
+def test_ngram_similarity() -> None:
+    # TODO
+    # assert ...
+    for n in range(1, 4):
+        _check_symmetry(_string_distances.ngram_similarity, n)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat/tests/test_target_encoder.py` & `dirty_cat-0.4.1/dirty_cat/tests/test_target_encoder.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-import numpy as np
-import pytest
-from sklearn.exceptions import NotFittedError
-
-from dirty_cat import _target_encoder
-
-
-def test_target_encoder():
-    lambda_ = _target_encoder.lambda_
-    X1 = np.array(
-        ["Red", "red", "green", "blue", "green", "green", "blue", "red"]
-    ).reshape(-1, 1)
-    X2 = np.array(
-        ["male", "male", "female", "male", "female", "female", "female", "male"]
-    ).reshape(-1, 1)
-    X = np.hstack([X1, X2])
-
-    # Case 1: binary-classification and regression
-    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
-    n = len(y)
-
-    Ey_ = 3 / 8
-    Eyx_ = {
-        "color": {"Red": 1, "red": 0, "green": 1 / 3, "blue": 0.5},
-        "gender": {"male": 0.5, "female": 0.25},
-    }
-    count_ = {
-        "color": {"Red": 1, "red": 2, "green": 3, "blue": 2},
-        "gender": {"male": 4, "female": 4},
-    }
-
-    encoder = _target_encoder.TargetEncoder()
-    encoder.fit(X, y)
-    for j in range(X.shape[1]):
-        assert np.array_equal(encoder.categories_[j], np.unique(X[:, j]))
-    assert Ey_ == encoder.Ey_
-    assert encoder.Eyx_[0] == Eyx_["color"]
-    assert encoder.Eyx_[1] == Eyx_["gender"]
-
-    Xtest1 = np.array(
-        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
-    ).reshape(-1, 1)
-    Xtest2 = np.array(
-        ["male", "male", "male", "male", "female", "female", "female", "female"]
-    ).reshape(-1, 1)
-    Xtest = np.hstack([Xtest1, Xtest2])
-
-    Xout = encoder.transform(Xtest)
-
-    ans_dict = {
-        var: {
-            cat: Eyx_[var][cat] * lambda_(count_[var][cat], n / len(count_[var]))
-            + Ey_ * (1 - lambda_(count_[var][cat], n / len(count_[var])))
-            for cat in Eyx_[var]
-        }
-        for var in Eyx_
-    }
-    ans = np.zeros((n, 2))
-    for j, col in enumerate(["color", "gender"]):
-        for i in range(n):
-            ans[i, j] = ans_dict[col][Xtest[i, j]]
-    assert np.array_equal(Xout, ans)
-
-    # Case 2: multiclass-classification
-    y = np.array([1, 0, 2, 1, 0, 1, 0, 0])
-    n = len(y)
-
-    encoder = _target_encoder.TargetEncoder(clf_type="multiclass-clf")
-    encoder.fit(X, y)
-
-    Ey_ = {0: 4 / 8, 1: 3 / 8, 2: 1 / 8}
-    Eyx_ = {
-        0: {
-            "color": {"Red": 0, "red": 1, "green": 1 / 3, "blue": 0.5},
-            "gender": {"male": 0.5, "female": 0.5},
-        },
-        1: {
-            "color": {"Red": 1, "red": 0, "green": 1 / 3, "blue": 0.5},
-            "gender": {"male": 0.5, "female": 0.25},
-        },
-        2: {
-            "color": {"Red": 0, "red": 0, "green": 1 / 3, "blue": 0},
-            "gender": {"male": 0, "female": 0.25},
-        },
-    }
-    assert np.array_equal(np.unique(y), encoder.classes_)
-    for k in [0, 1, 2]:
-        assert Ey_[k] == encoder.Ey_[k]
-        assert encoder.Eyx_[k][0] == Eyx_[k]["color"]
-        assert encoder.Eyx_[k][1] == Eyx_[k]["gender"]
-
-    count_ = {
-        "color": {"Red": 1, "red": 2, "green": 3, "blue": 2},
-        "gender": {"male": 4, "female": 4},
-    }
-    assert count_["color"] == encoder.counter_[0]
-    assert count_["gender"] == encoder.counter_[1]
-
-    ans_dict = {0: {}, 1: {}, 2: {}}
-    for k in [0, 1, 2]:
-        ans_dict[k] = {
-            var: {
-                cat: Eyx_[k][var][cat] * lambda_(count_[var][cat], n / len(count_[var]))
-                + Ey_[k] * (1 - lambda_(count_[var][cat], n / len(count_[var])))
-                for cat in Eyx_[k][var]
-            }
-            for var in Eyx_[k]
-        }
-
-    ans = np.zeros((n, 2 * 3))
-    Xtest1 = np.array(
-        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
-    ).reshape(-1, 1)
-    Xtest2 = np.array(
-        ["male", "male", "male", "male", "female", "female", "female", "female"]
-    ).reshape(-1, 1)
-    Xtest = np.hstack([Xtest1, Xtest2])
-    for k in [0, 1, 2]:
-        for j, col in enumerate(["color", "gender"]):
-            for i in range(n):
-                ans[i, 2 * j + k] = ans_dict[k][col][Xtest[i, j]]
-
-    Xout = encoder.transform(Xtest)
-    ans = np.zeros((n, 2 * 3))
-    Xtest1 = np.array(
-        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
-    ).reshape(-1, 1)
-    Xtest2 = np.array(
-        ["male", "male", "male", "male", "female", "female", "female", "female"]
-    ).reshape(-1, 1)
-    Xtest = np.hstack([Xtest1, Xtest2])
-    for k in [0, 1, 2]:
-        for j, col in enumerate(["color", "gender"]):
-            for i in range(n):
-                ans[i, j * 3 + k] = ans_dict[k][col][Xtest[i, j]]
-    encoder = _target_encoder.TargetEncoder(clf_type="multiclass-clf")
-    encoder.fit(X, y)
-    Xout = encoder.transform(Xtest)
-    assert np.array_equal(Xout, ans)
-
-
-input_types = ["list", "numpy", "pandas"]
-missings = ["", "aaa", "error"]
-
-
-@pytest.mark.parametrize("input_type", input_types)
-@pytest.mark.parametrize("missing", missings)
-def test_missing_values(input_type, missing):
-    X = [
-        ["Red", "male"],
-        [np.nan, "male"],
-        ["green", "female"],
-        ["blue", "male"],
-        ["green", "female"],
-        ["green", "female"],
-        ["blue", "female"],
-        [np.nan, np.nan],
-    ]
-
-    color_cat = ["Red", "", "green", "blue"]
-    gender_cat = ["male", "", "female"]
-
-    if input_type == "numpy":
-        X = np.array(X, dtype=object)
-    elif input_type == "pandas":
-        pd = pytest.importorskip("pandas")
-        X = pd.DataFrame(X)
-
-    # Case 1: binary-classification and regression
-    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
-
-    Ey_ = 3 / 8
-    Eyx_ = {
-        "color": {"Red": 1, "": 0, "green": 1 / 3, "blue": 0.5},
-        "gender": {"male": 2 / 3, "female": 0.25, "": 0},
-    }
-    count_ = {
-        "color": {"Red": 1, "": 2, "green": 3, "blue": 2},
-        "gender": {"male": 3, "female": 4, "": 1},
-    }
-
-    encoder = _target_encoder.TargetEncoder(handle_missing=missing)
-    if missing == "error":
-        with pytest.raises(ValueError, match=r"Found missing values in input"):
-            encoder.fit_transform(X, y)
-        return
-    elif missing == "":
-        encoder.fit_transform(X, y)
-
-        assert set(encoder.categories_[0]) == set(color_cat)
-        assert set(encoder.categories_[1]) == set(gender_cat)
-        assert Ey_ == encoder.Ey_
-        assert encoder.Eyx_[0] == Eyx_["color"]
-        assert encoder.Eyx_[1] == Eyx_["gender"]
-        assert dict(encoder.counter_[0]) == count_["color"]
-        assert dict(encoder.counter_[1]) == count_["gender"]
-    else:
-        with pytest.raises(ValueError, match=r"expected any of"):
-            encoder.fit_transform(X, y)
-        return
-
-
-@pytest.mark.parametrize("input_type", input_types)
-@pytest.mark.parametrize("missing", missings)
-def test_missing_values_transform(input_type, missing):
-    X = [
-        ["Red", "male"],
-        ["red", "male"],
-        ["green", "female"],
-        ["blue", "male"],
-        ["green", "female"],
-        ["green", "female"],
-        ["blue", "female"],
-        ["red", "male"],
-    ]
-
-    X_test = [
-        ["Red", "male"],
-        [np.nan, "male"],
-        ["green", "female"],
-        ["blue", "male"],
-        ["green", "female"],
-        ["green", "female"],
-        ["blue", "female"],
-        [np.nan, np.nan],
-    ]
-
-    if input_type == "numpy":
-        X_test = np.array(X_test, dtype=object)
-    elif input_type == "pandas":
-        pd = pytest.importorskip("pandas")
-        X_test = pd.DataFrame(X_test)
-
-    # Case 1: binary-classification and regression
-    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
-
-    Ey_ = 3 / 8
-
-    encoder = _target_encoder.TargetEncoder(
-        handle_unknown="ignore", handle_missing=missing
-    )
-    if missing == "error":
-        encoder.fit_transform(X, y)
-        with pytest.raises(ValueError, match=r"Found missing values in input"):
-            encoder.transform(X_test)
-    elif missing == "":
-        encoder.fit_transform(X, y)
-        ans = encoder.transform(X_test)
-
-        assert np.allclose(ans[1, 0], Ey_)
-        assert np.allclose(ans[-1, 0], Ey_)
-
-
-def test_errors():
-    """Test the different errors that may be raised during fit and transform"""
-    enc = _target_encoder.TargetEncoder(handle_unknown="blabla")
-    X = [[1], [2], [2], [3], [4]]
-    y = np.array([1, 2, 3, 4, 5])
-
-    with pytest.raises(ValueError, match="Got handle_unknown='blabla', but expected"):
-        enc.fit(X, y)
-
-    enc2 = _target_encoder.TargetEncoder(categories=[["blabla", "aa"]])
-    with pytest.raises(ValueError, match="Unsorted categories are not yet supported. "):
-        enc2.fit(X, y)
-
-    enc3 = _target_encoder.TargetEncoder(categories=[["aa", "blabla"]])
-    with pytest.raises(ValueError, match="Found unknown categories"):
-        enc3.fit(X, y)
-
-    X2 = [[1, "a"], [2, "b"], [4, "c"]]
-    X3 = [[5], [1], [4], [2]]
-    enc4 = _target_encoder.TargetEncoder()
-    enc4.fit(X, y)
-    with pytest.raises(ValueError, match="The number of features in the input data "):
-        enc4.transform(X2)
-    with pytest.raises(ValueError, match="Found unknown categories "):
-        enc4.transform(X3)
-
-def test_check_fitted_target_encoder():
-    """Test that calling transform before fit raises an error"""
-    enc = _target_encoder.TargetEncoder()
-    X = [[1], [2], [2], [3], [4]]
-    y = np.array([1, 2, 3, 4, 5])
-
-    with pytest.raises(NotFittedError, match="This TargetEncoder instance is not"):
-        enc.transform(X)
-    
-    enc.fit(X, y)
-    enc.transform(X)
+import numpy as np
+import pytest
+from sklearn.exceptions import NotFittedError
+
+from dirty_cat import _target_encoder
+
+
+def test_target_encoder():
+    lambda_ = _target_encoder.lambda_
+    X1 = np.array(
+        ["Red", "red", "green", "blue", "green", "green", "blue", "red"]
+    ).reshape(-1, 1)
+    X2 = np.array(
+        ["male", "male", "female", "male", "female", "female", "female", "male"]
+    ).reshape(-1, 1)
+    X = np.hstack([X1, X2])
+
+    # Case 1: binary-classification and regression
+    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
+    n = len(y)
+
+    Ey_ = 3 / 8
+    Eyx_ = {
+        "color": {"Red": 1, "red": 0, "green": 1 / 3, "blue": 0.5},
+        "gender": {"male": 0.5, "female": 0.25},
+    }
+    count_ = {
+        "color": {"Red": 1, "red": 2, "green": 3, "blue": 2},
+        "gender": {"male": 4, "female": 4},
+    }
+
+    encoder = _target_encoder.TargetEncoder()
+    encoder.fit(X, y)
+    for j in range(X.shape[1]):
+        assert np.array_equal(encoder.categories_[j], np.unique(X[:, j]))
+    assert Ey_ == encoder.Ey_
+    assert encoder.Eyx_[0] == Eyx_["color"]
+    assert encoder.Eyx_[1] == Eyx_["gender"]
+
+    Xtest1 = np.array(
+        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
+    ).reshape(-1, 1)
+    Xtest2 = np.array(
+        ["male", "male", "male", "male", "female", "female", "female", "female"]
+    ).reshape(-1, 1)
+    Xtest = np.hstack([Xtest1, Xtest2])
+
+    Xout = encoder.transform(Xtest)
+
+    ans_dict = {
+        var: {
+            cat: Eyx_[var][cat] * lambda_(count_[var][cat], n / len(count_[var]))
+            + Ey_ * (1 - lambda_(count_[var][cat], n / len(count_[var])))
+            for cat in Eyx_[var]
+        }
+        for var in Eyx_
+    }
+    ans = np.zeros((n, 2))
+    for j, col in enumerate(["color", "gender"]):
+        for i in range(n):
+            ans[i, j] = ans_dict[col][Xtest[i, j]]
+    assert np.array_equal(Xout, ans)
+
+    # Case 2: multiclass-classification
+    y = np.array([1, 0, 2, 1, 0, 1, 0, 0])
+    n = len(y)
+
+    encoder = _target_encoder.TargetEncoder(clf_type="multiclass-clf")
+    encoder.fit(X, y)
+
+    Ey_ = {0: 4 / 8, 1: 3 / 8, 2: 1 / 8}
+    Eyx_ = {
+        0: {
+            "color": {"Red": 0, "red": 1, "green": 1 / 3, "blue": 0.5},
+            "gender": {"male": 0.5, "female": 0.5},
+        },
+        1: {
+            "color": {"Red": 1, "red": 0, "green": 1 / 3, "blue": 0.5},
+            "gender": {"male": 0.5, "female": 0.25},
+        },
+        2: {
+            "color": {"Red": 0, "red": 0, "green": 1 / 3, "blue": 0},
+            "gender": {"male": 0, "female": 0.25},
+        },
+    }
+    assert np.array_equal(np.unique(y), encoder.classes_)
+    for k in [0, 1, 2]:
+        assert Ey_[k] == encoder.Ey_[k]
+        assert encoder.Eyx_[k][0] == Eyx_[k]["color"]
+        assert encoder.Eyx_[k][1] == Eyx_[k]["gender"]
+
+    count_ = {
+        "color": {"Red": 1, "red": 2, "green": 3, "blue": 2},
+        "gender": {"male": 4, "female": 4},
+    }
+    assert count_["color"] == encoder.counter_[0]
+    assert count_["gender"] == encoder.counter_[1]
+
+    ans_dict = {0: {}, 1: {}, 2: {}}
+    for k in [0, 1, 2]:
+        ans_dict[k] = {
+            var: {
+                cat: Eyx_[k][var][cat] * lambda_(count_[var][cat], n / len(count_[var]))
+                + Ey_[k] * (1 - lambda_(count_[var][cat], n / len(count_[var])))
+                for cat in Eyx_[k][var]
+            }
+            for var in Eyx_[k]
+        }
+
+    ans = np.zeros((n, 2 * 3))
+    Xtest1 = np.array(
+        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
+    ).reshape(-1, 1)
+    Xtest2 = np.array(
+        ["male", "male", "male", "male", "female", "female", "female", "female"]
+    ).reshape(-1, 1)
+    Xtest = np.hstack([Xtest1, Xtest2])
+    for k in [0, 1, 2]:
+        for j, col in enumerate(["color", "gender"]):
+            for i in range(n):
+                ans[i, 2 * j + k] = ans_dict[k][col][Xtest[i, j]]
+
+    Xout = encoder.transform(Xtest)
+    ans = np.zeros((n, 2 * 3))
+    Xtest1 = np.array(
+        ["Red", "red", "blue", "green", "Red", "red", "blue", "green"]
+    ).reshape(-1, 1)
+    Xtest2 = np.array(
+        ["male", "male", "male", "male", "female", "female", "female", "female"]
+    ).reshape(-1, 1)
+    Xtest = np.hstack([Xtest1, Xtest2])
+    for k in [0, 1, 2]:
+        for j, col in enumerate(["color", "gender"]):
+            for i in range(n):
+                ans[i, j * 3 + k] = ans_dict[k][col][Xtest[i, j]]
+    encoder = _target_encoder.TargetEncoder(clf_type="multiclass-clf")
+    encoder.fit(X, y)
+    Xout = encoder.transform(Xtest)
+    assert np.array_equal(Xout, ans)
+
+
+input_types = ["list", "numpy", "pandas"]
+missings = ["", "aaa", "error"]
+
+
+@pytest.mark.parametrize("input_type", input_types)
+@pytest.mark.parametrize("missing", missings)
+def test_missing_values(input_type, missing):
+    X = [
+        ["Red", "male"],
+        [np.nan, "male"],
+        ["green", "female"],
+        ["blue", "male"],
+        ["green", "female"],
+        ["green", "female"],
+        ["blue", "female"],
+        [np.nan, np.nan],
+    ]
+
+    color_cat = ["Red", "", "green", "blue"]
+    gender_cat = ["male", "", "female"]
+
+    if input_type == "numpy":
+        X = np.array(X, dtype=object)
+    elif input_type == "pandas":
+        pd = pytest.importorskip("pandas")
+        X = pd.DataFrame(X)
+
+    # Case 1: binary-classification and regression
+    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
+
+    Ey_ = 3 / 8
+    Eyx_ = {
+        "color": {"Red": 1, "": 0, "green": 1 / 3, "blue": 0.5},
+        "gender": {"male": 2 / 3, "female": 0.25, "": 0},
+    }
+    count_ = {
+        "color": {"Red": 1, "": 2, "green": 3, "blue": 2},
+        "gender": {"male": 3, "female": 4, "": 1},
+    }
+
+    encoder = _target_encoder.TargetEncoder(handle_missing=missing)
+    if missing == "error":
+        with pytest.raises(ValueError, match=r"Found missing values in input"):
+            encoder.fit_transform(X, y)
+        return
+    elif missing == "":
+        encoder.fit_transform(X, y)
+
+        assert set(encoder.categories_[0]) == set(color_cat)
+        assert set(encoder.categories_[1]) == set(gender_cat)
+        assert Ey_ == encoder.Ey_
+        assert encoder.Eyx_[0] == Eyx_["color"]
+        assert encoder.Eyx_[1] == Eyx_["gender"]
+        assert dict(encoder.counter_[0]) == count_["color"]
+        assert dict(encoder.counter_[1]) == count_["gender"]
+    else:
+        with pytest.raises(ValueError, match=r"expected any of"):
+            encoder.fit_transform(X, y)
+        return
+
+
+@pytest.mark.parametrize("input_type", input_types)
+@pytest.mark.parametrize("missing", missings)
+def test_missing_values_transform(input_type, missing):
+    X = [
+        ["Red", "male"],
+        ["red", "male"],
+        ["green", "female"],
+        ["blue", "male"],
+        ["green", "female"],
+        ["green", "female"],
+        ["blue", "female"],
+        ["red", "male"],
+    ]
+
+    X_test = [
+        ["Red", "male"],
+        [np.nan, "male"],
+        ["green", "female"],
+        ["blue", "male"],
+        ["green", "female"],
+        ["green", "female"],
+        ["blue", "female"],
+        [np.nan, np.nan],
+    ]
+
+    if input_type == "numpy":
+        X_test = np.array(X_test, dtype=object)
+    elif input_type == "pandas":
+        pd = pytest.importorskip("pandas")
+        X_test = pd.DataFrame(X_test)
+
+    # Case 1: binary-classification and regression
+    y = np.array([1, 0, 0, 1, 0, 1, 0, 0])
+
+    Ey_ = 3 / 8
+
+    encoder = _target_encoder.TargetEncoder(
+        handle_unknown="ignore", handle_missing=missing
+    )
+    if missing == "error":
+        encoder.fit_transform(X, y)
+        with pytest.raises(ValueError, match=r"Found missing values in input"):
+            encoder.transform(X_test)
+    elif missing == "":
+        encoder.fit_transform(X, y)
+        ans = encoder.transform(X_test)
+
+        assert np.allclose(ans[1, 0], Ey_)
+        assert np.allclose(ans[-1, 0], Ey_)
+
+
+def test_errors():
+    """Test the different errors that may be raised during fit and transform"""
+    enc = _target_encoder.TargetEncoder(handle_unknown="blabla")
+    X = [[1], [2], [2], [3], [4]]
+    y = np.array([1, 2, 3, 4, 5])
+
+    with pytest.raises(ValueError, match="Got handle_unknown='blabla', but expected"):
+        enc.fit(X, y)
+
+    enc2 = _target_encoder.TargetEncoder(categories=[["blabla", "aa"]])
+    with pytest.raises(ValueError, match="Unsorted categories are not yet supported. "):
+        enc2.fit(X, y)
+
+    enc3 = _target_encoder.TargetEncoder(categories=[["aa", "blabla"]])
+    with pytest.raises(ValueError, match="Found unknown categories"):
+        enc3.fit(X, y)
+
+    X2 = [[1, "a"], [2, "b"], [4, "c"]]
+    X3 = [[5], [1], [4], [2]]
+    enc4 = _target_encoder.TargetEncoder()
+    enc4.fit(X, y)
+    with pytest.raises(ValueError, match="The number of features in the input data "):
+        enc4.transform(X2)
+    with pytest.raises(ValueError, match="Found unknown categories "):
+        enc4.transform(X3)
+
+def test_check_fitted_target_encoder():
+    """Test that calling transform before fit raises an error"""
+    enc = _target_encoder.TargetEncoder()
+    X = [[1], [2], [2], [3], [4]]
+    y = np.array([1, 2, 3, 4, 5])
+
+    with pytest.raises(NotFittedError, match="This TargetEncoder instance is not"):
+        enc.transform(X)
+    
+    enc.fit(X, y)
+    enc.transform(X)
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat.egg-info/PKG-INFO` & `dirty_cat-0.4.1/dirty_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirty-cat
-Version: 0.4.0b2
+Version: 0.4.1
 Summary: Machine learning with dirty categories.
 Author: Patricio Cerda
 Author-email: patricio.cerda@inria.fr
 License: BSD
 Project-URL: Homepage, https://dirty-cat.github.io/
 Project-URL: Source, https://github.com/dirty-cat/dirty_cat
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
 
 If you like the package, please *spread the word*, and ⭐ `the repository <https://github.com/dirty-cat/dirty_cat/>`_!
 
 What can `dirty_cat` do?
 ------------------------
 
-`dirty_cat` provides tools (``SuperVectorizer``, ``fuzzy_join``...) and
+`dirty_cat` provides tools (``TableVectorizer``, ``fuzzy_join``...) and
 encoders (``GapEncoder``, ``MinHashEncoder``...) for **morphological similarities**,
 for which we usually identify three common cases: **similarities, typos and variations**
 
 `The first example notebook <https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html>`_
 goes in-depth on how to identify and deal with dirty data using the `dirty_cat` library.
 
 What `dirty_cat` does not
```

### Comparing `dirty_cat-0.4.0b2/dirty_cat.egg-info/SOURCES.txt` & `dirty_cat-0.4.1/dirty_cat.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+benchmarks/3_compare_encoders_perfs.py
 benchmarks/__init__.py
-benchmarks/bench_minhash.py
+benchmarks/bench_minhash_batch.py
+benchmarks/benchmark_fuzzy_join_hash.py
 benchmarks/encoders_time_memory_bench.py
 benchmarks/fuzzy_join_benchmark.py
 benchmarks/fuzzy_join_full_benchmark.py
 benchmarks/get_results.py
 benchmarks/similarity_scores_time_benchmark.py
-benchmarks/supervectorizer_tuning.py
+benchmarks/tablevectorizer_tuning.py
 benchmarks/utils/__init__.py
 benchmarks/utils/_argparser.py
 benchmarks/utils/_various.py
 benchmarks/utils/monitor.py
 dirty_cat/VERSION.txt
 dirty_cat/__init__.py
 dirty_cat/_check_dependencies.py
@@ -23,39 +25,41 @@
 dirty_cat/_fast_hash.py
 dirty_cat/_feature_augmenter.py
 dirty_cat/_fuzzy_join.py
 dirty_cat/_gap_encoder.py
 dirty_cat/_minhash_encoder.py
 dirty_cat/_similarity_encoder.py
 dirty_cat/_string_distances.py
-dirty_cat/_super_vectorizer.py
+dirty_cat/_table_vectorizer.py
 dirty_cat/_target_encoder.py
 dirty_cat/_utils.py
 dirty_cat.egg-info/PKG-INFO
 dirty_cat.egg-info/SOURCES.txt
 dirty_cat.egg-info/dependency_links.txt
 dirty_cat.egg-info/requires.txt
 dirty_cat.egg-info/top_level.txt
 dirty_cat/datasets/__init__.py
 dirty_cat/datasets/_fetching.py
 dirty_cat/datasets/_generating.py
+dirty_cat/datasets/_ken_embeddings.py
 dirty_cat/datasets/_utils.py
 dirty_cat/datasets/tests/__init__.py
 dirty_cat/datasets/tests/test_fetching.py
 dirty_cat/datasets/tests/test_generating.py
+dirty_cat/datasets/tests/test_ken_embeddings.py
 dirty_cat/datasets/tests/test_utils.py
 dirty_cat/tests/__init__.py
 dirty_cat/tests/test_datetime_encoder.py
 dirty_cat/tests/test_deduplicate.py
 dirty_cat/tests/test_docstrings.py
 dirty_cat/tests/test_fast_hash.py
 dirty_cat/tests/test_feature_augmenter.py
 dirty_cat/tests/test_fuzzy_join.py
 dirty_cat/tests/test_gap_encoder.py
 dirty_cat/tests/test_minhash_encoder.py
 dirty_cat/tests/test_similarity_encoder.py
 dirty_cat/tests/test_sklearn.py
 dirty_cat/tests/test_string_distances.py
-dirty_cat/tests/test_super_vectorizer.py
+dirty_cat/tests/test_table_vectorizer.py
 dirty_cat/tests/test_target_encoder.py
 dirty_cat/tests/test_utils.py
 dirty_cat/tests/utils.py
```

### Comparing `dirty_cat-0.4.0b2/setup.cfg` & `dirty_cat-0.4.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -28,48 +28,53 @@
 install_requires = 
 	scikit-learn>=0.23.0
 	numpy>=1.17.3
 	scipy>=1.4.0
 	pandas>=1.2.0
 	requests
 	joblib
+	pyarrow
 python_requires = >=3.8
 
 [options.extras_require]
 dev = 
 	pytest
 	pytest-cov
+	pytest-xdist
+	pytest-xdist[psutil]
 	coverage
 	mypy
 	numpydoc
 	flake8
+	openml
 doc = 
 	sphinx-gallery
 	sphinxext-opengraph
 	matplotlib
 	seaborn
 	statsmodels
 benchmarks = 
 	numpy
 	pandas
 	matplotlib
 	seaborn
+	tqdm
 min-py38 = 
 	scikit-learn==0.23.0
 	numpy==1.17.3
 	scipy==1.4.0
 	pandas==1.2.0
 min-py39 = 
-	scikit-learn==0.23.0
-	numpy==1.17.3
+	scikit-learn==0.24.0
+	numpy==1.19.3
 	scipy==1.6.0
 	pandas==1.2.0
 min-py310 = 
-	scikit-learn==0.24.0
-	numpy==1.23.0
+	scikit-learn==1.0.2
+	numpy==1.21.3
 	scipy==1.8.0
 	pandas==1.3.5
 
 [flake8]
 max-line-length = 88
 target-version = ['py310']
 ignore =
```

