# Comparing `tmp/fedot_ind-0.0.0.2.tar.gz` & `tmp/fedot_ind-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot_ind-0.0.0.2.tar", last modified: Mon Apr 17 16:13:59 2023, max compression
+gzip compressed data, was "fedot_ind-0.0.0.3.tar", last modified: Tue Apr 18 13:07:45 2023, max compression
```

## Comparing `fedot_ind-0.0.0.2.tar` & `fedot_ind-0.0.0.3.tar`

### file list

```diff
@@ -1,222 +1,228 @@
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.391926 fedot_ind-0.0.0.2/
--rw-r--r--   0 technocreep   (501) staff       (20)     1538 2022-12-15 12:09:15.000000 fedot_ind-0.0.0.2/LICENSE.md
--rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-17 16:13:59.391521 fedot_ind-0.0.0.2/PKG-INFO
--rw-r--r--   0 technocreep   (501) staff       (20)    11792 2023-04-12 14:14:03.000000 fedot_ind-0.0.0.2/README.rst
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.334892 fedot_ind-0.0.0.2/docs/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/docs/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.335229 fedot_ind-0.0.0.2/fedot_ind/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.337861 fedot_ind-0.0.0.2/fedot_ind/api/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/api/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6483 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/api/main.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2103 2023-04-17 14:31:09.000000 fedot_ind-0.0.0.2/fedot_ind/api/main_example.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.341000 fedot_ind-0.0.0.2/fedot_ind/api/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4103 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/checkers_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)      170 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/decorator_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1118 2023-04-11 09:33:56.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/hp_generator_collection.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1575 2023-04-04 13:16:30.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/metafeatures.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-06 15:26:37.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/method_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6950 2023-04-17 16:02:07.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/reader_collections.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1130 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/reporter.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1910 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/api/utils/saver_collections.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.341295 fedot_ind-0.0.0.2/fedot_ind/core/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.341508 fedot_ind-0.0.0.2/fedot_ind/core/architecture/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.342052 fedot_ind-0.0.0.2/fedot_ind/core/architecture/abstraction/
--rw-r--r--   0 technocreep   (501) staff       (20)     2137 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/abstraction/Decorators.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/abstraction/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.342760 fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      980 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/classification_datasets.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2953 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/object_detection_datasets.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.345040 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/
--rw-r--r--   0 technocreep   (501) staff       (20)     1593 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/BenchmarkTests.py
--rw-r--r--   0 technocreep   (501) staff       (20)    24415 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/CVModule.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7612 2023-04-17 15:08:00.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12041 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.347005 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4925 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7239 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8900 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/classification.py
--rw-r--r--   0 technocreep   (501) staff       (20)       29 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/computer_vision.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.348130 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/
--rw-r--r--   0 technocreep   (501) staff       (20)     3496 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/Analyzer.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7559 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/results_picker.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.348788 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/visualisation/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      983 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.350321 fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/
--rw-r--r--   0 technocreep   (501) staff       (20)     9997 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/DatasetLoader.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2054 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2267 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/InputData.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.351978 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1784 2023-04-05 13:01:09.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/hyperparams.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3598 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/pipeline_factory.py
--rw-r--r--   0 technocreep   (501) staff       (20)      781 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/task_factory.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2885 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.352974 fedot_ind-0.0.0.2/fedot_ind/core/architecture/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)     1027 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/utils/Testing.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      250 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/architecture/utils/utils.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.353737 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/
--rw-r--r--   0 technocreep   (501) staff       (20)     2216 2023-04-06 14:35:18.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/BaseEnsembler.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.354178 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/baseline/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/baseline/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6232 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/baseline/kernel_ensemble.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.354939 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/static/
--rw-r--r--   0 technocreep   (501) staff       (20)    12592 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/static/RankEnsembler.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/ensemble/static/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.355380 fedot_ind-0.0.0.2/fedot_ind/core/metrics/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.356643 fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1200 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/basis_loss.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4303 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/soft_dtw.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2560 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/svd_loss.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4920 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/metrics/metrics_implementation.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.357645 fedot_ind-0.0.0.2/fedot_ind/core/models/
--rw-r--r--   0 technocreep   (501) staff       (20)     3734 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/BaseExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2442 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/EnsembleExtractor.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.357888 fedot_ind-0.0.0.2/fedot_ind/core/models/TSAnomalyDetector/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-11-15 14:20:59.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/TSAnomalyDetector/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.359065 fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1818 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/classification_models.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4815 2023-04-04 16:16:22.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/decomposed_conv.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8080 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/sfp_models.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.359475 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.360644 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/
--rw-r--r--   0 technocreep   (501) staff       (20)      680 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3523 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8191 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/FileObject.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.361517 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/area/
--rw-r--r--   0 technocreep   (501) staff       (20)     7413 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/area/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.362743 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    18877 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/kalman.py
--rw-r--r--   0 technocreep   (501) staff       (20)    17420 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/sigma.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.363705 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7968 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/func_pca.py
--rw-r--r--   0 technocreep   (501) staff       (20)    11329 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/sst.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.364723 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      274 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/utils/get_time.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7055 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/utils/math_utils.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.365420 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/vector/
--rw-r--r--   0 technocreep   (501) staff       (20)     5062 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/vector/AngleBasedDetector.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/detection/vector/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.366770 fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/
--rw-r--r--   0 technocreep   (501) staff       (20)     8578 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/ErrorRunner.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5714 2023-04-04 13:40:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/error_correction.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5427 2023-03-22 10:47:48.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/static_booster.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.368005 fedot_ind-0.0.0.2/fedot_ind/core/models/nn/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/nn/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12206 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/nn/inception.py
--rw-r--r--   0 technocreep   (501) staff       (20)      615 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/nn/modules.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.369340 fedot_ind-0.0.0.2/fedot_ind/core/models/signal/
--rw-r--r--   0 technocreep   (501) staff       (20)     3758 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/signal/RecurrenceExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5643 2023-04-17 14:27:21.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/signal/SignalExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)      956 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/signal/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.370080 fedot_ind-0.0.0.2/fedot_ind/core/models/spectral/
--rw-r--r--   0 technocreep   (501) staff       (20)    12405 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/spectral/SSAExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/spectral/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.370878 fedot_ind-0.0.0.2/fedot_ind/core/models/statistical/
--rw-r--r--   0 technocreep   (501) staff       (20)     3671 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/statistical/StatsExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/statistical/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.371720 fedot_ind-0.0.0.2/fedot_ind/core/models/topological/
--rw-r--r--   0 technocreep   (501) staff       (20)     4878 2023-04-17 14:17:48.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/topological/TopologicalExtractor.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/models/topological/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.372637 fedot_ind-0.0.0.2/fedot_ind/core/operation/
--rw-r--r--   0 technocreep   (501) staff       (20)     2151 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/IndustrialCachableOperation.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.373505 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/
--rw-r--r--   0 technocreep   (501) staff       (20)     5974 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.374188 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/matrix_decomposition/
--rw-r--r--   0 technocreep   (501) staff       (20)     3996 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.374825 fedot_ind-0.0.0.2/fedot_ind/core/operation/dummy/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/dummy/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      549 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/dummy/dummy_operation.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.375445 fedot_ind-0.0.0.2/fedot_ind/core/operation/filtration/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/filtration/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      512 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/filtration/quantile_filtration.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.376089 fedot_ind-0.0.0.2/fedot_ind/core/operation/interfaces/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/interfaces/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2561 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.377617 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.378275 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/DMD/
--rw-r--r--   0 technocreep   (501) staff       (20)     3523 2023-04-17 12:29:35.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/DMD/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2732 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/FeatureSpace.py
--rw-r--r--   0 technocreep   (501) staff       (20)     7772 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/ModelStructure.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     8581 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/sfp_tools.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3535 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/svd_tools.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.379949 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/
--rw-r--r--   0 technocreep   (501) staff       (20)     9911 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/DataTransformer.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2912 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py
--rw-r--r--   0 technocreep   (501) staff       (20)    13768 2023-04-05 16:47:37.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/WindowSelection.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.383705 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2620 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py
--rw-r--r--   0 technocreep   (501) staff       (20)     4732 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3013 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/chebyshev.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5649 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/data_driven.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2044 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/fourier.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2931 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/legendre.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1264 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/power.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2938 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/wavelet.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.384753 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3065 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/eigen.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3399 2023-04-06 15:26:37.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/hankel.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.386155 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    10503 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/sequences.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5276 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/statistical.py
--rw-r--r--   0 technocreep   (501) staff       (20)    10224 2023-04-17 14:18:26.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/topological.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.387190 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     5223 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/lp_reg.py
--rw-r--r--   0 technocreep   (501) staff       (20)     2712 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/spectrum.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.388469 fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)      832 2022-10-19 15:44:11.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/alt_booster.py
--rw-r--r--   0 technocreep   (501) staff       (20)     3180 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/cache.py
--rw-r--r--   0 technocreep   (501) staff       (20)    28639 2022-11-11 14:23:34.000000 fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/ts_reader.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.389094 fedot_ind-0.0.0.2/fedot_ind/core/optimizer/
--rw-r--r--   0 technocreep   (501) staff       (20)     1893 2023-04-17 14:51:42.000000 fedot_ind-0.0.0.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/optimizer/__init__.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.390217 fedot_ind-0.0.0.2/fedot_ind/core/repository/
--rw-r--r--   0 technocreep   (501) staff       (20)     1072 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.2/fedot_ind/core/repository/IndustrialDispatcher.py
--rw-r--r--   0 technocreep   (501) staff       (20)     1861 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/repository/IndustrialOperationParameters.py
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.2/fedot_ind/core/repository/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)     6337 2023-04-17 14:42:19.000000 fedot_ind-0.0.0.2/fedot_ind/core/repository/initializer_industrial_models.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.391002 fedot_ind-0.0.0.2/fedot_ind/core/tuning/
--rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.2/fedot_ind/core/tuning/__init__.py
--rw-r--r--   0 technocreep   (501) staff       (20)    12575 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.2/fedot_ind/core/tuning/search_space.py
-drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-17 16:13:59.336971 fedot_ind-0.0.0.2/fedot_ind.egg-info/
--rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-17 16:13:59.000000 fedot_ind-0.0.0.2/fedot_ind.egg-info/PKG-INFO
--rw-r--r--   0 technocreep   (501) staff       (20)     8158 2023-04-17 16:13:59.000000 fedot_ind-0.0.0.2/fedot_ind.egg-info/SOURCES.txt
--rw-r--r--   0 technocreep   (501) staff       (20)        1 2023-04-17 16:13:59.000000 fedot_ind-0.0.0.2/fedot_ind.egg-info/dependency_links.txt
--rw-r--r--   0 technocreep   (501) staff       (20)      442 2023-04-17 16:13:59.000000 fedot_ind-0.0.0.2/fedot_ind.egg-info/requires.txt
--rw-r--r--   0 technocreep   (501) staff       (20)       15 2023-04-17 16:13:59.000000 fedot_ind-0.0.0.2/fedot_ind.egg-info/top_level.txt
--rw-r--r--   0 technocreep   (501) staff       (20)       38 2023-04-17 16:13:59.392032 fedot_ind-0.0.0.2/setup.cfg
--rw-r--r--   0 technocreep   (501) staff       (20)     1845 2023-04-17 16:13:55.000000 fedot_ind-0.0.0.2/setup.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.075063 fedot_ind-0.0.0.3/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1538 2022-12-15 12:09:15.000000 fedot_ind-0.0.0.3/LICENSE.md
+-rw-r--r--   0 technocreep   (501) staff       (20)      103 2023-04-18 12:59:24.000000 fedot_ind-0.0.0.3/MANIFEST.in
+-rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:07:45.074519 fedot_ind-0.0.0.3/PKG-INFO
+-rw-r--r--   0 technocreep   (501) staff       (20)    11792 2023-04-12 14:14:03.000000 fedot_ind-0.0.0.3/README.rst
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.006349 fedot_ind-0.0.0.3/docs/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/docs/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.006577 fedot_ind-0.0.0.3/fedot_ind/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.009510 fedot_ind-0.0.0.3/fedot_ind/api/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6483 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/api/main.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2103 2023-04-17 14:31:09.000000 fedot_ind-0.0.0.3/fedot_ind/api/main_example.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.012668 fedot_ind-0.0.0.3/fedot_ind/api/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4103 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/checkers_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      170 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/decorator_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1118 2023-04-11 09:33:56.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/hp_generator_collection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1575 2023-04-04 13:16:30.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/metafeatures.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6950 2023-04-17 16:02:07.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/reader_collections.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1130 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/reporter.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1910 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/api/utils/saver_collections.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.013083 fedot_ind-0.0.0.3/fedot_ind/core/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.013403 fedot_ind-0.0.0.3/fedot_ind/core/architecture/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.014293 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2137 2023-04-04 13:43:51.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/Decorators.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.015586 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      980 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/classification_datasets.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2953 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/object_detection_datasets.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.018080 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1593 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/BenchmarkTests.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    24415 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/CVModule.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7612 2023-04-17 15:08:00.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12041 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.020725 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4925 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7239 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/anomaly_detection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8900 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/classification.py
+-rw-r--r--   0 technocreep   (501) staff       (20)       29 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/computer_vision.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.022896 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3496 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/Analyzer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7602 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/results_picker.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    32241 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/ucr_datasets.json
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.023811 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      983 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.025903 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/
+-rw-r--r--   0 technocreep   (501) staff       (20)     9997 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/DatasetLoader.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2054 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2267 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/InputData.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.028283 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1784 2023-04-05 13:01:09.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/hyperparams.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3599 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/pipeline_factory.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      781 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/task_factory.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2885 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.029563 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1027 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/Testing.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      250 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/utils.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.030465 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2216 2023-04-06 14:35:18.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/BaseEnsembler.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.031185 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     6258 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/kernel_ensemble.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.032123 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/
+-rw-r--r--   0 technocreep   (501) staff       (20)    12592 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/RankEnsembler.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.032812 fedot_ind-0.0.0.3/fedot_ind/core/metrics/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.034782 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1200 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/basis_loss.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4303 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/soft_dtw.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2560 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/svd_loss.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4920 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/metrics/metrics_implementation.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.036547 fedot_ind-0.0.0.3/fedot_ind/core/models/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3734 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/BaseExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2442 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/EnsembleExtractor.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.036911 fedot_ind-0.0.0.3/fedot_ind/core/models/TSAnomalyDetector/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-11-15 14:20:59.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/TSAnomalyDetector/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.038654 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1818 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/classification_models.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4815 2023-04-04 16:16:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/decomposed_conv.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8080 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/sfp_models.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.039213 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.040760 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/
+-rw-r--r--   0 technocreep   (501) staff       (20)      680 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3521 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8193 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/FileObject.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.041539 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/
+-rw-r--r--   0 technocreep   (501) staff       (20)     7413 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.043985 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    18879 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/kalman.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    17411 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/sigma.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.045570 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7969 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/func_pca.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    11329 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/sst.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.046861 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      274 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/get_time.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7050 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/math_utils.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.047617 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/
+-rw-r--r--   0 technocreep   (501) staff       (20)     5055 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/AngleBasedDetector.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.049051 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/
+-rw-r--r--   0 technocreep   (501) staff       (20)     8578 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/ErrorRunner.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5714 2023-04-04 13:40:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/error_correction.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5397 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/static_booster.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.050217 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12206 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/inception.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      615 2023-04-06 12:05:38.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/nn/modules.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.052104 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3758 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/RecurrenceExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5643 2023-04-17 14:27:21.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/SignalExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      956 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/signal/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.052911 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/
+-rw-r--r--   0 technocreep   (501) staff       (20)    12405 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/SSAExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.053765 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3671 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/StatsExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 09:33:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.054359 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/
+-rw-r--r--   0 technocreep   (501) staff       (20)     4878 2023-04-17 14:17:48.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/TopologicalExtractor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/models/topological/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.054883 fedot_ind-0.0.0.3/fedot_ind/core/operation/
+-rw-r--r--   0 technocreep   (501) staff       (20)     2151 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/IndustrialCachableOperation.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-08-30 11:53:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.055662 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/
+-rw-r--r--   0 technocreep   (501) staff       (20)     5974 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.056252 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3996 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.056841 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      549 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/dummy_operation.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.057409 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      512 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/quantile_filtration.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.057992 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2561 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.059865 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.060559 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/
+-rw-r--r--   0 technocreep   (501) staff       (20)     3615 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2732 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/FeatureSpace.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     7772 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/ModelStructure.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     8581 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/sfp_tools.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3535 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/svd_tools.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.061857 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/
+-rw-r--r--   0 technocreep   (501) staff       (20)     9911 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/DataTransformer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2912 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    13768 2023-04-05 16:47:37.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/WindowSelection.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.064788 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2620 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/abstract_basis.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     4741 2023-04-17 16:54:22.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3013 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/chebyshev.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5649 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/data_driven.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2044 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/fourier.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2931 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/legendre.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1264 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/power.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2938 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/wavelet.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.065895 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3065 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/eigen.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3399 2023-04-06 15:26:37.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/hankel.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.067359 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2022-12-20 11:07:41.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    10503 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/sequences.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5276 2023-04-17 12:56:39.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/statistical.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    10224 2023-04-17 14:18:26.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/topological.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.068386 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     5223 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/lp_reg.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     2712 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/spectrum.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.069795 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)      832 2022-10-19 15:44:11.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/alt_booster.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     3180 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/cache.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    28639 2022-11-11 14:23:34.000000 fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/ts_reader.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.070452 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1893 2023-04-17 14:51:42.000000 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/optimizer/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.071577 fedot_ind-0.0.0.3/fedot_ind/core/repository/
+-rw-r--r--   0 technocreep   (501) staff       (20)     1072 2023-04-17 12:56:40.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialDispatcher.py
+-rw-r--r--   0 technocreep   (501) staff       (20)     1861 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialOperationParameters.py
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-03-24 12:37:20.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/__init__.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.072876 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-18 12:47:03.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    14574 2023-04-04 16:07:26.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/data_operation_repository.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     3058 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/default_operation_params.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     1932 2023-04-17 14:44:27.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/data/industrial_data_operation_repository.json
+-rw-r--r--   0 technocreep   (501) staff       (20)     6337 2023-04-17 14:42:19.000000 fedot_ind-0.0.0.3/fedot_ind/core/repository/initializer_industrial_models.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.073794 fedot_ind-0.0.0.3/fedot_ind/core/tuning/
+-rw-r--r--   0 technocreep   (501) staff       (20)        0 2023-04-17 12:28:29.000000 fedot_ind-0.0.0.3/fedot_ind/core/tuning/__init__.py
+-rw-r--r--   0 technocreep   (501) staff       (20)    12575 2023-04-05 16:58:17.000000 fedot_ind-0.0.0.3/fedot_ind/core/tuning/search_space.py
+drwxr-xr-x   0 technocreep   (501) staff       (20)        0 2023-04-18 13:07:45.008220 fedot_ind-0.0.0.3/fedot_ind.egg-info/
+-rw-r--r--   0 technocreep   (501) staff       (20)     8908 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/PKG-INFO
+-rw-r--r--   0 technocreep   (501) staff       (20)     8428 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/SOURCES.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)        1 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/dependency_links.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)      442 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/requires.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)       15 2023-04-18 13:07:44.000000 fedot_ind-0.0.0.3/fedot_ind.egg-info/top_level.txt
+-rw-r--r--   0 technocreep   (501) staff       (20)       38 2023-04-18 13:07:45.075209 fedot_ind-0.0.0.3/setup.cfg
+-rw-r--r--   0 technocreep   (501) staff       (20)     1929 2023-04-18 13:07:40.000000 fedot_ind-0.0.0.3/setup.py
```

### Comparing `fedot_ind-0.0.0.2/LICENSE.md` & `fedot_ind-0.0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/PKG-INFO` & `fedot_ind-0.0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot_ind
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Automated machine learning framework for time series analysis
 Home-page: https://github.com/aimclub/Fedot.Industrial
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Keywords: automated machine learning,time series analysis,anomaly detection,classification
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fedot_ind-0.0.0.2/README.rst` & `fedot_ind-0.0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/main.py` & `fedot_ind-0.0.0.3/fedot_ind/api/main.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/main_example.py` & `fedot_ind-0.0.0.3/fedot_ind/api/main_example.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/checkers_collections.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/checkers_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/hp_generator_collection.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/hp_generator_collection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/metafeatures.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/metafeatures.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/reader_collections.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/reader_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/reporter.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/reporter.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/api/utils/saver_collections.py` & `fedot_ind-0.0.0.3/fedot_ind/api/utils/saver_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/abstraction/Decorators.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/abstraction/Decorators.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/classification_datasets.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/classification_datasets.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/datasets/object_detection_datasets.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/datasets/object_detection_datasets.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/BenchmarkTests.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/BenchmarkTests.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/CVModule.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/CVModule.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TImeSeriesClassifierPreset.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/experiment/TimeSeriesClassifier.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/abstract_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/pipelines/classification.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/pipelines/classification.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/Analyzer.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/Analyzer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/results_picker.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/results_picker.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Args:
         path (str): path to folder with experiments. Default is ``None`` and it means that path
                     is ``results_of_experiments``.
         launch_type (str or int): number of launch to be extracted. Default is ``max`` and it means that the best launch
                                   will be extracted.
 
     Examples:
-        >>> from fedot_ind.core import ResultsPicker
+        >>> from fedot_ind.core.architecture.postprocessing.results_picker import ResultsPicker
         >>> collector = ResultsPicker(path='to_your_results_folder', launch_type='max')
         >>> metrics_df = parser.run(get_metrics_df=True)
         >>> metrics_df.to_csv('metrics.csv')
 
     """
 
     def __init__(self, path: str = None, launch_type: Union[str, int] = 'max'):
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/DatasetLoader.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/DatasetLoader.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/FeatureBuilder.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/preprocessing/InputData.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/preprocessing/InputData.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/hyperparams.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/hyperparams.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/pipeline_factory.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/pipeline_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from enum import Enum
+
 from fedot_ind.core.models.detection.probalistic.kalman import UnscentedKalmanFilter
-from fedot_ind.core.models.detection.subspaces.sst import SingularSpectrumTransformation
-from fedot_ind.core.operation.transformation.basis.chebyshev import ChebyshevBasis
-from fedot_ind.core.operation.transformation.basis.data_driven import DataDrivenBasisImplementation
-from fedot_ind.core.operation.transformation.basis.fourier import FourierBasisImplementation
-from fedot_ind.core.operation.transformation.basis.wavelet import WaveletBasisImplementation
 from fedot_ind.core.models.detection.subspaces.func_pca import FunctionalPCA
+from fedot_ind.core.models.detection.subspaces.sst import SingularSpectrumTransformation
 from fedot_ind.core.models.signal.RecurrenceExtractor import RecurrenceExtractor
 from fedot_ind.core.models.signal.SignalExtractor import SignalExtractor
 from fedot_ind.core.models.statistical.StatsExtractor import StatsExtractor
 from fedot_ind.core.models.topological.TopologicalExtractor import TopologicalExtractor
+from fedot_ind.core.operation.transformation.basis.chebyshev import ChebyshevBasis
+from fedot_ind.core.operation.transformation.basis.data_driven import DataDrivenBasisImplementation
+from fedot_ind.core.operation.transformation.basis.fourier import FourierBasisImplementation
+from fedot_ind.core.operation.transformation.basis.wavelet import WaveletBasisImplementation
 
 
 class BasisTransformations(Enum):
     chebyshev = ChebyshevBasis
     datadriven = DataDrivenBasisImplementation
     wavelet = WaveletBasisImplementation
     Fourier = FourierBasisImplementation
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/task_factory.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/task_factory.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/settings/typical_torch_datasets_params.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/architecture/utils/Testing.py` & `fedot_ind-0.0.0.3/fedot_ind/core/architecture/utils/Testing.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/ensemble/BaseEnsembler.py` & `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/BaseEnsembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/ensemble/baseline/kernel_ensemble.py` & `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/baseline/kernel_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from MKLpy.algorithms import MEMO, CKA
 from MKLpy.scheduler import ReduceOnWorsening
 from MKLpy.callbacks import EarlyStopping
 from fedot_ind.core.architecture.pipelines.classification import ClassificationPipelines
 from fedot_ind.core.architecture.preprocessing.DatasetLoader import DataLoader
 from scipy.spatial.distance import pdist, squareform
-from fedot_ind.core.architecture import KernelFeatureGenerator
+from fedot_ind.core.architecture.settings.pipeline_factory import KernelFeatureGenerator
 
 
 class KernelEnsembler(ClassificationPipelines):
     def __init__(self, train_data, test_data):
         super().__init__(train_data, test_data)
         self.n_classes = np.unique(self.train_target)
         if self.n_classes.shape[0] > 2:
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/ensemble/static/RankEnsembler.py` & `fedot_ind-0.0.0.3/fedot_ind/core/ensemble/static/RankEnsembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/basis_loss.py` & `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/basis_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/soft_dtw.py` & `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/soft_dtw.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/metrics/loss/svd_loss.py` & `fedot_ind-0.0.0.3/fedot_ind/core/metrics/loss/svd_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/metrics/metrics_implementation.py` & `fedot_ind-0.0.0.3/fedot_ind/core/metrics/metrics_implementation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/BaseExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/BaseExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/EnsembleExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/EnsembleExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/classification_models.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/classification_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/decomposed_conv.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/decomposed_conv.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/cnn/sfp_models.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/cnn/sfp_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AbstractDataOperation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/AnomalyZone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-
-from typing import Mapping, List
-
+from typing import List, Mapping
 
 
 class AnomalyZone:
     """
         + This class contains all data of one anomaly +
         Be careful, this class uses both for dataset objects of anomalies and for 
         anomalies that we are looking at!
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/abstract_objects/FileObject.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/abstract_objects/FileObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import List, Mapping
+
 from fedot_ind.core.models.detection.abstract_objects.AnomalyZone import AnomalyZone
 
+
 class FileObject:
     """
     This class contains all data that contains in one file - time series, lables,
     transformation params, anomalies list
     """
     def __init__(self, 
             test_data: List[float],
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/area/ThresholdZonesDetector.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/kalman.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/kalman.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from functools import partial
-import numpy as np
+import sys
 from copy import deepcopy
+from functools import partial
 from math import log
-import sys
+
+import numpy as np
+from numpy import dot, eye, zeros
 from sklearn.preprocessing import MinMaxScaler
-from numpy import dot, zeros, eye
+
 from fedot_ind.core.architecture.experiment.TimeSeriesClassifier import TimeSeriesClassifier
 from fedot_ind.core.models.detection.probalistic.sigma import MerweScaledSigmaPoints
 from fedot_ind.core.operation.transformation.data.hankel import get_x_y_pairs
 
 
 def reshape_z(z, dim_z, ndim):
     """ensure z is a (dim_z, 1) shaped vector"""
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/probalistic/sigma.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/probalistic/sigma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
-from scipy.linalg import cholesky, block_diag
-
-from numpy import zeros, vstack, eye, array
+from numpy import array, eye, zeros
+from scipy.linalg import block_diag, cholesky
 
 
 class MerweScaledSigmaPoints:
     """
     Generates sigma points and weights according to Van der Merwe's
     2004 dissertation[1] for the UnscentedKalmanFilter class. It
     parametizes the sigma points using alpha, beta, kappa terms, and
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/func_pca.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/func_pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from scipy.linalg import solve_triangular
 from sklearn.decomposition import PCA
 from fedot_ind.core.operation.filtration.quantile_filtration import quantile_filter
 # from core.operation.transformation.regularization.lp_reg import compute_penalty_matrix
 
+
 class FunctionalPCA:
     """
     Principal component analysis.
     Class that implements functional principal component analysis for both
     basis and natural representations of the data.
 
     Parameters:
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/subspaces/sst.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/subspaces/sst.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/utils/math_utils.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/utils/math_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from statistics import mean
 from scipy.signal import savgol_filter
-from fedot_ind.core.models.detection.utils.get_time \
-    import get_current_time
+from fedot_ind.core.models.detection.utils.get_time import get_current_time
+
 
 def NormalizeData(ts: list, return_numpy: bool = False):
     """
     Normalization method for time seroes. 
     Output time series' values are between 0.0 and 1.0
 
     Args:
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/detection/vector/AngleBasedDetector.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/detection/vector/AngleBasedDetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from fedot_ind.core.models.detection.utils.get_time \
-    import time_now
-from fedot_ind.core.models.detection.abstract_objects.AbstractDataOperation import AbstractDataOperation
-
-from fedot_ind.core.models.detection.utils.math_utils import NormalizeData
-
 from typing import Mapping
+
 from scipy import spatial
 
+from fedot_ind.core.models.detection.abstract_objects.AbstractDataOperation import AbstractDataOperation
 from fedot_ind.core.models.detection.abstract_objects.FileObject import FileObject
+from fedot_ind.core.models.detection.utils.get_time import time_now
+from fedot_ind.core.models.detection.utils.math_utils import NormalizeData
 
 """
 
 input format:
 
     dict with "data" and "lables" fields
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/ErrorRunner.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/ErrorRunner.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/error_correction.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/error_correction.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/ecm/static_booster.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/ecm/static_booster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import logging
 import warnings
 
-warnings.simplefilter(action='ignore', category=FutureWarning)
-import pandas as pd
 import numpy as np
-from sklearn.metrics import accuracy_score, f1_score
-from fedot.core.log import default_log as Logger
-from fedot.core.pipelines.node import PrimaryNode
+import pandas as pd
 from fedot.core.data.data import InputData
-from fedot.core.repository.tasks import Task, TaskTypesEnum
-from fedot.core.repository.dataset_types import DataTypesEnum
+from fedot.core.pipelines.node import PrimaryNode
 from fedot.core.pipelines.pipeline import Pipeline
+from fedot.core.repository.dataset_types import DataTypesEnum
+from fedot.core.repository.tasks import Task, TaskTypesEnum
+from sklearn.metrics import accuracy_score, f1_score
+
+warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 class StaticBooster:
     CYCLES = 1
 
     def __init__(self, X_train, y_train, base_predict, timeout, threshold=0):
 
@@ -21,15 +22,15 @@
         self.y_train = y_train
         self.base_predict = base_predict
         self.threshold = threshold
         self.timeout = round(timeout / 4)
         self.booster_features = {}
         self.check_table = pd.DataFrame()
 
-        self.logger = Logger(self.__class__.__name__)
+        self.logger = logging.getLogger('StaticBooster')
 
     def run_boosting(self):
         self.logger.info('Started boosting')
 
         target_diff_1 = self.decompose_target(previous_predict=self.base_predict,
                                               previous_target=self.y_train.reshape(-1))
         prediction_1, model_1 = self.api_model(target_diff=target_diff_1, node='linear')
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/nn/inception.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/nn/inception.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/nn/modules.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/nn/modules.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/signal/RecurrenceExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/RecurrenceExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/signal/SignalExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/SignalExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/signal/WindowedFeaturesExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/spectral/SSAExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/spectral/SSAExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/statistical/StatsExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/statistical/StatsExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/models/topological/TopologicalExtractor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/models/topological/TopologicalExtractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/IndustrialCachableOperation.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/IndustrialCachableOperation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/SpectrumDecomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/decomposition/matrix_decomposition/DMDecomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/dummy/dummy_operation.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/dummy/dummy_operation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/filtration/quantile_filtration.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/filtration/quantile_filtration.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/DMD/PhysicDMD.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from fedot_ind.core.operation.decomposition.matrix_decomposition.DMDecomposition import *
+
+
 class piDMD:
     """
     Computes a dynamic mode decomposition when the solution matrix is
     constrained to lie in a matrix manifold.
     The options available for the "method"
     - "exact", "exactSVDS"
     - "orthogonal"
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/FeatureSpace.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/FeatureSpace.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/ModelStructure.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/ModelStructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
 import os
 import time
-from typing import List, Dict
+from typing import Dict, List
 
 import torch
 from torch.utils.tensorboard import SummaryWriter
 
-from fedot_ind.core.metrics.loss.svd_loss import OrthogonalLoss, HoyerLoss
+from fedot_ind.core.metrics.loss.svd_loss import HoyerLoss, OrthogonalLoss
 from fedot_ind.core.models.cnn.decomposed_conv import DecomposedConv2d
 from fedot_ind.core.models.cnn.sfp_models import SFP_MODELS
-from fedot_ind.core.operation.optimization.sfp_tools import zerolize_filters, prune_resnet_state_dict
-from fedot_ind.core.operation.optimization.svd_tools import energy_threshold_pruning, decompose_module
+from fedot_ind.core.operation.optimization.sfp_tools import prune_resnet_state_dict, zerolize_filters
+from fedot_ind.core.operation.optimization.svd_tools import decompose_module, energy_threshold_pruning
 
 
 class GeneralizedStructureOptimization:
     """Generalized class for model structure optimization.
 
     Args:
         experimenter: An instance of the experimenter class, e.g.
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/sfp_tools.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/sfp_tools.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/optimization/svd_tools.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/optimization/svd_tools.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/DataTransformer.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/DataTransformer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/FeatureSpaceReductor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/WindowSelection.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/WindowSelection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/abstract_basis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/basis_tmp_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from fedot_ind.core.architecture.postprocessing.Analyzer import PerformanceAnalyzer
 from fedot_ind.core.models.spectral.SSAExtractor import SSAExtractor
-from fedot_ind.core.models.statistical.StatsExtractor import StatsRunner
+from fedot_ind.core.models.statistical.StatsExtractor import StatsExtractor
 from fedot_ind.core.operation.optimization.FeatureSpace import VarianceSelector
 from fedot_ind.core.architecture.experiment.TimeSeriesClassifier import TimeSeriesClassifier
 from fedot_ind.core.architecture.preprocessing.DatasetLoader import DataLoader
 from fedot_ind.core.operation.transformation.basis.legendre import LegenderBasis
 
 
 def get_results(model, features, target):
@@ -61,15 +61,15 @@
                                         window_sizes={dataset_name: [30]},
                                         spectral_hyperparams={'combine_eigenvectors': False,
                                                            'correlation_level': 0.8})
     train_feats_spectral_basic = spectral_model_basic.get_features(train[0], dataset_name)
     test_feats_spectral_basic = spectral_model_basic.get_features(test[0], dataset_name)
     train_eigenvectors_spectral_basic = spectral_model_basic.eigenvectors_list_train
 
-    quantile_model_basic = StatsRunner(window_mode=True)
+    quantile_model_basic = StatsExtractor(window_mode=True)
     train_feats_baseline = quantile_model_basic.get_features(update_train, dataset_name)
     test_feats_baseline = quantile_model_basic.get_features(update_test, dataset_name)
 
     model_features = {
         'spectral_basic': train_feats_spectral_basic,
         'quantile': train_feats_baseline
     }
@@ -89,13 +89,13 @@
         'timeout': 2,
         'max_depth': 4,
         'max_arity': 2,
         'cv_folds': 2,
         'logging_level': 20,
         'n_jobs': 2
     })
-    quantile_model_basic = StatsRunner(window_mode=True)
+    quantile_model_basic = StatsExtractor(window_mode=True)
     train_feats_baseline = quantile_model_basic.get_features(update_train, dataset_name)
     test_feats_baseline = quantile_model_basic.get_features(update_test, dataset_name)
     IndustrialModelBaseline = clf.fit(train_features=train_feats_baseline, train_target=train_target)[0]
     baseline_results = get_results(clf, test_feats_baseline, test_target)
     predict_baseline = clf.predict(test_feats_baseline)['label']
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/chebyshev.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/chebyshev.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/data_driven.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/data_driven.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/fourier.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/fourier.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/legendre.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/legendre.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/power.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/power.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/basis/wavelet.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/basis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/eigen.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/eigen.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/data/hankel.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/data/hankel.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/sequences.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/sequences.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/statistical.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/statistical.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/extraction/topological.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/extraction/topological.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/lp_reg.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/lp_reg.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/transformation/regularization/spectrum.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/transformation/regularization/spectrum.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/alt_booster.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/alt_booster.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/cache.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/cache.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/operation/utils/ts_reader.py` & `fedot_ind-0.0.0.3/fedot_ind/core/operation/utils/ts_reader.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py` & `fedot_ind-0.0.0.3/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/repository/IndustrialDispatcher.py` & `fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialDispatcher.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/repository/IndustrialOperationParameters.py` & `fedot_ind-0.0.0.3/fedot_ind/core/repository/IndustrialOperationParameters.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/repository/initializer_industrial_models.py` & `fedot_ind-0.0.0.3/fedot_ind/core/repository/initializer_industrial_models.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind/core/tuning/search_space.py` & `fedot_ind-0.0.0.3/fedot_ind/core/tuning/search_space.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.0.0.2/fedot_ind.egg-info/PKG-INFO` & `fedot_ind-0.0.0.3/fedot_ind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot-ind
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Automated machine learning framework for time series analysis
 Home-page: https://github.com/aimclub/Fedot.Industrial
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Keywords: automated machine learning,time series analysis,anomaly detection,classification
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fedot_ind-0.0.0.2/fedot_ind.egg-info/SOURCES.txt` & `fedot_ind-0.0.0.3/fedot_ind.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+MANIFEST.in
 README.rst
 setup.py
 docs/__init__.py
 fedot_ind/__init__.py
 fedot_ind.egg-info/PKG-INFO
 fedot_ind.egg-info/SOURCES.txt
 fedot_ind.egg-info/dependency_links.txt
@@ -12,15 +13,14 @@
 fedot_ind/api/main.py
 fedot_ind/api/main_example.py
 fedot_ind/api/utils/__init__.py
 fedot_ind/api/utils/checkers_collections.py
 fedot_ind/api/utils/decorator_collections.py
 fedot_ind/api/utils/hp_generator_collection.py
 fedot_ind/api/utils/metafeatures.py
-fedot_ind/api/utils/method_collections.py
 fedot_ind/api/utils/reader_collections.py
 fedot_ind/api/utils/reporter.py
 fedot_ind/api/utils/saver_collections.py
 fedot_ind/core/__init__.py
 fedot_ind/core/architecture/__init__.py
 fedot_ind/core/architecture/abstraction/Decorators.py
 fedot_ind/core/architecture/abstraction/__init__.py
@@ -36,14 +36,15 @@
 fedot_ind/core/architecture/pipelines/abstract_pipeline.py
 fedot_ind/core/architecture/pipelines/anomaly_detection.py
 fedot_ind/core/architecture/pipelines/classification.py
 fedot_ind/core/architecture/pipelines/computer_vision.py
 fedot_ind/core/architecture/postprocessing/Analyzer.py
 fedot_ind/core/architecture/postprocessing/__init__.py
 fedot_ind/core/architecture/postprocessing/results_picker.py
+fedot_ind/core/architecture/postprocessing/ucr_datasets.json
 fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
 fedot_ind/core/architecture/postprocessing/visualisation/matrix_vis.py
 fedot_ind/core/architecture/preprocessing/DatasetLoader.py
 fedot_ind/core/architecture/preprocessing/FeatureBuilder.py
 fedot_ind/core/architecture/preprocessing/InputData.py
 fedot_ind/core/architecture/preprocessing/__init__.py
 fedot_ind/core/architecture/settings/__init__.py
@@ -157,9 +158,13 @@
 fedot_ind/core/operation/utils/ts_reader.py
 fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
 fedot_ind/core/optimizer/__init__.py
 fedot_ind/core/repository/IndustrialDispatcher.py
 fedot_ind/core/repository/IndustrialOperationParameters.py
 fedot_ind/core/repository/__init__.py
 fedot_ind/core/repository/initializer_industrial_models.py
+fedot_ind/core/repository/data/__init__.py
+fedot_ind/core/repository/data/data_operation_repository.json
+fedot_ind/core/repository/data/default_operation_params.json
+fedot_ind/core/repository/data/industrial_data_operation_repository.json
 fedot_ind/core/tuning/__init__.py
 fedot_ind/core/tuning/search_space.py
```

### Comparing `fedot_ind-0.0.0.2/setup.py` & `fedot_ind-0.0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'fedot_ind'
-VERSION = '0.0.0.2'
+VERSION = '0.0.0.3'
 AUTHOR = 'NSS Lab'
 AUTHOR_EMAIL = 'itmo.nss.team@gmail.com'
 SHORT_DESCRIPTION = 'Automated machine learning framework for time series analysis'
 LONG_DESC_TYPE = 'text/x-rst'
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
-EXCLUDED_PACKAGES = ['test*', 'examples', 'cases', 'benchmark']
+EXCLUDED_PACKAGES = ['test*', 'examples', 'cases', 'benchmark', '*.csv']
 URL = 'https://github.com/aimclub/Fedot.Industrial'
 REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
 KEYWORDS = 'automated machine learning, time series analysis, anomaly detection, classification'
 
 
 def _readlines(*names: str, **kwargs) -> List[str]:
@@ -44,14 +44,15 @@
     description=SHORT_DESCRIPTION,
     long_description=README,
     long_description_content_type=LONG_DESC_TYPE,
     url=URL,
     python_requires=REQUIRES_PYTHON,
     license=LICENSE,
     packages=setuptools.find_packages(exclude=EXCLUDED_PACKAGES),
+    # package_data={'ucr_datasets': ['postprocessing/ucr_datasets.json']},
     include_package_data=True,
     install_requires=_get_requirements('requirements.txt'),
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
```

