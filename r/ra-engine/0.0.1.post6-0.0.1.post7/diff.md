# Comparing `tmp/ra_engine-0.0.1.post6.tar.gz` & `tmp/ra_engine-0.0.1.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra_engine-0.0.1.post6.tar", last modified: Thu Mar 30 10:28:44 2023, max compression
+gzip compressed data, was "ra_engine-0.0.1.post7.tar", last modified: Tue Apr 18 03:36:21 2023, max compression
```

## Comparing `ra_engine-0.0.1.post6.tar` & `ra_engine-0.0.1.post7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.194658 ra_engine-0.0.1.post6/ra_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/ra_engine/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/core/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/ra_engine/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/ml/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/ml/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/ml/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/ml/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/ra_engine/runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/runners/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/ra_engine/type_def/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/type_def/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/type_def/creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/type_def/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/ra_engine/type_def/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/ra_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-30 10:28:44.000000 ra_engine-0.0.1.post6/ra_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-30 10:28:44.000000 ra_engine-0.0.1.post6/ra_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:28:44.000000 ra_engine-0.0.1.post6/ra_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 10:28:44.000000 ra_engine-0.0.1.post6/ra_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 10:28:44.000000 ra_engine-0.0.1.post6/ra_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:44.198658 ra_engine-0.0.1.post6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-03-30 10:28:28.000000 ra_engine-0.0.1.post6/tests/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-18 03:36:21.951425 ra_engine-0.0.1.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/core/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/ml/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/ml/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/ml/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/ml/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/runners/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine/type_def/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/type_def/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/type_def/creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/type_def/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/ra_engine/type_def/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/ra_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-18 03:36:21.000000 ra_engine-0.0.1.post7/ra_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 03:36:21.000000 ra_engine-0.0.1.post7/ra_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:36:21.000000 ra_engine-0.0.1.post7/ra_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 03:36:21.000000 ra_engine-0.0.1.post7/ra_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 03:36:21.000000 ra_engine-0.0.1.post7/ra_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:36:21.951425 ra_engine-0.0.1.post7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:21.947425 ra_engine-0.0.1.post7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-18 03:36:11.000000 ra_engine-0.0.1.post7/tests/test_regression.py
```

### Comparing `ra_engine-0.0.1.post6/ra_engine/ml/classification.py` & `ra_engine-0.0.1.post7/ra_engine/ml/classification.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/ra_engine/ml/regression.py` & `ra_engine-0.0.1.post7/ra_engine/ml/regression.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/ra_engine/ml/timeseries.py` & `ra_engine-0.0.1.post7/ra_engine/ml/timeseries.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/ra_engine/runners/ml.py` & `ra_engine-0.0.1.post7/ra_engine/runners/ml.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,42 @@
 from ra_engine.core.app import RAEApp
 import requests
 from ra_engine.type_def.results import Response
 from ra_engine.core.app import App
 
 
 class SKLRunner:
-    rae_app: RAEApp = None
+    app: RAEApp = None
     pred_df: pd.DataFrame = None
     pred_config: Union[dict, None] = None
     endpoint: str = "/api/v1/runner/skl"
-    _app: App = None
 
     def __init__(
         self, app: RAEApp, pred_df: pd.DataFrame, pred_config: Union[dict, None] = None
     ):
-        self.rae_app: RAEApp = app
+        self.app: RAEApp = app
         self.pred_df = pred_df
         self.pred_config = pred_config
-        self._app: App = app.app()
-        if self._app is None:
-            raise ValueError("RAEApp is not initialized. Please run app.init() first.")
-        if self._app.result is None:
-            raise ValueError(
-                "Provided RAEApp is not authenticated properly. Please check your credentials."
-            )
+
+        if self.app is None:
+            raise ValueError("RAEApp is not initialized properly.")
+        if self.app.credentials is None:
+            raise ValueError("Provided RAEApp is not have credentials.")
+        if self.app.credentials.apiKey is None:
+            raise ValueError("Provided RAEApp is doesn't have any API Key.")
 
     def inputs(self) -> dict:
         return {
             "data": self.pred_df.to_dict(),
             "config": self.pred_config,
         }
 
     def exec(self, id: str):
         response = requests.get(
-            self.rae_app.credentials.host + self.endpoint + f"/{id}",
+            self.app.credentials.host + self.endpoint + f"/{id}",
             json=self.inputs(),
             headers={
                 "Content-Type": "application/json",
-                "Authorization": f"Bearer {self._app.result['jwt']}",
+                "X-Api-Key": self.app.credentials.apiKey,
             },
         )
         return Response(response)
```

### Comparing `ra_engine-0.0.1.post6/ra_engine/type_def/ml.py` & `ra_engine-0.0.1.post7/ra_engine/type_def/ml.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/ra_engine/type_def/results.py` & `ra_engine-0.0.1.post7/ra_engine/type_def/results.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/ra_engine.egg-info/SOURCES.txt` & `ra_engine-0.0.1.post7/ra_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/setup.py` & `ra_engine-0.0.1.post7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ra_engine",
-    version="0.0.1-rev6",
+    version="0.0.1-rev7",
     license="MIT",
     author="Navindu Dananaga",
     author_email="navindudananga123@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ra_engine-0.0.1.post6/tests/test_classification.py` & `ra_engine-0.0.1.post7/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ra_engine-0.0.1.post6/tests/test_regression.py` & `ra_engine-0.0.1.post7/tests/test_regression.py`

 * *Files identical despite different names*

