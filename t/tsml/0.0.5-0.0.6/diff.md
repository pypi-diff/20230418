# Comparing `tmp/tsml-0.0.5.tar.gz` & `tmp/tsml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.0.5.tar", last modified: Thu Apr  6 15:04:25 2023, max compression
+gzip compressed data, was "tsml-0.0.6.tar", last modified: Mon Apr 17 23:08:33 2023, max compression
```

## Comparing `tsml-0.0.5.tar` & `tsml-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.716956 tsml-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-06 15:04:12.000000 tsml-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-06 15:04:12.000000 tsml-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-06 15:04:25.716956 tsml-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-06 15:04:12.000000 tsml-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-06 15:04:12.000000 tsml-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:04:25.716956 tsml-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10672 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml/convolution_based/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/convolution_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/deep_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/deep_learning/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/dictionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/dictionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/distance_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/feature_based/_catch22.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45975 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.708956 tsml-0.0.5/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.712956 tsml-0.0.5/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81471 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/tests/_sklearn_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/tests/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.712956 tsml-0.0.5/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    23960 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/transformations/_summary_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.712956 tsml-0.0.5/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.712956 tsml-0.0.5/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.712956 tsml-0.0.5/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.716956 tsml-0.0.5/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-06 15:04:12.000000 tsml-0.0.5/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:04:25.704956 tsml-0.0.5/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-06 15:04:25.000000 tsml-0.0.5/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-06 15:04:25.000000 tsml-0.0.5/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:04:25.000000 tsml-0.0.5/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-06 15:04:25.000000 tsml-0.0.5/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 15:04:25.000000 tsml-0.0.5/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-17 23:08:24.000000 tsml-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 23:08:24.000000 tsml-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 23:08:33.908886 tsml-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 23:08:24.000000 tsml-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 23:08:24.000000 tsml-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:08:33.908886 tsml-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.896886 tsml-0.0.6/tsml/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/convolution_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/convolution_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/deep_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/deep_learning/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/dictionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dictionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/distance_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/feature_based/_catch22.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45975 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81519 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/_sklearn_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.904886 tsml-0.0.6/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23960 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/transformations/_summary_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.908886 tsml-0.0.6/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 23:08:24.000000 tsml-0.0.6/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:33.900886 tsml-0.0.6/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 23:08:33.000000 tsml-0.0.6/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.0.5/LICENSE` & `tsml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/PKG-INFO` & `tsml-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.0.5/pyproject.toml` & `tsml-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.0.5"
+version = "0.0.6"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.middlehurst@uea.ac.uk"},
     {name = "Tony Bagnall", email = "ajb@uea.ac.uk"},
 ]
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
```

### Comparing `tsml-0.0.5/tsml/base.py` & `tsml-0.0.6/tsml/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,29 +107,32 @@
             self._check_n_features(
                 out[0] if isinstance(out, tuple) else out, reset=reset
             )
 
         return out
 
     def _convert_X(
-        self, X: Union[np.ndarray, List[np.ndarray]], concatenate_channels: bool = False
+        self,
+        X: Union[np.ndarray, List[np.ndarray]],
+        pad_unequal: bool = False,
+        concatenate_channels: bool = False,
     ) -> Union[np.ndarray, List[np.ndarray]]:
         dtypes = self._get_tags()["X_types"]
 
         if isinstance(X, np.ndarray) and X.ndim == 3:
             if "3darray" in dtypes:
                 return X
             elif dtypes[0] == "2darray":
                 if X.shape[1] == 1 or concatenate_channels:
                     return X.reshape((X.shape[0], -1))
                 else:
                     raise ValueError(
-                        "Can only convert 3D numpy array with 1 channel to 2D numpy "
-                        f"array if concatenate_channels is True, found {X.shape[1]} "
-                        "channels."
+                        "Can only convert 3D numpy array with more than 1 channel to "
+                        "2D numpy array if concatenate_channels is True, found "
+                        f"{X.shape[1]} channels."
                     )
             elif dtypes[0] == "np_list":
                 return [x for x in X]
         elif isinstance(X, np.ndarray) and X.ndim == 2:
             if "2darray" in dtypes:
                 return X
             elif dtypes[0] == "3darray":
@@ -138,35 +141,51 @@
                 return [x.reshape(1, X.shape[1]) for x in X]
         elif isinstance(X, list) and all(
             isinstance(x, np.ndarray) and x.ndim == 2 for x in X
         ):
             if "np_list" in dtypes:
                 return X
             elif dtypes[0] == "3darray":
+                if not pad_unequal and not all(x.shape[1] == X[0].shape[1] for x in X):
+                    raise ValueError(
+                        "Can only convert list of 2D numpy arrays with unequal length "
+                        "data to 3D numpy array if pad_unequal is True, found "
+                        "different series lengths."
+                    )
+
                 max_len = max(x.shape[1] for x in X)
                 arr = np.zeros((len(X), X[0].shape[0], max_len))
 
                 for i, x in enumerate(X):
                     arr[i, :, : x.shape[1]] = x
 
                 return arr
             elif dtypes[0] == "2darray":
                 if X[0].shape[0] == 1 or concatenate_channels:
+                    if not pad_unequal and not all(
+                        x.shape[1] == X[0].shape[1] for x in X
+                    ):
+                        raise ValueError(
+                            "Can only convert list of 2D numpy arrays with unequal "
+                            "length data to 2D numpy array if pad_unequal is True, "
+                            "found different series lengths."
+                        )
+
                     max_len = max(x.shape[1] for x in X)
                     arr = np.zeros((len(X), X[0].shape[0], max_len))
 
                     for i, x in enumerate(X):
                         arr[i, :, : x.shape[1]] = x
 
                     return arr.reshape((arr.shape[0], -1))
                 else:
                     raise ValueError(
-                        "Can only convert list of 2D numpy arrays with 1 channel to 2D "
-                        "numpy array if concatenate_channels is True, found "
-                        f"{X[0].shape[0]} channels."
+                        "Can only convert list of 2D numpy arrays with more than 1 "
+                        "channel to 2D numpy array if concatenate_channels is True, "
+                        f"found {X[0].shape[0]} channels."
                     )
         else:
             raise ValueError(
                 "X must be a 2D/3D numpy array or a list of 2D numpy arrays, got "
                 f"{f'list of {type(X[0])}' if isinstance(X, list) else type(X)} "
                 "instead."
             )
```

### Comparing `tsml-0.0.5/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.0.6/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/__init__.py` & `tsml-0.0.6/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/datasets/_data_io.py` & `tsml-0.0.6/tsml/datasets/_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/dummy/_dummy.py` & `tsml-0.0.6/tsml/dummy/_dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return self
 
         self._clf = SklearnDummyClassifier(
             strategy=self.strategy,
             random_state=self.random_state,
             constant=self.constant,
         )
-        self._clf.fit(np.zeros(X.shape), y)
+        self._clf.fit(None, y)
 
         return self
 
     def predict(self, X) -> np.ndarray:
         """"""
         check_is_fitted(self)
 
@@ -137,15 +137,18 @@
             return np.repeat([[1]], X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
         return self._clf.predict_proba(np.zeros(X.shape))
 
     def _more_tags(self):
-        return {"X_types": ["3darray", "2darray", "np_list"]}
+        return {
+            "X_types": ["3darray", "2darray", "np_list"],
+            "equal_length_only": False,
+        }
 
 
 class DummyRegressor(RegressorMixin, BaseTimeSeriesEstimator):
     """DummyRegressor makes predictions that ignore the input features.
 
     This regressor is useful as a simple baseline to compare with other
     (real) regressors. Do not use it for real problems.
@@ -201,33 +204,36 @@
         self.constant = constant
         self.quantile = quantile
 
         super(DummyRegressor, self).__init__()
 
     def fit(self, X, y):
         """"""
-        X, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
+        _, y = self._validate_data(X=X, y=y, ensure_min_series_length=1)
 
         self._reg = SklearnDummyRegressor(
             strategy=self.strategy, constant=self.constant, quantile=self.quantile
         )
-        self._reg.fit(np.zeros(X.shape), y)
+        self._reg.fit(None, y)
 
         return self
 
     def predict(self, X):
         """"""
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=1)
 
         return self._reg.predict(np.zeros(X.shape))
 
     def _more_tags(self):
-        return {"X_types": ["3darray", "2darray", "np_list"]}
+        return {
+            "X_types": ["3darray", "2darray", "np_list"],
+            "equal_length_only": False,
+        }
 
 
 class DummyClusterer(ClusterMixin, BaseTimeSeriesEstimator):
     """DummyRegressor makes predictions that ignore the input features.
 
     This cluster makes no effort to form reasonable clusters, and is primarily used
     for interface testing. Do not use it for real problems.
@@ -287,8 +293,11 @@
         elif self.strategy == "random":
             rng = check_random_state(self.random_state)
             return rng.randint(self.n_clusters, size=len(X), dtype=np.int32)
         else:
             raise ValueError(f"Unknown strategy {self.strategy}")
 
     def _more_tags(self):
-        return {"X_types": ["3darray", "2darray", "np_list"]}
+        return {
+            "X_types": ["3darray", "2darray", "np_list"],
+            "equal_length_only": False,
+        }
```

### Comparing `tsml-0.0.5/tsml/feature_based/_catch22.py` & `tsml-0.0.6/tsml/feature_based/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/__init__.py` & `tsml-0.0.6/tsml/interval_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_base.py` & `tsml-0.0.6/tsml/interval_based/_base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_cif.py` & `tsml-0.0.6/tsml/interval_based/_cif.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_interval_forest.py` & `tsml-0.0.6/tsml/interval_based/_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_interval_pipelines.py` & `tsml-0.0.6/tsml/interval_based/_interval_pipelines.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_rise.py` & `tsml-0.0.6/tsml/interval_based/_rise.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_stsf.py` & `tsml-0.0.6/tsml/interval_based/_stsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/interval_based/_tsf.py` & `tsml-0.0.6/tsml/interval_based/_tsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/shapelet_based/_stc.py` & `tsml-0.0.6/tsml/shapelet_based/_stc.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/tests/_sklearn_checks.py` & `tsml-0.0.6/tsml/tests/_sklearn_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1325,24 +1325,24 @@
         )
         msg = (
             "The classifier {} does not raise an error when the number of "
             "features in {} is different from the number of features in "
             "fit."
         )
 
-        if not tags["no_validation"]:
-            if tags["pairwise"]:
-                with raises(
-                    ValueError,
-                    err_msg=msg_pairwise.format(name, "predict"),
-                ):
-                    classifier.predict(X.reshape(-1, 1))
-            else:
-                with raises(ValueError, err_msg=msg.format(name, "predict")):
-                    classifier.predict(X.T)
+        # if not tags["no_validation"]:
+        #     if tags["pairwise"]:
+        #         with raises(
+        #             ValueError,
+        #             err_msg=msg_pairwise.format(name, "predict"),
+        #         ):
+        #             classifier.predict(X.reshape(-1, 1))
+        #     else:
+        #         with raises(ValueError, err_msg=msg.format(name, "predict")):
+        #             classifier.predict(X.T)
         if hasattr(classifier, "decision_function"):
             try:
                 # decision_function agrees with predict
                 decision = classifier.decision_function(X)
                 if n_classes == 2:
                     if not tags["multioutput_only"]:
                         assert decision.shape == (n_samples,)
@@ -1374,28 +1374,28 @@
         if hasattr(classifier, "predict_proba"):
             # predict_proba agrees with predict
             y_prob = classifier.predict_proba(X)
             assert y_prob.shape == (n_samples, n_classes)
             assert_array_equal(np.argmax(y_prob, axis=1), y_pred)
             # check that probas for all classes sum to one
             assert_array_almost_equal(np.sum(y_prob, axis=1), np.ones(n_samples))
-            if not tags["no_validation"]:
-                # raises error on malformed input for predict_proba
-                if tags["pairwise"]:
-                    with raises(
-                        ValueError,
-                        err_msg=msg_pairwise.format(name, "predict_proba"),
-                    ):
-                        classifier.predict_proba(X.reshape(-1, 1))
-                else:
-                    with raises(
-                        ValueError,
-                        err_msg=msg.format(name, "predict_proba"),
-                    ):
-                        classifier.predict_proba(X.T)
+            # if not tags["no_validation"]:
+            #     # raises error on malformed input for predict_proba
+            #     if tags["pairwise"]:
+            #         with raises(
+            #             ValueError,
+            #             err_msg=msg_pairwise.format(name, "predict_proba"),
+            #         ):
+            #             classifier.predict_proba(X.reshape(-1, 1))
+            #     else:
+            #         with raises(
+            #             ValueError,
+            #             err_msg=msg.format(name, "predict_proba"),
+            #         ):
+            #             classifier.predict_proba(X.T)
             if hasattr(classifier, "predict_log_proba"):
                 # predict_log_proba is a transformation of predict_proba
                 y_log_prob = classifier.predict_log_proba(X)
                 assert_allclose(y_log_prob, np.log(y_prob), 8, atol=1e-9)
                 assert_array_equal(np.argsort(y_log_prob), np.argsort(y_prob))
```

### Comparing `tsml-0.0.5/tsml/tests/estimator_checks.py` & `tsml-0.0.6/tsml/tests/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/tests/test_interface.py` & `tsml-0.0.6/tsml/tests/test_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,28 +28,28 @@
         raise ValueError(f"Invalid data_type: {data_type}")
 
 
 @pytest.mark.parametrize("input_type", ("3darray", "2darray", "np_list"))
 def test_convert_X_to_3d_array(input_type):
     est = _3dArrayDummy()
     X, old_shape = _generate_conversion_test_X(input_type)
-    X = est._convert_X(X)
+    X = est._convert_X(X, pad_unequal=True)
 
     assert isinstance(X, np.ndarray)
     assert X.ndim == 3
     assert X.shape == old_shape
 
     est._validate_data(X)
 
 
 @pytest.mark.parametrize("input_type", ("3darray", "2darray", "np_list"))
 def test_convert_X_to_2d_array(input_type):
     est = _2dArrayDummy()
     X, old_shape = _generate_conversion_test_X(input_type)
-    X = est._convert_X(X, concatenate_channels=True)
+    X = est._convert_X(X, concatenate_channels=True, pad_unequal=True)
 
     assert isinstance(X, np.ndarray)
     assert X.ndim == 2
     assert X.shape == (old_shape[0], old_shape[2] * old_shape[1])
 
     est._validate_data(X)
```

### Comparing `tsml-0.0.5/tsml/transformations/__init__.py` & `tsml-0.0.6/tsml/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_ar_coefficient.py` & `tsml-0.0.6/tsml/transformations/_ar_coefficient.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_catch22.py` & `tsml-0.0.6/tsml/transformations/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_function_transformer.py` & `tsml-0.0.6/tsml/transformations/_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_interval_extraction.py` & `tsml-0.0.6/tsml/transformations/_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_periodogram.py` & `tsml-0.0.6/tsml/transformations/_periodogram.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_sfa.py` & `tsml-0.0.6/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_shapelet_transform.py` & `tsml-0.0.6/tsml/transformations/_shapelet_transform.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/transformations/_summary_features.py` & `tsml-0.0.6/tsml/transformations/_summary_features.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/_tags.py` & `tsml-0.0.6/tsml/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/discovery.py` & `tsml-0.0.6/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/numba_functions/general.py` & `tsml-0.0.6/tsml/utils/numba_functions/general.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/numba_functions/stats.py` & `tsml-0.0.6/tsml/utils/numba_functions/stats.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/testing.py` & `tsml-0.0.6/tsml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/utils/validation.py` & `tsml-0.0.6/tsml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/vector/_cit.py` & `tsml-0.0.6/tsml/vector/_cit.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/vector/_rotation_forest.py` & `tsml-0.0.6/tsml/vector/_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml/vector/tests/test_rotation_forest.py` & `tsml-0.0.6/tsml/vector/tests/test_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.0.5/tsml.egg-info/PKG-INFO` & `tsml-0.0.6/tsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.0.5
+Version: 0.0.6
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.0.5/tsml.egg-info/SOURCES.txt` & `tsml-0.0.6/tsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

