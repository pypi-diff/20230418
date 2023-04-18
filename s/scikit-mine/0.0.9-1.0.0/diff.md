# Comparing `tmp/scikit-mine-0.0.9.tar.gz` & `tmp/scikit-mine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-mine-0.0.9.tar", last modified: Fri Dec 30 15:12:00 2022, max compression
+gzip compressed data, was "scikit-mine-1.0.0.tar", last modified: Tue Apr 18 09:02:56 2023, max compression
```

## Comparing `scikit-mine-0.0.9.tar` & `scikit-mine-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/scikit_mine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-30 15:12:00.000000 scikit-mine-0.0.9/scikit_mine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-30 15:12:00.807963 scikit-mine-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/_instacart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/_samples_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16482 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/fimi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/emerging/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/emerging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/emerging/mbdldorber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/feature_extraction/slim_vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/graph/graphmdl/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)    36137 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/code_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/code_table_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/graph_mdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/label_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/graph/graphmdl/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44108 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/test/test_graph_mdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    35639 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/graph/graphmdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/itemsets/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/itemsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15288 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/itemsets/lcm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/itemsets/slim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/itemsets/slim_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/periodic/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/periodic/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)    21376 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/periodic/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 15:12:00.803963 scikit-mine-0.0.9/skmine/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/preprocessing/mdlp_discretizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2022-12-30 15:11:46.000000 scikit-mine-0.0.9/skmine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.340591 scikit-mine-1.0.0/scikit_mine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 09:02:56.000000 scikit-mine-1.0.0/scikit_mine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.340591 scikit-mine-1.0.0/skmine/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.340591 scikit-mine-1.0.0/skmine/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/_samples_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/fimi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.340591 scikit-mine-1.0.0/skmine/emerging/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/emerging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/emerging/mbdldorber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/feature_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/feature_extraction/slim_vectorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/graph/graphmdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/code_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/code_table_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/graph_mdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/label_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/graph/graphmdl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44108 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/test/test_graph_mdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35639 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/graph/graphmdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/itemsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/itemsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/itemsets/lcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/itemsets/slim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/itemsets/slim_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/periodic/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/candidate_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/class_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/data_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/extract_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53181 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/pattern_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/periodic/run_mine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:02:56.344591 scikit-mine-1.0.0/skmine/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/preprocessing/mdlp_discretizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-04-18 09:02:42.000000 scikit-mine-1.0.0/skmine/utils.py
```

### Comparing `scikit-mine-0.0.9/LICENSE` & `scikit-mine-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, scikit-mine
+Copyright (c) 2022, scikit-mine
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `scikit-mine-0.0.9/PKG-INFO` & `scikit-mine-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: scikit-mine
-Version: 0.0.9
+Version: 1.0.0
 Summary: Pattern mining in Python
 Home-page: https://github.com/scikit-mine/scikit-mine
 Download-URL: https://github.com/scikit-mine/scikit-mine
 Maintainer: scikit-mine team
 Maintainer-email: skm-dev@inria.fr
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/x-rst
@@ -66,36 +65,39 @@
 
 
 scikit-mine is a Python module for pattern mining built on top of
 Pandas/Numpy/SciPy and is distributed under the 3-Clause BSD license.
 
 It is currently maintained by a team of volunteers.
 
-See examples in the tutorials; the notebooks are available here_.
+See examples in the tutorials; the notebooks are available here_. To execute the tutorials, you will have to install jupyter notebook or jupyterlab (https://jupyter.org/install)
 
 
 .. _here: https://github.com/scikit-mine/scikit-mine/tree/master/docs/tutorials
 
 
 Dependencies
 ------------
 
-scikit-mine requires Python>=3.7,
+scikit-mine requires Python>=3.8,
 and some extra dependencies
 
 * scipy>=1.2.1
 * pandas>=1.0.0
-* pyroaring
+* pyroaring>=0.3.4
 * joblib>=0.11.1
 * sortedcontainers>=2.1.0
-* dataclasses
-* networkx~=2.5.1
-* wget
+* dataclasses>=0.6
+* networkx
+* wget>=3.2
+* scikit-learn
+* graphviz
+* matplotlib
+* pydot
 
-**scikit-learn** is not a dependency. However, scikit-mine is **contiuously tested for interactions with scikit-learn**
 
 Development
 -----------
 
 This project is funded by the `INRIA center in Rennes, Brittany, France <https://www.inria.fr/fr/centre-inria-rennes-bretagne-atlantique>`_.
 
 We welcome new contributors of all experience levels.
```

### Comparing `scikit-mine-0.0.9/README.rst` & `scikit-mine-1.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -37,36 +37,39 @@
 
 
 scikit-mine is a Python module for pattern mining built on top of
 Pandas/Numpy/SciPy and is distributed under the 3-Clause BSD license.
 
 It is currently maintained by a team of volunteers.
 
-See examples in the tutorials; the notebooks are available here_.
+See examples in the tutorials; the notebooks are available here_. To execute the tutorials, you will have to install jupyter notebook or jupyterlab (https://jupyter.org/install)
 
 
 .. _here: https://github.com/scikit-mine/scikit-mine/tree/master/docs/tutorials
 
 
 Dependencies
 ------------
 
-scikit-mine requires Python>=3.7,
+scikit-mine requires Python>=3.8,
 and some extra dependencies
 
 * scipy>=1.2.1
 * pandas>=1.0.0
-* pyroaring
+* pyroaring>=0.3.4
 * joblib>=0.11.1
 * sortedcontainers>=2.1.0
-* dataclasses
-* networkx~=2.5.1
-* wget
+* dataclasses>=0.6
+* networkx
+* wget>=3.2
+* scikit-learn
+* graphviz
+* matplotlib
+* pydot
 
-**scikit-learn** is not a dependency. However, scikit-mine is **contiuously tested for interactions with scikit-learn**
 
 Development
 -----------
 
 This project is funded by the `INRIA center in Rennes, Brittany, France <https://www.inria.fr/fr/centre-inria-rennes-bretagne-atlantique>`_.
 
 We welcome new contributors of all experience levels.
```

### Comparing `scikit-mine-0.0.9/scikit_mine.egg-info/PKG-INFO` & `scikit-mine-1.0.0/scikit_mine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: scikit-mine
-Version: 0.0.9
+Version: 1.0.0
 Summary: Pattern mining in Python
 Home-page: https://github.com/scikit-mine/scikit-mine
 Download-URL: https://github.com/scikit-mine/scikit-mine
 Maintainer: scikit-mine team
 Maintainer-email: skm-dev@inria.fr
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/x-rst
@@ -66,36 +65,39 @@
 
 
 scikit-mine is a Python module for pattern mining built on top of
 Pandas/Numpy/SciPy and is distributed under the 3-Clause BSD license.
 
 It is currently maintained by a team of volunteers.
 
-See examples in the tutorials; the notebooks are available here_.
+See examples in the tutorials; the notebooks are available here_. To execute the tutorials, you will have to install jupyter notebook or jupyterlab (https://jupyter.org/install)
 
 
 .. _here: https://github.com/scikit-mine/scikit-mine/tree/master/docs/tutorials
 
 
 Dependencies
 ------------
 
-scikit-mine requires Python>=3.7,
+scikit-mine requires Python>=3.8,
 and some extra dependencies
 
 * scipy>=1.2.1
 * pandas>=1.0.0
-* pyroaring
+* pyroaring>=0.3.4
 * joblib>=0.11.1
 * sortedcontainers>=2.1.0
-* dataclasses
-* networkx~=2.5.1
-* wget
+* dataclasses>=0.6
+* networkx
+* wget>=3.2
+* scikit-learn
+* graphviz
+* matplotlib
+* pydot
 
-**scikit-learn** is not a dependency. However, scikit-mine is **contiuously tested for interactions with scikit-learn**
 
 Development
 -----------
 
 This project is funded by the `INRIA center in Rennes, Brittany, France <https://www.inria.fr/fr/centre-inria-rennes-bretagne-atlantique>`_.
 
 We welcome new contributors of all experience levels.
```

### Comparing `scikit-mine-0.0.9/setup.py` & `scikit-mine-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
                'Intended Audience :: Developers',
                'License :: OSI Approved',
                'Programming Language :: Python',
                'Programming Language :: Python :: 3.11',
                'Programming Language :: Python :: 3.10',
                'Programming Language :: Python :: 3.9',
                'Programming Language :: Python :: 3.8',
-               'Programming Language :: Python :: 3.7',
                'Topic :: Software Development',
                'Topic :: Scientific/Engineering',
                'Operating System :: Microsoft :: Windows',
                'Operating System :: POSIX',
                'Operating System :: Unix',
                'Operating System :: MacOS']
```

### Comparing `scikit-mine-0.0.9/skmine/callbacks.py` & `scikit-mine-1.0.0/skmine/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Callback API for scikit-mine
 """
-from inspect import signature, getsource
-
 import re
+from inspect import signature, getsource
 
 
 def has_self_assigment(f):
     """
     Parameters
     ----------
     f: callable
 
-    check if no assignement is made on the ``self`` keyword
+    check if no assignment is made on the ``self`` keyword
     """
     try:
         p = r"self(\.\w+)?\s*=.*"
         return any(re.finditer(p, getsource(f)))
     except TypeError:
         return False
 
@@ -96,17 +95,32 @@
     def _frozen(self, *args, **kwargs):
         raise NotImplementedError(f"{type(self)} is immutable")
 
     __setitem__ = _frozen
     update = _frozen
 
     def __call__(self, miner):
-        miner_methods = [
-            f_name for f_name in dir(miner) if callable(getattr(miner, f_name))
-        ]
+        # print("dir(miner)", dir(miner))
+        # print("miner", miner)
+        # print("miner transform", getattr(miner, "transform"))
+        # print("miner update", getattr(miner, "update"),miner.update )
+        # print("miner set_output",miner.set_output )
+
+        miner_methods = []
+        for f_name in dir(miner):
+            try:
+                if callable(getattr(miner, f_name)):
+                    miner_methods.append(f_name)
+            except:
+                print(f"warning : `f_name`='{f_name}' return an error for `callable(getattr(miner, f_name)`")
+
+                # miner_methods = [
+        #     f_name for f_name in dir(miner) if callable(getattr(miner, f_name))
+        # ]
+
         for f_name in self.keys():
             if not f_name in miner_methods:
                 raise ValueError(
                     f"{f_name} found in callbacks while there is not corresponding function"
                 )
 
         for callback_name, callback in self.items():
@@ -119,14 +133,15 @@
 def _print_positive_gain(self, data_size, model_size, *_):
     diff = (self.model_size_ + self.data_size_) - (data_size + model_size)
     if diff > 0.01:
         print(
             "data size : {:.2f} | model size : {:.2f}".format(data_size, model_size)
         )
 
+
 def _print_candidates_size(self, candidates):
     print("{} new candidates considered".format(len(candidates)))
 
 
 mdl_prints = CallBacks(
     evaluate=_print_positive_gain, generate_candidates=_print_candidates_size
 )
```

### Comparing `scikit-mine-0.0.9/skmine/datasets/_base.py` & `scikit-mine-1.0.0/skmine/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-mine-0.0.9/skmine/datasets/_samples_generator.py` & `scikit-mine-1.0.0/skmine/datasets/_samples_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Density of the resulting dataset
     random_state : int, RandomState instance, default=None
         Determines random number generation for dataset creation. Pass an int
         for reproducible output across multiple function calls.
 
     References
     ----------
-    .. [1] F. Flouvat, F. De Marchi, JM. Petit
+    .. F. Flouvat, F. De Marchi, JM. Petit
            "A new classification of datasets for frequent itemsets", 2009
 
     Example
     -------
     >>> from skmine.datasets import make_transactions
     >>> make_transactions(n_transactions=5, n_items=20, density=.25)  # doctest: +SKIP
     0    [0, 6, 18, 10, 1, 12]
```

### Comparing `scikit-mine-0.0.9/skmine/datasets/fimi.py` & `scikit-mine-1.0.0/skmine/datasets/fimi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Base IO for all FIMI datasets
 All datasets are available here : `http://fimi.uantwerpen.be/data/`
 """
-import os
-import wget
 import gzip
+import os
 
 import pandas as pd
+import wget
 
 from ._base import get_data_home
 
 BASE_URL_FIMI = "http://fimi.uantwerpen.be/data/"
 BASE_URL_CGI = "https://cgi.csc.liv.ac.uk/~frans/KDD/Software/LUCS-KDD-DN/DataSets/"
 
 
@@ -206,27 +206,27 @@
 
     Examples
     --------
     >>> from skmine.datasets.fimi import fetch_mushroom
     >>> from skmine.datasets.utils import describe
     >>> X, y = fetch_mushroom(return_y=True)
     >>> describe(X)['n_items']
-    119
+    117
     >>> y.value_counts()
     0    4208
     1    3916
     Name: mushroom, dtype: int64
     """
     mush = fetch_any("mushroom.dat", base_url=BASE_URL_FIMI, data_home=data_home)
     if return_y:
         y = mush.str[0].replace(2, 0)  # 2 is edible, 1 is poisonous
         X = mush.str[1:]
-        return mush, y
-
-    return mush
+        return X, y
+    else:
+        return mush
 
 
 def fetch_pumsb(data_home=None):
     """Fetch and return the pumsb dataset (Frequent Itemset Mining)
 
     The Pumsb dataset contains census data for population and housing.
 
@@ -402,15 +402,16 @@
 
     """
     iris = fetch_any("iris.D19.N150.C3.num.gz", base_url=BASE_URL_CGI, data_home=data_home)
     if return_y:
         y = iris.str[-1]
         X = iris.str[:-1]
         return X, y
-    return iris
+    else:
+        return iris
 
 
 def fetch_breast(data_home=None, return_y=False):
     """Fetch and return the discretized breast dataset (Frequent Itemset Mining)
 
     This dataset corresponds to the breast dataset which has been discretized into 20 items.
     The last column (items: 19, 20) corresponds to the targets and can be useful for classification.
@@ -441,15 +442,16 @@
 
     """
     breast = fetch_any("breast.D20.N699.C2.num", base_url=BASE_URL_CGI, data_home=data_home)
     if return_y:
         y = breast.str[-1]
         X = breast.str[:-1]
         return X, y
-    return breast
+    else:
+        return breast
 
 
 def fetch_tictactoe(data_home=None, return_y=False):
     """Fetch and return the discretized tictactoe dataset (Frequent Itemset Mining)
 
     This dataset corresponds to the tictactoe dataset which has been discretized into 29 items.
     The last column (items: 28, 29) corresponds to the targets and can be useful for classification.
@@ -481,8 +483,9 @@
 
     """
     tictactoe = fetch_any("ticTacToe.D29.N958.C2.num", base_url=BASE_URL_CGI, data_home=data_home)
     if return_y:
         y = tictactoe.str[-1]
         X = tictactoe.str[:-1]
         return X, y
-    return tictactoe
+    else:
+        return tictactoe
```

### Comparing `scikit-mine-0.0.9/skmine/datasets/utils.py` & `scikit-mine-1.0.0/skmine/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-mine-0.0.9/skmine/emerging/mbdldorber.py` & `scikit-mine-1.0.0/skmine/emerging/mbdldorber.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from itertools import combinations
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 
-from ..base import BaseMiner
+from ..base import BaseMiner, DiscovererMixin
 from ..itemsets.lcm import LCMMax
 from ..utils import _check_growth_rate, _check_min_supp, filter_maximal, filter_minimal
 
 
 def border_diff(U, S):
     """
     Given a pair of borders <{∅}, {U}> and <{∅}, {S}>,
@@ -98,15 +98,15 @@
             if any((e.issuperset(set(pat)) for e in left)):
                 continue
             patterns.append(pat)
 
     return pd.Series(patterns)
 
 
-class MBDLLBorder(BaseMiner):
+class MBDLLBorder(BaseMiner, DiscovererMixin):
     """
     MBD-LLBorder aims at discovering patterns characterizing the difference
     between two collections of data.
 
     It first discovers ``two sets of maximal itemsets``, one for each collection.
     It then looks for borders of these sets, and characterizes the difference
     by only manipulating theses borders.
@@ -144,17 +144,17 @@
     ----------
     .. [1]
         Guozhu Dong, Jinyan Li
         "Efficient Mining of Emerging Patterns : Discovering Trends and Differences", 1999
     """
 
     def __init__(self, min_growth_rate=2, min_supp=0.1, n_jobs=1):
-        self.min_supp = _check_min_supp(min_supp, accept_absolute=False)
+        _check_min_supp(min_supp, accept_absolute=False)
+        self.min_supp = min_supp
         self.min_growth_rate = _check_growth_rate(min_growth_rate)
-        self.borders_ = None
         self.n_jobs = n_jobs
 
     def fit(self, D, y):
         """
         fit MBD-LLBorder on D, splitted on y
 
         This is done in two steps
@@ -168,25 +168,24 @@
             Where every entry contains singular items
             Items must be both hashable and comparable
 
         y : array-like of shape (n_samples,)
             Targets on which to split D
             Must contain only two disctinct values, i.e len(np.unique(y)) == 2
         """
+
         labels = np.unique(y)
         assert len(labels) == 2
         assert isinstance(D, pd.Series)  # TODO : accept tabular data
 
         D1, D2 = D[y == labels[0]], D[y == labels[1]]
 
         # TODO : replace LCMMax by some more efficient method
-        right_border_d1 = LCMMax(min_supp=self.min_supp).fit_discover(D1)
-        right_border_d2 = LCMMax(
-            min_supp=self.min_growth_rate * self.min_supp
-        ).fit_discover(D2)
+        right_border_d1 = LCMMax(min_supp=self.min_supp).fit_transform(D1)
+        right_border_d2 = LCMMax(min_supp=self.min_growth_rate * self.min_supp).fit_transform(D2)
 
         right_border_d1 = right_border_d1.itemset.map(set).tolist()
         right_border_d2 = right_border_d2.itemset.map(set).tolist()
 
         self.borders_ = mbdllborder(right_border_d1, right_border_d2)
 
         return self
```

### Comparing `scikit-mine-0.0.9/skmine/feature_extraction/slim_vectorizer.py` & `scikit-mine-1.0.0/skmine/feature_extraction/slim_vectorizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 SLIM vectorizer, using SLIM as a feature extraction scheme
 """
 
 import numpy as np
 import pandas as pd
 
-from ..base import TransformerMixin
-from ..itemsets import SLIM
-from ..itemsets.slim import _to_vertical, cover
+from skmine.itemsets import SLIM
+from skmine.itemsets.slim import _to_vertical, cover
 
 STRATEGIES = ("codes", "one-hot")
 
 
 def _filter_stop_items(D, stop_items):
     for t in D:
         yield set(t).difference(stop_items)
 
 
-class SLIMVectorizer(SLIM, TransformerMixin):
+class SLIMVectorizer(SLIM):
     """SLIM mining, turned into a feature extraction step for sklearn
 
     `k` new itemsets (associations of one or more items) are learned at training time
 
     The model (pattern set) is then used to cover new data, in order of usage.
     This is similar to one-hot-encoding, except the dimension will be much more concise,
     because the columns will be patterns learned via an MDL criterion.
@@ -47,15 +46,16 @@
         Set of items to filter out while ingesting the input data.
 
 
     Examples
     --------
     >>> from skmine.feature_extraction import SLIMVectorizer
     >>> D = [['bananas', 'milk'], ['milk', 'bananas', 'cookies'], ['cookies', 'butter', 'tea']]
-    >>> SLIMVectorizer(k=2).fit_transform(D)
+    >>> res  = SLIMVectorizer(k=2).fit_transform(D)
+    >>> print(res.to_string())
        (bananas, milk)  (cookies,)
     0              0.4         0.0
     1              0.4         0.4
     2              0.0         0.4
 
 
     See Also
@@ -66,29 +66,29 @@
     -----
     This transformer does not output scipy.sparse matrices,
     as SLIM should learn a concise description of the data,
     and covering new data with this small set of high usage
     patterns should output matrices with very few zeros.
     """
 
-    def __init__(self, strategy="codes", *, k=5, pruning=False, stop_items=None, **kwargs):
+    def __init__(self, strategy="codes", k=5, pruning=False, stop_items=None, **kwargs):
         super().__init__(**kwargs)
         self.k = k
         self.pruning = pruning
         self.stop_items = stop_items
         if strategy not in STRATEGIES:
             raise ValueError(f"strategy must be one of {STRATEGIES}")
         self.strategy = strategy
 
     def fit(self, D, y=None):
         if self.stop_items is not None:
             D = _filter_stop_items(D, stop_items=self.stop_items)
         return super().fit(D)
 
-    def transform(self, D, y=None):
+    def transform(self, newD, y=None, **tsf_params) -> pd.DataFrame:
         """Transform new data
 
         Parameters
         ----------
         D: iterable
             transactional data
 
@@ -98,17 +98,16 @@
             a dataframe of `len(D)` rows and `self.k` columns
 
         See Also
         --------
         skmine.itemsets.SLIM.cover
         """
         stop_items = self.stop_items or set()
-        D_sct, _len = _to_vertical(D, stop_items=stop_items, return_len=True)
-
-        code_lengths = self.discover(return_tids=False, singletons=True, drop_null_usage=False)
+        D_sct, _len = _to_vertical(newD, stop_items=stop_items, return_len=True)
+        code_lengths = super().transform(newD, return_tids=False, singletons=True, drop_null_usage=False)
         code_lengths = pd.Series(code_lengths["usage"].values, index=code_lengths["itemset"].apply(tuple))
         code_lengths = code_lengths[code_lengths.index.map(set(D_sct).issuperset)]
 
         isets = code_lengths.nlargest(self.k)  # real usages sorted in decreasing order
         covers = cover(D_sct, isets.index)
 
         mat = np.zeros(shape=(_len, len(covers)))
```

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/candidate.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/candidate.py`

 * *Files identical despite different names*

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/code_table.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/code_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import logging
+import math
 import time
 from collections import defaultdict
+
+import networkx as nx
 import numpy
 import pandas
-from .code_table_row import CodeTableRow
-import math
-import networkx as nx
+
 import skmine.graph.graphmdl.utils as utils
+from .code_table_row import CodeTableRow
 
 
 class CodeTable:
     """
         Code table inspired from Krimp algorithm.
 
         It's composed by the non singleton pattern and their information (usage, ports) who represented by a row
```

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/code_table_row.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/code_table_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from skmine.graph.graphmdl import utils
 import math
 
+from skmine.graph.graphmdl import utils
+
 
 class CodeTableRow:
     """
         Object to represent a row of the code table
         Its concerns only non-singleton pattern
 
         Parameters
```

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/graph_mdl.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/graph_mdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import copy
-import logging
 import time
-import networkx
+
 from skmine.base import BaseMiner
-from skmine.graph.graphmdl.label_codes import LabelCodes
+from skmine.graph.graphmdl import utils
 from skmine.graph.graphmdl.code_table import CodeTable
 from skmine.graph.graphmdl.code_table_row import CodeTableRow
-from skmine.graph.graphmdl import utils
+from skmine.graph.graphmdl.label_codes import LabelCodes
 
 
 def _order_pruning_rows(row):
     """ Sort the pruning row by their usage"""
     return row.pattern_usage()
```

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/label_codes.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/label_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from networkx import Graph
+
 import skmine.graph.graphmdl.utils as utils
 
 
 class LabelCodes:
     """
       It is only a storage for label frequency in the initial data graph
```

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/test/test_graph_mdl.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/test/test_graph_mdl.py`

 * *Files identical despite different names*

### Comparing `scikit-mine-0.0.9/skmine/graph/graphmdl/utils.py` & `scikit-mine-1.0.0/skmine/graph/graphmdl/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-mine-0.0.9/skmine/itemsets/lcm.py` & `scikit-mine-1.0.0/skmine/itemsets/lcm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,90 +7,89 @@
 #          Luis Galárraga <galarraga@luisgalarraga.de>
 #          Hermann Courteille <hermann.courteille@irisa.fr>
 #          Cyril Regan <cyril.regan@loria.fr>
 #          Thomas Betton <thomas.betton@irisa.fr>
 #
 # License: BSD 3 clause
 
+import os
+import shutil
 from collections import defaultdict
 from itertools import takewhile
+
 import pandas as pd
-import os
-import shutil
 from joblib import Parallel, delayed
-from sortedcontainers import SortedDict
 from pyroaring import BitMap as Bitmap
+from sklearn.base import BaseEstimator
+from sklearn.utils.validation import check_is_fitted
+from sortedcontainers import SortedDict
 
+from skmine.base import TransformerMixin
 from ..utils import _check_min_supp
 from ..utils import filter_maximal
 
-from ..base import BaseMiner
 
-
-class LCM(BaseMiner):
+class LCM(TransformerMixin, BaseEstimator):
     """
     Linear time Closed item set Miner.
 
     LCM can be used as a **generic purpose** miner, yielding some patterns
     that will be later submitted to a custom acceptance criterion.
 
     It can also be used to simply discover the set of **closed itemsets** from
     a transactional dataset.
 
     Parameters
     ----------
     min_supp: int or float, default=0.2
-        The minimum support for itemsets to be rendered in the output
-        Either an int representing the absolute support, or a float for relative support
-        Default to 0.2 (20%)
+        The minimum support for itemsets to be rendered in the output either an int representing the absolute support,
+        or a float for relative support. By Default to 0.2 (20%)
 
     n_jobs : int, default=1 The number of jobs to use for the computation. Each single item is attributed a job to
         discover potential itemsets, considering this item as a root in the search space. **Processes are preferred**
         over threads. **Carefully adjust the number of jobs** otherwise the results may be corrupted especially if you
         have the following warning: UserWarning: A worker stopped while some jobs were given to the executor.
 
     References
     ----------
-    .. [1]
-        Takeaki Uno, Masashi Kiyomi, Hiroki Arimura
+    .. [1] Takeaki Uno, Masashi Kiyomi, Hiroki Arimura
         "LCM ver. 2: Efficient mining algorithms for frequent/closed/maximal itemsets", 2004
 
     .. [2] Alexandre Termier
         "Pattern mining rock: more, faster, better"
 
     Examples
     --------
 
     >>> from skmine.itemsets import LCM
     >>> from skmine.datasets.fimi import fetch_chess
     >>> chess = fetch_chess()
     >>> lcm = LCM(min_supp=2000)
-    >>> patterns = lcm.fit_discover(chess)
+    >>> patterns = lcm.fit_transform(chess)
     >>> patterns.head()
         itemset  support
     0      [58]     3195
     1      [52]     3185
     2  [52, 58]     3184
     3      [29]     3181
     4  [29, 58]     3180
     >>> patterns[patterns.itemset.map(len) > 3]  # doctest: +SKIP
     """
 
     def __init__(self, *, min_supp=0.2, n_jobs=1, verbose=False):
-        _check_min_supp(min_supp)
         self.min_supp = min_supp  # cf docstring: minimum support provided by user
-        self.max_length = -1  # maximum length of an itemset
-        self.verbose = verbose
-        self._min_supp = _check_min_supp(self.min_supp)
-        self.item_to_tids = SortedDict()  # Dict : key item ordered by decreasing frequency , value : tids for this
-        # item
-        self.ord_item_freq = []  # list of ordered item by decreasing frequency
         self.n_jobs = n_jobs  # number of jobs launched by joblib
-        self.lexicographic_order = False  # if true, the items of each itemset are returned in lexicographical order
-        self.return_tids = False
+        self.verbose = verbose
+
+    def _more_tags(self):
+        return {
+            "non_deterministic": True,
+            "preserves_dtype": False,
+            "no_validation": True,
+        }
 
     def fit(self, D, y=None):
         """
         fit LCM on the transactional database, by keeping records of singular items
         and their transaction ids.
 
         Parameters
@@ -104,60 +103,67 @@
 
         Raises
         ------
         TypeError
             if any entry in D is not iterable itself OR if any item is not **hashable**
             OR if all items are not **comparable** with each other.
         """
+
+        self._validate_data(D, force_all_finite=False, accept_sparse=False, ensure_2d=False, ensure_min_samples=1,
+                            dtype=list)
         n_transactions_ = 0
         item_to_tids_ = defaultdict(Bitmap)
         for transaction in D:
             for item in transaction:
                 item_to_tids_[item].add(n_transactions_)
             n_transactions_ += 1
 
+        _check_min_supp(self.min_supp)
         if isinstance(self.min_supp, float):  # make support absolute if needed
-            self._min_supp = self.min_supp * n_transactions_
+            self.min_supp_ = self.min_supp * n_transactions_
+        else:
+            self.min_supp_ = self.min_supp
 
-        low_supp_items = [k for k, v in item_to_tids_.items() if len(v) < self._min_supp]
+        low_supp_items = [k for k, v in item_to_tids_.items() if len(v) < self.min_supp_]
         for item in low_supp_items:  # drop low freq items
             del item_to_tids_[item]
 
         ord_freq_list = sorted(item_to_tids_.items(), key=lambda item: len(item[1]), reverse=True)
         ord_freq_dic = defaultdict(Bitmap)
         ord_item_freq = []
         for idx, element in enumerate(ord_freq_list):
             item, tid = element
             ord_item_freq.append(item)
             ord_freq_dic[idx] = tid  # rename most frequent item like cat by 0, second  dog by 1
 
-        self.item_to_tids = SortedDict(ord_freq_dic)  # {0:tids0, 1:tids1 ....}
-        self.ord_item_freq = ord_item_freq  # [cat, dog, '0', ...]
+        self.item_to_tids_ = SortedDict(ord_freq_dic)  # {0:tids0, 1:tids1 ....}key item ordered by decreasing frequency
+        self.ord_item_freq_ = ord_item_freq  # [cat, dog, '0', ...] list of ordered item by decreasing frequency
+        self.n_features_in_ = D.shape[-1] if not isinstance(D, list) else len(D[-1])  # nb items
 
-        return self  # for call .fit().discover() in DiscovererMixin()
+        return self
 
-    def discover(self, *, return_tids=False, lexicographic_order=True, max_length=-1, out=None):
+    def transform(self, D, return_tids=False, lexicographic_order=True, max_length=-1, out=None):
         """Return the set of closed itemsets, with respect to the minimum support
 
         Parameters
         ----------
         D : pd.Series or Iterable
-            The input transactional database
-            Where every entry contain singular items
-            Items must be both hashable and comparable
+            The input transactional database where every entry contain singular items
+            must be both hashable and comparable. Does not influence the results.
+            Present for compatibility with scikit-learn.
 
         return_tids: bool, default=False
             Either to return transaction ids along with itemset.
             Default to False, will return supports instead
 
         lexicographic_order: bool, default=True
             Either the order of the items in each itemset is not ordered or the items are ordered lexicographically
 
-        max_length: int, default=-1 Maximum length of an itemset. By default, -1 means that LCM returns itemsets of
-        all lengths.
+        max_length: int, default=-1
+            Maximum length of an itemset. By default, -1 means that LCM returns itemsets of all lengths.
 
         out : str, default=None
             File where results are written. Discover return None. The 'out' option is usefull 
             to save memory : Instead of store all branch of lcm-tree in memory , each root 
             branch of lcm is written in a separated file in dir (TEMP_dir), and all files are
             concatenated in the final 'out' file.
 
@@ -177,64 +183,69 @@
                 tids        a bitmap tracking positions
                 ==========  =================================
 
         Example
         -------
         >>> from skmine.itemsets import LCM
         >>> D = [[1, 2, 3, 4, 5, 6], [2, 3, 5], [2, 5]]
-        >>> LCM(min_supp=2).fit_discover(D, lexicographic_order=True)
+        >>> LCM(min_supp=2).fit_transform(D, lexicographic_order=True)
              itemset  support
         0     [2, 5]        3
         1  [2, 3, 5]        2
-        >>> LCM(min_supp=2).fit_discover(D, return_tids=True)
+        >>> LCM(min_supp=2).fit_transform(D, return_tids=True)
              itemset  support       tids
         0     [2, 5]        3  (0, 1, 2)
         1  [2, 3, 5]        2     (0, 1)
         """
-        self.lexicographic_order = lexicographic_order
-        self.return_tids = return_tids
-        self.max_length = max_length
-        if out is None:  # store results in memory
+        self.lexicographic_order_ = lexicographic_order
+        self.return_tids_ = return_tids
+        self.max_length_ = max_length  # maximum length of an itemset,  -1 by default
+        self.out_ = out
+
+        check_is_fitted(self, 'n_features_in_')
+        n_features_in_ = D.shape[-1] if not isinstance(D, list) else len(D[-1])  # nb items
+        if n_features_in_ != self.n_features_in_:  # TODO : significant for one-hot D ,not for list of itemset
+            raise ValueError('Shape of input is different from what was seen in `fit`')
+
+        if self.out_ is None:  # store results in memory
             dfs = Parallel(n_jobs=self.n_jobs, prefer="processes")(
-                delayed(self._explore_root)(item, tids, root_file=None) for item, tids in
-                list(self.item_to_tids.items())
-            )  # dfs is a list of dataframe
-            # make sure we have something to concat
-            columns = ["itemset", "support"] if not self.return_tids else ["itemset", "support", "tids"]
+                delayed(self._explore_root)(item, tids, root_file=None)
+                for item, tids in list(self.item_to_tids_.items()))
+            # dfs is a list of dataframe    # make sure we have something to concat
+            columns = ["itemset", "support"] if not self.return_tids_ else ["itemset", "support", "tids"]
             df = pd.concat([pd.DataFrame(columns=columns)] + dfs, axis=0, ignore_index=True)
             df["support"] = pd.to_numeric(df["support"])
 
             return df
 
         else:  # store results in files
             temp_dir = 'TEMP_dir'  # temporary dir where root items branch files are written
             if os.path.exists(temp_dir):  # remove dir TEMP_dir if it exists
                 shutil.rmtree(temp_dir)
             os.mkdir(temp_dir)  # create dir TEMP_dir
 
             Parallel(n_jobs=self.n_jobs, prefer="processes")(
-                delayed(self._explore_root)(
-                    item, tids, root_file=f"{temp_dir}/root{k}.dat") for k, (
-                    item, tids) in enumerate(list(self.item_to_tids.items()))
-            )
+                delayed(self._explore_root)(item, tids, root_file=f"{temp_dir}/root{k}.dat")
+                for k, (item, tids) in enumerate(list(self.item_to_tids_.items())))
 
-            with open(out, 'w') as outfile:  # concatenate all itemsroot files located in temp_dir in a single file
+            with open(self.out_,
+                      'w') as outfile:  # concatenate all itemsroot files located in temp_dir in a single file
                 for fname in [f"{temp_dir}/root{k}.dat" for k in
-                              range(len(list(self.item_to_tids.items())))]:  # all items root files
+                              range(len(list(self.item_to_tids_.items())))]:  # all items root files
                     with open(fname) as infile:
                         for line in infile:
                             if line.strip():  # to skip empty lines
                                 outfile.write(line)
             shutil.rmtree(temp_dir)  # remove the temporary dir where root files are written
 
             return None
 
     def _explore_root(self, item, tids, root_file=None):
         it = self._inner((frozenset(), tids), item)
-        columns = ["itemset", "support"] if not self.return_tids else ["itemset", "support", "tids"]
+        columns = ["itemset", "support"] if not self.return_tids_ else ["itemset", "support", "tids"]
         df = pd.DataFrame(data=it, columns=columns)
 
         if self.verbose and not df.empty:
             print("LCM found {} new itemsets from root item : {}".format(len(df), item))
 
         if root_file is not None:  # for writing the items root files in dir self.temp_dir
 
@@ -243,57 +254,56 @@
 
             self.write_df_tofile(root_file, df)
             return None
         else:
             return df
 
     def _inner(self, p_tids, limit):
-
         p, tids = p_tids
         # project and reduce DB w.r.t P
         cp = (
             item
-            for item, ids in reversed(self.item_to_tids.items())
+            for item, ids in reversed(self.item_to_tids_.items())
             if tids.issubset(ids)
             if item not in p
         )
 
         # items are in reverse order, so the first consumed is the max
         max_k = next(takewhile(lambda e: e >= limit, cp), None)
 
         if max_k is not None and max_k == limit:
             p_prime = (p | set(cp) | {max_k})  # max_k has been consumed when calling next()
             # sorted items in ouput for better reproducibility
-            itemset = [self.ord_item_freq[ind] for ind in list(p_prime)]
-            itemset = sorted(itemset) if self.lexicographic_order else itemset
+            itemset = [self.ord_item_freq_[ind] for ind in list(p_prime)]
+            itemset = sorted(itemset) if self.lexicographic_order_ else itemset
 
-            if len(itemset) <= self.max_length or self.max_length == -1:
-                if not self.return_tids:
+            if len(itemset) <= self.max_length_ or self.max_length_ == -1:
+                if not self.return_tids_:
                     yield itemset, len(tids)
                 else:
                     yield itemset, len(tids), tids
 
-            candidates = self.item_to_tids.keys() - p_prime
+            candidates = self.item_to_tids_.keys() - p_prime
             candidates = candidates[: candidates.bisect_left(limit)]
             for new_limit in candidates:
-                ids = self.item_to_tids[new_limit]
-                if tids.intersection_cardinality(ids) >= self._min_supp:
+                ids = self.item_to_tids_[new_limit]
+                if tids.intersection_cardinality(ids) >= self.min_supp_:
                     # new pattern and its associated tids
                     new_p_tids = (p_prime, tids.intersection(ids))
                     yield from self._inner(new_p_tids, new_limit)
 
     def write_df_tofile(self, filename, df):
         with open(filename, 'w') as fw:  # write the items root files
             for index, row in df.iterrows():
                 fw.write(f"({row['support']}) {' '.join(map(str, row['itemset']))}\n")
-                if self.return_tids:
+                if self.return_tids_:
                     fw.write(f"{' '.join(map(str, row['tids']))}\n")
 
 
-class LCMMax(LCM):
+class LCMMax(LCM, TransformerMixin):
     """
     Linear time Closed item set Miner adapted to Maximal itemsets (or borders).
 
     A maximal itemset is an itemset with no frequent superset.
 
     Parameters
     ----------
@@ -313,61 +323,61 @@
     """
 
     def _inner(self, p_tids, limit):
         p, tids = p_tids
         # project and reduce DB w.r.t P
         cp = (
             item
-            for item, ids in reversed(self.item_to_tids.items())
+            for item, ids in reversed(self.item_to_tids_.items())
             if tids.issubset(ids)
             if item not in p
         )
         max_k = next(cp, None)  # items are in reverse order, so the first consumed is the max
 
         if max_k is not None and max_k == limit:
             p_prime = (p | set(cp) | {max_k})  # max_k has been consumed when calling next()
-            candidates = self.item_to_tids.keys() - p_prime
+            candidates = self.item_to_tids_.keys() - p_prime
             candidates = candidates[: candidates.bisect_left(limit)]
             no_cand = True
 
             for new_limit in candidates:
-                ids = self.item_to_tids[new_limit]
-                if tids.intersection_cardinality(ids) >= self._min_supp:
+                ids = self.item_to_tids_[new_limit]
+                if tids.intersection_cardinality(ids) >= self.min_supp_:
                     no_cand = False
                     # get new pattern and its associated tids
                     new_p_tids = (p_prime, tids.intersection(ids))
                     yield from self._inner(new_p_tids, new_limit)
 
             if no_cand:  # only if no child node. This is how we PRE-check for maximality
-                itemset = set([self.ord_item_freq[ind] for ind in p_prime])
+                itemset = set([self.ord_item_freq_[ind] for ind in p_prime])
 
-                if not self.return_tids:
+                if not self.return_tids_:
                     yield itemset, len(tids)
                 else:
                     yield itemset, len(tids), tids
 
-    def discover(self, *args, **kwargs):
+    def transform(self, X=None, *args, **kwargs):
         outfile = kwargs.get('out')
         kwargs['out'] = None
-        patterns = super().discover(**kwargs)
+        patterns = super().transform(X, **kwargs)
         # keep only maximal itemsets
         maximals = filter_maximal(patterns["itemset"])
         patterns = patterns[patterns.itemset.isin(maximals)].copy()
 
         # keeps only itemsets smaller than max_length
-        if self.max_length != -1:
-            length_mask = patterns.itemset.apply(lambda x: len(x) <= self.max_length)
+        if self.max_length_ != -1:
+            length_mask = patterns.itemset.apply(lambda x: len(x) <= self.max_length_)
             patterns = patterns[length_mask]
             patterns.reset_index(drop=True, inplace=True)
 
         # return a list of itemset sorted or not
         patterns.loc[:, "itemset"] = patterns["itemset"].map(
-            lambda i: sorted(list(i)) if self.lexicographic_order else list(i))
+            lambda i: sorted(list(i)) if self.lexicographic_order_ else list(i))
 
         if outfile:
             self.write_df_tofile(outfile, patterns)
             return None
         else:
             return patterns
 
-    setattr(discover, "__doc__", LCM.discover.__doc__.replace("closed", "maximal"))
-    setattr(discover, "__doc__", LCM.discover.__doc__.split("Example")[0])
+    setattr(transform, "__doc__", LCM.transform.__doc__.replace("closed", "maximal"))
+    setattr(transform, "__doc__", LCM.transform.__doc__.split("Example")[0])
```

### Comparing `scikit-mine-0.0.9/skmine/itemsets/slim.py` & `scikit-mine-1.0.0/skmine/itemsets/slim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """SLIM pattern discovery
 based on `https://eda.mmci.uni-saarland.de/pubs/2012/slim_directly_mining_descriptive_patterns-smets,vreeken.pdf
 and https://eda.rg.cispa.io/pres/ida14-slimmer-poster.pdf
 """
 
 # Authors: Rémi Adon <remi.adon@gmail.com>
 #          Thomas Betton <thomas.betton@irisa.fr>
+#          Hermann Courteille <hermann.courteille@irisa.fr>
+#          Cyril Regan <cyril.regan@loria.fr>
 # License: BSD 3 clause
 
+import time
 from collections import Counter, defaultdict
 from functools import lru_cache, reduce
 from itertools import chain
 
 import numpy as np
 import pandas as pd
-import time
-from sortedcontainers import SortedDict
 from pyroaring import BitMap as Bitmap
+from sklearn.base import BaseEstimator
+from sklearn.utils.validation import check_is_fitted
+from sortedcontainers import SortedDict
 
-
-from ..base import BaseMiner, InteractiveMiner, MDLOptimizer
+from skmine.base import TransformerMixin
 from ..utils import _check_D, supervised_to_unsupervised
-from sklearn.utils.validation import check_is_fitted
 
 
-def _to_vertical(D, stop_items=None, return_len=False):
+def _to_vertical(D, stop_items=None, return_len=False):  # -> tuple | dict
     if stop_items is None:
         stop_items = set()
     res = defaultdict(Bitmap)
     idx = 0
     for idx, transaction in enumerate(D):
         for e in transaction:
             if e not in stop_items:
                 res[e].add(idx)
     if return_len:  # correspond to the number of transactions
         return dict(res), idx + 1
     return dict(res)
 
 
-def _log2(values):
+def _log2(values) -> pd.Series:
     """
     This function calculates the log2 of a set of values.
     Be careful, if one of the values is 0, the function will return 0.
 
     Parameters
     ----------
     values: pd.Series
@@ -51,26 +53,26 @@
     -------
     pd.Series
         The set of values present in "values" after applying the log2 function with the correct index if there was one
         in a pd.Series.
     """
     res_index = values.index if isinstance(values, pd.Series) else None
     res = np.zeros(len(values), dtype=np.float32)
-    res[values != 0] = np.log2(values[values != 0]).astype(np.float32)
+    res[values != 0] = np.log2(values[values != 0]).astype(np.float32)  # TODO : see if pb in 0 issue Alex
     return pd.Series(res, index=res_index)
 
 
-def cover(sct: dict, itemsets: list):
+def cover(sct: dict, itemsets: list) -> dict:
     """
     cover a standard codetable sct given itemsets
 
     Parameters
     ----------
     sct: dict[object, Bitmap]
-        a standard codetable, i.e the vertical representation of a dataset
+        a standard codetable, i.e. the vertical representation of a dataset
     itemsets: list[frozenset]
         itemsets from a given codetable
 
     Note
     ----
         sct is modified inplace
     """
@@ -80,15 +82,15 @@
         usage = reduce(Bitmap.intersection, it).copy() if it else Bitmap()
         covers[iset] = usage
         for k in iset:
             sct[k] -= usage
     return covers
 
 
-class SLIM(BaseMiner, MDLOptimizer, InteractiveMiner):
+class SLIM(BaseEstimator, TransformerMixin):
     """SLIM: Directly Mining Descriptive Patterns
 
     SLIM looks for a compressed representation of transactional data.
     This compressed representation if a set of descriptive patterns,
     and can be used to:
 
     - provide a natively interpretable modeling of this data
@@ -110,15 +112,15 @@
         compression progress of the database gets weaker and weaker, so it may be useful to use this parameter.
 
 
     Examples
     --------
     >>> from skmine.itemsets import SLIM
     >>> D = [['bananas', 'milk'], ['milk', 'bananas', 'cookies'], ['cookies', 'butter', 'tea']]
-    >>> SLIM().fit(D).discover(singletons=True, return_tids=True)
+    >>> SLIM().fit(D).transform(D, singletons=True, return_tids=True)
                itemset    tids
     0  [bananas, milk]  (0, 1)
     1    [butter, tea]     (2)
     2        [cookies]  (1, 2)
 
     References
     ----------
@@ -126,20 +128,27 @@
         Smets, K & Vreeken, J
         "Slim: Directly Mining Descriptive Patterns", 2012
 
     .. [2] Gandhi, M & Vreeken, J
         "Slimmer, outsmarting Slim", 2014
     """
 
-    def __init__(self, *, pruning=True, max_time=-1, items=None):
+    def __init__(self, pruning=True, max_time=-1, items=None):
         self.pruning = pruning
         self.max_time = max_time
         self.items = items
 
-    def fit(self, X, y=None):  # pylint:disable = too-many-locals
+    def _more_tags(self):
+        return {
+            "non_deterministic": True,
+            "no_validation": True,
+            "preserves_dtype": [],
+        }
+
+    def fit(self, X, y=None):
         """fit SLIM on a transactional dataset
 
         This generates new candidate patterns and add those which improve compression,
         iteratibely refining ``self.codetable_``
 
 
         Parameters
@@ -147,21 +156,21 @@
         X: iterable of iterables or array-like
             Transactional dataset, either as an iterable of iterables
             or encoded as tabular binary data
 
         y: Ignored
             Not used, present here for API consistency by convention.
         """
-        self.starting_codes_ = None
-        self.standard_codetable_ = None
-        self.codetable_ = SortedDict()
-        self.model_size_ = None  # L(CT|D)
-        self.data_size_ = None  # L(D|CT)
-        self.is_fitted_ = True
+        if y is not None:
+            self.classes_ = np.unique(y)
 
+        self._validate_data(X, force_all_finite=False, accept_sparse=False, ensure_2d=False,
+                            ensure_min_samples=1, dtype=list)
+        self.n_features_in_ = X.shape[-1] if not isinstance(X, list) else len(X[-1])
+        # TODO : significant for one-hot D, not for list of itemset
         start = time.time()
         self.prefit(X, y=y)
         while True:
             seen_cands = set(self.codetable_.keys())
             candidates = self.generate_candidates(stack=seen_cands)
 
             if not candidates:  # if empty candidate generation
@@ -177,56 +186,97 @@
 
             if diff <= 0:  # if no more candidates are found that improve the model, we stop
                 break
 
             if self.max_time != -1 and time.time() - start > self.max_time:
                 break
 
+        self.is_fitted_ = True
         return self
 
-    def decision_function(self, D):
+    def get_code_length(self, D):
         """Compute covers on new data, and return code length
 
-        This function is named ``decision_function`` because code lengths
-        represent the distance between a point and the current codetable.
-
         Setting ``pruning`` to False when creating the model
         is recommended to cover unseen data, and especially when building a classifier.
 
         Parameters
         ----------
-        D: pd.DataFrame or np.ndarray
-            new data to make predictions on, in tabular format
+        D: list or np.ndarray or pd.DataFrame
+          new data to make predictions on, in tabular format.
 
+        Note
+        ----
+        type of input D should be the same as in one ingest in fit method
+
+        Returns
+        -------
+        codes_length : pandas.Series
+            codes length  for all itemset in D (float32)
         Example
         -------
         >>> from skmine.itemsets import SLIM; import pandas as pd
         >>> def to_tabular(D): return pd.Series(D).str.join('|').str.get_dummies(sep="|")
         >>> D = [['bananas', 'milk'], ['milk', 'bananas', 'cookies'], ['cookies', 'butter', 'tea']]
         >>> new_D = to_tabular([['cookies', 'butter']])
         >>> slim = SLIM().fit(to_tabular(D))
-        >>> slim.decision_function(new_D)
-        0   -5.584963
+        >>> slim.get_code_length(new_D)
+        0    5.584963
         dtype: float32
 
         See Also
         --------
         cover
         discover
         """
+
         mat = self.cover(D)
-        code_lengths = self.discover(singletons=True, return_tids=False, drop_null_usage=False)
+        code_lengths = self.transform(D, singletons=True, return_tids=False, drop_null_usage=False)
         # the codetable is Laplace corrected: the usage of each itemset is increased by 1 in order that all seen
         # items have a code
         code_lengths["usage"] += 1
-        code_lengths["code"] = _log2(code_lengths["usage"] / code_lengths["usage"].sum())
+        code_lengths["code"] = -_log2(code_lengths["usage"] / code_lengths["usage"].sum())
         mapping = {tuple(row['itemset']): row['code'] for _, row in code_lengths.iterrows()}
-        codes = mat.replace(True, mapping).sum(axis=1).astype(np.float32)
-        codes[codes == 0] = -np.inf  # zeros would fool a `shortest code wins` strategy
-        return codes
+        codes_length_D = mat.replace(True, mapping).sum(axis=1).astype(np.float32)
+        codes_length_D[codes_length_D == 0] = + np.inf  # zeros would fool a `shortest code wins` strategy
+
+        return codes_length_D
+
+    def decision_function(self, D):
+        """ Function use to predict class of itemset D (can be a list of iterable of itemset).
+         It is used by a classifier predict method, like in sklearn.multiclass.OneVsRestClassifier where
+         the highest values of decision_function among all classes.
+
+        The shorter code length ($cl \in ]0 + \infty[$) of D is,
+        the higher is the probability for D to belong to same class.
+        Therefore, mapping function _fonc(.)  should be monotonically decreasing on $]0 + \infty[$
+        We choose by default $_fonc(x)=exp(-0.2*x)$ to get probability in $]0,1]$ but other can be coded like
+        $_fonc(x)=-x$
+
+        Unlike to sklearn-convention (https://scikit-learn.org/stable/glossary.html#term-decision_function),
+        this decision function doesn't return a signed distance from a boundary because it's not easy to compute it.
+
+        Parameters
+        ----------
+        D: list or np.ndarray or pd.DataFrame
+          new data to make predictions on, in tabular format
+
+        Note
+        ----
+        type of input D should be the same as in one ingest in fit method
+
+        Returns
+        -------
+         prob : pandas.Series
+            probability for D to belong to the same class
+        """
+        _fonc = lambda x: np.exp(-0.2 * x)
+        x = self.get_code_length(D)
+        prob = _fonc(x)
+        return prob
 
     def generate_candidates(self, stack=None):
         """
         Generate candidates  from a copy of the codetable and return the candidates sorted in descending order of
         estimated gain.
         For each element of the codetable, the union with each following element is performed and an estimated gain is
         calculated. If this gain is positive, the union is returned.
@@ -268,17 +318,16 @@
                 new_usage_X = old_usage_X - new_usage_XY
                 new_usage_Y = old_usage_Y - new_usage_XY
                 old_countsum = sum(len(usage) for usage in codetable.values())
                 new_countsum = old_countsum - new_usage_XY
                 old_num_codes_with_non_zero_usage = sum(1 if len(usage) > 0 else 0 for usage in codetable.values())
                 new_num_codes_with_non_zero_usage = old_num_codes_with_non_zero_usage + 1 \
                                                     - (1 if new_usage_X == 0 else 0) - (1 if new_usage_Y == 0 else 0)
-                log_values = _log2(
-                    np.array([old_usage_X, old_usage_Y, new_usage_XY, new_usage_X, new_usage_Y, old_countsum,
-                              new_countsum]))
+                log_values = _log2(np.array([old_usage_X, old_usage_Y, new_usage_XY,
+                                             new_usage_X, new_usage_Y, old_countsum, new_countsum]))
 
                 # Estimation of the size of the database gain
                 gain_db_XY = -1 * (
                         -new_usage_XY * log_values[2] - new_usage_X * log_values[3] + old_usage_X * log_values[0]
                         - new_usage_Y * log_values[4] + old_usage_Y * log_values[1] + new_countsum *
                         log_values[6] - old_countsum * log_values[5])
 
@@ -318,15 +367,15 @@
 
                 if gain_XY > 0:
                     candidates.append((XY, gain_XY))
 
         # sort the itemsets by decreasing order gain
         return sorted(candidates, key=lambda e: e[1], reverse=True)
 
-    def evaluate(self, candidate):
+    def evaluate(self, candidate) -> tuple:  # -> tuple[float, float, dict]:
         """
         Evaluate ``candidate``, considering the current codetable and a dataset ``D``
 
         Parameters
         ----------
         candidate: frozenset
             a new candidate to be evaluated
@@ -335,29 +384,26 @@
         -------
         (float, float, dict)
             updated (data size, model size, codetable)
         """
         # Get the id (``idx``) of the insertion of ``candidate`` in codetable w.r.t the standard cover order
         idx = self.codetable_.bisect(candidate)
         ct = list(self.codetable_)
-        # Insert the candidate to the CT w.r.t the usage order
-        ct.insert(idx, candidate)
+        ct.insert(idx, candidate)  # Insert the candidate to the CT w.r.t the usage order
         D = {k: v.copy() for k, v in self.standard_codetable_.items()}
         # Get the cover a standard codetable D with CT itemsets
-        # CTc is sorted in Standard Cover Order like D
-        CTc = cover(D, ct)
-
+        CTc = cover(D, ct)  # CTc is sorted in Standard Cover Order like D
         data_size, model_size = self._compute_sizes(CTc)
 
         if self.pruning:
             CTc, data_size, model_size = self._prune(CTc, model_size, data_size)
 
         return data_size, model_size, CTc
 
-    def update(self, candidate=None, model_size=None, data_size=None, usages=None):
+    def update(self, candidate=None, model_size=None, data_size=None, usages=None) -> None:
         """
         Update the current codetable.
 
         If `candidate` is passed as None, `model_size`, `data_size` and `usages` will be used
         If `candidate` is not None, `model_size`, `data_size` and `usages`
         will be computed by calling `.evaluate`
 
@@ -369,16 +415,15 @@
         model_size: float, default=None
             new model size (in bits) to be set
 
         data_size: float
             new data size (in bits) to be set
 
         usages: dict, default=None
-            optional for usage outside this class
-            eg. if one simply needs to include an itemset in the current codetable
+            optional for usage outside this class e.g.if simply needs to include an itemset in the current codetable
             as in interactive data mining
 
         Raises
         ------
         AssertionError
         """
         assert not (candidate is None and usages is None)
@@ -389,21 +434,20 @@
         self.codetable_.update(usages)
         for iset in to_drop:
             del self.codetable_[iset]
 
         self.data_size_ = data_size
         self.model_size_ = model_size
 
-    def cover(self, D):
+    def cover(self, D) -> pd.DataFrame:
         """
         cover unseen data
 
         items never seen are dropped out
 
-
         Examples
         --------
         >>> from skmine.itemsets import SLIM
         >>> D = ["ABC", "AB", "BCD"]
         >>> s = SLIM().fit(D)
         >>> s.cover(["BC", "AB"])
            (A, B)   (B,)   (A,)   (C,)
@@ -416,109 +460,118 @@
         """
         if hasattr(D, "shape") and len(D.shape) == 2:  # tabular
             D = _check_D(D)
             D_sct = {k: Bitmap(np.where(D[k])[0]) for k in D.columns if k in self.standard_codetable_}
         else:  # transactional
             D_sct = _to_vertical(D)
 
-        isets = self.discover(singletons=True, return_tids=False, drop_null_usage=False)
+        isets = self.transform(D, singletons=True, return_tids=False, drop_null_usage=False)
         isets = [tuple(itemset) for itemset in isets[isets["itemset"].map(set(D_sct).issuperset)]["itemset"].to_list()]
         covers = cover(D_sct, isets)
 
         mat = np.zeros(shape=(len(D), len(covers)), dtype=bool)
         for idx, tids in enumerate(covers.values()):
             mat[tids, idx] = True
+
         return pd.DataFrame(mat, columns=list(covers.keys()))
 
-    def discover(self, singletons=True, return_tids=False, lexicographic_order=True, drop_null_usage=True,
-                 return_dl=False, out=None):
+    def transform(self, D, singletons=True, return_tids=False, lexicographic_order=True, drop_null_usage=True,
+                  return_dl=False, out=None):
         """Get a user-friendly copy of the codetable
 
         Parameters
         ----------
+        D: iterable of iterables or array-like
+            Transactional dataset, either as an iterable of iterables or encoded as tabular binary data.
+            Does not influence the results. Present for compatibility with scikit-learn.
+
         singletons: bool, default=True
             Either to include itemsets of length 1 in the result
 
         return_tids: bool, default=False
             Either returns the tids of each itemset associated with the coverage or simply the usage, i.e. the number of
             times the itemset is used, if set to False.
 
         lexicographic_order: bool, default=True
             Either the order of the items in each itemset is not ordered or the items are ordered lexicographically
 
         drop_null_usage: bool, default=True
-            Either to include itemset with no usage in the training data
-            (i.e itemsets under cover of other itemsets)
+            Either to include itemset with no usage in the training data (i.e itemsets under cover of other itemsets)
 
         return_dl: bool, default=False
             Display the total size of the model L(CT, D) according to MDL (Minimum Description Length) which is equal to
             the sum of the encoded database size L(D | CT) and the encoded table code size L(CT | D).
 
         out : str, default=None
             File where results are written. Discover return None. The file contains in parentheses the usage of the
             itemset located after the closing parenthesis. If the 'return_tids' option is enabled then the line under
             each itemset is a line of transaction ids containing the previous itemset.
 
         Example
         -------
         >>> from skmine.itemsets import SLIM
         >>> D = ["ABC", "AB", "BCD"]
-        >>> SLIM().fit(D).discover(singletons=True, return_tids=True, lexicographic_order=True, drop_null_usage=False)
-          itemset    tids
-        0  [A, B]  (0, 1)
-        1  [B, D]     (2)
-        2     [B]      ()
-        3     [A]      ()
-        4     [C]  (0, 2)
-        5     [D]      ()
+        >>> SLIM().fit_transform(D, singletons=True, return_tids=False, lexicographic_order=True, drop_null_usage=True)
+          itemset  usage
+        0  [A, B]      2
+        1  [B, D]      1
+        2     [C]      2
 
         Returns
         -------
-        pd.Series
-            codetable containing patterns and ids of transactions in which they are used
+        pd.Dataframe
+            codetable containing patterns and their usages or ids of transactions in which they are used
         """
+
         check_is_fitted(self, "is_fitted_")
+        self.drop_null_usage_ = drop_null_usage
+        self.singletons_ = singletons
+        self.lexicographic_order_ = lexicographic_order
+        self.return_tids_ = return_tids
+        self.out_ = out
+        self.return_dl_ = return_dl
 
         itemsets = []
         itids = []
         iusages = []
         for iset, tids in self.codetable_.items():
-            if len(tids) >= drop_null_usage and len(iset) > (not singletons):
-                itemsets.append(sorted(iset)) if lexicographic_order else itemsets.append(list(iset))
-                itids.append(tids) if return_tids else []
+            if len(tids) >= self.drop_null_usage_ and len(iset) > (not self.singletons_):
+                itemsets.append(sorted(iset)) if self.lexicographic_order_ else itemsets.append(list(iset))
+                itids.append(tids) if self.return_tids_ else []
                 iusages.append(len(tids))
 
-        if out is not None:
-            with open(out, 'w') as f:
+        if self.out_ is not None:
+            with open(self.out_, 'w') as f:
                 for i, (itemset, usage) in enumerate(zip(itemsets, iusages)):
                     line = "(" + str(usage) + ") " + " ".join(itemset) + "\n"
-                    if return_tids:
+                    if self.return_tids_:
                         line += " ".join(map(str, itids[i])) + "\n"
                     f.write(line)
             return None
         else:
-            df = pd.DataFrame(data={'itemset': itemsets, ('tids' if return_tids else 'usage'): (itids if return_tids
-                                                                                                else iusages)})
-            if return_dl:
+            df = pd.DataFrame(data={'itemset': itemsets,
+                                    ('tids' if self.return_tids_ else 'usage'): (
+                                        itids if self.return_tids_ else iusages)})
+            if self.return_dl_:
                 print("data_size :", self.data_size_)
                 print("model_size :", self.model_size_)
                 print("total_size :", self.data_size_ + self.model_size_)
             return df
 
-    def reconstruct(self):
-        """reconstruct the original data from the current `self.codetable_`. This is possible because SLIM is a
-        lossless algorithm .
+    def reconstruct(self) -> pd.Series:
+        """Reconstruct the original data from the current `self.codetable_`. This is possible because SLIM is a
+        lossless algorithm.
 
         Example
         -------
         >>> from skmine.itemsets import SLIM
         >>> D = ["ABC", "AB", "BCD"]
         >>> slim = SLIM()
-        >>> slim.fit(D).discover()  # doctest: +SKIP
-        >>> slim.reconstruct()  # doctest: +SKIP
+        >>> slim.fit(D) # doctest: +SKIP
+        >>> slim.reconstruct() # doctest: +SKIP
         0    [A, B, C]
         1       [A, B]
         2    [B, C, D]
         dtype: object
 
         Returns
         -------
@@ -543,25 +596,26 @@
 
         Unseen items will throw errors
         """
         a = items[-1]
         tids = self.standard_codetable_[a]
         if len(items) > 1:
             return tids & self.get_support(*items[:-1])
-        return tids
+        else:
+            return tids
 
-    def _standard_cover_order(self, itemset):
+    def _standard_cover_order(self, itemset) -> tuple:
         """
         Returns a tuple associated with an itemset,
         so that many itemsets can be sorted in Standard Cover Order :
         |X|↓ supp_D(X) ↓ lexicographically ↑
         """
         return -len(itemset), -len(self.get_support(*itemset)), tuple(itemset)
 
-    def prefit(self, D, y=None):
+    def prefit(self, D, y=None):  # -> self
         """
         Parameters
         ----------
         D: iterable of iterables or array-like
             Transactional dataset, either as an iterable of iterables
             or encoded as tabular binary data
 
@@ -569,22 +623,23 @@
         ----
         works in 3 steps
 
         1. ingest data `D`
         2. track bitmaps for the top `self.n_items` frequent items from `D`
         3. set `self.data_size_` and `self.model_size` given the standard codetable
         """
-        if hasattr(D, "ndim") and D.ndim == 2:
+        if hasattr(D, "ndim") and D.ndim == 2:  # TODO, refactor in fit method, with sklearn input checking !
             D = _check_D(D)
             if y is not None:
                 D = supervised_to_unsupervised(D, y)  # SKLEARN_COMPAT
             item_to_tids = {k: Bitmap(np.where(D[k])[0]) for k in D.columns}
         else:
             # compute tids for each item in Bitmap
             item_to_tids = _to_vertical(D)
+
         sct = pd.Series(item_to_tids)  # sct for "standard code table"
         # The usage of an itemset X ∈ CT (Code Table) is the number of transactions t ∈ D which have X in their cover.
         # A cover(t) is the set of itemsets X ∈ CT used to encode a transaction t
         usage = sct.map(len).astype(np.uint32)
         usage = usage.nlargest(len(sct))
         # Descending usage sorting
         sct = sct[usage.index]
@@ -643,15 +698,15 @@
         #             +              codes('B') + codes('C')  + codes('D')
         #           = 2codes('A') + 3codes('B') +2codes('C') + 1codes('D')
         #           = usage('A')*codes('A') + usage('B')*codes('B') + ...
         self.data_size_ = (codes * usage).sum()
 
         return self
 
-    def _compute_sizes(self, codetable):
+    def _compute_sizes(self, codetable) -> tuple:  # tuple[float, float]:
         """
         Compute sizes for both the data and the model
 
         .. math:: L(D|CT)
         .. math:: L(CT|D)
 
         Parameters
@@ -660,29 +715,27 @@
             A series mapping itemsets to their usage tids
 
         Returns
         -------
         tuple(float, float)
             (data_size, model_size)
         """
-        isets, usages = zip(
-            *((_[0], len(_[1])) for _ in codetable.items() if len(_[1]) > 0)
-        )
+        isets, usages = zip(*((_[0], len(_[1])) for _ in codetable.items() if len(_[1]) > 0))
         usages = np.array(usages, dtype=np.uint32)
         codes = -_log2(usages / usages.sum())
 
         counts = Counter(chain(*isets))
         stand_codes_sum = sum(self._starting_codes[item] * ctr for item, ctr in counts.items())
 
         model_size = stand_codes_sum + codes.sum()  # L(CTc|D) = L(X|ST) + L(X|CTc)
         data_size = (codes * usages).sum()
 
         return data_size, model_size
 
-    def _prune(self, CTc, model_size, data_size):
+    def _prune(self, CTc, model_size, data_size) -> tuple:  # tuple[dict, float, float]:
         """post prune a codetable considering itemsets for which usage has decreased
 
         Parameters
         ----------
         CTc: SortedDict
         model_size: float
             current model_size for ``codetable``
@@ -721,7 +774,10 @@
                 decreased = {k for k, v in CTp.items() if len(k) > 1 and len(v) < len(CTc[k])}
                 CTc.update(CTp)
                 del CTc[cand]
                 prune_set.update(decreased)
                 data_size, model_size = d_size, m_size
 
         return CTc, data_size, model_size
+
+    def __copy__(self):
+        return SLIM(items=self.items, pruning=self.pruning)
```

### Comparing `scikit-mine-0.0.9/skmine/itemsets/slim_classifier.py` & `scikit-mine-1.0.0/skmine/itemsets/slim_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import numpy as np
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_is_fitted
-from .slim import SLIM
 
-import numpy as np
-from functools import reduce
+from ..itemsets.slim import SLIM
 
 
 class SlimClassifier(BaseEstimator, ClassifierMixin):
     """
     Classifier using the SLIM compression algorithm. Works for binary and multi-class problems.
 
     This classifier uses one SLIM instance per class in the database, resulting in a code table per class.
@@ -36,14 +35,19 @@
         with the class from *classes_*  of the same index
     """
 
     def __init__(self, items=None, pruning=False):
         self.items = items
         self.pruning = pruning
 
+    def _more_tags(self):
+        return {"non_deterministic": True,
+                "no_validation": True,
+                "preserves_dtype": []}
+
     def fit(self, X, y):
         """Fit the model according to the given training data.
 
         Parameters
         ----------
         X: iterable, {array_like}
             containing n_transactions containing themselves n_items
@@ -52,14 +56,16 @@
             Target vector relative to X.
 
         Returns
         -------
         self : object
             An instance of the estimator
         """
+        self._validate_data(X, y, reset=True, validate_separately=False, force_all_finite=False,
+                            accept_sparse=False, ensure_2d=False, ensure_min_samples=0, dtype=list)
         self.classes_ = np.unique(y)
         self.classes_X_ = []
         self.models_ = []
 
         for c in self.classes_:
             transactions_classes = [transaction for transaction, target in zip(X, y) if target == c]
             self.classes_X_.append(transactions_classes)
@@ -79,23 +85,13 @@
 
         Returns
         -------
         y_pred : np.array of shape (n_samples,)
             Class labels for samples in X
         """
         check_is_fitted(self, "classes_")
+        self.models_scores = np.vstack([model.decision_function(X).values for model in self.models_]).T
 
-        if self.classes_ is None:
-            raise ValueError("fit must be called first.")
-
-        models_scores = {i: model.decision_function(X).values for i, model in enumerate(self.models_)}
-        predictions = []
-
-        for i in range(len(X)):
-            scores = [model[i] for model in models_scores.values()]
-            best_index = scores.index(reduce(lambda x, y: x if abs(y) > abs(x) else y, scores))
-            predictions.append(self.classes_[0] if best_index is None else self.classes_[best_index])
-
-        return np.array(predictions)
+        return self.classes_[self.models_scores.argmax(axis=1)]
 
     def __copy__(self):
-        return SlimClassifier(items=self.items, pruning=self.pruning)
+        return SlimClassifier(items=self.items, pruning=self.pruning)
```

### Comparing `scikit-mine-0.0.9/skmine/preprocessing/mdlp_discretizer.py` & `scikit-mine-1.0.0/skmine/preprocessing/mdlp_discretizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,23 @@
     generate_candidates = generate_cut_point
 
     def evaluate(self, y, start, end, cut_point):
         """
         Evaluate vector y of size ``end`` - ``start``,
         given a ``cutpoint``
         """
+
         entropy1, k1 = get_entropy_nb_ones(y[start:cut_point])
         entropy2, k2 = get_entropy_nb_ones(y[cut_point:end])
         whole_entropy, k0 = get_entropy_nb_ones(y[start:end])
 
         N = end - start
 
         part1 = 1 / N * ((cut_point - start) * entropy1 + (end - cut_point) * entropy2)
-        delta = np.log2(pow(3, k0) - 2) - (
-            k0 * whole_entropy - k1 * entropy1 - k2 * entropy2
-        )
+        delta = np.log2(pow(3, k0) - 2) - (k0 * whole_entropy - k1 * entropy1 - k2 * entropy2)
 
         gain = whole_entropy - part1
 
         return gain > 1 / N * (np.log2(N - 1) + delta)
 
     def fit(self, X, y):
         """
@@ -177,32 +176,34 @@
     >>> disc.fit(X, y)                          # doctest: +SKIP
     >>> disc.cut_points_                        # doctest: +SKIP
     {0: array([5.5, 6.2]), 1: array([2.9, 3.3]), 2: array([2.45, 4.9 ]), 3: array([0.8, 1.7])}
 
     """
 
     def __init__(self, random_state=None, n_jobs=1):
-        self.cut_points_ = dict()
         self.random_state = random_state
         self.n_jobs = n_jobs
-        self.discretizers_ = []
 
     def fit(self, X, y):
         """fit the MLDP discretizer on an input matrix ``X``, given a label vector ``y``.
 
         Parameters
         ----------
         X: np.ndarray or pd.DataFrame of shape (n_samples, n_features)
             The input matrix containing features. A set of cut points
             will be affected to each feature
 
         y : np.ndarray of pd.Series of shape(n_samples,)
             The label vector used to discretize ``X``
         """
+        self.cut_points_ = dict()
+        self.discretizers_ = []
+
         assert y is not None and np.issubdtype(y.dtype, np.integer)
+
         random_state = _check_random_state(self.random_state)
         permutation = random_state.permutation(len(X))
         _X = X.values if isinstance(X, pd.DataFrame) else X
         _y = y.values if isinstance(y, pd.Series) else y
         _X = _X[permutation]
         _y = _y[permutation]
 
@@ -216,25 +217,31 @@
         cut_points = [d.cut_points_ for d in discs]
 
         if isinstance(X, pd.DataFrame):
             self.cut_points_ = dict(zip(X.columns, cut_points))
         else:
             self.cut_points_ = dict(enumerate(cut_points))
 
+        # self.is_fitted_ = True
+
         return self
 
     def discover(self):
+        # check_is_fitted(self, "is_fitted_")
+
         """user-friendly view on cut points"""
         return pd.Series(self.cut_points_, dtype=object)
 
     def transform(self, X, y=None):  # pylint: disable=unused-argument
         """Discretizes the input matrix X
 
         This applies the cutpoints their respective columns
         """
+        # check_is_fitted(self, "is_fitted_")
+
         if isinstance(X, pd.DataFrame) and not set(self.cut_points_) == set(X.columns):
             raise ValueError(f"X columns should be {self.cut_points_.keys()}")
         _X = X.values if isinstance(X, pd.DataFrame) else X
 
         vects = Parallel(n_jobs=self.n_jobs, prefer="threads")(
             delayed(np.searchsorted)(cut_points, _X[:, idx])
             for idx, cut_points in enumerate(self.cut_points_.values())
```

### Comparing `scikit-mine-0.0.9/skmine/utils.py` & `scikit-mine-1.0.0/skmine/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 """
-utils functions
+Utils functions
 """
 
 import numbers
-from itertools import count
 
 import numpy as np
 import pandas as pd
 import scipy.sparse
 from numpy.core.numeric import normalize_axis_tuple
 from numpy.core.overrides import array_function_dispatch
 from numpy.lib.stride_tricks import as_strided
 from sortedcontainers import SortedList
 
 
-def _check_random_state(seed):
+def _check_random_state(seed) -> None:
     if seed is None or seed is np.random:
         return np.random.mtrand._rand
     if isinstance(seed, numbers.Integral):
         return np.random.RandomState(seed)
     if isinstance(seed, np.random.RandomState):
         return seed
-    raise ValueError(
-        f"{seed} cannot be used to seed a numpy.random.RandomState instance"
-    )
+    raise ValueError(f"{seed} cannot be used to seed a numpy.random.RandomState instance")
 
 
-def _check_min_supp(min_supp, accept_absolute=True):
+def _check_min_supp(min_supp, accept_absolute=True) -> None:
     if isinstance(min_supp, int):
         if not accept_absolute:
-            raise ValueError(
-                "Absolute support is prohibited, please provide a float value between 0 and 1"
-            )
+            raise ValueError("Absolute support is prohibited, please provide a float value between 0 and 1")
         if min_supp < 1:
             raise ValueError("Minimum support must be strictly positive")
     elif isinstance(min_supp, float):
         if min_supp < 0 or min_supp > 1:
             raise ValueError("Minimum support must be between 0 and 1")
     else:
         raise TypeError("Mimimum support must be of type int or float")
-    return min_supp
 
 
 def _check_growth_rate(gr):
     if not gr > 1:
         raise ValueError("growth ratio should be greater than 1")
-    return gr
+    else:
+        return gr
 
 
 def filter_maximal(itemsets):
     """filter maximal itemsets from a set of itemsets
 
     Parameters
     ----------
@@ -145,23 +140,25 @@
         raise TypeError("y should be an instance of np.ndarray or pd.Series")
 
     # TODO : pd.Categorical
     return y
 
 
 def _check_D_y(D, y=None):
+
     D = _check_D(D)
     if y is not None:
         y = _check_y(y)
+
     return D, y
 
 
 def intersect2d(ar1, ar2, return_indices=True):
     """
-    Find the intersection of two 2 dimnesional arrays
+    Find the intersection of two 2 dimensional arrays
 
     Return the sorted, unique rows that are both of the input arrays
 
     Parameters
     ----------
     x, y: array_like
         Input arrays
@@ -171,35 +168,35 @@
         Default is False
 
     Returns
     -------
     intersect2d: ndarray
         Sorted 2D array of common and unique rows
     comm1: ndarray
-        The indices of the first occurences of the common rows in `ar1`.
+        The indices of the first occurrences of the common rows in `ar1`.
         Only provided if `return_indices` is True
     comm2: ndarray
-        The indices of the first occurences of the common rows in `ar2`.
+        The indices of the first occurrences of the common rows in `ar2`.
         Only provided if `return_indices` is True
     """
     ar1, ar2 = np.asanyarray(ar1), np.asanyarray(ar2)
     assert ar1.ndim == ar2.ndim == 2
     _, x_ind, y_ind = np.intersect1d(ar1[:, 0], ar2[:, 0], return_indices=True)
     x, y = ar1[x_ind], ar2[y_ind]
     xy_where = np.argwhere((x == y).all(axis=1)).reshape(-1)
     x_ind = x_ind[xy_where]
+
     if return_indices:
         y_ind = y_ind[xy_where]
         return ar1[x_ind], x_ind, y_ind
-    return ar1[x_ind]
+    else:
+        return ar1[x_ind]
 
 
-def _sliding_window_view_dispatcher(
-    x, window_shape, axis=None, *, subok=None, writeable=None
-):
+def _sliding_window_view_dispatcher(x, window_shape, axis=None, *, subok=None, writeable=None):
     return (x,)
 
 
 @array_function_dispatch(_sliding_window_view_dispatcher)
 def sliding_window_view(x, window_shape, axis=None, *, subok=False, writeable=False):
     """
     COPIED from https://github.com/numpy/numpy/blob/v1.20.0/numpy/lib/stride_tricks.py#L122-L336
@@ -287,67 +284,57 @@
     window_shape_array = np.array(window_shape)
     if np.any(window_shape_array < 0):
         raise ValueError("`window_shape` cannot contain negative values")
 
     if axis is None:
         axis = tuple(range(x.ndim))
         if len(window_shape) != len(axis):
-            raise ValueError(
-                f"Since axis is `None`, must provide "
-                f"window_shape for all dimensions of `x`; "
-                f"got {len(window_shape)} window_shape elements "
-                f"and `x.ndim` is {x.ndim}."
-            )
+            raise ValueError(f"Since axis is `None`, must provide window_shape for all dimensions of `x`; "
+                             f"got {len(window_shape)} window_shape elements and `x.ndim` is {x.ndim}.")
     else:
         axis = normalize_axis_tuple(axis, x.ndim, allow_duplicate=True)
         if len(window_shape) != len(axis):
-            raise ValueError(
-                f"Must provide matching length window_shape and "
-                f"axis; got {len(window_shape)} window_shape "
-                f"elements and {len(axis)} axes elements."
-            )
+            raise ValueError(f"Must provide matching length window_shape and "
+                             f"axis; got {len(window_shape)} window_shape elements and {len(axis)} axes elements.")
 
     out_strides = x.strides + tuple(x.strides[ax] for ax in axis)
 
     # note: same axis can be windowed repeatedly
     x_shape_trimmed = list(x.shape)
     for ax, dim in zip(axis, window_shape):
         if x_shape_trimmed[ax] < dim:
             raise ValueError("window shape cannot be larger than input array shape")
         x_shape_trimmed[ax] -= dim - 1
     out_shape = tuple(x_shape_trimmed) + window_shape
-    return as_strided(
-        x, strides=out_strides, shape=out_shape, subok=subok, writeable=writeable
-    )
+    return as_strided(x, strides=out_strides, shape=out_shape, subok=subok, writeable=writeable)
 
 
 def bron_kerbosch(candidates: dict, clique=None, excluded=None, depth=0):
     """
     Bron-Kerbosch algorithm, from https://en.wikipedia.org/wiki/Bron%E2%80%93Kerbosch_algorithm
 
     Parameters
     ----------
     candidates: dict[object, list[object]]
         a mapping from each node to its existing neighbours
     """
     if not candidates and not excluded and clique is not None and len(clique) > 2:
         yield [_ for _ in clique]
-        return
+        return None
 
     # pass None as default arg instead of dict()
     # fix collisions in pytest, really obscure
     clique = clique or dict()
     excluded = excluded or dict()
 
     if depth > 20:
-        return
+        return None
 
     for node, neighbours in list(candidates.items()):
         new_clique = {**{node: neighbours}, **clique}
         new_candidates = {k: v for k, v in candidates.items() if k in neighbours}
         new_excluded = {k: v for k, v in excluded.items() if k in neighbours}
 
         yield from bron_kerbosch(new_candidates, new_clique, new_excluded)
 
         del candidates[node]
         excluded[node] = neighbours
-
```

