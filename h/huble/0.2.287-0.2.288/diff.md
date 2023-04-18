# Comparing `tmp/huble-0.2.287.tar.gz` & `tmp/huble-0.2.288.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huble-0.2.287.tar", max compression
+gzip compressed data, was "huble-0.2.288.tar", max compression
```

## Comparing `huble-0.2.287.tar` & `huble-0.2.288.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.287/README.md
--rw-r--r--   0        0        0      684 2023-04-18 09:58:43.376142 huble-0.2.287/pyproject.toml
--rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.287/src/huble/__init__.py
--rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.287/src/huble/automl/__init__.py
--rw-r--r--   0        0        0     5002 2023-04-17 11:57:46.692196 huble-0.2.287/src/huble/automl/automl.py
--rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.287/src/huble/connector/__init__.py
--rw-r--r--   0        0        0      569 2023-04-18 09:58:29.285907 huble-0.2.287/src/huble/connector/dataset.py
--rw-r--r--   0        0        0     1575 2023-04-18 09:28:46.847827 huble-0.2.287/src/huble/connector/deployment.py
--rw-r--r--   0        0        0     1925 2023-04-18 09:27:53.123802 huble-0.2.287/src/huble/connector/experiment.py
--rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.287/src/huble/error/__init__.py
--rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.287/src/huble/error/decorators.py
--rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.287/src/huble/error/exceptions.py
--rw-r--r--   0        0        0      447 2023-04-18 09:17:59.948453 huble-0.2.287/src/huble/main.py
--rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.287/src/huble/sklearn/__init__.py
--rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.287/src/huble/sklearn/essentials/__init__.py
--rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.287/src/huble/sklearn/essentials/essentail_params.ts
--rw-r--r--   0        0        0     1264 2023-04-18 09:20:57.986135 huble-0.2.287/src/huble/sklearn/essentials/function.py
--rw-r--r--   0        0        0     1009 2023-04-18 09:18:48.801995 huble-0.2.287/src/huble/sklearn/essentials/handler.py
--rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.287/src/huble/sklearn/evaluate.py
--rw-r--r--   0        0        0     3475 2023-04-18 09:29:15.541539 huble-0.2.287/src/huble/sklearn/generate.py
--rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.287/src/huble/sklearn/graph.py
--rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.287/src/huble/sklearn/metrics/__init__.py
--rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.287/src/huble/sklearn/metrics/metrics.py
--rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.287/src/huble/sklearn/process/__init__.py
--rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.287/src/huble/sklearn/process/functions.py
--rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.287/src/huble/sklearn/process/handler.py
--rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.287/src/huble/sklearn/process/preprocess_params.ts
--rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.287/src/huble/sklearn/train/__init__.py
--rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.287/src/huble/sklearn/train/functions.py
--rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.287/src/huble/sklearn/train/handler.py
--rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.287/src/huble/sklearn/train/model_params.ts
--rw-r--r--   0        0        0      304 2023-04-17 11:56:37.991446 huble-0.2.287/src/huble/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.287/src/huble/util/convert_to_reactflow_graph.py
--rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.287/src/huble/util/data_types.py
--rw-r--r--   0        0        0      898 2023-04-17 11:56:37.991446 huble-0.2.287/src/huble/util/feature_selection.py
--rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.287/src/huble/util/inference_pipeline.py
--rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.287/src/huble/util/recommend_model.py
--rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.287/src/huble/util/typed_params.py
--rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.287/src/huble/util/verify_builder_pipeline.py
--rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.287/src/huble/util/verify_ml.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.287/setup.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.287/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.288/README.md
+-rw-r--r--   0        0        0      684 2023-04-18 10:13:32.981027 huble-0.2.288/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.288/src/huble/__init__.py
+-rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.288/src/huble/automl/__init__.py
+-rw-r--r--   0        0        0     5002 2023-04-17 11:57:46.692196 huble-0.2.288/src/huble/automl/automl.py
+-rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.288/src/huble/connector/__init__.py
+-rw-r--r--   0        0        0      587 2023-04-18 10:13:25.574236 huble-0.2.288/src/huble/connector/dataset.py
+-rw-r--r--   0        0        0     1575 2023-04-18 09:28:46.847827 huble-0.2.288/src/huble/connector/deployment.py
+-rw-r--r--   0        0        0     1925 2023-04-18 09:27:53.123802 huble-0.2.288/src/huble/connector/experiment.py
+-rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.288/src/huble/error/__init__.py
+-rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.288/src/huble/error/decorators.py
+-rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.288/src/huble/error/exceptions.py
+-rw-r--r--   0        0        0      447 2023-04-18 09:17:59.948453 huble-0.2.288/src/huble/main.py
+-rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.288/src/huble/sklearn/__init__.py
+-rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.288/src/huble/sklearn/essentials/__init__.py
+-rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.288/src/huble/sklearn/essentials/essentail_params.ts
+-rw-r--r--   0        0        0     1264 2023-04-18 09:20:57.986135 huble-0.2.288/src/huble/sklearn/essentials/function.py
+-rw-r--r--   0        0        0     1009 2023-04-18 09:18:48.801995 huble-0.2.288/src/huble/sklearn/essentials/handler.py
+-rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.288/src/huble/sklearn/evaluate.py
+-rw-r--r--   0        0        0     3475 2023-04-18 09:29:15.541539 huble-0.2.288/src/huble/sklearn/generate.py
+-rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.288/src/huble/sklearn/graph.py
+-rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.288/src/huble/sklearn/metrics/__init__.py
+-rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.288/src/huble/sklearn/metrics/metrics.py
+-rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.288/src/huble/sklearn/process/__init__.py
+-rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.288/src/huble/sklearn/process/functions.py
+-rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.288/src/huble/sklearn/process/handler.py
+-rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.288/src/huble/sklearn/process/preprocess_params.ts
+-rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.288/src/huble/sklearn/train/__init__.py
+-rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.288/src/huble/sklearn/train/functions.py
+-rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.288/src/huble/sklearn/train/handler.py
+-rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.288/src/huble/sklearn/train/model_params.ts
+-rw-r--r--   0        0        0      304 2023-04-17 11:56:37.991446 huble-0.2.288/src/huble/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.288/src/huble/util/convert_to_reactflow_graph.py
+-rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.288/src/huble/util/data_types.py
+-rw-r--r--   0        0        0      898 2023-04-17 11:56:37.991446 huble-0.2.288/src/huble/util/feature_selection.py
+-rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.288/src/huble/util/inference_pipeline.py
+-rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.288/src/huble/util/recommend_model.py
+-rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.288/src/huble/util/typed_params.py
+-rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.288/src/huble/util/verify_builder_pipeline.py
+-rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.288/src/huble/util/verify_ml.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.288/setup.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.288/PKG-INFO
```

### Comparing `huble-0.2.287/pyproject.toml` & `huble-0.2.288/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huble"
-version = "0.2.287"
+version = "0.2.288"
 description = ""
 authors = ["Rugz007 <rugvedsomwanshi007@gmail.com>"]
 maintainers = [
     "Arjit Agarwal <arjitagarwal123@gmail.com>",
     "Ashmika Gupte <ashmikagupte01@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `huble-0.2.287/src/huble/automl/automl.py` & `huble-0.2.288/src/huble/automl/automl.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/connector/dataset.py` & `huble-0.2.288/src/huble/connector/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pandas as pd
 import boto3
 from ..util.data_types import get_dataframe_types
 import boto3
 
 
 class Dataset:
-    def __init__(self, file_name) -> None:
-        self.file_name = file_name
-        self.dataframe = self.__load_dataset(file_name)
+    def __init__(self, url) -> None:
+        self.file_name = url
+        self.dataframe = self.__load_dataset(url)
 
-    def __load_dataset(self, file_name: str) -> pd.DataFrame:
-        return pd.read_csv("https://const-bucket.s3.ap-south-1.amazonaws.com/" + file_name)
+    def __load_dataset(self, url: str) -> pd.DataFrame:
+        print("Loading dataset from S3: ", url)
+        return pd.read_csv("https://const-bucket.s3.ap-south-1.amazonaws.com/" + url)
 
     def parse_dataset(self):
         data_dict = get_dataframe_types(self.dataframe)
         data_dict["rows"] = len(self.dataframe.axes[0])
         return data_dict
```

### Comparing `huble-0.2.287/src/huble/connector/deployment.py` & `huble-0.2.288/src/huble/connector/deployment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/connector/experiment.py` & `huble-0.2.288/src/huble/connector/experiment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/error/decorators.py` & `huble-0.2.288/src/huble/error/decorators.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/error/exceptions.py` & `huble-0.2.288/src/huble/error/exceptions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/essentials/essentail_params.ts` & `huble-0.2.288/src/huble/sklearn/essentials/essentail_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/essentials/function.py` & `huble-0.2.288/src/huble/sklearn/essentials/function.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/essentials/handler.py` & `huble-0.2.288/src/huble/sklearn/essentials/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/evaluate.py` & `huble-0.2.288/src/huble/sklearn/evaluate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/generate.py` & `huble-0.2.288/src/huble/sklearn/generate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/graph.py` & `huble-0.2.288/src/huble/sklearn/graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/metrics/metrics.py` & `huble-0.2.288/src/huble/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/process/__init__.py` & `huble-0.2.288/src/huble/sklearn/process/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/process/functions.py` & `huble-0.2.288/src/huble/sklearn/process/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/process/handler.py` & `huble-0.2.288/src/huble/sklearn/process/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/process/preprocess_params.ts` & `huble-0.2.288/src/huble/sklearn/process/preprocess_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/train/__init__.py` & `huble-0.2.288/src/huble/sklearn/train/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/train/functions.py` & `huble-0.2.288/src/huble/sklearn/train/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/train/handler.py` & `huble-0.2.288/src/huble/sklearn/train/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/sklearn/train/model_params.ts` & `huble-0.2.288/src/huble/sklearn/train/model_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/convert_to_reactflow_graph.py` & `huble-0.2.288/src/huble/util/convert_to_reactflow_graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/data_types.py` & `huble-0.2.288/src/huble/util/data_types.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/feature_selection.py` & `huble-0.2.288/src/huble/util/feature_selection.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/inference_pipeline.py` & `huble-0.2.288/src/huble/util/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/typed_params.py` & `huble-0.2.288/src/huble/util/typed_params.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/verify_builder_pipeline.py` & `huble-0.2.288/src/huble/util/verify_builder_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/src/huble/util/verify_ml.py` & `huble-0.2.288/src/huble/util/verify_ml.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.287/setup.py` & `huble-0.2.288/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'pandas>=1.3.5,<2.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'scikit-learn==1.1.2',
  'scipy>=1.7.0,<1.8.0']
 
 setup_kwargs = {
     'name': 'huble',
-    'version': '0.2.287',
+    'version': '0.2.288',
     'description': '',
     'long_description': '',
     'author': 'Rugz007',
     'author_email': 'rugvedsomwanshi007@gmail.com',
     'maintainer': 'Arjit Agarwal',
     'maintainer_email': 'arjitagarwal123@gmail.com',
     'url': 'None',
```

### Comparing `huble-0.2.287/PKG-INFO` & `huble-0.2.288/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huble
-Version: 0.2.287
+Version: 0.2.288
 Summary: 
 Author: Rugz007
 Author-email: rugvedsomwanshi007@gmail.com
 Maintainer: Arjit Agarwal
 Maintainer-email: arjitagarwal123@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: Programming Language :: Python :: 3
```

