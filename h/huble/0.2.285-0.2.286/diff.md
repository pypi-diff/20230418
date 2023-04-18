# Comparing `tmp/huble-0.2.285.tar.gz` & `tmp/huble-0.2.286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huble-0.2.285.tar", max compression
+gzip compressed data, was "huble-0.2.286.tar", max compression
```

## Comparing `huble-0.2.285.tar` & `huble-0.2.286.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.285/README.md
--rw-r--r--   0        0        0      684 2023-04-17 12:40:41.774829 huble-0.2.285/pyproject.toml
--rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.285/src/huble/__init__.py
--rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.285/src/huble/automl/__init__.py
--rw-r--r--   0        0        0     5002 2023-04-17 11:57:46.692196 huble-0.2.285/src/huble/automl/automl.py
--rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.285/src/huble/connector/__init__.py
--rw-r--r--   0        0        0      651 2023-04-17 12:36:32.151630 huble-0.2.285/src/huble/connector/dataset.py
--rw-r--r--   0        0        0     1564 2023-02-04 14:11:21.308460 huble-0.2.285/src/huble/connector/deployment.py
--rw-r--r--   0        0        0     2499 2023-02-17 05:24:53.511354 huble-0.2.285/src/huble/connector/experiment.py
--rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.285/src/huble/error/__init__.py
--rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.285/src/huble/error/decorators.py
--rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.285/src/huble/error/exceptions.py
--rw-r--r--   0        0        0      421 2023-02-04 12:16:33.294928 huble-0.2.285/src/huble/main.py
--rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.285/src/huble/sklearn/__init__.py
--rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.285/src/huble/sklearn/essentials/__init__.py
--rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.285/src/huble/sklearn/essentials/essentail_params.ts
--rw-r--r--   0        0        0     1269 2023-04-17 11:56:37.991446 huble-0.2.285/src/huble/sklearn/essentials/function.py
--rw-r--r--   0        0        0      983 2023-04-17 12:07:07.254917 huble-0.2.285/src/huble/sklearn/essentials/handler.py
--rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.285/src/huble/sklearn/evaluate.py
--rw-r--r--   0        0        0     3466 2023-02-24 09:49:44.133824 huble-0.2.285/src/huble/sklearn/generate.py
--rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.285/src/huble/sklearn/graph.py
--rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.285/src/huble/sklearn/metrics/__init__.py
--rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.285/src/huble/sklearn/metrics/metrics.py
--rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.285/src/huble/sklearn/process/__init__.py
--rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.285/src/huble/sklearn/process/functions.py
--rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.285/src/huble/sklearn/process/handler.py
--rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.285/src/huble/sklearn/process/preprocess_params.ts
--rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.285/src/huble/sklearn/train/__init__.py
--rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.285/src/huble/sklearn/train/functions.py
--rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.285/src/huble/sklearn/train/handler.py
--rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.285/src/huble/sklearn/train/model_params.ts
--rw-r--r--   0        0        0      304 2023-04-17 11:56:37.991446 huble-0.2.285/src/huble/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.285/src/huble/util/convert_to_reactflow_graph.py
--rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.285/src/huble/util/data_types.py
--rw-r--r--   0        0        0      898 2023-04-17 11:56:37.991446 huble-0.2.285/src/huble/util/feature_selection.py
--rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.285/src/huble/util/inference_pipeline.py
--rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.285/src/huble/util/recommend_model.py
--rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.285/src/huble/util/typed_params.py
--rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.285/src/huble/util/verify_builder_pipeline.py
--rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.285/src/huble/util/verify_ml.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.285/setup.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.285/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.286/README.md
+-rw-r--r--   0        0        0      684 2023-04-18 09:29:22.948304 huble-0.2.286/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.286/src/huble/__init__.py
+-rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.286/src/huble/automl/__init__.py
+-rw-r--r--   0        0        0     5002 2023-04-17 11:57:46.692196 huble-0.2.286/src/huble/automl/automl.py
+-rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.286/src/huble/connector/__init__.py
+-rw-r--r--   0        0        0      654 2023-04-17 13:39:21.408744 huble-0.2.286/src/huble/connector/dataset.py
+-rw-r--r--   0        0        0     1575 2023-04-18 09:28:46.847827 huble-0.2.286/src/huble/connector/deployment.py
+-rw-r--r--   0        0        0     1925 2023-04-18 09:27:53.123802 huble-0.2.286/src/huble/connector/experiment.py
+-rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.286/src/huble/error/__init__.py
+-rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.286/src/huble/error/decorators.py
+-rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.286/src/huble/error/exceptions.py
+-rw-r--r--   0        0        0      447 2023-04-18 09:17:59.948453 huble-0.2.286/src/huble/main.py
+-rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.286/src/huble/sklearn/__init__.py
+-rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.286/src/huble/sklearn/essentials/__init__.py
+-rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.286/src/huble/sklearn/essentials/essentail_params.ts
+-rw-r--r--   0        0        0     1264 2023-04-18 09:20:57.986135 huble-0.2.286/src/huble/sklearn/essentials/function.py
+-rw-r--r--   0        0        0     1009 2023-04-18 09:18:48.801995 huble-0.2.286/src/huble/sklearn/essentials/handler.py
+-rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.286/src/huble/sklearn/evaluate.py
+-rw-r--r--   0        0        0     3475 2023-04-18 09:29:15.541539 huble-0.2.286/src/huble/sklearn/generate.py
+-rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.286/src/huble/sklearn/graph.py
+-rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.286/src/huble/sklearn/metrics/__init__.py
+-rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.286/src/huble/sklearn/metrics/metrics.py
+-rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.286/src/huble/sklearn/process/__init__.py
+-rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.286/src/huble/sklearn/process/functions.py
+-rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.286/src/huble/sklearn/process/handler.py
+-rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.286/src/huble/sklearn/process/preprocess_params.ts
+-rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.286/src/huble/sklearn/train/__init__.py
+-rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.286/src/huble/sklearn/train/functions.py
+-rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.286/src/huble/sklearn/train/handler.py
+-rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.286/src/huble/sklearn/train/model_params.ts
+-rw-r--r--   0        0        0      304 2023-04-17 11:56:37.991446 huble-0.2.286/src/huble/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.286/src/huble/util/convert_to_reactflow_graph.py
+-rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.286/src/huble/util/data_types.py
+-rw-r--r--   0        0        0      898 2023-04-17 11:56:37.991446 huble-0.2.286/src/huble/util/feature_selection.py
+-rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.286/src/huble/util/inference_pipeline.py
+-rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.286/src/huble/util/recommend_model.py
+-rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.286/src/huble/util/typed_params.py
+-rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.286/src/huble/util/verify_builder_pipeline.py
+-rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.286/src/huble/util/verify_ml.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.286/setup.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.286/PKG-INFO
```

### Comparing `huble-0.2.285/pyproject.toml` & `huble-0.2.286/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huble"
-version = "0.2.285"
+version = "0.2.286"
 description = ""
 authors = ["Rugz007 <rugvedsomwanshi007@gmail.com>"]
 maintainers = [
     "Arjit Agarwal <arjitagarwal123@gmail.com>",
     "Ashmika Gupte <ashmikagupte01@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `huble-0.2.285/src/huble/automl/automl.py` & `huble-0.2.286/src/huble/automl/automl.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/connector/dataset.py` & `huble-0.2.286/src/huble/connector/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, url) -> None:
         self.url = url
         self.dataframe = self.__load_dataset(url)
 
     def __load_dataset(self, url: str) -> pd.DataFrame:
         bucket = "const-bucket"
         file_name = url.split("/")[-1]
-        s3 = boto3.client('s3') 
+        s3 = boto3.client('s3',{}) 
         obj = s3.get_object(Bucket= bucket, Key= file_name)
         return pd.read_csv(obj['Body'])
 
     def parse_dataset(self):
         data_dict = get_dataframe_types(self.dataframe)
         data_dict["rows"] = len(self.dataframe.axes[0])
         return data_dict
```

### Comparing `huble-0.2.285/src/huble/connector/deployment.py` & `huble-0.2.286/src/huble/connector/deployment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import requests
 from .experiment import Experiment
 
 class Deployment:
 
     def generate_code(self, experiment_id: str):
         experiment = Experiment(experiment_id=experiment_id)
         with open("deployment.py", "w") as f:
             f.write("import requests")
             f.write("\nimport os")
             f.write("\nimport pandas as pd")
             f.write("\nfrom pydantic import BaseModel")
-            f.write("\nfrom huble import Experiment")
+            f.write("\nfrom huble import Experiment,Dataset")
             f.write("\nfrom typing import Union")
             f.write("\nimport joblib")
             f.write("\nexperiment_id = os.getenv(\"EXPERIMENT_ID\")")
             f.write(f"\nexperiment = Experiment(experiment_id)")
             f.write("\n")
             f.write("\nclass RequestBody(BaseModel):")
             for column in experiment.input_format["columns"]:
               if(column['name'] != "index"):
                 f.write(f"\n\t{column['name']}: Union[int, float]")
             f.write("\n")
             f.write(f"\nmodel_url = experiment.modelURL")
-            f.write('\nmodel_content = requests.get(f"https://ipfs.filebase.io/ipfs/{model_url}")')
+            f.write('\nmodel_content = requests.get(f"https://const-bucket.s3.ap-south-1.amazonaws.com/{model_url}")')
             f.write("\nopen('model.joblib', 'wb').write(model_content.content)")
             f.write("\nmodel = joblib.load('model.joblib')")
             f.write("\n")
             f.write("\n")
             f.write("\ndef predict(request_body: RequestBody):")
             f.write("\n\trequest_body = request_body.dict()")
             f.write("\n\tX = pd.DataFrame(request_body, index=[0])")
```

### Comparing `huble-0.2.285/src/huble/error/decorators.py` & `huble-0.2.286/src/huble/error/decorators.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/error/exceptions.py` & `huble-0.2.286/src/huble/error/exceptions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/essentials/essentail_params.ts` & `huble-0.2.286/src/huble/sklearn/essentials/essentail_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/essentials/function.py` & `huble-0.2.286/src/huble/sklearn/essentials/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 from ...util.data_types import get_dataframe_types
 from ...util.feature_selection import select_features
 
 # @function_error_handling("train_test_split")
 def train_test_split(**params):
     data = params["data"]
     target = params["target_column"]
-    model=params['model']
+    model = params["model"]
     X = data.drop([target], axis=1)
     data_dict = get_dataframe_types(X)
     data = select_features(data, target, model)
-    train_dataset, test_dataset = sklearn_tts(
-        data, test_size=params["parameters"]["test_size"], random_state=42
-    )
+    train_dataset, test_dataset = sklearn_tts(data, test_size=params["parameters"]["test_size"], random_state=42)
     return train_dataset, test_dataset, data_dict
 
 
 # @function_error_handling("train_model")
 def train_model(**params):
-    task_type = params['task_type']
+    task_type = params["task_type"]
     data = params["data"]
     model = params["model"]
-    if task_type=='clustering':
+    if task_type == "clustering":
         Model = model.fit(data)
-    else:        
+    else:
         y = data[params["column"]]
         X = data.drop(params["column"], axis=1)
- 
+
         Model = model.fit(X, y)
-    filename = 'model.joblib'
+    filename = f'model-{params["id"]}.joblib'
     joblib.dump(Model, filename)
     return Model, filename
```

### Comparing `huble-0.2.285/src/huble/sklearn/essentials/handler.py` & `huble-0.2.286/src/huble/sklearn/essentials/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 class EssentialsHandler:
     def __init__(self) -> None:
         pass
 
-    def return_function(self, function_name: str, params: dict, task_type: str, target_column: str):
+    def return_function(self, function_name: str, params: dict, task_type: str, target_column: str,id:str):
 
         essentials = {
             "Train-Test Split": self.__train_test_split,
             "Train Model": self.__train_model,
         }
-        return essentials[function_name](params=params, task_type=task_type, target_column=target_column)
+        return essentials[function_name](params=params, task_type=task_type, target_column=target_column,id=id)
 
     def __train_test_split(self, params, target_column, **kwargs):
         parameters = {
             "test_size": params["test_size"],
         }
         return f"training_dataset, test_dataset, input_format = huble.sklearn.train_test_split(data=data,parameters={parameters}, target_column='{target_column}, model=model')"
 
-    def __train_model(self, params, task_type, target_column, **kwargs):
-        return f"Model, filename = huble.sklearn.train_model(data=training_dataset, model=model, column='{target_column}', task_type='{task_type}')"
+    def __train_model(self, params, task_type, target_column,id, **kwargs):
+        return f"Model, filename = huble.sklearn.train_model(data=training_dataset, model=model, column='{target_column}', task_type='{task_type}',id='{id}')"
```

### Comparing `huble-0.2.285/src/huble/sklearn/evaluate.py` & `huble-0.2.286/src/huble/sklearn/evaluate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/generate.py` & `huble-0.2.286/src/huble/sklearn/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .process.handler import PreprocessHandler
 from .train.handler import ModelHandler
 from .essentials.handler import EssentialsHandler
 from .graph import Graph
 from ..util import get_typed_params
 
 
-def generate_file(graph, target_column, task_type, colab=False):
+def generate_file(graph, target_column, task_type,id, colab=False):
     g = Graph(len(graph["nodes"]))
     graph_dict = {}
     for i in graph["nodes"]:
         graph_dict[(i["data"]["name"])] = i
     map = {}
     j = 0
     while j < (len(graph["nodes"])):
@@ -65,15 +65,15 @@
                     )
                 )
                 f.write("\n")
             elif steps_list[i] == "essential":
                 f.write(
                     "\t"
                     + essentials_handler.return_function(
-                        function_name=node["data"]["name"], params=params, task_type=task_type, target_column= target_column
+                        function_name=node["data"]["name"], params=params, task_type=task_type, target_column= target_column,id=id
                     )
                 )
                 f.write("\n")
             elif steps_list[i] == "evaluate_model":
                 f.write(
                     # TODO: make changes for clustering
                     f"\tmetrics, feature_importance_dict = huble.sklearn.evaluate_model(model=Model, training_dataset=training_dataset, test_dataset=test_dataset, target_column= '{target_column}', task_type='{task_type}' )"
```

### Comparing `huble-0.2.285/src/huble/sklearn/graph.py` & `huble-0.2.286/src/huble/sklearn/graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/metrics/metrics.py` & `huble-0.2.286/src/huble/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/process/__init__.py` & `huble-0.2.286/src/huble/sklearn/process/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/process/functions.py` & `huble-0.2.286/src/huble/sklearn/process/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/process/handler.py` & `huble-0.2.286/src/huble/sklearn/process/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/process/preprocess_params.ts` & `huble-0.2.286/src/huble/sklearn/process/preprocess_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/train/__init__.py` & `huble-0.2.286/src/huble/sklearn/train/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/train/functions.py` & `huble-0.2.286/src/huble/sklearn/train/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/train/handler.py` & `huble-0.2.286/src/huble/sklearn/train/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/sklearn/train/model_params.ts` & `huble-0.2.286/src/huble/sklearn/train/model_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/convert_to_reactflow_graph.py` & `huble-0.2.286/src/huble/util/convert_to_reactflow_graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/data_types.py` & `huble-0.2.286/src/huble/util/data_types.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/feature_selection.py` & `huble-0.2.286/src/huble/util/feature_selection.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/inference_pipeline.py` & `huble-0.2.286/src/huble/util/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/typed_params.py` & `huble-0.2.286/src/huble/util/typed_params.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/verify_builder_pipeline.py` & `huble-0.2.286/src/huble/util/verify_builder_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/src/huble/util/verify_ml.py` & `huble-0.2.286/src/huble/util/verify_ml.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.285/setup.py` & `huble-0.2.286/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'pandas>=1.3.5,<2.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'scikit-learn==1.1.2',
  'scipy>=1.7.0,<1.8.0']
 
 setup_kwargs = {
     'name': 'huble',
-    'version': '0.2.285',
+    'version': '0.2.286',
     'description': '',
     'long_description': '',
     'author': 'Rugz007',
     'author_email': 'rugvedsomwanshi007@gmail.com',
     'maintainer': 'Arjit Agarwal',
     'maintainer_email': 'arjitagarwal123@gmail.com',
     'url': 'None',
```

### Comparing `huble-0.2.285/PKG-INFO` & `huble-0.2.286/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huble
-Version: 0.2.285
+Version: 0.2.286
 Summary: 
 Author: Rugz007
 Author-email: rugvedsomwanshi007@gmail.com
 Maintainer: Arjit Agarwal
 Maintainer-email: arjitagarwal123@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: Programming Language :: Python :: 3
```

