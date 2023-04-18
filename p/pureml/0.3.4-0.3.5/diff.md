# Comparing `tmp/pureml-0.3.4.tar.gz` & `tmp/pureml-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.4.tar", max compression
+gzip compressed data, was "pureml-0.3.5.tar", max compression
```

## Comparing `pureml-0.3.4.tar` & `pureml-0.3.5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11370 2023-04-05 12:44:15.330474 pureml-0.3.4/README.md
--rw-r--r--   0        0        0      734 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/__init__.py
--rw-r--r--   0        0        0     2534 2023-02-10 14:59:50.822240 pureml-0.3.4/pureml/cli/__init__.py
--rw-r--r--   0        0        0     8756 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/auth.py
--rw-r--r--   0        0        0     1046 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3198 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/main.py
--rw-r--r--   0        0        0     3236 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.4/pureml/cli/public.pem
--rw-r--r--   0        0        0     1696 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7290 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2116 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/components/__init__.py
--rw-r--r--   0        0        0     1748 2023-03-15 11:32:06.993246 pureml-0.3.4/pureml/components/auth.py
--rw-r--r--   0        0        0    15690 2023-04-08 14:57:03.440354 pureml-0.3.4/pureml/components/dataset.py
--rw-r--r--   0        0        0       99 2023-04-05 12:44:15.342474 pureml-0.3.4/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     7073 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6852 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6830 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9667 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6801 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/image.py
--rw-r--r--   0        0        0     2052 2023-04-05 12:44:15.358475 pureml-0.3.4/pureml/components/log/log.py
--rw-r--r--   0        0        0     6045 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     6016 2023-04-05 12:44:15.702483 pureml-0.3.4/pureml/components/log/params.py
--rw-r--r--   0        0        0     6198 2023-04-10 21:10:47.279602 pureml-0.3.4/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6214 2023-04-10 21:10:47.311604 pureml-0.3.4/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6084 2023-04-10 21:10:47.323604 pureml-0.3.4/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6909 2023-04-05 12:44:15.698483 pureml-0.3.4/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6308 2023-04-05 12:44:15.698483 pureml-0.3.4/pureml/components/log/video.py
--rw-r--r--   0        0        0    13620 2023-04-08 23:11:11.562439 pureml-0.3.4/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.4/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.4/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.4/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.4/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.4/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.4/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.4/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.4/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.4/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.4/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.4/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.4/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.4/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.4/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.4/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.4/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.4/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.4/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.4/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.4/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.4/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.4/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.4/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.4/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.4/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.4/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.4/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.4/pureml/package/__init__.py
--rw-r--r--   0        0        0     6324 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/package/docker.py
--rw-r--r--   0        0        0     5913 2023-04-05 12:44:15.486478 pureml-0.3.4/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.4/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.4/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.4/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.4/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      365 2023-04-05 12:44:15.486478 pureml-0.3.4/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2325 2023-04-15 12:47:43.506059 pureml-0.3.4/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.4/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.4/pureml/schema/dataset.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.4/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.4/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.4/pureml/schema/paths.py
--rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.4/pureml/schema/predict.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.4/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.4/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.4/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.4/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.4/pureml/utils/constants.py
--rw-r--r--   0        0        0     2998 2023-03-15 11:32:07.825248 pureml-0.3.4/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.4/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.4/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.4/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.4/pureml/utils/predict.py
--rw-r--r--   0        0        0      815 2023-02-10 14:59:51.066213 pureml-0.3.4/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.4/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.4/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.4/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.4/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1927 2023-04-15 12:47:43.510059 pureml-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    13291 1970-01-01 00:00:00.000000 pureml-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11370 2023-04-05 12:44:15.330474 pureml-0.3.5/README.md
+-rw-r--r--   0        0        0      734 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/__init__.py
+-rw-r--r--   0        0        0     2534 2023-02-10 14:59:50.822240 pureml-0.3.5/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9059 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/cli/auth.py
+-rw-r--r--   0        0        0     1046 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3198 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/main.py
+-rw-r--r--   0        0        0     3236 2023-04-18 20:20:22.611483 pureml-0.3.5/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.5/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1696 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7290 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2116 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/components/__init__.py
+-rw-r--r--   0        0        0     1748 2023-03-15 11:32:06.993246 pureml-0.3.5/pureml/components/auth.py
+-rw-r--r--   0        0        0    15690 2023-04-08 14:57:03.440354 pureml-0.3.5/pureml/components/dataset.py
+-rw-r--r--   0        0        0       99 2023-04-05 12:44:15.342474 pureml-0.3.5/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     7073 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6852 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6830 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9667 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6801 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2052 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/components/log/log.py
+-rw-r--r--   0        0        0     6045 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     6016 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6198 2023-04-10 21:10:47.279602 pureml-0.3.5/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6214 2023-04-10 21:10:47.311604 pureml-0.3.5/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6084 2023-04-10 21:10:47.323604 pureml-0.3.5/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6909 2023-04-05 12:44:15.698483 pureml-0.3.5/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6308 2023-04-05 12:44:15.698483 pureml-0.3.5/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13620 2023-04-08 23:11:11.562439 pureml-0.3.5/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.5/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.5/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.5/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.5/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.5/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.5/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.5/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.5/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.5/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.5/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.5/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.5/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.5/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.5/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.5/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.5/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.5/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.5/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6324 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/package/docker.py
+-rw-r--r--   0        0        0     5913 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.5/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.5/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.5/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.5/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      365 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2578 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.5/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.5/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.5/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/schema/predict.py
+-rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.5/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.5/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.5/pureml/utils/constants.py
+-rw-r--r--   0        0        0     2998 2023-03-15 11:32:07.825248 pureml-0.3.5/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.5/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.5/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.5/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.5/pureml/utils/predict.py
+-rw-r--r--   0        0        0      815 2023-02-10 14:59:51.066213 pureml-0.3.5/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.5/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.5/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.5/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1927 2023-04-18 20:24:19.682573 pureml-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    13291 1970-01-01 00:00:00.000000 pureml-0.3.5/PKG-INFO
```

### Comparing `pureml-0.3.4/README.md` & `pureml-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/__init__.py` & `pureml-0.3.5/pureml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from .evaluate import grader, eval
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

### Comparing `pureml-0.3.4/pureml/cli/__init__.py` & `pureml-0.3.5/pureml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/cli/auth.py` & `pureml-0.3.5/pureml/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,24 @@
         url = urljoin(backend_base_url, url_path_1)
 
         response = requests.post(url, json=data)
 
         if not response.ok:
             print(f"[red]Could not create account! Please try again later")
             return
-        print(
-            f"[green]Successfully created your account! You can now login using ```pure auth login```"
-        )
+        elif response.status_code == 202:
+            print(f"[green]Successfully created your account! You need to verify your email to login!")
+            print(
+                f"[green]You can then login using `pureml auth login`"
+            )
+        else:
+            print(f"[green]Successfully created your account!")
+            print(
+                f"[green]You can now login using `pureml auth login`"
+            )
     except Exception as e:
         print(f"[red]Could not create account! Please try again later")
         print(e)
 
 @app.command()
 def login(
     backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance"),
```

### Comparing `pureml-0.3.4/pureml/cli/helpers.py` & `pureml-0.3.5/pureml/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/cli/main.py` & `pureml-0.3.5/pureml/cli/main.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/cli/orgs.py` & `pureml-0.3.5/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/cli/puremlconfig.py` & `pureml-0.3.5/pureml/cli/puremlconfig.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/cli/secrets.py` & `pureml-0.3.5/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/__init__.py` & `pureml-0.3.5/pureml/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/auth.py` & `pureml-0.3.5/pureml/components/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/dataset.py` & `pureml-0.3.5/pureml/components/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/arrays.py` & `pureml-0.3.5/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/artifacts.py` & `pureml-0.3.5/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/audio.py` & `pureml-0.3.5/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/figure.py` & `pureml-0.3.5/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/image.py` & `pureml-0.3.5/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/log.py` & `pureml-0.3.5/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/metrics.py` & `pureml-0.3.5/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/params.py` & `pureml-0.3.5/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/pip_requirement.py` & `pureml-0.3.5/pureml/components/log/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/predict.py` & `pureml-0.3.5/pureml/components/log/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/resources.py` & `pureml-0.3.5/pureml/components/log/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/tabular.py` & `pureml-0.3.5/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/log/video.py` & `pureml-0.3.5/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/components/model.py` & `pureml-0.3.5/pureml/components/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/config/parser.py` & `pureml-0.3.5/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/dataset.py` & `pureml-0.3.5/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/load_data.py` & `pureml-0.3.5/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/model.py` & `pureml-0.3.5/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/pip_requirements.py` & `pureml-0.3.5/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/predict.py` & `pureml-0.3.5/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/decorators/transformer.py` & `pureml-0.3.5/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/classification.py` & `pureml-0.3.5/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/eval.py` & `pureml-0.3.5/pureml/evaluate/eval.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/grade.py` & `pureml-0.3.5/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.5/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.5/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/f1.py` & `pureml-0.3.5/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/mae.py` & `pureml-0.3.5/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/mse.py` & `pureml-0.3.5/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/precision.py` & `pureml-0.3.5/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/recall.py` & `pureml-0.3.5/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.5/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/evaluate/regression.py` & `pureml-0.3.5/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/lineage/data/create_lineage.py` & `pureml-0.3.5/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/package/docker.py` & `pureml-0.3.5/pureml/package/docker.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/package/fastapi.py` & `pureml-0.3.5/pureml/package/fastapi.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/__init__.py` & `pureml-0.3.5/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_framework.py` & `pureml-0.3.5/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.5/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.5/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.5/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.5/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.5/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.5/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.5/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.5/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.5/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/packaging.py` & `pureml-0.3.5/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/packaging/packaging_utils.py` & `pureml-0.3.5/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/predictor/predictor.py` & `pureml-0.3.5/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/schema/backend.py` & `pureml-0.3.5/pureml/schema/backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,66 @@
 from pydantic import BaseModel, root_validator
 from .singleton import Singleton_BaseModel
 import typing
 import os
+import typer
 
 from pathlib import Path
 from pureml.cli.puremlconfig import PureMLConfigYML
 
 
 project_path = Path.cwd()
 if Path.exists(project_path / "puremlconfig.yml"):
     puremlconfig = PureMLConfigYML(project_path / "puremlconfig.yml")
 else:
     puremlconfig = None
 
 
 def get_backend_base_url(backend_url: str = None):
-    if backend_url is not None and backend_url != "":
+    if (
+        backend_url is not None
+        and backend_url != ""
+        and type(backend_url) == typer.Option
+    ):
         # override backend url (command specific option)
         return backend_url
     if puremlconfig is not None:
         # user configured backend url (self-hosted or custom pureml backend instance)
-        backend_url = puremlconfig.data["backend_url"] if "backend_url" in puremlconfig.data else "https://pureml-development.up.railway.app/api/"
+        backend_url = (
+            puremlconfig.data["backend_url"]
+            if "backend_url" in puremlconfig.data
+            else "https://pureml-development.up.railway.app/api/"
+        )
     else:
         # default backend url (production cloud backend)
         backend_url = "https://pureml-development.up.railway.app/api/"
     return backend_url
 
+
 def get_frontend_base_url(frontend_url: str = None):
-    if frontend_url is not None and frontend_url != "":
+    if (
+        frontend_url is not None
+        and frontend_url != ""
+        and type(frontend_url) == typer.Option
+    ):
         # override frontend url (command specific option)
         return frontend_url
     if puremlconfig is not None:
         # user configured frontend url (self-hosted or custom pureml frontend instance)
-        frontend_url = puremlconfig.data["frontend_url"] if "frontend_url" in puremlconfig.data else "https://pureml.com/"
+        frontend_url = (
+            puremlconfig.data["frontend_url"]
+            if "frontend_url" in puremlconfig.data
+            else "https://pureml.com/"
+        )
     else:
         # default frontend url (production cloud frontend)
         frontend_url = "https://pureml.com/"
     return frontend_url
 
+
 class BackendSchema(Singleton_BaseModel):
 
     BASE_URL: str = get_backend_base_url()
     FRONTEND_BASE_URL: str = get_frontend_base_url()
     INTEGRATIONS: dict = {
         "s3": {
             "name": "AWS S3 Object Storage",
@@ -57,12 +76,12 @@
             "secrets": [
                 "access_key_id",
                 "access_key_secret",
                 "account_id",
                 "bucket_name",
                 "public_url",
             ],
-        }
+        },
     }
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `pureml-0.3.4/pureml/schema/packaging.py` & `pureml-0.3.5/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/schema/paths.py` & `pureml-0.3.5/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/schema/predict.py` & `pureml-0.3.5/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/config.py` & `pureml-0.3.5/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/constants.py` & `pureml-0.3.5/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/hash.py` & `pureml-0.3.5/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/log_utils.py` & `pureml-0.3.5/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/package.py` & `pureml-0.3.5/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/pipeline.py` & `pureml-0.3.5/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/predict.py` & `pureml-0.3.5/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/readme.py` & `pureml-0.3.5/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/resources.py` & `pureml-0.3.5/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pureml/utils/version_utils.py` & `pureml-0.3.5/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.4/pyproject.toml` & `pureml-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
```

### Comparing `pureml-0.3.4/PKG-INFO` & `pureml-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
```

