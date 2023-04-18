# Comparing `tmp/tuned-lens-0.0.3.tar.gz` & `tmp/tuned-lens-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuned-lens-0.0.3.tar", last modified: Wed Mar 15 00:56:02 2023, max compression
+gzip compressed data, was "tuned-lens-0.0.4.tar", last modified: Tue Apr 18 03:12:02 2023, max compression
```

## Comparing `tuned-lens-0.0.3.tar` & `tuned-lens-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.923587 tuned-lens-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-15 00:56:02.923587 tuned-lens-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 00:56:02.923587 tuned-lens-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.915587 tuned-lens-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_load_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tests/test_subspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.919587 tuned-lens-0.0.3/tuned_lens/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.919587 tuned-lens-0.0.3/tuned_lens/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/causal/ablation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/causal/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/causal/subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/causal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/model_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.919587 tuned-lens-0.0.3/tuned_lens/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/_model_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/downstream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/nn/probe_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.919587 tuned-lens-0.0.3/tuned_lens/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/plotting/interventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/plotting/plot_lens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/residual_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.923587 tuned-lens-0.0.3/tuned_lens/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/argparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/cbe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/downstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/eval_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/scripts/train_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.923587 tuned-lens-0.0.3/tuned_lens/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/logit_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/stats/residual_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-15 00:55:53.000000 tuned-lens-0.0.3/tuned_lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:56:02.919587 tuned-lens-0.0.3/tuned_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-15 00:56:02.000000 tuned-lens-0.0.3/tuned_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_load_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_subspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tuned_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/ablation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/model_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/_model_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/downstream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/lenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/plotting/plot_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/residual_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/argparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/cbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/eval_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/train_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/logit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/residual_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tuned_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/top_level.txt
```

### Comparing `tuned-lens-0.0.3/LICENSE` & `tuned-lens-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/PKG-INFO` & `tuned-lens-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,68 @@
-Metadata-Version: 2.1
-Name: tuned-lens
-Version: 0.0.3
-Summary: Tools for understanding how transformer predictions are built layer-by-layer
-License: MIT License
-Keywords: nlp,interpretability,language-models,explainable-ai
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: notebooks
-License-File: LICENSE
-
 # Tuned Lens 🔎
-Tools for understanding how transformer predictions are built layer-by-layer
+<a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+<a target="_blank" href="https://huggingface.co/spaces/AlignmentResearch/tuned-lens">
+<img src="https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-sm-dark.svg", alt="Open in Spaces">
+</a>
 
-![Using the Tuned-lens](https://user-images.githubusercontent.com/12176390/224879115-8bc95f26-68e4-4f43-9b4c-06ca5934a29d.png)
 
-This package provides a simple interface training and evaluating __tuned lenses__. A tuned lens allows us to peak at the iterative computations that a transformer is using the compute the next token.
+Tools for understanding how transformer predictions are built layer-by-layer.
 
-A lens into a transformer with n layers allows you to replace the last $m$ layers of the model with an [affine transformation](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html) (we call these affine translators).
+<img src=https://user-images.githubusercontent.com/12176390/224879115-8bc95f26-68e4-4f43-9b4c-06ca5934a29d.png>
 
-This skips over these last few layers and lets you see the best prediction that can be made from the model's intermediate representations, i.e. the residual stream, at layer $n - m$. Since the representations may be rotated, shifted, or stretched from layer to layer it's useful to train an affine specifically on each layer. This training is what differentiates this method from simpler approaches that decode the residual stream of the network directly using the unembeding layer i.e. the [logit lens](https://www.lesswrong.com/posts/AcKRB8wDpdaN6v6ru/interpreting-gpt-the-logit-lens). We explain this process and its applications in a forthcoming paper "Eliciting Latent Predictions from Transformers with the Tuned Lens".
+This package provides a simple interface for training and evaluating __tuned lenses__. A tuned lens allows us to peek at the iterative computations a transformer uses to compute the next token.
 
-### Acknowledgments
-Originally concieved by [Igor Ostrovsky](https://twitter.com/igoro?lang=en) and [Stella Biderman](www.stellabiderman) at [EleutherAI](www.eleuther.ai), this library was built as a collaboration between FAR and EleutherAI researchers.
 
-> **Warning**
-> This package has not reached 1.0 yet. Expect the public interface to change regularly and without a major version bump.
-
-## Install instructions
-### Installing From Source
-First you will need to install the basic prerequisites into a virtual environment
-* Python 3.9+
-* Pytorch 1.12.0+
+## What is a Lens?
+<img alt="A diagram showing how a translator within the lens allows you to skip intermediate layers." src="https://user-images.githubusercontent.com/12176390/227057947-1ef56811-f91f-48ff-8d2d-ff04cc599125.png"  width=400/>
 
-then you can simply install the package using pip.
-```
-git clone https://github.com/AlignmentResearch/tuned-lens
-cd tuned-lens
-pip install .
-```
+A lens into a transformer with _n_ layers allows you to replace the last _m_ layers of the model with an [affine transformation](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html) (we call these affine translators). Each affine translator is trained to minimize the KL divergence between its prediction and the final output distribution of the original model. This means that after training, the tuned lens allows you to skip over these last few layers and see the best prediction that can be made from the model's intermediate representations, i.e., the residual stream, at layer _n - m_.
 
-### Install Using Docker
-If you prefer to run the code from within a container you can use the provided docker
-file
-```
-git clone https://github.com/AlignmentResearch/tuned-lens
-cd tuned-lens
-docker build -t tuned-lens-prod --target prod .
-```
+The reason we need to train an affine translator is that the representations may be rotated, shifted, or stretched from layer to layer. This training differentiates this method from simpler approaches that unembed the residual stream of the network directly using the unembedding matrix, i.e., the [logit lens](https://www.lesswrong.com/posts/AcKRB8wDpdaN6v6ru/interpreting-gpt-the-logit-lens). We explain this process and its applications in the paper [Eliciting Latent Predictions from Transformers with the Tuned Lens](https://arxiv.org/abs/2303.08112).
 
-## Quick Start Guid
-### Downloading the datasets
-```
-wget https://the-eye.eu/public/AI/pile/val.jsonl.zst
-unzstd val.jsonl.zst
+### Acknowledgments
+Originally conceived by [Igor Ostrovsky](https://twitter.com/igoro) and [Stella Biderman](https://www.stellabiderman.com/) at [EleutherAI](https://www.eleuther.ai/), this library was built as a collaboration between FAR and EleutherAI researchers.
 
-wget https://the-eye.eu/public/AI/pile/test.jsonl.zst
-unzstd test.jsonl.zst
-```
+## Install Instructions
+### Installing from PyPI
+First, you will need to install the basic prerequisites into a virtual environment:
+* Python 3.9+
+* PyTorch 1.13.0+
 
-### Evaluating a Lens
-Once you have a lens file either by training it yourself of by downloading it. You
-can run various evaluations on it using the provided evaluation command.
+Then, you can simply install the package using pip.
 ```
-tuned-lens eval gpt2 test.jsonl --lens gpt-2-lens
-    --dataset the_pile all \
-    --split validation \
-    --output lens_eval_results.json
+pip install tuned-lens
 ```
 
+### Installing the container
+If you prefer to run the training scripts from within a container, you can use the provided Docker container.
 
-### Training a Lens
-This will train a tuned lens on gpt-2 with the default hyper parameters.
-
-```bash
-tuned-lens train gpt2 val.jsonl
-    --dataset the_pile all \
-    --split validation \
-    --output gpt-2-lens
 ```
-
-> **Note**
-> This will download the entire validation set of the pile which is over 30 GBs. If you
-> are doing this within a docker file it's recommended to mount external storage to huggingface's
-> cache directory.
+docker pull ghcr.io/alignmentresearch/tuned-lens:latest
+docker run --rm tuned-lens:latest tuned-lens --help
+```
 
 ## Contributing
-Make sure to install the dev dependencies and install the pre-commit hooks
+Make sure to install the dev dependencies and install the pre-commit hooks.
 ```
+$ git clone https://github.com/AlignmentResearch/tuned-lens.git
 $ pip install -e ".[dev]"
 $ pre-commit install
 ```
 
+## Citation
 
-## Citation Information
-
-If you find this library useful, please cite it as
+If you find this library useful, please cite it as:
 
 ```bibtex
 @article{belrose2023eliciting,
   title={Eliciting Latent Predictions from Transformers with the Tuned Lens},
   authors={Belrose, Nora and Furman, Zach and Smith, Logan and Halawi, Danny and McKinney, Lev and Ostrovsky, Igor and Biderman, Stella and Steinhardt, Jacob},
   journal={to appear},
   year={2023}
 }
 ```
+
+> **Warning**
+> This package has not reached 1.0. Expect the public interface to change regularly and without a major version bumps.
```

### Comparing `tuned-lens-0.0.3/pyproject.toml` & `tuned-lens-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -11,30 +11,37 @@
 license = {text = "MIT License"}
 dependencies = [
     "accelerate",
     "datasets",
     "plotly>=5.13.1",
     "scikit-learn",
     "zstandard",
-    # Needed for Fully Sharded Data Parallel
-    "torch>=1.12.0",
+    "torch>=1.13.0",
     "transformers",
     "huggingface_hub>=0.12.1",
 ]
-version = "0.0.3"
+version = "0.0.4"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "bump2version",
     "pytest-skip-slow",
     "pytest",
 ]
+docs = [
+    "furo",
+    "myst-parser",
+    "sphinx",
+    "sphinx-autodoc-typehints",
+    "sphinx-rtd-theme",
+]
 test = [
     "pytest-skip-slow",
+    "pytest-cov",
     "pytest",
     "mock",
 ]
 notebooks = [
     "ipywidgets",
 ]
 
@@ -45,15 +52,15 @@
 namespaces = false
 
 [tool.pytest.ini_options]
 addini = "slow : mark tests as slow these will be skipped by default"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
+select = ["E", "F", "D"]
 ignore = []
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
@@ -89,9 +96,17 @@
 # Assume Python 3.10.
 target-version = "py310"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"docs/**.py" = ["D"]
+"tests/**.py" = ["D"]
+"tuned_lens/stats/**.py" = ["D"]
+"tuned_lens/causal/**.py" = ["D"]
+"tuned_lens/nn/probe_dict.py" = ["D"]
```

### Comparing `tuned-lens-0.0.3/tests/test_decoder.py` & `tuned-lens-0.0.4/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_distance.py` & `tuned-lens-0.0.4/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_feature_extraction.py` & `tuned-lens-0.0.4/tests/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_lenses.py` & `tuned-lens-0.0.4/tests/test_lenses.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_plotting.py` & `tuned-lens-0.0.4/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_stats.py` & `tuned-lens-0.0.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tests/test_subspaces.py` & `tuned-lens-0.0.4/tests/test_subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/__main__.py` & `tuned-lens-0.0.4/tuned_lens/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Script to train or evaluate a set of tuned lenses for a language model."""
+
 from .scripts.lens import main as lens_main
 from argparse import ArgumentParser
 from contextlib import nullcontext, redirect_stdout
 from pathlib import Path
 import os
 import torch.distributed as dist
 
 
 def run():
+    """Run the script."""
     parser = ArgumentParser(
         description="Train or evaluate a set of tuned lenses for a language model.",
     )
     # Arguments shared by train and eval; see https://stackoverflow.com/a/56595689.
     parent_parser = ArgumentParser(add_help=False)
     parent_parser.add_argument(
         "model_name", type=str, help="Name of model to use in the Huggingface Hub."
@@ -20,14 +23,19 @@
         type=str,
         default=("the_pile", "all"),
         nargs="*",
         help="Name of dataset to use. Can either be a local .jsonl file or a name "
         "suitable to be passed to the HuggingFace load_dataset function.",
     )
     parent_parser.add_argument(
+        "--cpu-offload",
+        action="store_true",
+        help="Use CPU offloading. Must be combined with --fsdp.",
+    )
+    parent_parser.add_argument(
         "--fsdp",
         action="store_true",
         help="Run the model with Fully Sharded Data Parallelism.",
     )
     parent_parser.add_argument(
         "--loss",
         type=str,
@@ -86,14 +94,19 @@
     parent_parser.add_argument(
         "--tokenizer",
         type=str,
         help="Name of pretrained tokenizer to use from the Huggingface Hub. If None, "
         'will use AutoTokenizer.from_pretrained("<model name>").',
     )
     parent_parser.add_argument(
+        "--tokenizer-type",
+        type=str,
+        help="Name of tokenizer class to use. If None, will use AutoTokenizer.",
+    )
+    parent_parser.add_argument(
         "--token-shift",
         type=int,
         default=None,
         help="How to shift the labels wrt the input tokens (1 = next token, "
         "0 = current token, -1 = previous token, etc.)",
     )
```

### Comparing `tuned-lens-0.0.3/tuned_lens/causal/subspaces.py` & `tuned-lens-0.0.4/tuned_lens/causal/subspaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Provides tools for extracting causal bases from models and ablating subspaces"""
 from ..model_surgery import get_transformer_layers
 from ..nn import Decoder, TunedLens
 from ..utils import maybe_all_reduce
 from .utils import derange
 from contextlib import contextmanager
 from tqdm.auto import trange
 from typing import Iterable, Literal, NamedTuple, Optional, Union, Sequence
@@ -14,14 +15,23 @@
 def ablate_subspace(
     model: th.nn.Module,
     A: th.Tensor,
     layer_index: int,
     mode: Literal["mean", "resample", "zero"] = "zero",
     orthonormal: bool = False,
 ):
+    """Context manager that ablates a subspace of activations.
+
+    Args:
+        model: A hugging face transformer model.
+        A: Either a 2D matrix whose column space is to be removed, or a 1D vector whose
+            span is to be removed.
+        layer_index: The index of the layer to ablate.
+        orthonormal: if True, `A` is assumed to be orthonormal.
+    """
     _, layers = get_transformer_layers(model)
 
     def wrapper(_, __, outputs):
         h, *extras = outputs
         h_ = remove_subspace(h, A, mode, orthonormal)
 
         return h_, *extras
@@ -152,15 +162,15 @@
                 max_iter=max_iter,
             )
 
             def closure():
                 nonlocal energy_delta, nfev, last_energy
                 nfev += 1
 
-                opt.zero_grad()
+                opt.zero_grad(set_to_none=False)
                 v_ = project(v)
                 h_ = remove_subspace(hiddens[i], v_, mode=mode, orthonormal=True)
 
                 if isinstance(model, Decoder):
                     logits = model(h_)
                 elif isinstance(model, TunedLens):
                     logits = model(h_, i)
@@ -186,15 +196,15 @@
 
                 if pbar:
                     pbar.set_postfix(energy=last_energy.item())
 
                 if not loss.isfinite():
                     print("Loss is not finite")
                     loss = th.tensor(0.0, device=device)
-                    opt.zero_grad()
+                    opt.zero_grad(set_to_none=False)
 
                 return loss
 
             while nfev < max_iter:
                 opt.step(closure)  # type: ignore
                 v.data = project(v.data)
```

### Comparing `tuned-lens-0.0.3/tuned_lens/causal/utils.py` & `tuned-lens-0.0.4/tuned_lens/causal/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/data.py` & `tuned-lens-0.0.4/tuned_lens/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Tools for tokenizing and manipulating text datasets."""
 from datasets import Dataset, DatasetDict
 from functools import partial
 from multiprocessing import cpu_count
 from transformers import PreTrainedTokenizerBase
 from typing import TypeVar, Union
 import logging
 import math
```

### Comparing `tuned-lens-0.0.3/tuned_lens/load_artifacts.py` & `tuned-lens-0.0.4/tuned_lens/load_artifacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Load lens artifacts from the hub or locally storage."""
 from typing import Optional, Tuple
 from pathlib import Path
 import os
 
 from huggingface_hub import hf_hub_download
 
 
@@ -10,24 +11,26 @@
     repo_id: Optional[str] = None,
     repo_type: Optional[str] = None,
     revision: Optional[str] = None,
     config_file: str = "config.json",
     ckpt_file: str = "params.pt",
     subfolder: str = "lens",
 ) -> Tuple[Path, Path]:
-    """First checks for lens resource locally then tries to download it from the hub
+    """First checks for lens resource locally then tries to download it from the hub.
 
     Args:
         resource_id: The id of the lens resource.
         repo_id: The repository to download the lens from. Defaults to
             'AlignmentResearch/tuned-lens'. However, this default can be overridden by
             setting the TUNED_LENS_REPO_ID environment variable.
         repo_type: The type of repository to download the lens from. Defaults to
             'space'. However, this default can be overridden by setting the
             TUNED_LENS_REPO_TYPE environment variable.
+        config_file: The name of the config file in the folder contain the lens.
+        ckpt_file: The name of the checkpoint file in the folder contain the lens.
         revision: The revision of the lens to download.
         subfolder: The subfolder of the repository to download the lens from.
 
     Returns:
         * The path to the config.json file
         * The path to the params.pt file
```

### Comparing `tuned-lens-0.0.3/tuned_lens/model_surgery.py` & `tuned-lens-0.0.4/tuned_lens/model_surgery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+"""Tools for finding and modifying components in a transformer model."""
+
 from contextlib import contextmanager
 from transformers import PreTrainedModel
 from typing import Any, Generator, Optional, Type, TypeVar, Union
 import torch as th
 
 
 def get_value_for_key(obj: Any, key: str) -> Any:
     """Get a value using `__getitem__` if `key` is numeric and `getattr` otherwise."""
     return obj[int(key)] if key.isdigit() else getattr(obj, key)
 
 
 def set_value_for_key_(obj: Any, key: str, value: Any) -> None:
-    """
-    Set value in-place using `__getitem__` if `key` is numeric and `getattr` otherwise.
-    """
+    """Set value in-place if `key` is numeric and `getattr` otherwise."""
     if key.isdigit():
         obj[int(key)] = value
     else:
         setattr(obj, key, value)
 
 
 def get_key_path(model: th.nn.Module, key_path: str) -> Any:
```

### Comparing `tuned-lens-0.0.3/tuned_lens/nn/_model_specific.py` & `tuned-lens-0.0.4/tuned_lens/nn/_model_specific.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/nn/decoder.py` & `tuned-lens-0.0.4/tuned_lens/nn/decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,66 @@
+"""Provides a class for mapping transformer hidden states to logits (and vice versa)."""
 from dataclasses import dataclass
 from torch.autograd.functional import hessian
 from torch.distributions import Distribution
 from transformers import PreTrainedModel
 from typing import cast, Callable, Literal, Optional
 from tuned_lens.model_surgery import get_final_layer_norm, get_transformer_layers
 from tuned_lens.stats import kl_divergence
 from tuned_lens.utils import maybe_unpack
 import torch as th
 
 
 @dataclass
 class InversionOutput:
-    """Output of `Decoder.invert`"""
+    """Output of `Decoder.invert`."""
 
     preimage: th.Tensor
     grad_norm: th.Tensor
     kl: th.Tensor
     loss: th.Tensor
     nfev: int
 
     hessian: Optional[th.Tensor]
 
 
 class Decoder(th.nn.Module):
     """Module that maps transformer hidden states to logits (and vice versa).
 
-    This class can be instantiated in two ways:
-    1. From a HuggingFace model, in which case it will extract the unembedding
-        matrix and layer norm from the model.
-    2. From scratch, in which case it will initialize the unembedding matrix
-        and layer norm with the provided `d_model` and `vocab_size` args.
-    The second option mainly exists for compatibility with PyTorch state dicts.
+    This class can be instantiated in two ways: (1) From a HuggingFace model, in which
+    case it will extract the unembedding matrix and layer norm from the model; (2) From
+    scratch, in which case it will initialize the unembedding matrix and layer norm
+    with the provided `d_model` and `vocab_size` args. The second option mainly exists
+    for compatibility with PyTorch state dicts.
     """
 
     def __init__(
         self,
         model: Optional[PreTrainedModel] = None,
         num_transformer_layers: int = 0,
         *,
         # Automatically set when model is provided
         d_model: Optional[int] = None,
         vocab_size: Optional[int] = None,
         # Overridden by model if provided
         norm_eps: float = 1e-5,
     ):
+        """Initialize the decoder.
+
+        Args:
+            model: A HuggingFace model from which to extract the unembedding matrix.
+            num_transformer_layers: To leave at the end of the transformer.
+
+        Automatically set if the model is provided.
+
+        KWArgs:
+            d_model: The dimensionality of the hidden states.
+            vocab_size: The size of the vocabulary.
+            norm_eps: The epsilon value for the layer norm.
+        """
         super().__init__()
 
         self.num_transformer_layers = num_transformer_layers
         self.transformer_layers = th.nn.ModuleList()
 
         # Initializing from scratch without a model
         if not model:
@@ -179,16 +192,23 @@
         Args:
             logits: Tensor of shape `[..., vocab_size]` containing logits to invert.
             compute_hessian: Whether to compute and return the Hessian of the inversion
                 objective at the solution.
             h0: Initial guess for the hidden state. If `None`, the least-squares
                 solution of the linear equation xU = logits is used, where U is the
                 unembedding matrix.
+            max_iter: Maximum number of iterations for the optimizer to take.
             optimizer: Optimization algorithm to use. Currently, only "lbfgs" and "sgd"
                 are supported.
+            prior_weight: The weight of the prior distribution is given in the loss.
+            prior: Prior distribution over hidden states used to regularize
+                the inversion.
+            step_size: The step size for the optimizer.
+            tol: Tolerance for the inversion objective.
+            transform: Callable = lambda x: x,
             weight: Optional tensor of shape `[..., vocab_size]` containing weights
                 for each vocabulary item. If `None`, all classes are weighted equally.
         """
         d_model = cast(int, self.unembedding.in_features)
         leading_dims = logits.shape[:-1]
 
         if h0 is None:
@@ -238,15 +258,15 @@
         nfev = 0  # Number of function evals, like in scipy.optimize.minimize
         loss, kl = log_p.new_tensor(th.inf), log_p.new_tensor(th.inf)
 
         def closure():
             nonlocal nfev, loss, kl
             nfev += 1
 
-            opt.zero_grad()
+            opt.zero_grad(set_to_none=False)
             loss, kl = compute_loss(h_star)
 
             if not loss.isfinite():
                 raise RuntimeError("Inversion objective is not finite.")
 
             loss.backward()
             return loss
```

### Comparing `tuned-lens-0.0.3/tuned_lens/nn/downstream_wrapper.py` & `tuned-lens-0.0.4/tuned_lens/nn/downstream_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Provides a wrapper for implementing downstream evaluation with a tuned lens."""
 from .lenses import TunedLens
 from ..utils import pytree_map
 from transformers import PreTrainedModel, PreTrainedTokenizerBase
 from typing import Iterable, NamedTuple, Optional
 import torch as th
 import torch.distributed as dist
 
@@ -19,32 +20,36 @@
 
     def __init__(
         self,
         model: PreTrainedModel,
         tokenizer: PreTrainedTokenizerBase,
         tuned_lens: Optional[TunedLens] = None,
     ):
+        """Construct a new DownstreamWrapper."""
         super().__init__()
 
         local_rank = dist.get_rank() if dist.is_initialized() else 0
         self.device = th.device(local_rank)
         self.model = model
         self.tokenizer = tokenizer
         self.tuned_lens = tuned_lens
         if self.tuned_lens:
             self.tuned_lens.eval()
 
     @property
-    def max_length(self):
+    def max_length(self) -> int:
+        """Maximum length the context window."""
         return getattr(self.model.config, "max_position_embeddings", 2048)
 
-    def tok_encode(self, string: str):
+    def tok_encode(self, string: str) -> list[int]:
+        """Encode a string into a list of token IDs."""
         return self.tokenizer.encode(string, add_special_tokens=False)
 
     def forward(self, request, prompt: str) -> DownstreamResult:
+        """Process command line request and return a DownstreamResult."""
         _, target_raw = request.args
 
         # sanity check
         assert len(prompt) > 0
         assert len(target_raw) > 0
         assert len(target_raw) <= self.max_length
```

### Comparing `tuned-lens-0.0.3/tuned_lens/nn/lenses.py` & `tuned-lens-0.0.4/tuned_lens/nn/lenses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Provides lenses for decoding hidden states into logits."""
 from copy import deepcopy
 import inspect
 from logging import warn
 from pathlib import Path
 import json
 import abc
 
@@ -14,15 +15,15 @@
 
 
 class Lens(abc.ABC, th.nn.Module):
     """Abstract base class for all Lens."""
 
     @abc.abstractmethod
     def forward(self, h: th.Tensor, idx: int) -> th.Tensor:
-        """Decode hidden states into logits"""
+        """Decode hidden states into logits."""
 
 
 class LogitLens(Lens):
     """Decodes the residual stream into logits using the unembeding matrix."""
 
     layer_norm: th.nn.LayerNorm
     unembedding: th.nn.Linear
@@ -196,14 +197,15 @@
                 return self.input_translator
             else:
                 item -= 1
 
         return self.layer_translators[item]
 
     def __iter__(self) -> Generator[th.nn.Module, None, None]:
+        """Get iterator over the translators within the lens."""
         if isinstance(self.input_translator, th.nn.Module):
             yield self.input_translator
 
         yield from self.layer_translators
 
     @classmethod
     def load(cls, resource_id: str, **kwargs) -> "TunedLens":
@@ -236,15 +238,15 @@
                     )
                     new_key = key.replace(old_key, "translator")
                     state[new_key] = state.pop(key)
 
         # Drop unrecognized config keys
         unrecognized = set(config) - set(inspect.getfullargspec(cls).kwonlyargs)
         for key in unrecognized:
-            print(f"TunedLens.load: ignoring config key '{key}'")
+            warn(f"Ignoring config key '{key}'")
             del config[key]
 
         lens = cls(**config)
 
         if num_extras := config.get("extra_layers"):
             # This is sort of a hack but AutoConfig doesn't appear to have a from_dict
             # for some reason.
@@ -266,25 +268,36 @@
                     for i in range(num_extras)
                 ]
             )
 
         lens.load_state_dict(state)
         return lens
 
-    def save(self, path: Union[Path, str], ckpt: str = "params.pt") -> None:
+    def save(
+        self,
+        path: Union[Path, str],
+        ckpt: str = "params.pt",
+        config: str = "config.json",
+    ) -> None:
+        """Save the lens to a directory.
+
+        Args:
+            path : The path to the directory to save the lens to.
+            ckpt : The name of the checkpoint file to save the parameters to.
+            config : The name of the config file to save the config to.
+        """
         path = Path(path)
         path.mkdir(exist_ok=True, parents=True)
         th.save(self.state_dict(), path / ckpt)
 
-        with open(path / "config.json", "w") as f:
+        with open(path / config, "w") as f:
             json.dump(self.config, f)
 
     def normalize_(self):
         """Canonicalize the transforms by centering their weights and biases."""
-
         for linear in self:
             assert isinstance(linear, th.nn.Linear)
 
             A, b = linear.weight.data, linear.bias.data
             A -= A.mean(dim=0, keepdim=True)
             b -= b.mean()
 
@@ -303,26 +316,27 @@
         h = self.extra_layers(h)
         while isinstance(h, tuple):
             h, *_ = h
 
         return self.unembedding(self.layer_norm(h))
 
     def forward(self, h: th.Tensor, idx: int) -> th.Tensor:
-        """Transform and then decode the hidden states into logits"""
+        """Transform and then decode the hidden states into logits."""
         # Sanity check to make sure we don't finetune the decoder
         # if any(p.requires_grad for p in self.parameters(recurse=False)):
         #     raise RuntimeError("Make sure to freeze the decoder")
 
         # We're learning a separate unembedding for each layer
         if not self.config["reuse_unembedding"]:
             h_ = self.layer_norm(h)
             return self[idx](h_)
 
         h = self.transform_hidden(h, idx)
         return self.to_logits(h)
 
     def __len__(self) -> int:
+        """Return the number of layer translators in the lens."""
         N = len(self.layer_translators)
         if self.input_translator:
             N += 1
 
         return N
```

### Comparing `tuned-lens-0.0.3/tuned_lens/plotting/plot_lens.py` & `tuned-lens-0.0.4/tuned_lens/plotting/plot_lens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Plot a lens table for some given text and model."""
+
 from ..nn.lenses import Lens
 from ..residual_stream import ResidualStream, record_residual_stream
 from transformers import (
     PreTrainedModel,
     PreTrainedTokenizer,
     PreTrainedTokenizerFast,
 )
@@ -34,48 +36,48 @@
     min_prob: float = 0.0,
     max_string_len: Optional[int] = 7,
     ellipsis: str = "…",
     newline_replacement: str = "\\n",
     newline_token: str = "Ċ",
     whitespace_token: str = "Ġ",
     whitespace_replacement: str = "_",
-    topk_diff: bool = False,
     topk: int = 10,
+    topk_diff: bool = False,
 ) -> go.Figure:
     """Plot a lens table for the given text.
 
     Args:
         model: The model to be examined.
         tokenizer: The tokenizer to use for encoding the text.
         lens: The lens use for intermediate predictions.
-
-    KWArgs:
         text: The text to use for evaluated. If not provided, the input_ids will be
             used.
         input_ids: The input IDs to use for evaluated. If not provided, the text will
             be encoded.
         mask_input: Forbid the lens from predicting the input tokens.
         start_pos: The first token id to visualize.
         end_pos: The token id to stop visualizing before.
-        extra_decoder_layers: The number of extra decoder layers to apply after before
-            the unembeding.
+        extra_decoder_layers: The number of extra decoder layers to apply after
+            before the unembeding.
         layer_stride: The number of layers to skip between each layer displayed.
-        metric: The metric to use for the lens table.
+        statistic: The statistic to use for the lens table.
             * ce: The cross entropy between the labels and the lens predictions.
             * entropy: The entropy of the lens prediction.
             * forward_kl: The KL divergence between the model and the lens.
             * max_prob: The probability of the most likely token.
         min_prob: At least one token must have a probability greater than this for the
             lens prediction to be displayed.
         max_string_len: If not None, clip the string representation of the tokens to
             this length and add an ellipsis.
         ellipsis: The string to use for the ellipsis.
         newline_replacement: The string to replace newline tokens with.
-        newline_token: The token to replace with newline_replacement.
+        newline_token: The substring to replace with newline_replacement.
         whitespace_replacement: The string to replace whitespace tokens with.
+        whitespace_token: The substring to replace with whitespace_replacement.
+        topk: The number of tokens to visualize when hovering over a cell.
         topk_diff: If true show the top k tokens where the metric has changed the from
             the previous layer.
 
     Returns:
         A plotly figure containing the lens table.
     """
     if topk < 1:
@@ -191,14 +193,26 @@
 
 def compute_statistics(
     statistic: Statistic,
     hidden_lps: ResidualStream,
     model_logits: th.Tensor,
     targets: th.Tensor,
 ) -> PlotableStatistic:
+    """Compute a statistic for each layer in the stream.
+
+    Args:
+        statistic: The statistic to compute. One of "ce", "entropy", "kl", "kl_div".
+        hidden_lps: The stream of hidden layer log probabilities produced by a lens.
+        model_logits: The logits produced by the model.
+        targets: The target ids for the sequence.
+
+    Returns:
+        A named tuple containing the statistics value at each layer and position
+        and its name and units.
+    """
     if statistic == "ce":
         assert targets.shape == hidden_lps[-1].shape[:-1], (
             "Batch and sequence lengths of targets and log probs must match."
             f"Got {targets.shape} and {hidden_lps[-1].shape[:-1]} respectively."
         )
         num_tokens = targets.nelement()
         targets = targets.reshape(num_tokens)
```

### Comparing `tuned-lens-0.0.3/tuned_lens/residual_stream.py` & `tuned-lens-0.0.4/tuned_lens/residual_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Provides a class for collecting and manipulating transformer hidden states."""
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from itertools import starmap, zip_longest
 
 from .model_surgery import get_transformer_layers
 from typing import Callable, Generator, Iterable, Optional, overload, Type, Union
 import torch as th
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/argparsers.py` & `tuned-lens-0.0.4/tuned_lens/scripts/argparsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+"""Provides function for creating the argument parse for the CBE command."""
 from argparse import ArgumentParser
 from pathlib import Path
 
 
 def get_cbe_parser() -> ArgumentParser:
     """Return the parser for the `bases` subcommand."""
-
     parser = ArgumentParser(
         description="Train or evaluate a set of causal bases for a language model.",
         add_help=False,
     )
 
     # Arguments shared by train and eval; see https://stackoverflow.com/a/56595689.
     parent_parser = ArgumentParser(add_help=False)
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/cbe.py` & `tuned-lens-0.0.4/tuned_lens/scripts/cbe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Sub commands for extracting and evaluating causal bases."""
 from argparse import Namespace
 from datasets import Dataset
 from itertools import islice
 from torch.utils.data import DataLoader
 from transformers import PreTrainedModel
 from tqdm.auto import tqdm
 from typing import Optional
@@ -15,14 +16,15 @@
 @th.autocast("cuda", enabled=th.cuda.is_available())
 @th.no_grad()
 def eval_bases(
     args: Namespace,
     model: PreTrainedModel,
     data: Dataset,
 ):
+    """Sub command for evaluating a set of causal bases."""
     assert args.output is not None
 
     local_rank = dist.get_rank() if dist.is_initialized() else 0
     basis_paths = {int(p.stem.split("_")[1]): p for p in args.bases.glob("layer_*.pt")}
     L = len(basis_paths)
     K = args.k
 
@@ -80,14 +82,15 @@
 
 def extract_bases(
     args: Namespace,
     model: PreTrainedModel,
     data: Dataset,
     lens: Optional[TunedLens],
 ):
+    """Sub command for extracting causal basis from a model and lens."""
     local_rank = dist.get_rank() if dist.is_initialized() else 0
     args.output.mkdir(parents=True, exist_ok=True)
 
     data = data.shuffle(seed=args.seed)  # type: ignore[arg-type]
     batch = send_to_device(data[: args.per_gpu_batch_size], th.device(local_rank))
 
     with th.autocast("cuda"), th.no_grad():
@@ -101,11 +104,7 @@
         labels=batch["input_ids"] if args.loss == "ce" else None,
         mode=args.mode,
         no_translator=args.no_translator,
     )
     for i, basis in enumerate(basis_iter):
         if local_rank == 0:
             th.save(basis, args.output / f"layer_{i}.pt")
-
-
-def main(args):
-    pass
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/downstream.py` & `tuned-lens-0.0.4/tuned_lens/scripts/downstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Provides Sub command for downstream evaluation."""
 from argparse import Namespace
 from collections import defaultdict
 from datasets import Dataset
 from hashlib import md5
 from tqdm.auto import tqdm
 from transformers import PreTrainedTokenizerBase
 from typing import Iterable, MutableSequence
@@ -24,14 +25,15 @@
 @th.no_grad()
 def downstream_loop(
     args: Namespace,
     model: th.nn.Module,
     lens: TunedLens,
     tokenizer: PreTrainedTokenizerBase,
 ):
+    """Downstream evaluation loop for the tuned lens model."""
     from lm_eval.metrics import stderr_for_metric
     from lm_eval.tasks import get_task_dict
 
     os.environ["TOKENIZERS_PARALLELISM"] = str(not dist.is_initialized())
 
     local_rank = dist.get_rank() if dist.is_initialized() else 0
     world_size = dist.get_world_size() if dist.is_initialized() else 1
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/eval_loop.py` & `tuned-lens-0.0.4/tuned_lens/scripts/eval_loop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+"""Evaluation loop for the tuned lens model."""
 from argparse import Namespace
 from datasets import Dataset
 from collections import defaultdict
 from itertools import islice
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 from transformers import PreTrainedModel
 from typing import Optional
 from tuned_lens.residual_stream import record_residual_stream
 from tuned_lens.stats import ResidualStats, LogitStats
 from tuned_lens.nn import Decoder, TunedLens
-from tuned_lens.stats import CalibrationError
 from tuned_lens.utils import (
     maybe_all_cat,
     maybe_all_reduce,
-    maybe_shift_labels,
-    maybe_shift_preds,
+    shift_labels,
+    shift_preds,
     pytree_map,
     pytree_stack,
     send_to_device,
 )
 import torch as th
 import torch.distributed as dist
 
@@ -28,14 +28,23 @@
 def eval_loop(
     args: Namespace,
     model: PreTrainedModel,
     data: Dataset,
     lens: Optional[TunedLens],
     nats_to_bpb_ratio: float,
 ):
+    """Trains a TunedLens model against a transformer on a dataset.
+
+    Args:
+        args: The command-line arguments see __main__.py train subcommand.
+        model: The transformer model to train.
+        data: The dataset to train on.
+        lens: The TunedLens model to train.
+        nats_to_bpb_ratio: The ratio of nats to bits per byte for the dataset.
+    """
     local_rank = dist.get_rank() if dist.is_initialized() else 0
     dl = DataLoader(
         data.shuffle(seed=args.seed),  # type: ignore[arg-type],
         batch_size=args.per_gpu_batch_size,
     )
     if lens:
         lens.eval()
@@ -55,33 +64,30 @@
     output_dir.mkdir(exist_ok=True, parents=True)
 
     _to_logits = lens.to_logits if lens else Decoder(model)
     L = model.config.num_hidden_layers
     batches = []
     transfer_batches = []
 
-    final_calibration = CalibrationError()
     grad_alignments = [[] for _ in range(L)]
-    ll_calibration = [CalibrationError() for _ in range(L)]
-    tl_calibration = [CalibrationError() for _ in range(L)]
 
     final_logit_stats = LogitStats()
     ll_statistics = [LogitStats() for _ in range(L)]
     tl_statistics = [LogitStats() for _ in range(L)]
 
     pbar = tqdm(dl, desc="Evaluating", position=local_rank, total=total)
     for batch in pbar:
         batch = send_to_device(batch, th.device(local_rank))
         with record_residual_stream(model) as stream:
             output = model(**batch)
 
         shift = args.token_shift if args.token_shift is not None else 1
         final_lps = output.logits.log_softmax(dim=-1)
         final_probs = final_lps.exp()
-        labels = maybe_shift_labels(batch["input_ids"], shift)
+        labels = shift_labels(batch["input_ids"], shift)
 
         batch_output = defaultdict(dict)
         transfer_ces = th.zeros(L, L, device=final_lps.device)
         transfer_kls = th.zeros(L, L, device=final_lps.device)
 
         # Compute logit lens eval and statistics
         for (j, d), (name, h) in zip(enumerate(stream.residuals()), stream.items()):
@@ -91,15 +97,15 @@
 
             with th.set_grad_enabled(args.grad_alignment):
                 baseline_lps = _to_logits(h).log_softmax(dim=-1)
 
                 # Note that we don't reduce the loss here, since we want to look at
                 # the full distribution of losses across tokens and samples
                 losses = th.nn.functional.cross_entropy(
-                    maybe_shift_preds(baseline_lps, shift).flatten(0, 1),
+                    shift_preds(baseline_lps, shift).flatten(0, 1),
                     labels.flatten(),
                     reduction="none",
                 )
                 avg_loss = losses.mean()
 
             if args.grad_alignment:
                 avg_loss.backward()
@@ -108,17 +114,14 @@
                 grad_alignments[j].append(
                     th.nn.functional.cosine_similarity(
                         h.grad.flatten(1), d.flatten(1), dim=-1
                     )
                 )
                 h.grad = None
 
-            ll_calibration[j].update(
-                labels, maybe_shift_preds(baseline_lps.exp(), shift)
-            )
             ll_statistics[j].update(baseline_lps, assume_normalized=True)
 
             batch_output["baseline_ce"][name] = losses
             batch_output["baseline_entropy"][name] = th.sum(
                 -baseline_lps.exp() * baseline_lps, dim=-1
             )
             batch_output["baseline_kl"][name] = th.sum(
@@ -128,51 +131,49 @@
         # Compute tuned lens eval and statistics if applicable
         if lens:
             for j, (name, h) in zip(range(L), stream.items()):
                 lens_lps = lens(h, idx=j).log_softmax(dim=-1)
                 lens_probs = lens_lps.exp()
 
                 batch_output["lens_ce"][name] = th.nn.functional.cross_entropy(
-                    maybe_shift_preds(lens_lps, shift).flatten(0, 1),
+                    shift_preds(lens_lps, shift).flatten(0, 1),
                     labels.flatten(),
                     reduction="none",
                 )
                 batch_output["lens_entropy"][name] = th.sum(
                     -lens_probs * lens_lps, dim=-1
                 )
                 batch_output["lens_kl"][name] = th.sum(
                     final_probs * (final_lps - lens_lps), dim=-1
                 )
-                tl_calibration[j].update(labels, maybe_shift_preds(lens_probs, shift))
                 tl_statistics[j].update(lens_lps, assume_normalized=True)
 
                 if args.transfer:
                     # Each iteration of the loop processes a different *probe* layer i
                     # for the test layer j.
                     for i in range(L):
                         transfer_lps = lens(h, idx=i).log_softmax(dim=-1)
                         transfer_ces[i, j] = th.nn.functional.cross_entropy(
-                            maybe_shift_preds(transfer_lps, shift).flatten(0, 1),
+                            shift_preds(transfer_lps, shift).flatten(0, 1),
                             labels.flatten(),
                         )
                         transfer_kls[i, j] = th.sum(
                             lens_probs * (lens_lps - transfer_lps), dim=-1
                         ).mean()
 
-        final_calibration.update(labels, maybe_shift_preds(final_probs, shift))
         final_logit_stats.update(final_lps, assume_normalized=True)
         if args.residual_stats:
             # Drop the first token because it's weird
             rest = stream.map(lambda x: x[:, 1:])
 
             delta_stats.update(rest.residuals())
             stream_stats.update(rest)
 
         batch_output["baseline_ce"]["final"] = th.nn.functional.cross_entropy(
-            maybe_shift_preds(final_lps, shift).flatten(0, 1),
+            shift_preds(final_lps, shift).flatten(0, 1),
             labels.flatten(),
             reduction="none",
         )
         batch_output["baseline_entropy"]["final"] = th.sum(
             -final_probs * final_lps, dim=-1
         )
         th.save(batch_output, output_dir / f"batch_{pbar.n}.pt")
@@ -201,34 +202,24 @@
 
     # first_token_stats.all_reduce_()
     delta_stats.all_reduce_()
     stream_stats.all_reduce_()
     for stats in ll_statistics:
         stats.all_reduce_()
 
-    final_calibration.all_gather_()
-    for cal in ll_calibration:
-        cal.all_gather_()
-
     if lens:
         for stats in tl_statistics:
             stats.all_reduce_()
-        for cal in tl_calibration:
-            cal.all_gather_()
 
     if args.grad_alignment:
         grad_alignments = [maybe_all_cat(th.cat(x, dim=0)) for x in grad_alignments]
         if local_rank == 0:
             th.save(grad_alignments, root_dir / "grad_alignments.pt")
 
     if local_rank == 0:
         th.save(delta_stats, root_dir / "delta_stats.pt")
         th.save(stream_stats, root_dir / "stream_stats.pt")
 
         th.save(final_logit_stats, root_dir / "final_logit_stats.pt")
         th.save(ll_statistics, root_dir / "ll_logit_stats.pt")
         if lens:
             th.save(tl_statistics, root_dir / "tl_logit_stats.pt")
-            th.save(tl_calibration, root_dir / "tl_calibration.pt")
-
-        th.save(final_calibration, root_dir / "final_calibration.pt")
-        th.save(ll_calibration, root_dir / "ll_calibration.pt")
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/lens.py` & `tuned-lens-0.0.4/tuned_lens/scripts/lens.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import pickle
 import shutil
 import torch as th
 import torch.distributed as dist
 
 
 def main(args):
+    """The main entry point for the command line script."""
     local_rank = dist.get_rank() if dist.is_initialized() else 0
 
     # Deterministically choose a temporary cache directory shared
     # by all ranks using MD5 hash of the command line arguments
     if args.no_cache:
         cache_dir = f"/tmp/{md5(pickle.dumps(args)).hexdigest()}"
     else:
@@ -98,30 +99,34 @@
         print(f"Using '{layer_cls.__name__}' for transformer_auto_wrap_policy.")
 
         model = FSDP(
             model,
             auto_wrap_policy=partial(
                 transformer_auto_wrap_policy, transformer_layer_cls={layer_cls}
             ),
-            cpu_offload=CPUOffload(offload_params=True),
+            cpu_offload=CPUOffload(offload_params=args.cpu_offload),
             device_id=local_rank,
             # This turns out to be important for training speed
             forward_prefetch=True,
             mixed_precision=MixedPrecision(
                 param_dtype=th.float16,
                 reduce_dtype=th.float16,
                 buffer_dtype=th.float16,
             ),
         )
+    elif args.cpu_offload:
+        raise ValueError("CPU offload requires FSDP.")
     else:
         model.to(local_rank)
 
-    # Load tokenizer & data
     tokenizer = AutoTokenizer.from_pretrained(
-        args.tokenizer or args.model_name, use_fast=not args.slow_tokenizer
+        args.tokenizer or args.model_name,
+        revision=args.revision,
+        use_fast=not args.slow_tokenizer,
+        tokenizer_type=args.tokenizer_class,
     )
     assert isinstance(tokenizer, PreTrainedTokenizerBase)
     silence_datasets_messages()
 
     if args.command == "downstream":
         downstream_loop(args, model, lens, tokenizer)
         return
```

### Comparing `tuned-lens-0.0.3/tuned_lens/scripts/train_loop.py` & `tuned-lens-0.0.4/tuned_lens/scripts/train_loop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,45 @@
+"""Training loop for training a TunedLens model against a transformer on a dataset."""
 from argparse import Namespace
 from collections import defaultdict
 from datasets import Dataset
 from itertools import islice
 from torch.distributed.optim import ZeroRedundancyOptimizer
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 from transformers import get_linear_schedule_with_warmup
 from tuned_lens import TunedLens
 from tuned_lens.residual_stream import ResidualStream
 from tuned_lens.utils import (
     maybe_all_reduce,
-    maybe_shift_labels,
-    maybe_shift_preds,
+    shift_labels,
+    shift_preds,
     send_to_device,
 )
 import torch as th
 import torch.distributed as dist
 
 
 def train_loop(
     args: Namespace,
     model: th.nn.Module,
     data: Dataset,
     lens: TunedLens,
     nats_to_bpb: float,
 ):
+    """Trains a TunedLens model against a transformer on a dataset.
+
+    Args:
+        args: The command-line arguments see __main__.py train subcommand.
+        model: The transformer model to train.
+        data: The dataset to train on.
+        lens: The TunedLens model to train.
+        nats_to_bpb: The ratio of nats to bits per byte for the dataset.
+    """
     lens_size = sum(p.numel() * p.element_size() for p in lens.parameters())
     print(f"Tuned lens memory usage: {lens_size / 2 ** 20:.2f} MB per GPU")
 
     if args.constant:
         for probe in lens:
             probe.weight.requires_grad_(False)
 
@@ -162,22 +172,22 @@
 
             # Match the *current* token distribution by default
             if shift is None:
                 shift = 0
         else:
             raise NotImplementedError(f"Unknown loss {args.loss}")
 
-        labels = maybe_shift_labels(labels, shift)
+        labels = shift_labels(labels, shift)
 
         # We do this sequentially to save VRAM
         for i, (name, h) in enumerate(stream.items()):
             # bfloat16 has larger dynamic range than float16 and seems to be better for
             # computing log softmax & KL loss
             with th.autocast("cuda", dtype=th.bfloat16):
-                logits = maybe_shift_preds(ddp_lens(h, idx=i), shift)
+                logits = shift_preds(ddp_lens(h, idx=i), shift)
 
                 if args.loss == "ce":
                     loss = th.nn.functional.cross_entropy(
                         logits.flatten(0, -2), labels.flatten()
                     )
                 elif args.loss == "kl":
                     loss = th.sum(
@@ -201,15 +211,15 @@
 
             scaled_loss.backward()
 
         step, rem = divmod(batch_idx, grad_acc_steps)
         if rem == 0:
             th.nn.utils.clip_grad_norm_(lens.parameters(), 1.0)
             opt.step()
-            opt.zero_grad()
+            opt.zero_grad(set_to_none=False)
             scheduler.step()
 
             if local_rank == 0 and args.wandb:
                 import wandb
 
                 log_dict = {
                     k: th.stack(v).mean() * nats_to_bpb for k, v in metrics.items()
```

### Comparing `tuned-lens-0.0.3/tuned_lens/stats/anomaly.py` & `tuned-lens-0.0.4/tuned_lens/stats/anomaly.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/stats/dimensionality.py` & `tuned-lens-0.0.4/tuned_lens/stats/dimensionality.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/stats/distance.py` & `tuned-lens-0.0.4/tuned_lens/stats/distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.3/tuned_lens/stats/logit_stats.py` & `tuned-lens-0.0.4/tuned_lens/stats/logit_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             [log_alpha],
             line_search_fn="strong_wolfe",
             max_iter=max_iter,
             tolerance_change=tol,
         )
 
         def closure():
-            opt.zero_grad()
+            opt.zero_grad(set_to_none=False)
 
             # See http://jonathan-huang.org/research/dirichlet/dirichlet.pdf,
             # page 5 for the formula
             alpha = log_alpha.exp()
             normalizer = alpha.sum().lgamma() - alpha.lgamma().sum()
             loss = -(normalizer + (alpha - 1) @ self.sufficient_stats)
             loss.backward()
```

### Comparing `tuned-lens-0.0.3/tuned_lens/stats/residual_stats.py` & `tuned-lens-0.0.4/tuned_lens/stats/residual_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Compute online mean and covariance for residual streams."""
+
 from ..residual_stream import ResidualStream
 from typing import Optional
 import torch as th
 
 
 class ResidualStats:
     """Online mean and covariance matrix computation for residual streams.
@@ -9,14 +11,20 @@
     Shape and device are lazily inferred from the first stream that is passed to
     `update()`. The mean and variance are computed using the Welford algorithm.
     Streams are automatically cast to full precision before updating the stats.
     """
 
     # By default we accumulate in double precision to minimize numerical error
     def __init__(self, cov: bool = True, dtype: th.dtype = th.float64):
+        """Create a new ResidualStats object.
+
+        Args:
+            cov: Whether to compute the covariance matrix.
+            dtype: The dtype to use for calculations.
+        """
         self._mu: Optional[ResidualStream] = None
         self._M2: Optional[ResidualStream] = None
         self._mean_norm: Optional[ResidualStream] = None
 
         self.cov = cov
         self.dtype = dtype
         self.n: int = 0
@@ -96,8 +104,9 @@
         """Return the current estimate of the variance."""
         if not self._M2 or self.n < 2:
             raise ValueError("Not enough data")
 
         return self._M2.map(lambda x: th.linalg.diagonal(x).div(self.n - 1).to(dtype))
 
     def __repr__(self) -> str:
+        """Return a string representation of the object."""
         return f"ResidualStats(n={self.n})"
```

### Comparing `tuned-lens-0.0.3/tuned_lens/utils.py` & `tuned-lens-0.0.4/tuned_lens/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utilities for distributed training and handling nested collections of tensors."""
+
 from itertools import islice
 from typing import cast, Any, Callable, Iterable, Sequence, Type, TypeVar, Union
 import torch as th
 import torch.distributed as dist
 
 
 T = TypeVar("T")
@@ -12,32 +14,35 @@
     if not isinstance(obj, typ):
         raise TypeError(f"Expected {typ.__name__}, got {type(obj).__name__}")
 
     return cast(typ, obj)
 
 
 def maybe_all_cat(x: th.Tensor) -> th.Tensor:
+    """Concatenate a tensor across all processes."""
     if not dist.is_initialized():
         return x
 
     buffer = x.new_empty([dist.get_world_size() * x.shape[0], *x.shape[1:]])
     dist.all_gather_into_tensor(buffer, x)
     return buffer
 
 
 def maybe_all_gather_lists(lst: list) -> list:
+    """Gather a list of objects from all processes."""
     if not dist.is_initialized():
         return lst
 
     lists = [[] for _ in range(dist.get_world_size())]
     dist.all_gather_object(lists, lst)
     return sum(lists, [])
 
 
 def maybe_all_reduce(x: th.Tensor, op: str = "mean") -> th.Tensor:
+    """Reduce a tensor across all processes."""
     if not dist.is_initialized():
         return x
 
     if op == "sum":
         dist.all_reduce(x, op=dist.ReduceOp.SUM)
     elif op == "mean":
         dist.all_reduce(x, op=dist.ReduceOp.SUM)
@@ -52,24 +57,44 @@
     """Unpack a tuple if it's a tuple, otherwise return the value."""
     if isinstance(x, tuple):
         x, *_ = x
 
     return x
 
 
-def maybe_shift_labels(x: th.Tensor, shift: int):
+def shift_labels(x: th.Tensor, shift: int):
+    """Shift labels by a given amount.
+
+    Args:
+        x: (batch x seq_len) labels to shift.
+        shift: Amount to shift by. Positive values take from the start, negative values
+            negative values take from the end.
+
+    Returns:
+        (batch x (seq_len - shift)) labels shifted by the given amount.
+    """
     if shift > 0:
         return x[:, shift:]
     if shift < 0:
         return x[:, :shift]
 
     return x
 
 
-def maybe_shift_preds(x: th.Tensor, shift: int):
+def shift_preds(x: th.Tensor, shift: int):
+    """Shift predictions by a given amount.
+
+    Args:
+        x: (batch x seq_len) predictions to shift.
+        shift: Amount to shift by. Positive values take from the end, negative values
+            from the start.
+
+    Returns:
+        (batch x (seq_len - shift)) predictions shifted by the given amount.
+    """
     if shift > 0:
         return x[:, :-shift]
     if shift < 0:
         return x[:, -shift:]
 
     return x
 
@@ -103,17 +128,23 @@
         for elem in tree:
             yield from pytree_flatten(elem)
 
 
 def pytree_map(
     func: Callable[[th.Tensor], Any], tree: TreeType, strict: bool = True
 ) -> TreeType:
-    """
-    Recursively apply a function to all tensors in a pytree, returning the results
-    in a new pytree with the same structure. Non-tensor leaves are copied.
+    """Recursively apply a function to all tensors in a pytree.
+
+    Args:
+        func: Function to apply to each tensor.
+        tree: Pytree to apply the function to.
+        strict: If True, raise an error if a non-tensor leaf is encountered.
+
+    Returns:
+        A new pytree with the same structure. Non-tensor leaves are copied.
     """
     # Stopping condition
     if isinstance(tree, th.Tensor):
         return func(tree)
 
     # Recursive case
     if isinstance(tree, dict):
@@ -130,37 +161,51 @@
             f"Found leaf '{tree}' of unsupported type '{type(tree).__name__}'- use "
             f"`strict=False` to ignore"
         )
     else:
         return tree
 
 
-def pytree_cat(trees: Sequence, dim: int = 0) -> AnyTree:
-    """
-    Concatenate pytrees along a given dimension, returning a new pytree with the same
-    structure. All pytrees are expected to have the same structure; undefined behavior
+def pytree_cat(trees: Sequence[AnyTree], dim: int = 0) -> AnyTree:
+    """Concatenate pytrees along a given dimension.
+
+    All pytrees are expected to use the same collection; undefined behavior
     will occur if this is not the case.
+
+    Args:
+        trees: Sequence of pytrees containing tensors to concatenate.
+        dim: Dimension to concatenate along.
+
+    Returns:
+        - A new pytree with the same structure.
     """
     transposed_iter = zip(*(pytree_flatten(tree) for tree in trees))
     leaf_iter = (th.cat(seq, dim) for seq in transposed_iter)
     try:
         return pytree_map(lambda _: next(leaf_iter), trees[0])  # type: ignore
     except (RuntimeError, StopIteration) as e:
         # Calling next() on an exhausted generator raises a RuntimeError, annoyingly
         if isinstance(e, StopIteration) or "StopIteration" in str(e):
             raise TypeError("All pytrees must have the same structure") from e
         else:
             raise
 
 
 def pytree_stack(trees: Sequence, dim: int = 0) -> AnyTree:
-    """
-    Stack pytrees along a given dimension, returning a new pytree with the same
-    structure. All pytrees are expected to have the same structure; undefined behavior
+    """Stack pytrees along a given dimension.
+
+    All pytrees are expected to use the same collection; undefined behavior
     will occur if this is not the case.
+
+    Args:
+        trees: Sequence of pytrees containing tensors to stack.
+        dim: Dimension to concatenate along.
+
+    Returns:
+        A new pytree with the same structure.
     """
     if not len(trees):
         raise ValueError("Cannot stack empty sequence of pytrees")
 
     transposed_iter = zip(*(pytree_flatten(tree) for tree in trees))
     leaf_iter = (th.stack(seq, dim) for seq in transposed_iter)
     try:
```

### Comparing `tuned-lens-0.0.3/tuned_lens.egg-info/PKG-INFO` & `tuned-lens-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,82 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: notebooks
 License-File: LICENSE
 
 # Tuned Lens 🔎
-Tools for understanding how transformer predictions are built layer-by-layer
+<a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+<a target="_blank" href="https://huggingface.co/spaces/AlignmentResearch/tuned-lens">
+<img src="https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-sm-dark.svg", alt="Open in Spaces">
+</a>
 
-![Using the Tuned-lens](https://user-images.githubusercontent.com/12176390/224879115-8bc95f26-68e4-4f43-9b4c-06ca5934a29d.png)
 
-This package provides a simple interface training and evaluating __tuned lenses__. A tuned lens allows us to peak at the iterative computations that a transformer is using the compute the next token.
+Tools for understanding how transformer predictions are built layer-by-layer.
 
-A lens into a transformer with n layers allows you to replace the last $m$ layers of the model with an [affine transformation](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html) (we call these affine translators).
+<img src=https://user-images.githubusercontent.com/12176390/224879115-8bc95f26-68e4-4f43-9b4c-06ca5934a29d.png>
 
-This skips over these last few layers and lets you see the best prediction that can be made from the model's intermediate representations, i.e. the residual stream, at layer $n - m$. Since the representations may be rotated, shifted, or stretched from layer to layer it's useful to train an affine specifically on each layer. This training is what differentiates this method from simpler approaches that decode the residual stream of the network directly using the unembeding layer i.e. the [logit lens](https://www.lesswrong.com/posts/AcKRB8wDpdaN6v6ru/interpreting-gpt-the-logit-lens). We explain this process and its applications in a forthcoming paper "Eliciting Latent Predictions from Transformers with the Tuned Lens".
+This package provides a simple interface for training and evaluating __tuned lenses__. A tuned lens allows us to peek at the iterative computations a transformer uses to compute the next token.
 
-### Acknowledgments
-Originally concieved by [Igor Ostrovsky](https://twitter.com/igoro?lang=en) and [Stella Biderman](www.stellabiderman) at [EleutherAI](www.eleuther.ai), this library was built as a collaboration between FAR and EleutherAI researchers.
 
-> **Warning**
-> This package has not reached 1.0 yet. Expect the public interface to change regularly and without a major version bump.
+## What is a Lens?
+<img alt="A diagram showing how a translator within the lens allows you to skip intermediate layers." src="https://user-images.githubusercontent.com/12176390/227057947-1ef56811-f91f-48ff-8d2d-ff04cc599125.png"  width=400/>
 
-## Install instructions
-### Installing From Source
-First you will need to install the basic prerequisites into a virtual environment
-* Python 3.9+
-* Pytorch 1.12.0+
+A lens into a transformer with _n_ layers allows you to replace the last _m_ layers of the model with an [affine transformation](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html) (we call these affine translators). Each affine translator is trained to minimize the KL divergence between its prediction and the final output distribution of the original model. This means that after training, the tuned lens allows you to skip over these last few layers and see the best prediction that can be made from the model's intermediate representations, i.e., the residual stream, at layer _n - m_.
 
-then you can simply install the package using pip.
-```
-git clone https://github.com/AlignmentResearch/tuned-lens
-cd tuned-lens
-pip install .
-```
+The reason we need to train an affine translator is that the representations may be rotated, shifted, or stretched from layer to layer. This training differentiates this method from simpler approaches that unembed the residual stream of the network directly using the unembedding matrix, i.e., the [logit lens](https://www.lesswrong.com/posts/AcKRB8wDpdaN6v6ru/interpreting-gpt-the-logit-lens). We explain this process and its applications in the paper [Eliciting Latent Predictions from Transformers with the Tuned Lens](https://arxiv.org/abs/2303.08112).
 
-### Install Using Docker
-If you prefer to run the code from within a container you can use the provided docker
-file
-```
-git clone https://github.com/AlignmentResearch/tuned-lens
-cd tuned-lens
-docker build -t tuned-lens-prod --target prod .
-```
-
-## Quick Start Guid
-### Downloading the datasets
-```
-wget https://the-eye.eu/public/AI/pile/val.jsonl.zst
-unzstd val.jsonl.zst
+### Acknowledgments
+Originally conceived by [Igor Ostrovsky](https://twitter.com/igoro) and [Stella Biderman](https://www.stellabiderman.com/) at [EleutherAI](https://www.eleuther.ai/), this library was built as a collaboration between FAR and EleutherAI researchers.
 
-wget https://the-eye.eu/public/AI/pile/test.jsonl.zst
-unzstd test.jsonl.zst
-```
+## Install Instructions
+### Installing from PyPI
+First, you will need to install the basic prerequisites into a virtual environment:
+* Python 3.9+
+* PyTorch 1.13.0+
 
-### Evaluating a Lens
-Once you have a lens file either by training it yourself of by downloading it. You
-can run various evaluations on it using the provided evaluation command.
+Then, you can simply install the package using pip.
 ```
-tuned-lens eval gpt2 test.jsonl --lens gpt-2-lens
-    --dataset the_pile all \
-    --split validation \
-    --output lens_eval_results.json
+pip install tuned-lens
 ```
 
+### Installing the container
+If you prefer to run the training scripts from within a container, you can use the provided Docker container.
 
-### Training a Lens
-This will train a tuned lens on gpt-2 with the default hyper parameters.
-
-```bash
-tuned-lens train gpt2 val.jsonl
-    --dataset the_pile all \
-    --split validation \
-    --output gpt-2-lens
 ```
-
-> **Note**
-> This will download the entire validation set of the pile which is over 30 GBs. If you
-> are doing this within a docker file it's recommended to mount external storage to huggingface's
-> cache directory.
+docker pull ghcr.io/alignmentresearch/tuned-lens:latest
+docker run --rm tuned-lens:latest tuned-lens --help
+```
 
 ## Contributing
-Make sure to install the dev dependencies and install the pre-commit hooks
+Make sure to install the dev dependencies and install the pre-commit hooks.
 ```
+$ git clone https://github.com/AlignmentResearch/tuned-lens.git
 $ pip install -e ".[dev]"
 $ pre-commit install
 ```
 
+## Citation
 
-## Citation Information
-
-If you find this library useful, please cite it as
+If you find this library useful, please cite it as:
 
 ```bibtex
 @article{belrose2023eliciting,
   title={Eliciting Latent Predictions from Transformers with the Tuned Lens},
   authors={Belrose, Nora and Furman, Zach and Smith, Logan and Halawi, Danny and McKinney, Lev and Ostrovsky, Igor and Biderman, Stella and Steinhardt, Jacob},
   journal={to appear},
   year={2023}
 }
 ```
+
+> **Warning**
+> This package has not reached 1.0. Expect the public interface to change regularly and without a major version bumps.
```

### Comparing `tuned-lens-0.0.3/tuned_lens.egg-info/SOURCES.txt` & `tuned-lens-0.0.4/tuned_lens.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,34 +22,30 @@
 tuned_lens.egg-info/SOURCES.txt
 tuned_lens.egg-info/dependency_links.txt
 tuned_lens.egg-info/entry_points.txt
 tuned_lens.egg-info/requires.txt
 tuned_lens.egg-info/top_level.txt
 tuned_lens/causal/__init__.py
 tuned_lens/causal/ablation.py
-tuned_lens/causal/intervention.py
 tuned_lens/causal/subspaces.py
 tuned_lens/causal/utils.py
 tuned_lens/nn/__init__.py
 tuned_lens/nn/_model_specific.py
 tuned_lens/nn/decoder.py
 tuned_lens/nn/downstream_wrapper.py
 tuned_lens/nn/lenses.py
-tuned_lens/nn/probe_dict.py
 tuned_lens/plotting/__init__.py
-tuned_lens/plotting/interventions.py
 tuned_lens/plotting/plot_lens.py
 tuned_lens/scripts/__init__.py
 tuned_lens/scripts/argparsers.py
 tuned_lens/scripts/cbe.py
 tuned_lens/scripts/downstream.py
 tuned_lens/scripts/eval_loop.py
 tuned_lens/scripts/lens.py
 tuned_lens/scripts/train_loop.py
 tuned_lens/stats/__init__.py
 tuned_lens/stats/anomaly.py
-tuned_lens/stats/calibration.py
 tuned_lens/stats/dimensionality.py
 tuned_lens/stats/distance.py
 tuned_lens/stats/logit_stats.py
 tuned_lens/stats/rank.py
 tuned_lens/stats/residual_stats.py
```

