# Comparing `tmp/cdk_webapp_skeleton-0.3.dev5.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev5.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev6.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev5.tar` & `cdk_webapp_skeleton-0.3.dev6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev5/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     3548 2023-04-18 14:40:42.929056 cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-18 14:41:26.065956 cdk_webapp_skeleton-0.3.dev5/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev6/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     3842 2023-04-18 19:51:19.346762 cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-18 20:46:51.023841 cdk_webapp_skeleton-0.3.dev6/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev6/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev5/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev6/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,23 @@
             "FlaskLambdaThrottles",
             metric=self.webapp_lambda_func.metric_throttles(),
             evaluation_periods=1,
             threshold=0,
             comparison_operator=cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD,
         )
 
+        cloudwatch.Alarm(
+            scope,
+            "FlaskLambdaErrors",
+            metric=self.webapp_lambda_func.metric_errors(),
+            evaluation_periods=1,
+            threshold=0,
+            comparison_operator=cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD,
+        )
+
         root_hosted_zone = branch_config.get_hosted_zone(scope)
         if root_hosted_zone is not None:
             backend_domain_name = "api." + branch_config.domain_name
 
             backend_certificate = certificatemanager.Certificate(
                 scope,
                 "apiCert",
```

### Comparing `cdk_webapp_skeleton-0.3.dev5/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev5"
+version = "0.3.dev6"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev5/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev5
+Version: 0.3.dev6
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

