# Comparing `tmp/tiledb-ml-0.9.2.tar.gz` & `tmp/tiledb-ml-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb-ml-0.9.2.tar", last modified: Fri Mar 17 12:25:10 2023, max compression
+gzip compressed data, was "tiledb-ml-0.9.3.tar", last modified: Tue Apr 18 17:28:20 2023, max compression
```

## Comparing `tiledb-ml-0.9.2.tar` & `tiledb-ml-0.9.3.tar`

### file list

```diff
@@ -1,92 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/examples/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/examples/cloud/models/
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/examples/cloud/serverless_training/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/data_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/model_load_and_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/model_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/examples/models/
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/models/pytorch_tiledb_models_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/models/sklearn_tiledb_models_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/models/tensorflow_keras_tiledb_models_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/examples/readers/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/readers/pytorch_data_api_tiledb_dense.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23613 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/readers/pytorch_data_api_tiledb_sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/readers/tensorflow_data_api_tiledb_dense.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-17 12:25:10.736756 tiledb-ml-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/models/test_cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/models/test_pytorch_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/models/test_sklearn_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/models/test_tensorflow_keras_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/test_pytorch_collators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/test_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/test_tensor_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tests/readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.724756 tiledb-ml-0.9.2/tiledb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.728756 tiledb-ml-0.9.2/tiledb/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/tiledb/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/_cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/_file_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/models/tensorflow_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/tiledb/ml/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_pytorch_collators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/base_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/mapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/ragged.py
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-03-17 12:25:05.000000 tiledb-ml-0.9.2/tiledb/ml/readers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb/ml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:25:10.732756 tiledb-ml-0.9.2/tiledb_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 12:25:10.000000 tiledb-ml-0.9.2/tiledb_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.331370 tiledb-ml-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.339370 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.339370 tiledb-ml-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/tiledb-logo_color_no_margin_@4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.readers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/examples/cloud/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/cloud/serverless_training/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/data_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_load_and_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/examples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/pytorch_tiledb_models_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/sklearn_tiledb_models_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/tensorflow_keras_tiledb_models_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/examples/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_dense.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23613 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_dense.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_cloud_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_pytorch_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_sklearn_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_tensorflow_keras_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_pytorch_collators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_tensor_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/tiledb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tiledb/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.355370 tiledb-ml-0.9.3/tiledb/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_cloud_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_file_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/tensorflow_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.355370 tiledb-ml-0.9.3/tiledb/ml/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_pytorch_collators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ragged.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb/ml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/tiledb_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/top_level.txt
```

### Comparing `tiledb-ml-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/.github/workflows/ci.yml` & `tiledb-ml-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/.github/workflows/release.yml` & `tiledb-ml-0.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/CODE_OF_CONDUCT.md` & `tiledb-ml-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/CONTRIBUTING.md` & `tiledb-ml-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/LICENSE` & `tiledb-ml-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/PKG-INFO` & `tiledb-ml-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-ml
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package supports all machine learning functionality for TileDB Embedded and TileDB Cloud
 Home-page: https://github.com/TileDB-Inc/TileDB-ML
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TileDB-Inc/TileDB-ML/issues
 Project-URL: Documentation, https://docs.tiledb.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.2 Summary: Package supports
+Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.3 Summary: Package supports
 all machine learning functionality for TileDB Embedded and TileDB Cloud Home-
 page: https://github.com/TileDB-Inc/TileDB-ML Author: TileDB, Inc. Author-
 email: help@tiledb.io License: MIT Project-URL: Bug Tracker, https://
 github.com/TileDB-Inc/TileDB-ML/issues Project-URL: Documentation, https://
 docs.tiledb.com Keywords: tiledb,ml Platform: any Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
```

### Comparing `tiledb-ml-0.9.2/README.md` & `tiledb-ml-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.3/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.3/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.3/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/README.md` & `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/data_ingestion.py` & `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/model_load_and_predict.py` & `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_load_and_predict.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/cloud/serverless_training/pytorch/model_training.py` & `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_training.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/models/pytorch_tiledb_models_example.ipynb` & `tiledb-ml-0.9.3/examples/models/pytorch_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/models/sklearn_tiledb_models_example.ipynb` & `tiledb-ml-0.9.3/examples/models/sklearn_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/models/tensorflow_keras_tiledb_models_example.ipynb` & `tiledb-ml-0.9.3/examples/models/tensorflow_keras_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/readers/pytorch_data_api_tiledb_dense.ipynb` & `tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_dense.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825240100202478%*

 * *Differences: {"'cells'": "{3: {'outputs': [OrderedDict([('name', 'stderr'), ('output_type', 'stream'), ('text', "*

 * *            "['0.3%'])]), OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', "*

 * *            "['Downloading http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz\\n', "*

 * *            "'Downloading http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz to "*

 * *            "../data/MNIST/raw/train-images-idx3-ubyte.gz\\n'])]), OrderedDict([('name', "*

 * *            "'stderr'), ('output_type' […]*

```diff
@@ -48,15 +48,118 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "0.3%"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Downloading http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz to ../data/MNIST/raw/train-images-idx3-ubyte.gz\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100.0%\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Extracting ../data/MNIST/raw/train-images-idx3-ubyte.gz to ../data/MNIST/raw\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100.0%"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz to ../data/MNIST/raw/train-labels-idx1-ubyte.gz\n",
+                        "Extracting ../data/MNIST/raw/train-labels-idx1-ubyte.gz to ../data/MNIST/raw\n",
+                        "\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "19.9%"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Downloading http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz to ../data/MNIST/raw/t10k-images-idx3-ubyte.gz\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100.0%\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Extracting ../data/MNIST/raw/t10k-images-idx3-ubyte.gz to ../data/MNIST/raw\n",
+                        "\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz\n",
+                        "Downloading http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz to ../data/MNIST/raw/t10k-labels-idx1-ubyte.gz\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100.0%"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Extracting ../data/MNIST/raw/t10k-labels-idx1-ubyte.gz to ../data/MNIST/raw\n",
+                        "\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                }
+            ],
             "source": [
                 "data_home = os.path.join(os.path.pardir, \"data\")\n",
                 "data = torchvision.datasets.MNIST(root=data_home, train=False, download=True)"
             ]
         },
         {
             "cell_type": "code",
@@ -139,15 +242,24 @@
                 "Now we proceed with ingestion."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/Users/george/PycharmProjects/TileDB-ML/.venv/lib/python3.9/site-packages/tiledb/ctx.py:448: UserWarning: tiledb.default_ctx and scope_ctx will not function correctly due to bug in IPython contextvar support.  You must supply a Ctx object to each function for custom configuration options. Please consider upgrading to ipykernel >= 6!Please see https://github.com/TileDB-Inc/TileDB-Py/issues/667 for more information.\n",
+                        "  warnings.warn(\n"
+                    ]
+                }
+            ],
             "source": [
                 "data_dir = os.path.join(data_home, 'readers', 'pytorch', 'dense')\n",
                 "os.makedirs(data_dir, exist_ok=True)\n",
                 "\n",
                 "# Ingest images\n",
                 "training_images = os.path.join(data_dir, 'training_images')\n",
                 "if not os.path.exists(training_images):\n",
@@ -208,22 +320,14 @@
                         "  cell_order='row-major',\n",
                         "  tile_order='row-major',\n",
                         "  capacity=10000,\n",
                         "  sparse=False,\n",
                         ")\n",
                         "\n"
                     ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/george/PycharmProjects/TileDB-ML/.venv/lib/python3.9/site-packages/tiledb/ctx.py:410: UserWarning: tiledb.default_ctx and scope_ctx will not function correctly due to bug in IPython contextvar support.  You must supply a Ctx object to each function for custom configuration options. Please consider upgrading to ipykernel >= 6!Please see https://github.com/TileDB-Inc/TileDB-Py/issues/667 for more information.\n",
-                        "  warnings.warn(\n"
-                    ]
                 }
             ],
             "source": [
                 "images_array = tiledb.open(training_images)\n",
                 "labels_array = tiledb.open(training_labels)\n",
                 "\n",
                 "print(images_array.schema)\n",
@@ -250,15 +354,15 @@
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "<matplotlib.image.AxesImage at 0x12de28bb0>"
+                        "text/plain": "<matplotlib.image.AxesImage at 0x123788ca0>"
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
@@ -301,28 +405,29 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Train Epoch: 1 Batch: 0 Loss: 2.299262\n",
-                        "Train Epoch: 1 Batch: 100 Loss: 2.262452\n",
-                        "Train Epoch: 1 Batch: 200 Loss: 2.162849\n",
-                        "Train Epoch: 1 Batch: 300 Loss: 1.927302\n",
-                        "Train Epoch: 1 Batch: 400 Loss: 1.646087\n",
-                        "Train Epoch: 2 Batch: 0 Loss: 1.446454\n",
-                        "Train Epoch: 2 Batch: 100 Loss: 1.314963\n",
-                        "Train Epoch: 2 Batch: 200 Loss: 1.376722\n",
-                        "Train Epoch: 2 Batch: 300 Loss: 1.400400\n",
-                        "Train Epoch: 2 Batch: 400 Loss: 1.291488\n"
+                        "Train Epoch: 1 Batch: 0 Loss: 2.304748\n",
+                        "Train Epoch: 1 Batch: 100 Loss: 2.277155\n",
+                        "Train Epoch: 1 Batch: 200 Loss: 2.203359\n",
+                        "Train Epoch: 1 Batch: 300 Loss: 1.895098\n",
+                        "Train Epoch: 1 Batch: 400 Loss: 1.497304\n",
+                        "Train Epoch: 2 Batch: 0 Loss: 1.435658\n",
+                        "Train Epoch: 2 Batch: 100 Loss: 1.305221\n",
+                        "Train Epoch: 2 Batch: 200 Loss: 0.990590\n",
+                        "Train Epoch: 2 Batch: 300 Loss: 1.103210\n",
+                        "Train Epoch: 2 Batch: 400 Loss: 0.903957\n"
                     ]
                 }
             ],
             "source": [
+                "import multiprocessing\n",
                 "import torch.nn as nn\n",
                 "import torch.optim as optim\n",
                 "\n",
                 "from tiledb.ml.readers.pytorch import PyTorchTileDBDataLoader\n",
                 "from tiledb.ml.readers.types import ArrayParams\n",
                 "\n",
                 "class Net(nn.Module):\n",
@@ -345,19 +450,23 @@
                 "\n",
                 "def do_random_noise(img, mag=0.1):\n",
                 "    noise = np.random.uniform(-1, 1,img.shape)*mag\n",
                 "    img = img + noise\n",
                 "    img = np.clip(img,0,1)\n",
                 "    return img\n",
                 "\n",
-                "\n",
                 "ctx = tiledb.Ctx({'sm.memory_budget': 1024**2})\n",
                 "with tiledb.open(training_images, ctx=ctx) as x, tiledb.open(training_labels, ctx=ctx) as y:\n",
+                "    # Because of this issue (https://github.com/pytorch/pytorch/issues/59451#issuecomment-854883855) we avoid using multiple workers on Jupyter.\n",
                 "    train_loader = PyTorchTileDBDataLoader(\n",
-                "        ArrayParams(x, fn=do_random_noise), ArrayParams(y), batch_size=128,\n",
+                "        ArrayParams(x, fn=do_random_noise),\n",
+                "        ArrayParams(y),\n",
+                "        batch_size=128,\n",
+                "        num_workers=0,\n",
+                "        shuffle_buffer_size=256,\n",
                 "    )\n",
                 "\n",
                 "    net = Net(shape=(28, 28))\n",
                 "    criterion = nn.CrossEntropyLoss()\n",
                 "    optimizer = optim.SGD(net.parameters(), lr=0.01, momentum=0.5)\n",
                 "\n",
                 "    for epoch in range(1, 3):\n",
@@ -370,31 +479,38 @@
                 "            loss = criterion(outputs, labels.to(torch.float).type(torch.LongTensor))\n",
                 "            loss.backward()\n",
                 "            optimizer.step()\n",
                 "            if batch_idx % 100 == 0:\n",
                 "                print('Train Epoch: {} Batch: {} Loss: {:.6f}'.format(\n",
                 "                epoch, batch_idx, loss.item()))"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.13"
+            "version": "3.9.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `tiledb-ml-0.9.2/examples/readers/pytorch_data_api_tiledb_sparse.ipynb` & `tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/readers/tensorflow_data_api_tiledb_dense.ipynb` & `tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_dense.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb` & `tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/setup.cfg` & `tiledb-ml-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/setup.py` & `tiledb-ml-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/models/test_cloud_utils.py` & `tiledb-ml-0.9.3/tests/models/test_cloud_utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/models/test_pytorch_models.py` & `tiledb-ml-0.9.3/tests/models/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/models/test_sklearn_models.py` & `tiledb-ml-0.9.3/tests/models/test_sklearn_models.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/models/test_tensorflow_keras_models.py` & `tiledb-ml-0.9.3/tests/models/test_tensorflow_keras_models.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/readers/test_pytorch.py` & `tiledb-ml-0.9.3/tests/readers/test_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,24 @@
     @pytest.mark.parametrize("shuffle_buffer_size", [0, 16])
     @pytest.mark.parametrize("num_workers", [0, 2])
     def test_dataloader(
         self, tmpdir, spec, batch_size, shuffle_buffer_size, num_workers
     ):
         def test(*all_array_params):
             try:
+                persistent_workers = num_workers > 0
+
                 dataloader = PyTorchTileDBDataLoader(
                     *all_array_params,
                     shuffle_buffer_size=shuffle_buffer_size,
                     batch_size=batch_size,
                     num_workers=num_workers,
+                    persistent_workers=persistent_workers,
                 )
+
             except NotImplementedError:
                 assert num_workers and (
                     torchdata.__version__ < "0.4"
                     or spec.tensor_kind is not TensorKind.DENSE
                 )
             else:
                 assert isinstance(dataloader, torch.utils.data.DataLoader)
```

### Comparing `tiledb-ml-0.9.2/tests/readers/test_pytorch_collators.py` & `tiledb-ml-0.9.3/tests/readers/test_pytorch_collators.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/readers/test_ranges.py` & `tiledb-ml-0.9.3/tests/readers/test_ranges.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/readers/test_tensor_schema.py` & `tiledb-ml-0.9.3/tests/readers/test_tensor_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,12 +163,14 @@
     schema = ArrayParams(array, key_dim, fields, dim_selectors).tensor_schema
     max_weight = schema.max_partition_weight
     key_ranges = list(schema.key_range.partition_by_weight(max_weight))
     for i, key_range in enumerate(key_ranges):
         # query succeeds without incomplete retries
         schema.query[key_range.min : key_range.max]
 
-        if i < len(key_ranges) - 1:
-            # querying a larger slice should fail
-            with pytest.raises(tiledb.TileDBError) as ex:
-                schema.query[key_range.min : key_ranges[i + 1].min]
-            assert "py.max_incomplete_retries" in str(ex.value)
+        # Check incomplete retries error only in the Sparse Case.
+        if type(array) is tiledb.SparseArray:
+            if i < len(key_ranges) - 1:
+                # querying a larger slice should fail
+                with pytest.raises(tiledb.TileDBError) as ex:
+                    schema.query[key_range.min : key_ranges[i + 1].min]
+                assert "py.max_incomplete_retries" in str(ex.value)
```

### Comparing `tiledb-ml-0.9.2/tests/readers/test_tensorflow.py` & `tiledb-ml-0.9.3/tests/readers/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tests/readers/utils.py` & `tiledb-ml-0.9.3/tests/readers/utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/_base.py` & `tiledb-ml-0.9.3/tiledb/ml/models/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,30 +79,30 @@
     def save(self, *, meta: Optional[Meta] = None) -> None:
         """Abstract method that saves a machine learning model as a TileDB array.
         :param meta: Extra metadata to save in a TileDB array.
         """
 
     @abstractmethod
     def load(self, *, timestamp: Optional[Timestamp] = None) -> Artifact:
-        """Abstract method that loads a machine learning model from a TileDB array.
+        """Abstract method that loads a machine learning model from a `TileDB` array.
 
         :param timestamp: Range of timestamps to load fragments of the array which live
             in the specified time range.
         """
 
     def get_weights(self, timestamp: Optional[Timestamp] = None) -> Weights:
         """
-        Returns model's weights. Works for Tensorflow Keras and PyTorch
+        Returns model's weights. Works for `Tensorflow Keras` and `PyTorch`
         """
         with tiledb.open(self.uri, ctx=self.ctx, timestamp=timestamp) as model_array:
             return cast(Weights, self._get_model_param(model_array, "model"))
 
     def get_optimizer_weights(self, timestamp: Optional[Timestamp] = None) -> Weights:
         """
-        Returns optimizer's weights. Works for Tensorflow Keras and PyTorch
+        Returns optimizer's weights. Works for `Tensorflow Keras` and `PyTorch`
         """
         with tiledb.open(self.uri, ctx=self.ctx, timestamp=timestamp) as model_array:
             return cast(Weights, self._get_model_param(model_array, "optimizer"))
 
     @abstractmethod
     def preview(self) -> str:
         """
```

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/_cloud_utils.py` & `tiledb-ml-0.9.3/tiledb/ml/models/_cloud_utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/_file_properties.py` & `tiledb-ml-0.9.3/tiledb/ml/models/_file_properties.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/pytorch.py` & `tiledb-ml-0.9.3/tiledb/ml/models/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 
 import tiledb
 
 from ._base import Meta, TileDBArtifact, Timestamp
 
 
 class PyTorchTileDBModel(TileDBArtifact[torch.nn.Module]):
-    """
-    Class that implements all functionality needed to save PyTorch models as
-    TileDB arrays and load PyTorch models from TileDB arrays.
+    """Class that implements all functionality needed to save `PyTorch` models as
+    `TileDB` arrays and load `PyTorch` models from `TileDB` arrays.
     """
 
     Name = "PYTORCH"
     Version = torch.__version__
 
     def __init__(
         self,
@@ -34,20 +33,19 @@
 
     def save(
         self,
         *,
         meta: Optional[Meta] = None,
         summary_writer: Optional[SummaryWriter] = None,
     ) -> None:
-        """
-        Save a PyTorch model as a TileDB array.
+        """Save a `PyTorch` model as a `TileDB` array.
 
         :param summary_writer:
-        :param meta: Extra metadata to save in a TileDB array.
-        :param summary_writer: Contains summary writer object for storing Tensorboard data.
+        :param meta: Extra metadata to save in a `TileDB` array.
+        :param summary_writer: Contains summary writer object for storing `Tensorboard` data.
         """
         if self.artifact is None:
             raise RuntimeError("Model is not initialized")
 
         # Serialize model state dictionary.
         serialized_model_dict = pickle.dumps(self.artifact.state_dict(), protocol=4)
 
@@ -76,22 +74,21 @@
         self,
         *,
         model: Optional[torch.nn.Module] = None,
         optimizer: Optional[Optimizer] = None,
         timestamp: Optional[Timestamp] = None,
         callback: bool = False,
     ) -> Any:
-        """
-        Load switch, i.e, decide between __load (TileDB-ML<=0.8.0) or __load_v2 (TileDB-ML>0.8.0).
+        """*Load switch, i.e, decide between __load (TileDB-ML<=0.8.0) or __load_v2 (TileDB-ML>0.8.0).*
 
-        :param model: A defined PyTorch model.
-        :param optimizer: A defined PyTorch optimizer.
+        :param model: A defined `PyTorch` model.
+        :param optimizer: A defined `PyTorch` optimizer.
         :param timestamp: Range of timestamps to load fragments of the array which live in the specified time range.
-        :param callback: Boolean variable if True will store Callback data into saved directory
-        :return: A dictionary with attributes other than model or optimizer state_dict.
+        :param callback: Boolean variable if `True` will store `Callback` data into saved directory
+        :return: A dictionary with attributes other than model or optimizer `state_dict`.
         """
         with tiledb.open(self.uri, ctx=self.ctx, timestamp=timestamp) as model_array:
             if self._use_legacy_schema(model_array):
                 return self.__load_legacy(model_array, model, optimizer, callback)
             else:
                 return self.__load(model_array, model, optimizer, callback)
 
@@ -154,13 +151,12 @@
         model.load_state_dict(self._get_model_param(model_array, "model"))
         if optimizer:
             optimizer.load_state_dict(self._get_model_param(model_array, "optimizer"))
         if callback:
             self._load_tensorboard(model_array)
 
     def preview(self) -> str:
-        """
-        Create a string representation of the model.
+        """Create a string representation of the model.
 
         :return: str. A string representation of the models internal configuration.
         """
         return str(self.artifact) if self.artifact else ""
```

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/sklearn.py` & `tiledb-ml-0.9.3/tiledb/ml/models/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         namespace: Optional[str] = None,
         ctx: Optional[tiledb.Ctx] = None,
         model: Optional[BaseEstimator] = None,
     ):
         super().__init__(uri, namespace, ctx, model)
 
     def save(self, *, meta: Optional[Meta] = None) -> None:
-        """
-        Save a Sklearn model as a TileDB array.
+        """Save a Sklearn model as a TileDB array.
 
         :param meta: Extra metadata to save in a TileDB array.
         """
         if self.artifact is None:
             raise RuntimeError("Model is not initialized")
 
         # Serialize model
@@ -45,18 +44,17 @@
         # Create TileDB model array
         if not tiledb.array_exists(uri=self.uri):
             self._create_array(fields=["model"])
 
         self._write_array(model_params={"model": serialized_model}, meta=meta)
 
     def load(self, *, timestamp: Optional[Timestamp] = None) -> BaseEstimator:
-        """
-        Load switch, i.e, decide between __load (TileDB-ML<=0.8.0) or __load_v2 (TileDB-ML>0.8.0).
-
+        """Load switch, i.e, decide between __load (TileDB-ML<=0.8.0) or __load_v2 (TileDB-ML>0.8.0).
         Load a Sklearn model from a TileDB array.
+
         :param timestamp: Range of timestamps to load fragments of the array which live
             in the specified time range.
         :return: A Sklearn model object.
         """
         with tiledb.open(self.uri, ctx=self.ctx, timestamp=timestamp) as model_array:
             if self._use_legacy_schema(model_array):
                 return self.__load_legacy(model_array)
@@ -67,28 +65,26 @@
     def __load_legacy(model_array: tiledb.Array) -> BaseEstimator:
         return pickle.loads(model_array[:]["model_params"].item(0))
 
     def __load(self, model_array: tiledb.Array) -> BaseEstimator:
         return self._get_model_param(model_array, "model")
 
     def preview(self, *, display: str = "text") -> str:
-        """
-        Create a text representation of the model.
+        """Create a text representation of the model.
 
-        :param display. If ‘diagram’, estimators will be displayed as a diagram in an
+        :param display: If ‘diagram’, estimators will be displayed as a diagram in an
             HTML format when shown in a jupyter notebook. If ‘text’, estimators will be
             displayed as text.
-        :return. A string representation of the models internal configuration.
+        :return: A string representation of the models internal configuration.
         """
         if self.artifact:
             with config_context(display=display):
                 return str(self.artifact)
         else:
             return ""
 
     def _serialize_model(self) -> bytes:
-        """
-        Serialize a Sklearn model with pickle.
+        """Serialize a Sklearn model with pickle.
 
         :return: Pickled Sklearn model.
         """
         return pickle.dumps(self.artifact, protocol=4)
```

### Comparing `tiledb-ml-0.9.2/tiledb/ml/models/tensorflow_keras.py` & `tiledb-ml-0.9.3/tiledb/ml/models/tensorflow_keras.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_pytorch_collators.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_pytorch_collators.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/__init__.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/base.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/base_sparse.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base_sparse.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/dense.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/dense.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/mapped.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/mapped.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/query.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/query.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/ragged.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ragged.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/ranges.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ranges.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/sparse.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/pytorch.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,22 @@
     shuffle_buffer_size: int = 0,
     **kwargs: Any,
 ) -> DataLoader:
     """Return a DataLoader for loading data from TileDB arrays.
 
     :param all_array_params: One or more `ArrayParams` instances, one per TileDB array.
     :param shuffle_buffer_size: Number of elements from which this dataset will sample.
-    **kwargs: Should contain all parameters for PyTorch Dataloader. At the moment TileDB-ML can support ONLY the
-    following PyTorch Dataloader arguments:
-        batch_size: How many samples per batch to load (default: ``1``).
-        prefetch_factor: Number of batches loaded in advance by each worker. Not applicable (and should not be
-        given) when `num_workers` is 0.
-        num_workers: How many subprocesses to use for data loading. 0 means that the data will be loaded in the main
-        process. Note: when `num_workers` > 1 yielded batches may be shuffled even if `shuffle_buffer_size` is zero.
-        persistent_workers: If ``True``, the data loader will not shutdown the worker processes after a dataset has
-        been consumed once. This allows to maintain the workers `Dataset` instances alive. (default: ``False``)
-        timeout: if positive, the timeout value for collecting a batch from workers. Should always be non-negative.
-        (default: ``0``)
-        drop_last: Set to ``True`` to drop the last incomplete batch, if the dataset size is not divisible by the
-        batch size. If ``False`` and the size of dataset is not divisible by the batch size, then the last batch
-        will be smaller. (default: ``False``)
+
+    Keyword Args:  Contains all parameters for PyTorch Dataloader.
+        - batch_size: How many samples per batch to load (default: ``1``).
+        - prefetch_factor: Number of batches loaded in advance by each worker. Not applicable (and should not be given) when `num_workers` is 0.
+        - num_workers: How many subprocesses to use for data loading. 0 means that the data will be loaded in the main process. Note: when `num_workers` > 1 yielded batches may be shuffled even if `shuffle_buffer_size` is zero.
+        - persistent_workers: If ``True``, the data loader will not shutdown the worker processes after a dataset has been consumed once. This allows to maintain the workers `Dataset` instances alive. (default: ``False``)
+        - timeout: if positive, the timeout value for collecting a batch from workers. Should always be non-negative. (default: ``0``)
+        - drop_last: Set to ``True`` to drop the last incomplete batch, if the dataset size is not divisible by the batch size. If ``False`` and the size of dataset is not divisible by the batch size, then the last batch will be smaller. (default: ``False``)
 
     Users should NOT pass (TileDB-ML either doesn't support or implements internally the corresponding functionality)
     the following arguments: 'shuffle', 'sampler', 'batch_sampler', 'worker_init_fn' and 'collate_fn'.
     """
     is_batched = kwargs.get("batch_size", 1) is not None
 
     schemas = []
@@ -85,25 +79,16 @@
         datapipe = datapipe.flatmap(datapipe_for_key_range)
     else:
         # create a datapipe that reads and unbatches the tensors for the whole key range
         datapipe = datapipe_for_key_range(key_range=key_range)
 
     # shuffle the unbatched rows if shuffle_buffer_size > 0
     if shuffle_buffer_size:
-        # load the rows to be shuffled
-        # don't batch them (batch_size=None) or collate them (collate_fn=_identity)
-        row_loader = DataLoader(
-            datapipe, num_workers=num_workers, batch_size=None, collate_fn=_identity
-        )
-        # create a new datapipe for these rows
-        datapipe = DeferredIterableIterDataPipe(iter, row_loader)
         # shuffle the datapipe items
         datapipe = datapipe.shuffle(buffer_size=shuffle_buffer_size)
-        # run the shuffling on this process, not on workers
-        kwargs["num_workers"] = 0
 
     # construct an appropriate collate function
     collator = Collator.from_schemas(*schemas)
     kwargs["collate_fn"] = collator.collate if is_batched else collator.convert
 
     # return the DataLoader for the final datapipe
     return DataLoader(datapipe, **kwargs)
@@ -125,15 +110,14 @@
 
 def _get_unbatched_datapipe(
     key_range: InclusiveRange[Any, int],
     schemas: Sequence[TensorSchema[TensorLike]],
     map_fns: Sequence[Union[Callable, None]],
 ) -> IterDataPipe[Union[TensorLikeOrTuple, Tuple[TensorLikeOrTuple, ...]]]:
     """Return a datapipe over unbatched rows for the given schemas and key range.
-
     If `len(schemas) == 1`, each item of the datapipe is either a single `TensorLike`
     or a sequence of `TensorLike`s, depending on `schemas[0].num_fields`.
     If `len(schemas) > 1`, each item of the datapipe is a tuple of (`TensorLike` or
     sequence of `TensorLike`s, depending on `schema.num_fields`), one for each schema.
     """
     schema_dps = [
         DeferredIterableIterDataPipe(_unbatch_tensors, schema, key_range).map(
@@ -151,15 +135,14 @@
 
 def _unbatch_tensors(
     schema: TensorSchema[TensorLike], key_range: InclusiveRange[Any, int]
 ) -> Iterator[TensorLikeOrTuple]:
     """
     Generate batches of `TensorLike`s for the given schema and key range and then unbatch
     them into single "rows".
-
     If `schema.num_fields == 1`, each "row" is a single `TensorLike`
     If `schema.num_fields > 1`, each "row" is a sequence of `TensorLike`s
     """
     batches = schema.iter_tensors(
         key_range.partition_by_weight(schema.max_partition_weight)
     )
     if schema.num_fields > 1:
```

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/tensorflow.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/tensorflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 Tensor = Union[np.ndarray, tf.SparseTensor]
 
 
 def TensorflowTileDBDataset(
     *all_array_params: ArrayParams,
     num_workers: int = 0,
 ) -> tf.data.Dataset:
-    """Return a tf.data.Dataset for loading data from TileDB arrays.
+    """
+    Return a tf.data.Dataset for loading data from TileDB arrays.
+
     :param all_array_params: One or more `ArrayParams` instances, one per TileDB array.
     :param num_workers: If greater than zero, create a threadpool of `num_workers` threads
         used to fetch inputs asynchronously and in parallel.
     """
     schemas = []
     for array_params in all_array_params:
         schema = array_params.tensor_schema
```

### Comparing `tiledb-ml-0.9.2/tiledb/ml/readers/types.py` & `tiledb-ml-0.9.3/tiledb/ml/readers/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,37 +9,34 @@
 if TYPE_CHECKING:
     from ._tensor_schema import TensorSchema
 
 Selector = Union[slice, Sequence[int]]
 
 
 class TensorKind(enum.Enum):
-    """Kind of tensor."""
+    """Kind of tensor"""
 
     DENSE = enum.auto()
     SPARSE_COO = enum.auto()
     SPARSE_CSR = enum.auto()
     RAGGED = enum.auto()
 
 
 @dataclass(frozen=True)
 class ArrayParams:
     """
     Data class specifying the parameters for loading tensors from a TileDB array.
 
-    Public attributes:
-    - array: TileDB array to be accessed
-    - key_dim: Name (or index) of the array key dimension. Defaults to the first dimension.
-    - fields: Fields (dimensions and attributes) to be retrieved from array. Defaults to
-      all attributes of the array.
-    - dim_selectors: Mapping from dimension name to a slice or sequence of indices of this
-      dimension to select.
-    - tensor_kind: kind of tensor desired. If not specified, it is determined based on the
-      array schema.
-    - fn: Function being applied over each item.
+    Attributes:
+        - **array:** TileDB array to be accessed
+        - **key_dim:** Name (or index) of the array key dimension. Defaults to the first dimension.
+        - **fields:** Fields (dimensions and attributes) to be retrieved from array. Defaults to all attributes of the array.
+        - **dim_selectors:** Mapping from dimension name to a slice or sequence of indices of this dimension to select.
+        - **tensor_kind:** kind of tensor desired. If not specified, it is determined based on the array schema.
+        - **fn:** Function being applied over each item.
     """
 
     array: tiledb.Array
     key_dim: Union[int, str] = 0
     fields: Sequence[str] = ()
     dim_selectors: Mapping[str, Selector] = field(default_factory=dict)
     tensor_kind: Optional[TensorKind] = None
```

### Comparing `tiledb-ml-0.9.2/tiledb_ml.egg-info/PKG-INFO` & `tiledb-ml-0.9.3/tiledb_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-ml
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package supports all machine learning functionality for TileDB Embedded and TileDB Cloud
 Home-page: https://github.com/TileDB-Inc/TileDB-ML
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TileDB-Inc/TileDB-ML/issues
 Project-URL: Documentation, https://docs.tiledb.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.2 Summary: Package supports
+Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.3 Summary: Package supports
 all machine learning functionality for TileDB Embedded and TileDB Cloud Home-
 page: https://github.com/TileDB-Inc/TileDB-ML Author: TileDB, Inc. Author-
 email: help@tiledb.io License: MIT Project-URL: Bug Tracker, https://
 github.com/TileDB-Inc/TileDB-ML/issues Project-URL: Documentation, https://
 docs.tiledb.com Keywords: tiledb,ml Platform: any Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
```

### Comparing `tiledb-ml-0.9.2/tiledb_ml.egg-info/SOURCES.txt` & `tiledb-ml-0.9.3/tiledb_ml.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 README.md
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
 .github/workflows/release.yml
+docs/Makefile
+docs/conf.py
+docs/index.rst
+docs/make.bat
+docs/modules.rst
+docs/tiledb.ml.models.rst
+docs/tiledb.ml.readers.rst
+docs/tiledb.ml.rst
+docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png
+docs/_static/custom.css
+docs/_static/favicon.ico
+docs/_static/tiledb-logo_color_no_margin_@4x.png
 examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb
 examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb
 examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb
 examples/cloud/serverless_training/pytorch/README.md
 examples/cloud/serverless_training/pytorch/data_ingestion.py
 examples/cloud/serverless_training/pytorch/model_load_and_predict.py
 examples/cloud/serverless_training/pytorch/model_training.py
```

