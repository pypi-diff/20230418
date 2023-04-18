# Comparing `tmp/fedot_ind-0.0.0.3.tar.gz` & `tmp/fedot_ind-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot_ind-0.0.0.3.tar", last modified: Tue Apr 18 13:07:45 2023, max compression
+gzip compressed data, was "fedot_ind-0.0.0.4.tar", last modified: Tue Apr 18 13:29:50 2023, max compression
```

## Comparing `fedot_ind-0.0.0.3.tar` & `fedot_ind-0.0.0.4.tar`

### file list

```diff
@@ -1,228 +1,229 @@
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.075063 fedot_ind-0.0.0.3/
--rw-r--r--   0 technocreep   (501) staff       (20)     1538 2022-12-15 12:09:15.000000 fedot_ind-0.0.0.3/LICENSE.md
--rw-r--r--   0 technocreep   (501) staff       (20)      103 2023-04-18 12:59:24.000000 fedot_ind-0.0.0.3/MANIFEST.in
--rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:07:45.074519 fedot_ind-0.0.0.3/PKG-INFO
--rw-r--r--   0 technocreep   (501) staff       (20)    11792 2023-04-12 14:14:03.000000 fedot_ind-0.0.0.3/README.rst
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.006349 fedot_ind-0.0.0.3/docs/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/docs/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.006577 fedot_ind-0.0.0.3/fedot_ind/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.009510 fedot_ind-0.0.0.3/fedot_ind/api/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6483 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/api/main.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2103 2023-04-17 14:31:09.000000 fedot_ind-0.0.0.3/fedot_ind/api/main_example.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.012668 fedot_ind-0.0.0.3/fedot_ind/api/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4103 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/checkers_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)      170 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/decorator_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1118 2023-04-11 09:33:56.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/hp_generator_collection.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1575 2023-04-04 13:16:30.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/metafeatures.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6950 2023-04-17 16:02:07.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/reader_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1130 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/reporter.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1910 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/saver_collections.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.013083 fedot_ind-0.0.0.3/fedot_ind/core/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.013403 fedot_ind-0.0.0.3/fedot_ind/core/architecture/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.014293 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/
--rw-r--r--   0 technocreep   (501) staff       (20)     2137 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/Decorators.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.015586 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      980 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/classification_datasets.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2953 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/object_detection_datasets.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.018080 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/
--rw-r--r--   0 technocreep   (501) staff       (20)     1593 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/BenchmarkTests.py
--rw-r--r--   0 technocreep   (501) staff       (20)    24415 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/CVModule.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7612 2023-04-17 15:08:00.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12041 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.020725 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4925 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7239 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/anomaly_detection.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8900 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/classification.py
--rw-r--r--   0 technocreep   (501) staff       (20)       29 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/computer_vision.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.022896 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/
--rw-r--r--   0 technocreep   (501) staff       (20)     3496 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/Analyzer.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7602 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/results_picker.py
--rw-r--r--   0 technocreep   (501) staff       (20)    32241 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/ucr_datasets.json
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.023811 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      983 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.025903 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/
--rw-r--r--   0 technocreep   (501) staff       (20)     9997 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/DatasetLoader.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2054 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2267 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/InputData.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.028283 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1784 2023-04-05 13:01:09.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/hyperparams.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3599 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/pipeline_factory.py
--rw-r--r--   0 technocreep   (501) staff       (20)      781 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/task_factory.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2885 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.029563 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)     1027 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/Testing.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      250 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/utils.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.030465 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/
--rw-r--r--   0 technocreep   (501) staff       (20)     2216 2023-04-06 14:35:18.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/BaseEnsembler.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.031185 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6258 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/kernel_ensemble.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.032123 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/
--rw-r--r--   0 technocreep   (501) staff       (20)    12592 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/RankEnsembler.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.032812 fedot_ind-0.0.0.3/fedot_ind/core/metrics/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.034782 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1200 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/basis_loss.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4303 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/soft_dtw.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2560 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/svd_loss.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4920 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/metrics_implementation.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.036547 fedot_ind-0.0.0.3/fedot_ind/core/models/
--rw-r--r--   0 technocreep   (501) staff       (20)     3734 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/BaseExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2442 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/EnsembleExtractor.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.036911 fedot_ind-0.0.0.3/fedot_ind/core/models/TSAnomalyDetector/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-11-15 14:20:59.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/TSAnomalyDetector/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.038654 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1818 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/classification_models.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4815 2023-04-04 16:16:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/decomposed_conv.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8080 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/sfp_models.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.039213 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.040760 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/
--rw-r--r--   0 technocreep   (501) staff       (20)      680 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3521 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8193 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/FileObject.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.041539 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/
--rw-r--r--   0 technocreep   (501) staff       (20)     7413 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.043985 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    18879 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/kalman.py
--rw-r--r--   0 technocreep   (501) staff       (20)    17411 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/sigma.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.045570 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7969 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/func_pca.py
--rw-r--r--   0 technocreep   (501) staff       (20)    11329 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/sst.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.046861 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      274 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/get_time.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7050 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/math_utils.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.047617 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/
--rw-r--r--   0 technocreep   (501) staff       (20)     5055 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/AngleBasedDetector.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.049051 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/
--rw-r--r--   0 technocreep   (501) staff       (20)     8578 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/ErrorRunner.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5714 2023-04-04 13:40:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/error_correction.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5397 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/static_booster.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.050217 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12206 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/inception.py
--rw-r--r--   0 technocreep   (501) staff       (20)      615 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/modules.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.052104 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/
--rw-r--r--   0 technocreep   (501) staff       (20)     3758 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/RecurrenceExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5643 2023-04-17 14:27:21.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/SignalExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)      956 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.052911 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/
--rw-r--r--   0 technocreep   (501) staff       (20)    12405 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/SSAExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.053765 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/
--rw-r--r--   0 technocreep   (501) staff       (20)     3671 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/StatsExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.054359 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/
--rw-r--r--   0 technocreep   (501) staff       (20)     4878 2023-04-17 14:17:48.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/TopologicalExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.054883 fedot_ind-0.0.0.3/fedot_ind/core/operation/
--rw-r--r--   0 technocreep   (501) staff       (20)     2151 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/IndustrialCachableOperation.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.055662 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/
--rw-r--r--   0 technocreep   (501) staff       (20)     5974 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.056252 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/
--rw-r--r--   0 technocreep   (501) staff       (20)     3996 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.056841 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      549 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/dummy_operation.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.057409 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      512 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/quantile_filtration.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.057992 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2561 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.059865 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.060559 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/
--rw-r--r--   0 technocreep   (501) staff       (20)     3615 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2732 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/FeatureSpace.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7772 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/ModelStructure.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8581 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/sfp_tools.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3535 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/svd_tools.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.061857 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/
--rw-r--r--   0 technocreep   (501) staff       (20)     9911 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/DataTransformer.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2912 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py
--rw-r--r--   0 technocreep   (501) staff       (20)    13768 2023-04-05 16:47:37.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/WindowSelection.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.064788 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2620 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/abstract_basis.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4741 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3013 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/chebyshev.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5649 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/data_driven.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2044 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/fourier.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2931 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/legendre.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1264 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/power.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2938 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/wavelet.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.065895 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3065 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/eigen.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3399 2023-04-06 15:26:37.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/hankel.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.067359 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    10503 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/sequences.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5276 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/statistical.py
--rw-r--r--   0 technocreep   (501) staff       (20)    10224 2023-04-17 14:18:26.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/topological.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.068386 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5223 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/lp_reg.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2712 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/spectrum.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.069795 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      832 2022-10-19 15:44:11.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/alt_booster.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3180 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/cache.py
--rw-r--r--   0 technocreep   (501) staff       (20)    28639 2022-11-11 14:23:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/ts_reader.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.070452 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/
--rw-r--r--   0 technocreep   (501) staff       (20)     1893 2023-04-17 14:51:42.000000 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.071577 fedot_ind-0.0.0.3/fedot_ind/core/repository/
--rw-r--r--   0 technocreep   (501) staff       (20)     1072 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialDispatcher.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1861 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialOperationParameters.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.072876 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-18 12:47:03.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    14574 2023-04-04 16:07:26.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/data_operation_repository.json
--rw-r--r--   0 technocreep   (501) staff       (20)     3058 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/default_operation_params.json
--rw-r--r--   0 technocreep   (501) staff       (20)     1932 2023-04-17 14:44:27.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/industrial_data_operation_repository.json
--rw-r--r--   0 technocreep   (501) staff       (20)     6337 2023-04-17 14:42:19.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/initializer_industrial_models.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.073794 fedot_ind-0.0.0.3/fedot_ind/core/tuning/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/tuning/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12575 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/tuning/search_space.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.008220 fedot_ind-0.0.0.3/fedot_ind.egg-info/
--rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/PKG-INFO
--rw-r--r--   0 technocreep   (501) staff       (20)     8428 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/SOURCES.txt
--rw-r--r--   0 technocreep   (501) staff       (20)        1 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/dependency_links.txt
--rw-r--r--   0 technocreep   (501) staff       (20)      442 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/requires.txt
--rw-r--r--   0 technocreep   (501) staff       (20)       15 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/top_level.txt
--rw-r--r--   0 technocreep   (501) staff       (20)       38 2023-04-18 13:07:45.075209 fedot_ind-0.0.0.3/setup.cfg
--rw-r--r--   0 technocreep   (501) staff       (20)     1929 2023-04-18 13:07:40.000000 fedot_ind-0.0.0.3/setup.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.469271 fedot_ind-0.0.0.4/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1538 2022-12-15 12:09:15.000000 fedot_ind-0.0.0.4/LICENSE.md
+-rw-r--r--   0 technocreep   (501) staff       (20)       93 2023-04-18 13:18:51.000000 fedot_ind-0.0.0.4/MANIFEST.in
+-rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:29:50.468689 fedot_ind-0.0.0.4/PKG-INFO
+-rw-r--r--   0 technocreep   (501) staff       (20)    11792 2023-04-12 14:14:03.000000 fedot_ind-0.0.0.4/README.rst
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.361895 fedot_ind-0.0.0.4/docs/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/docs/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.362305 fedot_ind-0.0.0.4/fedot_ind/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.366159 fedot_ind-0.0.0.4/fedot_ind/api/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/api/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6483 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/api/main.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2103 2023-04-17 14:31:09.000000 fedot_ind-0.0.0.4/fedot_ind/api/main_example.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.371438 fedot_ind-0.0.0.4/fedot_ind/api/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4103 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/checkers_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      170 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/decorator_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1118 2023-04-11 09:33:56.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/hp_generator_collection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1575 2023-04-04 13:16:30.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/metafeatures.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6950 2023-04-17 16:02:07.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/reader_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1130 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/reporter.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1910 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/api/utils/saver_collections.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.372201 fedot_ind-0.0.0.4/fedot_ind/core/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.372595 fedot_ind-0.0.0.4/fedot_ind/core/architecture/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.373944 fedot_ind-0.0.0.4/fedot_ind/core/architecture/abstraction/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2137 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/abstraction/Decorators.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/abstraction/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.375609 fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      980 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/classification_datasets.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2953 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/object_detection_datasets.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.379772 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1593 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/BenchmarkTests.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    24415 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/CVModule.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7612 2023-04-17 15:08:00.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12041 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.382830 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4925 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7239 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/anomaly_detection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8900 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/classification.py
+-rw-r--r--   0 technocreep   (501) staff       (20)       29 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/computer_vision.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.386125 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/
+-rw-r--r--   0 technocreep   (501) staff       (20)     6148 2023-04-18 13:19:25.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/.DS_Store
+-rw-r--r--   0 technocreep   (501) staff       (20)     3496 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/Analyzer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7602 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/results_picker.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    32241 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/ucr_datasets.json
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.387462 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/visualisation/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      983 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.390472 fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/
+-rw-r--r--   0 technocreep   (501) staff       (20)     9997 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/DatasetLoader.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2054 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2267 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/InputData.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.393472 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1784 2023-04-05 13:01:09.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/hyperparams.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3599 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/pipeline_factory.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      781 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/task_factory.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2885 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.395195 fedot_ind-0.0.0.4/fedot_ind/core/architecture/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1027 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/utils/Testing.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      250 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/architecture/utils/utils.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.396613 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2216 2023-04-06 14:35:18.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/BaseEnsembler.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.397499 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/baseline/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/baseline/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6258 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/baseline/kernel_ensemble.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.398962 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/static/
+-rw-r--r--   0 technocreep   (501) staff       (20)    12592 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/static/RankEnsembler.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/ensemble/static/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.399749 fedot_ind-0.0.0.4/fedot_ind/core/metrics/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.401966 fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1200 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/basis_loss.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4303 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/soft_dtw.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2560 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/svd_loss.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4920 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/metrics/metrics_implementation.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.404053 fedot_ind-0.0.0.4/fedot_ind/core/models/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3734 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/BaseExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2442 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/EnsembleExtractor.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.404448 fedot_ind-0.0.0.4/fedot_ind/core/models/TSAnomalyDetector/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-11-15 14:20:59.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/TSAnomalyDetector/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.406706 fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1818 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/classification_models.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4815 2023-04-04 16:16:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/decomposed_conv.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8080 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/sfp_models.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.407415 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.410193 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/
+-rw-r--r--   0 technocreep   (501) staff       (20)      680 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3521 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8193 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/FileObject.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.411285 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/area/
+-rw-r--r--   0 technocreep   (501) staff       (20)     7413 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/area/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.412906 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    18879 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/kalman.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    17411 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/sigma.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.415202 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7969 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/func_pca.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    11329 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/sst.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.416793 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      274 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/utils/get_time.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7050 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/utils/math_utils.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.418234 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/vector/
+-rw-r--r--   0 technocreep   (501) staff       (20)     5055 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/vector/AngleBasedDetector.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/detection/vector/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.420661 fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/
+-rw-r--r--   0 technocreep   (501) staff       (20)     8578 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/ErrorRunner.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5714 2023-04-04 13:40:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/error_correction.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5397 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/static_booster.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.422544 fedot_ind-0.0.0.4/fedot_ind/core/models/nn/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/nn/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12206 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/nn/inception.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      615 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/nn/modules.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.425447 fedot_ind-0.0.0.4/fedot_ind/core/models/signal/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3758 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/signal/RecurrenceExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5643 2023-04-17 14:27:21.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/signal/SignalExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      956 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/signal/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.426607 fedot_ind-0.0.0.4/fedot_ind/core/models/spectral/
+-rw-r--r--   0 technocreep   (501) staff       (20)    12405 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/spectral/SSAExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/spectral/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.427729 fedot_ind-0.0.0.4/fedot_ind/core/models/statistical/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3671 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/statistical/StatsExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/statistical/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.428770 fedot_ind-0.0.0.4/fedot_ind/core/models/topological/
+-rw-r--r--   0 technocreep   (501) staff       (20)     4878 2023-04-17 14:17:48.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/topological/TopologicalExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/models/topological/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.429851 fedot_ind-0.0.0.4/fedot_ind/core/operation/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2151 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/IndustrialCachableOperation.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.431016 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/
+-rw-r--r--   0 technocreep   (501) staff       (20)     5974 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.432167 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/matrix_decomposition/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3996 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.432962 fedot_ind-0.0.0.4/fedot_ind/core/operation/dummy/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/dummy/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      549 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/dummy/dummy_operation.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.434066 fedot_ind-0.0.0.4/fedot_ind/core/operation/filtration/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/filtration/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      512 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/filtration/quantile_filtration.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.435211 fedot_ind-0.0.0.4/fedot_ind/core/operation/interfaces/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/interfaces/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2561 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.438666 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.440350 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/DMD/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3615 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/DMD/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2732 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/FeatureSpace.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7772 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/ModelStructure.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8581 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/sfp_tools.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3535 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/svd_tools.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.443738 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/
+-rw-r--r--   0 technocreep   (501) staff       (20)     9911 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/DataTransformer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2912 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    13768 2023-04-05 16:47:37.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/WindowSelection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.449860 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2620 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/abstract_basis.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4741 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3013 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/chebyshev.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5649 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/data_driven.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2044 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/fourier.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2931 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/legendre.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1264 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/power.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2938 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/wavelet.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.451765 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3065 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/eigen.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3399 2023-04-06 15:26:37.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/hankel.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.454603 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    10503 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/sequences.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5276 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/statistical.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    10224 2023-04-17 14:18:26.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/topological.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.456668 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5223 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/lp_reg.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2712 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/spectrum.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.459261 fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      832 2022-10-19 15:44:11.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/alt_booster.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3180 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/cache.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    28639 2022-11-11 14:23:34.000000 fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/ts_reader.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.461352 fedot_ind-0.0.0.4/fedot_ind/core/optimizer/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1893 2023-04-17 14:51:42.000000 fedot_ind-0.0.0.4/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/optimizer/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.463760 fedot_ind-0.0.0.4/fedot_ind/core/repository/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1072 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/IndustrialDispatcher.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1861 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/IndustrialOperationParameters.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.466541 fedot_ind-0.0.0.4/fedot_ind/core/repository/data/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-18 12:47:03.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/data/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    14574 2023-04-04 16:07:26.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/data/data_operation_repository.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     3058 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/data/default_operation_params.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     1932 2023-04-17 14:44:27.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/data/industrial_data_operation_repository.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     6337 2023-04-17 14:42:19.000000 fedot_ind-0.0.0.4/fedot_ind/core/repository/initializer_industrial_models.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.467686 fedot_ind-0.0.0.4/fedot_ind/core/tuning/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.4/fedot_ind/core/tuning/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12575 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.4/fedot_ind/core/tuning/search_space.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:29:50.364625 fedot_ind-0.0.0.4/fedot_ind.egg-info/
+-rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:29:50.000000 fedot_ind-0.0.0.4/fedot_ind.egg-info/PKG-INFO
+-rw-r--r--   0 technocreep   (501) staff       (20)     8481 2023-04-18 13:29:50.000000 fedot_ind-0.0.0.4/fedot_ind.egg-info/SOURCES.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)        1 2023-04-18 13:29:50.000000 fedot_ind-0.0.0.4/fedot_ind.egg-info/dependency_links.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)      442 2023-04-18 13:29:50.000000 fedot_ind-0.0.0.4/fedot_ind.egg-info/requires.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)       15 2023-04-18 13:29:50.000000 fedot_ind-0.0.0.4/fedot_ind.egg-info/top_level.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)       38 2023-04-18 13:29:50.469416 fedot_ind-0.0.0.4/setup.cfg
+-rw-r--r--   0 technocreep   (501) staff       (20)     1920 2023-04-18 13:29:20.000000 fedot_ind-0.0.0.4/setup.py
```

### Comparing `fedot_ind-0.0.0.3/LICENSE.md` & `fedot_ind-0.0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/PKG-INFO` & `fedot_ind-0.0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot_ind
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: Automated machine learning framework for time series analysis
 Home-page: https://github.com/aimclub/Fedot.Industrial
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Keywords: automated machine learning,time series analysis,anomaly detection,classification
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fedot_ind-0.0.0.3/README.rst` & `fedot_ind-0.0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/main.py` & `fedot_ind-0.0.0.4/fedot_ind/api/main.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/main_example.py` & `fedot_ind-0.0.0.4/fedot_ind/api/main_example.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/checkers_collections.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/checkers_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/hp_generator_collection.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/hp_generator_collection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/metafeatures.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/metafeatures.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/reader_collections.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/reader_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/reporter.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/reporter.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/api/utils/saver_collections.py` & `fedot_ind-0.0.0.4/fedot_ind/api/utils/saver_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/Decorators.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/abstraction/Decorators.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/classification_datasets.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/classification_datasets.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/object_detection_datasets.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/datasets/object_detection_datasets.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/BenchmarkTests.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/BenchmarkTests.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/CVModule.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/CVModule.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/abstract_pipeline.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/abstract_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/anomaly_detection.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/classification.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/pipelines/classification.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/Analyzer.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/Analyzer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/results_picker.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/results_picker.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/ucr_datasets.json` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/ucr_datasets.json`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/DatasetLoader.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/DatasetLoader.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/InputData.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/preprocessing/InputData.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/hyperparams.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/hyperparams.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/pipeline_factory.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/task_factory.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/task_factory.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/Testing.py` & `fedot_ind-0.0.0.4/fedot_ind/core/architecture/utils/Testing.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/BaseEnsembler.py` & `fedot_ind-0.0.0.4/fedot_ind/core/ensemble/BaseEnsembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/kernel_ensemble.py` & `fedot_ind-0.0.0.4/fedot_ind/core/ensemble/baseline/kernel_ensemble.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/RankEnsembler.py` & `fedot_ind-0.0.0.4/fedot_ind/core/ensemble/static/RankEnsembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/basis_loss.py` & `fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/basis_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/soft_dtw.py` & `fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/soft_dtw.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/svd_loss.py` & `fedot_ind-0.0.0.4/fedot_ind/core/metrics/loss/svd_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/metrics/metrics_implementation.py` & `fedot_ind-0.0.0.4/fedot_ind/core/metrics/metrics_implementation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/BaseExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/BaseExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/EnsembleExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/EnsembleExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/classification_models.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/classification_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/decomposed_conv.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/decomposed_conv.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/sfp_models.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/cnn/sfp_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/FileObject.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/abstract_objects/FileObject.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/kalman.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/kalman.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/sigma.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/probalistic/sigma.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/func_pca.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/func_pca.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/sst.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/subspaces/sst.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/math_utils.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/AngleBasedDetector.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/detection/vector/AngleBasedDetector.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/ErrorRunner.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/ErrorRunner.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/error_correction.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/error_correction.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/static_booster.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/ecm/static_booster.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/nn/inception.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/nn/inception.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/nn/modules.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/nn/modules.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/RecurrenceExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/signal/RecurrenceExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/SignalExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/signal/SignalExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/SSAExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/spectral/SSAExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/StatsExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/statistical/StatsExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/models/topological/TopologicalExtractor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/models/topological/TopologicalExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/IndustrialCachableOperation.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/IndustrialCachableOperation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/dummy_operation.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/dummy/dummy_operation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/quantile_filtration.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/filtration/quantile_filtration.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/FeatureSpace.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/FeatureSpace.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/ModelStructure.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/ModelStructure.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/sfp_tools.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/sfp_tools.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/svd_tools.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/optimization/svd_tools.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/DataTransformer.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/DataTransformer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/WindowSelection.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/WindowSelection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/abstract_basis.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/abstract_basis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/chebyshev.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/chebyshev.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/data_driven.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/data_driven.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/fourier.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/fourier.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/legendre.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/legendre.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/power.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/power.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/wavelet.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/basis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/eigen.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/eigen.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/hankel.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/data/hankel.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/sequences.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/sequences.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/statistical.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/statistical.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/topological.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/extraction/topological.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/lp_reg.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/lp_reg.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/spectrum.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/transformation/regularization/spectrum.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/alt_booster.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/alt_booster.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/cache.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/cache.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/ts_reader.py` & `fedot_ind-0.0.0.4/fedot_ind/core/operation/utils/ts_reader.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py` & `fedot_ind-0.0.0.4/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialDispatcher.py` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/IndustrialDispatcher.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialOperationParameters.py` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/IndustrialOperationParameters.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/data/data_operation_repository.json` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/data/data_operation_repository.json`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/data/default_operation_params.json` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/data/default_operation_params.json`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/data/industrial_data_operation_repository.json` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/data/industrial_data_operation_repository.json`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/repository/initializer_industrial_models.py` & `fedot_ind-0.0.0.4/fedot_ind/core/repository/initializer_industrial_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind/core/tuning/search_space.py` & `fedot_ind-0.0.0.4/fedot_ind/core/tuning/search_space.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.3/fedot_ind.egg-info/PKG-INFO` & `fedot_ind-0.0.0.4/fedot_ind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot-ind
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: Automated machine learning framework for time series analysis
 Home-page: https://github.com/aimclub/Fedot.Industrial
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Keywords: automated machine learning,time series analysis,anomaly detection,classification
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fedot_ind-0.0.0.3/fedot_ind.egg-info/SOURCES.txt` & `fedot_ind-0.0.0.4/fedot_ind.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py
 fedot_ind/core/architecture/experiment/__init__.py
 fedot_ind/core/architecture/pipelines/__init__.py
 fedot_ind/core/architecture/pipelines/abstract_pipeline.py
 fedot_ind/core/architecture/pipelines/anomaly_detection.py
 fedot_ind/core/architecture/pipelines/classification.py
 fedot_ind/core/architecture/pipelines/computer_vision.py
+fedot_ind/core/architecture/postprocessing/.DS_Store
 fedot_ind/core/architecture/postprocessing/Analyzer.py
 fedot_ind/core/architecture/postprocessing/__init__.py
 fedot_ind/core/architecture/postprocessing/results_picker.py
 fedot_ind/core/architecture/postprocessing/ucr_datasets.json
 fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
 fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
 fedot_ind/core/architecture/preprocessing/DatasetLoader.py
```

### Comparing `fedot_ind-0.0.0.3/setup.py` & `fedot_ind-0.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'fedot_ind'
-VERSION = '0.0.0.3'
+VERSION = '0.0.0.4'
 AUTHOR = 'NSS Lab'
 AUTHOR_EMAIL = 'itmo.nss.team@gmail.com'
 SHORT_DESCRIPTION = 'Automated machine learning framework for time series analysis'
 LONG_DESC_TYPE = 'text/x-rst'
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
-EXCLUDED_PACKAGES = ['test*', 'examples', 'cases', 'benchmark', '*.csv']
+EXCLUDED_PACKAGES = ['test*', 'examples', 'cases', 'benchmark']
 URL = 'https://github.com/aimclub/Fedot.Industrial'
 REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
 KEYWORDS = 'automated machine learning, time series analysis, anomaly detection, classification'
 
 
 def _readlines(*names: str, **kwargs) -> List[str]:
```

