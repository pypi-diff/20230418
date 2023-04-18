# Comparing `tmp/autogluon.core-0.7.0b20230417.tar.gz` & `tmp/autogluon.core-0.7.0b20230418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.0b20230417.tar", last modified: Mon Apr 17 09:04:11 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.0b20230418.tar", last modified: Tue Apr 18 09:03:58 2023, max compression
```

## Comparing `autogluon.core-0.7.0b20230417.tar` & `autogluon.core-0.7.0b20230418.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.143294 autogluon.core-0.7.0b20230417/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:04:11.143294 autogluon.core-0.7.0b20230417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.127293 autogluon.core-0.7.0b20230417/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94065 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57864 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.135294 autogluon.core-0.7.0b20230417/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169377 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.139294 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-17 09:03:48.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 09:04:10.000000 autogluon.core-0.7.0b20230417/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:04:11.131293 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:04:11.000000 autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.200870 autogluon.core-0.7.0b20230418/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.200870 autogluon.core-0.7.0b20230418/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94065 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59618 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40090 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.208871 autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.212871 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 09:03:43.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:03:58.204871 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:03:58.000000 autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.0b20230417/PKG-INFO` & `autogluon.core-0.7.0b20230418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.0b20230417
+Version: 0.7.0b20230418
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.0b20230417/setup.py` & `autogluon.core-0.7.0b20230418/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/constants.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/dataset.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.utils.try_import import try_import_ray
 from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.log_utils import DuplicateFilter
-from .fold_fitting_strategy import AbstractFoldFittingStrategy, SequentialLocalFoldFittingStrategy, ParallelFoldFittingStrategy, ParallelLocalFoldFittingStrategy, ParallelDistributedFoldFittingStrategy
+from .fold_fitting_strategy import FoldFittingStrategy, SequentialLocalFoldFittingStrategy, ParallelFoldFittingStrategy, ParallelLocalFoldFittingStrategy, ParallelDistributedFoldFittingStrategy
 from ..abstract.abstract_model import AbstractModel
 from ..abstract.model_trial import model_trial, skip_hpo
 from ...constants import MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE, REFIT_FULL_SUFFIX
 from ...hpo.exceptions import EmptySearchSpace
 from ...utils.exceptions import TimeLimitExceeded
 from ...utils.loaders import load_pkl
 from ...utils.savers import save_pkl
@@ -172,14 +172,15 @@
              y_pseudo=None,
              k_fold=None,
              k_fold_start=0,
              k_fold_end=None,
              n_repeats=1,
              n_repeat_start=0,
              groups=None,
+             _skip_oof=False,
              **kwargs):
         use_child_oof = self.params.get('use_child_oof', False)
         if use_child_oof:
             if self.is_fit():
                 # TODO: We may want to throw an exception instead and avoid calling fit more than once
                 return self
             k_fold = 1
@@ -216,56 +217,62 @@
         if self.model_base is not None:
             self.save_model_base(self.model_base)
             self.model_base = None
 
         if self._oof_pred_proba is None and self.is_fit():
             self._load_oof()
 
-        if (not self._get_tags_child().get('can_refit_full', False) or k_fold == 1) and not self.params.get('save_bag_folds', True):
+        can_refit_full = self._get_tags_child().get('can_refit_full', False)
+
+        if (not can_refit_full or k_fold == 1) and not self.params.get('save_bag_folds', True):
             # TODO: This is a hack to avoid a very challenging situation:
             #  in high_quality preset we don't save fold models, but for models that don't support refit_full,
             #  they must copy the first fold model instead of fitting again.
             #  Therefore we must override save_bag_folds for these unsupported models so that the refit versions have a fold model to copy.
             #  This could be implemented better by only keeping the first fold model artifact and avoid saving the other fold model artifacts (lower disk usage)
             #  However, this is complex to code accounting for the fitting strategies and would be prone to difficult to diagnose bugs.
             self.params['save_bag_folds'] = True
             if k_fold != 1:
                 # Only log in the situation where functionality is currently suboptimal
                 logger.log(20, '\tForcing `save_bag_folds=True` because child model does not support `refit_full`.')
 
         save_bag_folds = self.params.get('save_bag_folds', True)
         if k_fold == 1:
-            self._fit_single(X=X, y=y, model_base=model_base, use_child_oof=use_child_oof, **kwargs)
+            self._fit_single(X=X, y=y, model_base=model_base, use_child_oof=use_child_oof, skip_oof=_skip_oof, **kwargs)
             return self
         else:
             refit_folds = self.params.get('refit_folds', False)
             if refit_folds:
+                if n_repeat_start != 0 or k_fold_start != 0:
+                    raise AssertionError(f'n_repeat_start and k_fold_start must be 0 with refit_folds=True, values: ({n_repeat_start}, {k_fold_start})')
+                if k_fold_end != k_fold:
+                    raise AssertionError(f'k_fold_end and k_fold must be equal with refit_folds=True, values: ({k_fold_end}, {k_fold})')
                 save_bag_folds = False
                 if kwargs.get('time_limit', None) is not None:
                     fold_start = n_repeat_start * k_fold + k_fold_start
                     fold_end = (n_repeats - 1) * k_fold + k_fold_end
                     folds_to_fit = fold_end - fold_start
                     # Reserve time for final refit model
                     kwargs['time_limit'] = kwargs['time_limit'] * folds_to_fit / (folds_to_fit + 1.2)
             self._fit_folds(X=X, y=y, model_base=model_base, X_pseudo=X_pseudo, y_pseudo=y_pseudo,
                             k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end,
                             n_repeats=n_repeats, n_repeat_start=n_repeat_start, save_folds=save_bag_folds, groups=groups, **kwargs)
-            # FIXME: Don't save folds except for refit
             # FIXME: Cleanup self
-            # FIXME: Don't add `_FULL` to name
             # FIXME: Support `can_refit_full=False` models
             if refit_folds:
-                refit_template = self.convert_to_refit_full_template()
+                refit_template = self.convert_to_refit_full_template(name_suffix=None)
                 refit_template.params['use_child_oof'] = False
                 kwargs['time_limit'] = None
-                refit_template.fit(X=X, y=y, k_fold=1, **kwargs)
+                # _skip_oof=True to avoid inferring on training data needlessly.
+                refit_template.fit(X=X, y=y, k_fold=1, _skip_oof=True, **kwargs)
                 refit_template._oof_pred_proba = self._oof_pred_proba
                 refit_template._oof_pred_model_repeats = self._oof_pred_model_repeats
                 refit_template._child_oof = True
                 refit_template.fit_time += self.fit_time + self.predict_time
+                refit_template.predict_time = self.predict_time
                 return refit_template
             else:
                 return self
 
     def _update_k_fold(self, k_fold, k_fold_end=None, verbose=True):
         """Update k_fold and k_fold_end in case num_folds was specified"""
         k_fold_override = self.params.get('num_folds', None)
@@ -341,65 +348,67 @@
         valid_indices = self._oof_pred_model_repeats > 0
         y = y[valid_indices]
         y_pred_proba = self.get_oof_pred_proba()[valid_indices]
         if sample_weight is not None:
             sample_weight = sample_weight[valid_indices]
         return self.score_with_y_pred_proba(y=y, y_pred_proba=y_pred_proba, sample_weight=sample_weight)
 
-    def _fit_single(self, X, y, model_base, use_child_oof, time_limit=None, **kwargs):
+    def _fit_single(self, X, y, model_base, use_child_oof, time_limit=None, skip_oof=False, **kwargs):
         if self.is_fit():
             raise AssertionError('Model is already fit.')
         if self._n_repeats != 0:
             raise ValueError(f'n_repeats must equal 0 when fitting a single model with k_fold == 1, value: {self._n_repeats}')
         model_base.name = f'{model_base.name}S1F1'
         model_base.set_contexts(path_context=self.path + model_base.name + os.path.sep)
         time_start_fit = time.time()
         model_base.fit(X=X, y=y, time_limit=time_limit, **kwargs)
         model_base.fit_time = time.time() - time_start_fit
         model_base.predict_time = None
-        X_len = len(X)
-
-        # Check if pred_proba is going to take too long
-        if time_limit is not None and X_len >= 10000:
-
-            max_allowed_time = time_limit * 1.3  # allow some buffer
-            time_left = max(
-                max_allowed_time - model_base.fit_time,
-                time_limit * 0.1,  # At least 10% of time_limit
-                10,  # At least 10 seconds
-            )
-            # Sample at most 500 rows to estimate prediction time of all rows
-            # TODO: Consider moving this into end of abstract model fit for all models.
-            #  Currently this only fixes problem when in bagged mode, if not bagging, then inference could still be problematic
-            n_sample = min(500, round(X_len * 0.1))
-            frac = n_sample / X_len
-            X_sample = X.sample(n=n_sample)
-            time_start_predict = time.time()
-            model_base.predict_proba(X_sample)
-            time_predict_frac = time.time() - time_start_predict
-            time_predict_estimate = time_predict_frac / frac
-            logger.log(15, f'\t{round(time_predict_estimate, 2)}s\t= Estimated out-of-fold prediction time...')
-            if time_predict_estimate > time_left:
-                logger.warning(f'\tNot enough time to generate out-of-fold predictions for model. Estimated time required was {round(time_predict_estimate, 2)}s compared to {round(time_left, 2)}s of available time.')
-                raise TimeLimitExceeded
-
-        if use_child_oof:
-            logger.log(15, '\t`use_child_oof` was specified for this model. It will function similarly to a bagged model, but will only fit one child model.')
-            time_start_predict = time.time()
-            if model_base._get_tags().get('valid_oof', False):
-                self._oof_pred_proba = model_base.get_oof_pred_proba(X=X, y=y)
+        if not skip_oof:
+            X_len = len(X)
+            # Check if pred_proba is going to take too long
+            if time_limit is not None and X_len >= 10000:
+
+                max_allowed_time = time_limit * 1.3  # allow some buffer
+                time_left = max(
+                    max_allowed_time - model_base.fit_time,
+                    time_limit * 0.1,  # At least 10% of time_limit
+                    10,  # At least 10 seconds
+                )
+                # Sample at most 500 rows to estimate prediction time of all rows
+                # TODO: Consider moving this into end of abstract model fit for all models.
+                #  Currently this only fixes problem when in bagged mode, if not bagging, then inference could still be problematic
+                n_sample = min(500, round(X_len * 0.1))
+                frac = n_sample / X_len
+                X_sample = X.sample(n=n_sample)
+                time_start_predict = time.time()
+                model_base.predict_proba(X_sample)
+                time_predict_frac = time.time() - time_start_predict
+                time_predict_estimate = time_predict_frac / frac
+                logger.log(15, f'\t{round(time_predict_estimate, 2)}s\t= Estimated out-of-fold prediction time...')
+                if time_predict_estimate > time_left:
+                    logger.warning(f'\tNot enough time to generate out-of-fold predictions for model. Estimated time required was {round(time_predict_estimate, 2)}s compared to {round(time_left, 2)}s of available time.')
+                    raise TimeLimitExceeded
+
+            if use_child_oof:
+                logger.log(15, '\t`use_child_oof` was specified for this model. It will function similarly to a bagged model, but will only fit one child model.')
+                time_start_predict = time.time()
+                if model_base._get_tags().get('valid_oof', False):
+                    self._oof_pred_proba = model_base.get_oof_pred_proba(X=X, y=y)
+                else:
+                    logger.warning('\tWARNING: `use_child_oof` was specified but child model does not have a dedicated `get_oof_pred_proba` method. This model may have heavily overfit validation scores.')
+                    self._oof_pred_proba = model_base.predict_proba(X=X)
+                self._child_oof = True
+                model_base.predict_time = time.time() - time_start_predict
+                model_base.val_score = model_base.score_with_y_pred_proba(y=y, y_pred_proba=self._oof_pred_proba)
             else:
-                logger.warning('\tWARNING: `use_child_oof` was specified but child model does not have a dedicated `get_oof_pred_proba` method. This model may have heavily overfit validation scores.')
-                self._oof_pred_proba = model_base.predict_proba(X=X)
-            self._child_oof = True
-            model_base.predict_time = time.time() - time_start_predict
-            model_base.val_score = model_base.score_with_y_pred_proba(y=y, y_pred_proba=self._oof_pred_proba)
-        else:
-            self._oof_pred_proba = model_base.predict_proba(X=X)  # TODO: Cheater value, will be overfit to valid set
-        self._oof_pred_model_repeats = np.ones(shape=len(X), dtype=np.uint8)
+                logger.log(30, f'\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! '
+                               f'This is probably a bug and should be investigated...')
+                self._oof_pred_proba = model_base.predict_proba(X=X)  # TODO: Cheater value, will be overfit to valid set
+            self._oof_pred_model_repeats = np.ones(shape=len(X), dtype=np.uint8)
         model_base.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
         if not self.params.get('save_bag_folds', True):
             model_base.model = None
         if self.low_memory:
             self.save_child(model_base)
         self.add_child(model=model_base, add_child_times=True)
         self._set_n_repeat_single()
@@ -465,15 +474,15 @@
                    time_limit=None,
                    sample_weight=None,
                    save_folds=True,
                    groups=None,
                    num_cpus=None,
                    num_gpus=None,
                    **kwargs):
-        fold_fitting_strategy = self._get_fold_fitting_strategy(model_base=model_base, num_gpus=num_gpus)
+        fold_fitting_strategy_cls = self._get_fold_fitting_strategy(model_base=model_base, num_gpus=num_gpus)
         # TODO: Preprocess data here instead of repeatedly
         # FIXME: Raise exception if multiclass/binary and a single val fold contains all instances of a class. (Can happen if custom groups is specified)
         time_start = time.time()
         if k_fold_start != 0:
             cv_splitter = self._cv_splitters[n_repeat_start]
         else:
             cv_splitter = self._get_cv_splitter(n_splits=k_fold, n_repeats=n_repeats, groups=groups)
@@ -508,24 +517,24 @@
             model_base=model_base, model_base_kwargs=kwargs,
             bagged_ensemble_model=self, X=X, y=y, X_pseudo=X_pseudo, y_pseudo=y_pseudo, sample_weight=sample_weight,
             time_limit=time_limit, time_start=time_start, models=models,
             oof_pred_proba=oof_pred_proba, oof_pred_model_repeats=oof_pred_model_repeats,
             save_folds=save_folds, num_cpus=num_cpus, num_gpus=num_gpus
         )
         # noinspection PyCallingNonCallable
-        if issubclass(fold_fitting_strategy, ParallelFoldFittingStrategy):
+        if issubclass(fold_fitting_strategy_cls, ParallelFoldFittingStrategy):
             fold_fitting_strategy_args['num_jobs'] = num_folds
             fold_fitting_strategy_args['num_folds_parallel'] = num_folds_parallel
-        if fold_fitting_strategy == ParallelDistributedFoldFittingStrategy:
+        if fold_fitting_strategy_cls == ParallelDistributedFoldFittingStrategy:
             fold_fitting_strategy_args['model_sync_path'] = DistributedContext.get_model_sync_path()
-        fold_fitting_strategy = fold_fitting_strategy(**fold_fitting_strategy_args)
+        fold_fitting_strategy: FoldFittingStrategy = fold_fitting_strategy_cls(**fold_fitting_strategy_args)
 
         if type(fold_fitting_strategy) == ParallelLocalFoldFittingStrategy and not fold_fitting_strategy.is_mem_sufficient():
             # If memory is not sufficient, fall back to sequential fold strategy
-            fold_fitting_strategy: AbstractFoldFittingStrategy = SequentialLocalFoldFittingStrategy(**fold_fitting_strategy_args)
+            fold_fitting_strategy: FoldFittingStrategy = SequentialLocalFoldFittingStrategy(**fold_fitting_strategy_args)
             logger.log(30, f'\tMemory not enough to fit {model_base.__class__.__name__} folds in parallel. Will do sequential fitting instead. '
                            f'\tConsider decreasing folds trained in parallel by passing num_folds_parallel to ag_args_ensemble when calling predictor.fit')
 
         logger.log(20, f'\tFitting {len(fold_fit_args_list)} child models '
                        f'({fold_fit_args_list[0]["fold_ctx"]["model_name_suffix"]} - {fold_fit_args_list[-1]["fold_ctx"]["model_name_suffix"]}) | '
                        f'Fitting with {fold_fitting_strategy.__class__.__name__}')
 
@@ -565,15 +574,15 @@
                                cv_splitter,
                                k_fold_start,
                                k_fold_end,
                                n_repeat_start,
                                n_repeat_end) -> (list, int, int):
         """
         Generates fold configs given a cv_splitter, k_fold start-end and n_repeat start-end.
-        Fold configs are used by inheritors of AbstractFoldFittingStrategy when fitting fold models.
+        Fold configs are used by inheritors of FoldFittingStrategy when fitting fold models.
 
         Returns a list of fold configs, the number of started repeats, and the number of finished repeats.
         """
         k_fold = cv_splitter.n_splits
         kfolds = cv_splitter.split(X=X, y=y)
 
         fold_start = n_repeat_start * k_fold + k_fold_start
@@ -750,23 +759,38 @@
             self.save_child(child)
 
     def get_compiler_name(self) -> str:
         assert self.is_fit(), "The model must be fit before calling the get_compiler_name method."
         return self.load_child(self.models[0]).get_compiler_name()
 
     # TODO: Multiply epochs/n_iterations by some value (such as 1.1) to account for having more training data than bagged models
-    def convert_to_refit_full_template(self):
+    def convert_to_refit_full_template(self, name_suffix=REFIT_FULL_SUFFIX) -> AbstractModel:
+        """
+        After calling this function, returned model should be able to be fit without X_val, y_val using the iterations trained by the original model.
+
+        Parameters
+        ----------
+        name_suffix : str, default = '_FULL'
+            If name_suffix is not None, will append name_suffix to self.name when creating the template model's name.
+            Be careful of setting to None or empty string, as this will lead to the template overwriting self on disk when saved.
+
+        Returns
+        -------
+        model_full_template : AbstractModel
+            Unfit model capable of being fit without X_val, y_val. Hyperparameters are based on post-fit self hyperparameters.
+        """
         init_args = self.get_params()
         init_args['hyperparameters']['save_bag_folds'] = True  # refit full models must save folds
         init_args['model_base'] = self.convert_to_refit_full_template_child()
-        init_args['name'] = init_args['name'] + REFIT_FULL_SUFFIX
+        if name_suffix:
+            init_args['name'] = init_args['name'] + name_suffix
         model_full_template = self.__class__(**init_args)
         return model_full_template
 
-    def convert_to_refit_full_template_child(self):
+    def convert_to_refit_full_template_child(self) -> AbstractModel:
         refit_params_trained = self._get_compressed_params_trained()
         refit_params = copy.deepcopy(self._get_model_base().get_params())
         refit_params['hyperparameters'].update(refit_params_trained)
         refit_child_template = self._child_type(**refit_params)
 
         return refit_child_template
```

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,15 +618,15 @@
     ):
         fold, folds_finished, folds_left, \
             folds_to_fit, is_last_fold, \
             model_name_suffix = self._get_fold_properties(fold_ctx)
         logger.debug(f'Folding resources per job {resources}')
         train_index, val_index = fold
         fold_ctx_ref = self.ray.put(fold_ctx)
-        save_bag_folds = self.bagged_ensemble_model.params.get('save_bag_folds', True)
+        save_bag_folds = self.save_folds
         kwargs_fold = kwargs.copy()
         is_pseudo = X_pseudo_ref is not None and y_pseudo_ref is not None
         if self.sample_weight is not None:
             if is_pseudo:
                 # TODO: Add support for sample_weight when pseudo is present
                 raise Exception('Sample weights given, but not used due to pseudo labelled data being given.')
             else:
```

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/space.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1484,14 +1484,18 @@
                 if self._time_limit is not None and self._time_train_start is not None:
                     time_left_total = self._time_limit - (fit_start_time - self._time_train_start)
                 else:
                     time_left_total = time_limit
                 fit_log_message += f' Training model for up to {round(time_limit, 2)}s of the {round(time_left_total, 2)}s of remaining time.'
             logger.log(20, fit_log_message)
 
+            if isinstance(model, BaggedEnsembleModel) and not compute_score:
+                # Do not perform OOF predictions when we don't compute a score.
+                model_fit_kwargs['_skip_oof'] = True
+
             # If model is not bagged model and not stacked then pseudolabeled data needs to be incorporated at this level
             # Bagged model does validation on the fit level where as single models do it separately. Hence this if statement
             # is required
             if not isinstance(model, BaggedEnsembleModel) and X_pseudo is not None and y_pseudo is not None and X_pseudo.columns.equals(X.columns):
                 X_w_pseudo = pd.concat([X, X_pseudo])
                 y_w_pseudo = pd.concat([y, y_pseudo])
                 model_fit_kwargs.pop('X_pseudo')
```

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.0b20230418/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.0b20230417
+Version: 0.7.0b20230418
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.0b20230417/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.0b20230418/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

