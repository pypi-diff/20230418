# Comparing `tmp/clearner-0.9.78.tar.gz` & `tmp/clearner-0.9.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearner-0.9.78.tar", last modified: Fri Feb 24 23:03:57 2023, max compression
+gzip compressed data, was "dist/clearner-0.9.79.tar", last modified: Tue Apr 18 02:17:00 2023, max compression
```

## Comparing `clearner-0.9.78.tar` & `clearner-0.9.79.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.78/LICENSE
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-02-24 23:03:57.000000 clearner-0.9.78/PKG-INFO
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/PKG-INFO
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/SOURCES.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/dependency_links.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/entry_points.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/requires.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-02-24 23:03:57.000000 clearner-0.9.78/clearner.egg-info/top_level.txt
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/__init__.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/analysis/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/analysis/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/analysis/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/analysis/plot.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25711 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/analysis/shap.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/api_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/api_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/api_worker/google_drive.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/callback_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/callback_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/callback_manager/callback.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/combine/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/combine/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/combine/combining_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/communication/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/communication/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/communication/communication_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/communication/email_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/configuration/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/configuration/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/column.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/combine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/communication.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/configuration.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/connection.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/data.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/defaults.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.78/learner/configuration/feature_engineering.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/model.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/configuration/outlier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/process.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/configuration/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/sample.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/segmenter.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/configuration/similarities.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8309 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/supported_items.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/configuration/validation.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/configuration/workspace.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/data_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/data_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.78/learner/data_worker/data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_mover.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    51763 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13030 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_sampler.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_segmenters.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/data_set.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/deep_tabular_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/image_data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/image_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/image_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/data_worker/output_handler.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/engines/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/engines/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/base_deep_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/base_standard_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/deep_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/deep_regressor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/engine_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/image_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/engines/standard_engines.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/feature_engineering/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/feature_engineering/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.78/learner/feature_engineering/feature_engineering.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/model_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/model_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/deep_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/deep_loop_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/deep_regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/extenders.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/image_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/layer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/loss_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/model_initializer.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/nn_utils.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/optimizer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/prediction_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/scheduler_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/model_manager/scorers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23624 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/model_manager/scoring_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2403 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/model_manager/similarities.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/outlier_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/outlier_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/outlier_manager/outlier_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/schema/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/schema/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/schema/credentials_schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/schema/logging.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/schema/meta_data.schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.78/learner/schema/schema.json
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/setup/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/setup/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/setup/logger.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.78/learner/setup/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/setup/parser.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/setup/setup.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/utilities/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/utilities/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/utilities/exclude.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3923 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/utilities/progress_bar.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/utilities/smtp.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/utilities/templates.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/utilities/timer.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-02-24 23:03:57.000000 clearner-0.9.78/learner/validator/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/validator/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/validator/column_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.78/learner/validator/data_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/validator/input_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/validator/model_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.78/learner/validator/output_validator.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.78/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2022-10-04 17:17:40.000000 clearner-0.9.78/requirements.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-02-24 23:03:57.000000 clearner-0.9.78/setup.cfg
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1768 2023-02-24 23:02:37.000000 clearner-0.9.78/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.79/LICENSE
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-04-18 02:17:00.000000 clearner-0.9.79/PKG-INFO
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/PKG-INFO
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/entry_points.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/requires.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-04-18 02:16:59.000000 clearner-0.9.79/clearner.egg-info/top_level.txt
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:16:59.000000 clearner-0.9.79/learner/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/__init__.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:16:59.000000 clearner-0.9.79/learner/analysis/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/analysis/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/analysis/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/analysis/plot.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25711 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/analysis/shap.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:16:59.000000 clearner-0.9.79/learner/api_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/api_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/api_worker/google_drive.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:16:59.000000 clearner-0.9.79/learner/callback_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/callback_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/callback_manager/callback.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/combine/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/combine/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/combine/combining_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/communication/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/communication/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/communication/communication_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/communication/email_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/configuration/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/configuration/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/column.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/combine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/communication.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/configuration.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/connection.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/data.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/defaults.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.79/learner/configuration/feature_engineering.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/model.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/configuration/outlier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/process.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/configuration/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/sample.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/segmenter.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/configuration/similarities.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8309 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/supported_items.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/configuration/validation.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/configuration/workspace.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/data_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/data_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.79/learner/data_worker/data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/data_mover.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 01:53:21.000000 clearner-0.9.79/learner/data_worker/data_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13030 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/data_sampler.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/data_segmenters.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/data_set.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/deep_tabular_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/image_data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/image_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/image_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/data_worker/output_handler.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/engines/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/engines/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/base_deep_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/base_standard_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/deep_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/deep_regressor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/engine_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/image_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/engines/standard_engines.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/feature_engineering/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/feature_engineering/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.79/learner/feature_engineering/feature_engineering.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/model_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/model_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/deep_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/deep_loop_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/deep_regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/extenders.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/image_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/layer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/loss_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/model_initializer.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/nn_utils.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/optimizer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/prediction_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/scheduler_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/model_manager/scorers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23624 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/model_manager/scoring_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2403 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/model_manager/similarities.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/outlier_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/outlier_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/outlier_manager/outlier_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/schema/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/schema/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/schema/credentials_schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/schema/logging.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/schema/meta_data.schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.79/learner/schema/schema.json
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/setup/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/setup/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/setup/logger.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.79/learner/setup/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/setup/parser.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/setup/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/utilities/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/utilities/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/utilities/exclude.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3923 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/utilities/progress_bar.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/utilities/smtp.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/utilities/templates.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/utilities/timer.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-04-18 02:17:00.000000 clearner-0.9.79/learner/validator/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/validator/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/validator/column_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.79/learner/validator/data_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/validator/input_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/validator/model_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.79/learner/validator/output_validator.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.79/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2022-10-04 17:17:40.000000 clearner-0.9.79/requirements.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-04-18 02:17:00.000000 clearner-0.9.79/setup.cfg
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1830 2023-04-18 02:16:50.000000 clearner-0.9.79/setup.py
```

### Comparing `clearner-0.9.78/LICENSE` & `clearner-0.9.79/LICENSE`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/clearner.egg-info/SOURCES.txt` & `clearner-0.9.79/clearner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/clearner.egg-info/requires.txt` & `clearner-0.9.79/clearner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/analysis/analysis.py` & `clearner-0.9.79/learner/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/analysis/plot.py` & `clearner-0.9.79/learner/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/analysis/shap.py` & `clearner-0.9.79/learner/analysis/shap.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/api_worker/google_drive.py` & `clearner-0.9.79/learner/api_worker/google_drive.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/callback_manager/callback.py` & `clearner-0.9.79/learner/callback_manager/callback.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/combine/combining_manager.py` & `clearner-0.9.79/learner/combine/combining_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/communication/communication_manager.py` & `clearner-0.9.79/learner/communication/communication_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/communication/email_manager.py` & `clearner-0.9.79/learner/communication/email_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/analysis.py` & `clearner-0.9.79/learner/configuration/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/column.py` & `clearner-0.9.79/learner/configuration/column.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/combine.py` & `clearner-0.9.79/learner/configuration/combine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/communication.py` & `clearner-0.9.79/learner/configuration/communication.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/configuration.py` & `clearner-0.9.79/learner/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/connection.py` & `clearner-0.9.79/learner/configuration/connection.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/data.py` & `clearner-0.9.79/learner/configuration/data.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/defaults.py` & `clearner-0.9.79/learner/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/feature_engineering.py` & `clearner-0.9.79/learner/configuration/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/model.py` & `clearner-0.9.79/learner/configuration/model.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/outlier.py` & `clearner-0.9.79/learner/configuration/outlier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/process.py` & `clearner-0.9.79/learner/configuration/process.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/recommender.py` & `clearner-0.9.79/learner/configuration/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/sample.py` & `clearner-0.9.79/learner/configuration/sample.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/segmenter.py` & `clearner-0.9.79/learner/configuration/segmenter.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/similarities.py` & `clearner-0.9.79/learner/configuration/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/supported_items.py` & `clearner-0.9.79/learner/configuration/supported_items.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/validation.py` & `clearner-0.9.79/learner/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/configuration/workspace.py` & `clearner-0.9.79/learner/configuration/workspace.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_loader.py` & `clearner-0.9.79/learner/data_worker/data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_manager.py` & `clearner-0.9.79/learner/data_worker/data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_mover.py` & `clearner-0.9.79/learner/data_worker/data_mover.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_processor.py` & `clearner-0.9.79/learner/data_worker/data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1078,16 +1078,23 @@
     from them to create the new columns.
 
     :param data: pandas dataframe
     :param cols: the date columns to be processed
     :return: the updated dataframe with the new columns
     """
     for col, date_items in cols.items():
-        data[col] = pd.to_datetime(data[col],
-                                   errors='coerce',
-                                   infer_datetime_format=True)
+        try:
+            data[col] = pd.to_datetime(data[col],
+                                       errors='coerce',
+                                       infer_datetime_format=True)
+        # if we have Tz-aware datetime.datetime, we'll get value error. In that case, we set utc to true
+        except ValueError:
+            data[col] = pd.to_datetime(data[col],
+                                       errors='coerce',
+                                       infer_datetime_format=True,
+                                       utc=True)
         for item in date_items:
             data.loc[:, f"{col}_{item}"] = getattr(data[col].dt, item)
 
     return data
```

### Comparing `clearner-0.9.78/learner/data_worker/data_sampler.py` & `clearner-0.9.79/learner/data_worker/data_sampler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_segmenters.py` & `clearner-0.9.79/learner/data_worker/data_segmenters.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/data_set.py` & `clearner-0.9.79/learner/data_worker/data_set.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/deep_tabular_data_manager.py` & `clearner-0.9.79/learner/data_worker/deep_tabular_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/image_data_loader.py` & `clearner-0.9.79/learner/data_worker/image_data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/image_data_manager.py` & `clearner-0.9.79/learner/data_worker/image_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/image_processor.py` & `clearner-0.9.79/learner/data_worker/image_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/data_worker/output_handler.py` & `clearner-0.9.79/learner/data_worker/output_handler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/base_deep_engine.py` & `clearner-0.9.79/learner/engines/base_deep_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/base_standard_engine.py` & `clearner-0.9.79/learner/engines/base_standard_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/deep_classifier.py` & `clearner-0.9.79/learner/engines/deep_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/deep_regressor.py` & `clearner-0.9.79/learner/engines/deep_regressor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/engine_manager.py` & `clearner-0.9.79/learner/engines/engine_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/image_classifier.py` & `clearner-0.9.79/learner/engines/image_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/recommender.py` & `clearner-0.9.79/learner/engines/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/engines/standard_engines.py` & `clearner-0.9.79/learner/engines/standard_engines.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/feature_engineering/feature_engineering.py` & `clearner-0.9.79/learner/feature_engineering/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/classifiers.py` & `clearner-0.9.79/learner/model_manager/classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/deep_classifiers.py` & `clearner-0.9.79/learner/model_manager/deep_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/deep_loop_manager.py` & `clearner-0.9.79/learner/model_manager/deep_loop_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/deep_regressors.py` & `clearner-0.9.79/learner/model_manager/deep_regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/extenders.py` & `clearner-0.9.79/learner/model_manager/extenders.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/image_classifiers.py` & `clearner-0.9.79/learner/model_manager/image_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/layer_manager.py` & `clearner-0.9.79/learner/model_manager/layer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/loss_manager.py` & `clearner-0.9.79/learner/model_manager/loss_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/model_initializer.py` & `clearner-0.9.79/learner/model_manager/model_initializer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/nn_utils.py` & `clearner-0.9.79/learner/model_manager/nn_utils.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/optimizer_manager.py` & `clearner-0.9.79/learner/model_manager/optimizer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/prediction_manager.py` & `clearner-0.9.79/learner/model_manager/prediction_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/regressors.py` & `clearner-0.9.79/learner/model_manager/regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/scheduler_manager.py` & `clearner-0.9.79/learner/model_manager/scheduler_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/scorers.py` & `clearner-0.9.79/learner/model_manager/scorers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/scoring_manager.py` & `clearner-0.9.79/learner/model_manager/scoring_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/model_manager/similarities.py` & `clearner-0.9.79/learner/model_manager/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/outlier_manager/outlier_manager.py` & `clearner-0.9.79/learner/outlier_manager/outlier_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/schema/logging.json` & `clearner-0.9.79/learner/schema/logging.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/schema/schema.json` & `clearner-0.9.79/learner/schema/schema.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/setup/logger.py` & `clearner-0.9.79/learner/setup/logger.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/setup/main.py` & `clearner-0.9.79/learner/setup/main.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/setup/parser.py` & `clearner-0.9.79/learner/setup/parser.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/setup/setup.py` & `clearner-0.9.79/learner/setup/setup.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/utilities/exclude.py` & `clearner-0.9.79/learner/utilities/exclude.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/utilities/progress_bar.py` & `clearner-0.9.79/learner/utilities/progress_bar.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/utilities/smtp.py` & `clearner-0.9.79/learner/utilities/smtp.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/utilities/templates.py` & `clearner-0.9.79/learner/utilities/templates.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/utilities/timer.py` & `clearner-0.9.79/learner/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/validator/column_validator.py` & `clearner-0.9.79/learner/validator/column_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/validator/data_validator.py` & `clearner-0.9.79/learner/validator/data_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/validator/input_validator.py` & `clearner-0.9.79/learner/validator/input_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/validator/model_validator.py` & `clearner-0.9.79/learner/validator/model_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/learner/validator/output_validator.py` & `clearner-0.9.79/learner/validator/output_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/requirements.txt` & `clearner-0.9.79/requirements.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.78/setup.py` & `clearner-0.9.79/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #! /usr/bin/env python
 import os
 from setuptools import setup, find_packages
 
 # to run the module do the following command:
 # python setup.py sdist
 
+# To upload to twine:
+# twine upload dist/<the .tar.gz file>
+
 
 def get_dependencies():
     """This function reads the requirements.txt file and creates a list of packages to be installed before Learner can
     be installed. In practice, we should be defining a separate dependencies in the setup because the requirements file
     is too restrictive but this is fine for now. As long as the users use docker containers or virtual environments,
     this should't cause any issues.
 
@@ -22,15 +25,15 @@
 def compile_learner():
     """Go through each package and modules, and compile them.
 
     :return: None
     """
     setup(
         name='clearner',
-        version='0.9.78',
+        version='0.9.79',
         description="Learner is a software platform for building production-ready machine learning models without writing any codes.",
         author="Prizmi LLC",
         author_email="contact@prizmi.ai",
         python_requires='>=3.7,<3.8',
         url="https://prizmi.ai/learner/home",
         license="Other",
         build_dir="build",
```

