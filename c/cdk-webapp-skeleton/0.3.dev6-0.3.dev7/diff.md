# Comparing `tmp/cdk_webapp_skeleton-0.3.dev6.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev6.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev7.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev6.tar` & `cdk_webapp_skeleton-0.3.dev7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev6/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     3842 2023-04-18 19:51:19.346762 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-18 20:46:51.023841 cdk_webapp_skeleton-0.3.dev6/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev7/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1544 2023-04-18 21:19:44.807699 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     4271 2023-04-18 21:20:47.703926 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-18 21:13:22.478124 cdk_webapp_skeleton-0.3.dev7/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev7/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             code_build_defaults=pipelines.CodeBuildOptions(
                 build_environment=codebuild.BuildEnvironment(
                     compute_type=codebuild.ComputeType.SMALL
                 ),
                 cache=codebuild.Cache.bucket(cache_bucket),
             ),
             cross_account_keys=False,
+            publish_assets_in_parallel=False,
         )
 
     def add_stage(self, stage: cdk.Stage) -> pipelines.StageDeployment:
         return self.cdk_pipeline.add_stage(stage)
 
     def build_pipeline(self):
         self.cdk_pipeline.build_pipeline()
```

### Comparing `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from aws_cdk import aws_apigateway as apigateway
 from aws_cdk import aws_certificatemanager as certificatemanager
 from aws_cdk import aws_cloudwatch as cloudwatch
+from aws_cdk import aws_codeguruprofiler as codeguruprofiler
 from aws_cdk import aws_lambda as _lambda
 from aws_cdk import aws_logs as logs
 from aws_cdk import aws_route53 as route53
 from aws_cdk import aws_route53_targets as route53_targets
 from constructs import Construct
 
 from .branch_config import BranchConfig
@@ -21,14 +22,26 @@
         lambda_runtime_environment=None,
         image_directory="webapp-backend",
     ):
         super().__init__(scope, _id)
         if lambda_runtime_environment is None:
             lambda_runtime_environment = {}
 
+        profiling_group = codeguruprofiler.ProfilingGroup(
+            scope,
+            "FlaskLambdaProfiler",
+            compute_platform=codeguruprofiler.ComputePlatform.AWS_LAMBDA,
+        )
+
+        lambda_runtime_environment.update(
+            {
+                "AWS_CODEGURU_PROFILER_GROUP_ARN": profiling_group.profiling_group_arn,
+            }
+        )
+
         self.webapp_lambda_func = _lambda.DockerImageFunction(
             scope,
             "FlaskLambda",
             code=_lambda.DockerImageCode.from_image_asset(directory=image_directory),
             environment=lambda_runtime_environment,
             tracing=_lambda.Tracing.ACTIVE,
         )
```

### Comparing `cdk_webapp_skeleton-0.3.dev6/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev6"
+version = "0.3.dev7"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev6/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev6
+Version: 0.3.dev7
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

