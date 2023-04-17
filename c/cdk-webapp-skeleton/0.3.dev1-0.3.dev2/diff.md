# Comparing `tmp/cdk_webapp_skeleton-0.3.dev1.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev1.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev2.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev1.tar` & `cdk_webapp_skeleton-0.3.dev2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev1/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     2906 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-08 16:25:51.192530 cdk_webapp_skeleton-0.3.dev1/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev2/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     3316 2023-04-17 22:07:43.056106 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-17 21:43:56.332756 cdk_webapp_skeleton-0.3.dev2/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev2/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from aws_cdk import aws_apigateway as apigateway
 from aws_cdk import aws_certificatemanager as certificatemanager
 from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_lambda as _lambda
+from aws_cdk import aws_logs as logs
 from aws_cdk import aws_route53 as route53
 from aws_cdk import aws_route53_targets as route53_targets
 from constructs import Construct
 
 from .branch_config import BranchConfig
 
 
@@ -14,26 +15,37 @@
 
     def __init__(
         self,
         scope: "Construct",
         _id: str,
         branch_config: BranchConfig,
         lambda_runtime_environment=None,
+        image_directory="webapp-backend",
     ):
         super().__init__(scope, _id)
         if lambda_runtime_environment is None:
             lambda_runtime_environment = {}
 
         self.webapp_lambda_func = _lambda.DockerImageFunction(
             scope,
             "FlaskLambda",
-            code=_lambda.DockerImageCode.from_image_asset(directory="webapp-backend"),
+            code=_lambda.DockerImageCode.from_image_asset(directory=image_directory),
             environment=lambda_runtime_environment,
         )
 
+        logs.MetricFilter(
+            scope,
+            "FlaskLambdaTimeouts",
+            log_group=self.webapp_lambda_func.log_group,
+            filter_pattern=logs.FilterPattern.literal("Task timed out"),
+            metric_name="Timeouts",
+            metric_namespace="FlaskLambda",
+            metric_value="1",
+        )
+
         cloudwatch.Alarm(
             scope,
             "FlaskLambdaThrottles",
             metric=self.webapp_lambda_func.metric_throttles(),
             evaluation_periods=1,
             threshold=0,
             comparison_operator=cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD,
```

### Comparing `cdk_webapp_skeleton-0.3.dev1/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev1"
+version = "0.3.dev2"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev1/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev1
+Version: 0.3.dev2
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

