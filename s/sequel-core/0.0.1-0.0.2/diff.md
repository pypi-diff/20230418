# Comparing `tmp/sequel-core-0.0.1.tar.gz` & `tmp/sequel-core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequel-core-0.0.1.tar", last modified: Tue Apr 18 13:28:45 2023, max compression
+gzip compressed data, was "sequel-core-0.0.2.tar", last modified: Tue Apr 18 15:48:41 2023, max compression
```

## Comparing `sequel-core-0.0.1.tar` & `sequel-core-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,110 @@
-drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 13:28:45.060125 sequel-core-0.0.1/
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1050 2023-04-18 13:03:45.000000 sequel-core-0.0.1/LICENSE
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3468 2023-04-18 13:28:45.060125 sequel-core-0.0.1/PKG-INFO
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2640 2023-04-06 11:32:02.000000 sequel-core-0.0.1/README.md
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1025 2023-04-18 13:27:58.000000 sequel-core-0.0.1/pyproject.toml
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      448 2023-04-06 11:32:05.000000 sequel-core-0.0.1/requirements.txt
-drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 13:28:45.056125 sequel-core-0.0.1/sequel/
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      259 2023-04-06 11:32:05.000000 sequel-core-0.0.1/sequel/__init__.py
-drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 13:28:45.056125 sequel-core-0.0.1/sequel_core.egg-info/
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3468 2023-04-18 13:28:45.000000 sequel-core-0.0.1/sequel_core.egg-info/PKG-INFO
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      350 2023-04-18 13:28:45.000000 sequel-core-0.0.1/sequel_core.egg-info/SOURCES.txt
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)        1 2023-04-18 13:28:45.000000 sequel-core-0.0.1/sequel_core.egg-info/dependency_links.txt
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      449 2023-04-18 13:28:45.000000 sequel-core-0.0.1/sequel_core.egg-info/requires.txt
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)        7 2023-04-18 13:28:45.000000 sequel-core-0.0.1/sequel_core.egg-info/top_level.txt
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)       38 2023-04-18 13:28:45.060125 sequel-core-0.0.1/setup.cfg
-drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 13:28:45.060125 sequel-core-0.0.1/tests/
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      468 2023-04-06 11:32:05.000000 sequel-core-0.0.1/tests/test_assertions.py
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1182 2023-04-06 11:32:05.000000 sequel-core-0.0.1/tests/test_backbone_jax.py
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      795 2023-04-06 11:32:05.000000 sequel-core-0.0.1/tests/test_backbone_pytorch.py
--rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1366 2023-04-06 11:32:05.000000 sequel-core-0.0.1/tests/test_benchmarks.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.020543 sequel-core-0.0.2/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1050 2023-04-18 13:03:45.000000 sequel-core-0.0.2/LICENSE
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3468 2023-04-18 15:48:41.020543 sequel-core-0.0.2/PKG-INFO
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2640 2023-04-06 11:32:02.000000 sequel-core-0.0.2/README.md
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1423 2023-04-18 15:48:23.000000 sequel-core-0.0.2/pyproject.toml
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      448 2023-04-18 14:13:25.000000 sequel-core-0.0.2/requirements.txt
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.008543 sequel-core-0.0.2/sequel/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      259 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/__init__.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.008543 sequel-core-0.0.2/sequel/algos/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)       92 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)    14029 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/base_algo.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.008543 sequel-core-0.0.2/sequel/algos/jax/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      656 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5269 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/jax/agem.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     4963 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/jax/der.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2067 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/jax/er.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1792 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/ewc.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)    10264 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/jax/jax_base_algo.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1334 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/joint.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2869 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/lfl.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2062 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/mas.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     6005 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/jax/mcsgd.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1978 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/jax/si.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/algos/pytorch/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      791 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3865 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/agem.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2413 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/der.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2092 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/er.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1711 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/ewc.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     6040 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/icarl.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1329 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/joint.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)    11491 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/kcl.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     7173 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/lamaml.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1584 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/lfl.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2069 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/mas.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5939 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/mcsgd.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     9157 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/pytorch/pytorch_base_algo.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2493 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/si.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/algos/pytorch/utils/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/utils/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1803 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/pytorch/utils/weight_gradient_manipulation.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/algos/utils/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      141 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/utils/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3928 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/algos/utils/callback_hooks.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      890 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/algos/utils/state_manager.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/backbones/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      100 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/backbones/__init__.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/backbones/jax/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      227 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2022 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/base_backbone.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1123 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/cnn.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1381 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/mlp.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      901 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/resnet.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2829 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/jax/utils.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/backbones/pytorch/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      316 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3722 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/base_backbone.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5363 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/cnn.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2078 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/mlp.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.012543 sequel-core-0.0.2/sequel/backbones/pytorch/model_factory/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)       65 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/model_factory/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1326 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/backbones/pytorch/model_factory/kcl.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3679 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/resnet.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1789 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/backbones/pytorch/utils.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel/benchmarks/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1389 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/benchmarks/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)    10644 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/benchmarks/base_benchmark.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5827 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/benchmarks/buffer.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5321 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/benchmarks/cifar.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     4964 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/benchmarks/memory.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     5691 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/benchmarks/mnist.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2930 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/benchmarks/tinyimagenet.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3077 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/benchmarks/utils.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel/utils/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      104 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/__init__.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel/utils/callbacks/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      669 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/callbacks/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3033 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/algo_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2128 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/callbacks/base_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1581 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/callbacks/dummy.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2527 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/input_visualization_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      911 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/memory_callback.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel/utils/callbacks/metrics/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      703 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/callbacks/metrics/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2031 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/metrics/jax_metric_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     4373 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/callbacks/metrics/jax_metrics.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     6706 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/metrics/metric_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3188 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/metrics/pytorch_metric_callback.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     4007 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/callbacks/tqdm_callback.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel/utils/loggers/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      369 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/loggers/__init__.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      915 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/loggers/base_logger.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2172 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/loggers/comet_logger.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2362 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/loggers/console_logger.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      995 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/loggers/logging.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1062 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/loggers/tensorboard_logger.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2298 2023-04-18 15:29:51.000000 sequel-core-0.0.2/sequel/utils/loggers/wandb_logger.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2474 2023-04-18 15:14:27.000000 sequel-core-0.0.2/sequel/utils/utils.py
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/sequel_core.egg-info/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     3468 2023-04-18 15:48:41.000000 sequel-core-0.0.2/sequel_core.egg-info/PKG-INFO
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     2906 2023-04-18 15:48:41.000000 sequel-core-0.0.2/sequel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)        1 2023-04-18 15:48:41.000000 sequel-core-0.0.2/sequel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      449 2023-04-18 15:48:41.000000 sequel-core-0.0.2/sequel_core.egg-info/requires.txt
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)        7 2023-04-18 15:48:41.000000 sequel-core-0.0.2/sequel_core.egg-info/top_level.txt
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)       38 2023-04-18 15:48:41.020543 sequel-core-0.0.2/setup.cfg
+drwxr-xr-x   0 ndimitri (229754) lts4-staffu (10426)        0 2023-04-18 15:48:41.016543 sequel-core-0.0.2/tests/
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      468 2023-04-06 11:32:05.000000 sequel-core-0.0.2/tests/test_assertions.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1182 2023-04-18 15:29:51.000000 sequel-core-0.0.2/tests/test_backbone_jax.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)      795 2023-04-18 15:29:51.000000 sequel-core-0.0.2/tests/test_backbone_pytorch.py
+-rw-r--r--   0 ndimitri (229754) lts4-staffu (10426)     1366 2023-04-18 15:29:51.000000 sequel-core-0.0.2/tests/test_benchmarks.py
```

### Comparing `sequel-core-0.0.1/LICENSE` & `sequel-core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sequel-core-0.0.1/PKG-INFO` & `sequel-core-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequel-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Continual Learning Framework for both Jax and PyTorch.
 Author-email: Nikolaos Dimitriadis <nikolaos.dimitriadis@epfl.ch>
 Project-URL: repository, https://github.com/nik-dim/sequel
 Project-URL: homepage, https://nik-dim.github.io/sequel-site/
 Project-URL: documentation, https://nik-dim.github.io/sequel-site/
 Project-URL: issue-tracker, https://github.com/nik-dim/sequel/issues
 Project-URL: releases, https://github.com/nik-dim/sequel/releases
```

### Comparing `sequel-core-0.0.1/README.md` & `sequel-core-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sequel-core-0.0.1/sequel_core.egg-info/PKG-INFO` & `sequel-core-0.0.2/sequel_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequel-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Continual Learning Framework for both Jax and PyTorch.
 Author-email: Nikolaos Dimitriadis <nikolaos.dimitriadis@epfl.ch>
 Project-URL: repository, https://github.com/nik-dim/sequel
 Project-URL: homepage, https://nik-dim.github.io/sequel-site/
 Project-URL: documentation, https://nik-dim.github.io/sequel-site/
 Project-URL: issue-tracker, https://github.com/nik-dim/sequel/issues
 Project-URL: releases, https://github.com/nik-dim/sequel/releases
```

### Comparing `sequel-core-0.0.1/tests/test_backbone_jax.py` & `sequel-core-0.0.2/tests/test_backbone_jax.py`

 * *Files identical despite different names*

### Comparing `sequel-core-0.0.1/tests/test_backbone_pytorch.py` & `sequel-core-0.0.2/tests/test_backbone_pytorch.py`

 * *Files identical despite different names*

### Comparing `sequel-core-0.0.1/tests/test_benchmarks.py` & `sequel-core-0.0.2/tests/test_benchmarks.py`

 * *Files identical despite different names*

