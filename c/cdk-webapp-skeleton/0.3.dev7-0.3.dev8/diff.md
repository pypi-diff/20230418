# Comparing `tmp/cdk_webapp_skeleton-0.3.dev7.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev7.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev8.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev7.tar` & `cdk_webapp_skeleton-0.3.dev8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev7/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1544 2023-04-18 21:19:44.807699 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     4271 2023-04-18 21:20:47.703926 cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-18 21:13:22.478124 cdk_webapp_skeleton-0.3.dev7/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev8/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1544 2023-04-18 21:19:44.807699 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     4334 2023-04-18 21:50:57.522135 cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-18 21:51:50.214877 cdk_webapp_skeleton-0.3.dev8/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev8/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev7/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev8/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.webapp_lambda_func = _lambda.DockerImageFunction(
             scope,
             "FlaskLambda",
             code=_lambda.DockerImageCode.from_image_asset(directory=image_directory),
             environment=lambda_runtime_environment,
             tracing=_lambda.Tracing.ACTIVE,
         )
+        profiling_group.grant_publish(self.webapp_lambda_func)
 
         logs.MetricFilter(
             scope,
             "FlaskLambdaTimeouts",
             log_group=self.webapp_lambda_func.log_group,
             filter_pattern=logs.FilterPattern.literal('"Task timed out"'),
             metric_name="Timeouts",
```

### Comparing `cdk_webapp_skeleton-0.3.dev7/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev7"
+version = "0.3.dev8"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev7/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev7
+Version: 0.3.dev8
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

