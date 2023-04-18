# Comparing `tmp/cdk_webapp_skeleton-0.3.dev2.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.3.dev2.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev3.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.3.dev2.tar` & `cdk_webapp_skeleton-0.3.dev3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev2/README.md
--rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     3316 2023-04-17 22:07:43.056106 cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0      593 2023-04-17 21:43:56.332756 cdk_webapp_skeleton-0.3.dev2/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev3/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     3433 2023-04-18 14:05:53.742373 cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-18 14:05:15.977194 cdk_webapp_skeleton-0.3.dev3/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev3/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.3.dev2/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.3.dev3/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,17 @@
                 branch_config.construct_id("WebappBackendApi"),
                 handler=self.webapp_lambda_func,
                 domain_name=apigateway.DomainNameOptions(
                     domain_name=backend_domain_name, certificate=backend_certificate
                 ),
                 disable_execute_api_endpoint=True,
                 default_cors_preflight_options=cors_options,
+                deploy_options=apigateway.StageOptions(
+                    tracing_enabled=True,
+                ),
             )
 
             route53.ARecord(
                 scope,
                 "BackendApiARecord",
                 zone=root_hosted_zone,
                 target=route53.RecordTarget.from_alias(
```

### Comparing `cdk_webapp_skeleton-0.3.dev2/pyproject.toml` & `cdk_webapp_skeleton-0.3.dev3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.3.dev2"
+version = "0.3.dev3"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.3.dev2/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.3.dev2
+Version: 0.3.dev3
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

