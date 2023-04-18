# Comparing `tmp/cdk-aws-lambda-powertools-layer-3.4.0.tar.gz` & `tmp/cdk-aws-lambda-powertools-layer-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-aws-lambda-powertools-layer-3.4.0.tar", last modified: Thu Apr 13 12:26:21 2023, max compression
+gzip compressed data, was "cdk-aws-lambda-powertools-layer-3.5.0.tar", last modified: Tue Apr 18 13:15:41 2023, max compression
```

## Comparing `cdk-aws-lambda-powertools-layer-3.4.0.tar` & `cdk-aws-lambda-powertools-layer-3.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:21.860581 cdk-aws-lambda-powertools-layer-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.4.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:26:00.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:26:21.864581 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-13 12:26:21.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 12:26:21.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:26:21.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 12:26:21.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 12:26:21.000000 cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.265545 cdk-aws-lambda-powertools-layer-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
```

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/LICENSE` & `cdk-aws-lambda-powertools-layer-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/PKG-INFO` & `cdk-aws-lambda-powertools-layer-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-lambda-powertools-layer
-Version: 3.4.0
+Version: 3.5.0
 Summary: A lambda layer for AWS Powertools for python and typescript
 Home-page: https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Author: Amazon Web Services
 License: MIT-0
 Project-URL: Source, https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/README.md` & `cdk-aws-lambda-powertools-layer-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/setup.py` & `cdk-aws-lambda-powertools-layer-3.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-aws-lambda-powertools-layer",
-    "version": "3.4.0",
+    "version": "3.5.0",
     "description": "A lambda layer for AWS Powertools for python and typescript",
     "license": "MIT-0",
     "url": "https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk_aws_lambda_powertools_layer",
         "cdk_aws_lambda_powertools_layer._jsii"
     ],
     "package_data": {
         "cdk_aws_lambda_powertools_layer._jsii": [
-            "cdk-aws-lambda-powertools-layer@3.4.0.jsii.tgz"
+            "cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz"
         ],
         "cdk_aws_lambda_powertools_layer": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.70.0, <3.0.0",
+        "aws-cdk-lib>=2.75.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer/__init__.py` & `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO` & `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-lambda-powertools-layer
-Version: 3.4.0
+Version: 3.5.0
 Summary: A lambda layer for AWS Powertools for python and typescript
 Home-page: https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Author: Amazon Web Services
 License: MIT-0
 Project-URL: Source, https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-lambda-powertools-layer-3.4.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt` & `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_aws_lambda_powertools_layer/py.typed
 src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
 src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
 src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
-src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.4.0.jsii.tgz
+src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz
```

