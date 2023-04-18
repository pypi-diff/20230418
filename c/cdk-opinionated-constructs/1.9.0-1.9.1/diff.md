# Comparing `tmp/cdk-opinionated-constructs-1.9.0.tar.gz` & `tmp/cdk-opinionated-constructs-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-1.9.0.tar", last modified: Tue Nov 22 22:09:47 2022, max compression
+gzip compressed data, was "cdk-opinionated-constructs-1.9.1.tar", last modified: Wed Nov 23 22:26:05 2022, max compression
```

## Comparing `cdk-opinionated-constructs-1.9.0.tar` & `cdk-opinionated-constructs-1.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.078113 cdk-opinionated-constructs-1.9.0/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-1.9.0/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-22 22:09:47.078198 cdk-opinionated-constructs-1.9.0/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    10420 2022-11-22 14:56:51.000000 cdk-opinionated-constructs-1.9.0/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.058318 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     7612 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5372 2022-11-06 20:49:59.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2607 2022-11-05 20:59:58.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:09:18.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    12206 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.077858 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-22 22:09:47.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      970 2022-11-22 22:09:47.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2022-11-22 22:09:47.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       47 2022-11-22 22:09:47.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2022-11-22 22:09:47.000000 cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2022-11-22 22:09:47.079425 cdk-opinionated-constructs-1.9.0/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      715 2022-11-22 22:09:41.000000 cdk-opinionated-constructs-1.9.0/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.059058 cdk-opinionated-constructs-1.9.0/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.0/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      878 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.068713 cdk-opinionated-constructs-1.9.0/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.0/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1591 2022-11-22 14:56:51.000000 cdk-opinionated-constructs-1.9.0/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.0/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2368 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1513 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1174 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2616 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-22 22:09:47.075502 cdk-opinionated-constructs-1.9.0/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.0/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.260687 cdk-opinionated-constructs-1.9.1/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-1.9.1/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-23 22:26:05.260763 cdk-opinionated-constructs-1.9.1/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    10354 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.240465 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     7612 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5299 2022-11-23 22:24:16.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2607 2022-11-05 20:59:58.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    12206 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.260270 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      355 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      970 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       47 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2022-11-23 22:26:05.000000 cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2022-11-23 22:26:05.261502 cdk-opinionated-constructs-1.9.1/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      715 2022-11-23 22:25:39.000000 cdk-opinionated-constructs-1.9.1/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.241167 cdk-opinionated-constructs-1.9.1/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      878 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.247653 cdk-opinionated-constructs-1.9.1/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1591 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-1.9.1/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2368 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1513 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-1.9.1/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2616 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2022-11-23 22:26:05.254670 cdk-opinionated-constructs-1.9.1/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-1.9.1/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-1.9.0/LICENSE` & `cdk-opinionated-constructs-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/README.md` & `cdk-opinionated-constructs-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,23 +58,22 @@
 import aws_cdk.aws_kms as kms
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NIST80053R5Checks, PCIDSS321Checks, HIPAASecurityChecks
 
 
 class TestSNSStack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated AWS SNS topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
 
         sns_construct = SNSTopic(self, id="topic")
-        sns_topic = sns_construct.create_sns_topic(topic_name="topic", master_key=shared_kms_key)
-        sns_construct.create_sns_topic_policy(sns_topic)
+        sns_construct.create_sns_topic(topic_name="topic", master_key=shared_kms_key)
 
         # Validate stack against AWS Solutions checklist
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
         Aspects.of(self).add(NIST80053R5Checks(log_ignores=True))
         Aspects.of(self).add(PCIDSS321Checks(log_ignores=True))
         Aspects.of(self).add(HIPAASecurityChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/lmb.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         """
 
         return lmb.CodeSigningConfig(self, "conde-signing-config", signing_profiles=[profile])
 
     def create_lambda_layer(self, code_path: str, construct_id: str = "supporting_libraries") -> lmb.LayerVersion:
         """Create lambda layer.
 
-        :param props: The dictionary which contain configuration values.
         :param code_path: path which contain lambda layer directory
         :param construct_id: construct id
         :return: Lambda layer
         """
         return lmb.LayerVersion(
             self,
             id=construct_id,
```

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-1.9.1/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/setup.cfg` & `cdk-opinionated-constructs-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/setup.py` & `cdk-opinionated-constructs-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="1.9.0",
+    version="1.9.1",
     description="AWS CDK constructs come without added security configurations.",
     long_description="Very rarely this is validated during the CI pipeline via tools like CDK-NAG. The idea behind this project is to create secured constructs from the start.",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
         "aws-cdk-lib>=2.51.1",
```

### Comparing `cdk-opinionated-constructs-1.9.0/test/app.py` & `cdk-opinionated-constructs-1.9.1/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/sns_stack.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 import aws_cdk.aws_kms as kms
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NIST80053R5Checks, PCIDSS321Checks, HIPAASecurityChecks
 
 
 class TestSNSStack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated AWS SNS topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
 
         sns_construct = SNSTopic(self, id="topic")
-        sns_topic = sns_construct.create_sns_topic(topic_name="topic", master_key=shared_kms_key)
-        sns_construct.create_sns_topic_policy(sns_topic)
+        sns_construct.create_sns_topic(topic_name="topic", master_key=shared_kms_key)
 
         # Validate stack against AWS Solutions checklist
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
         Aspects.of(self).add(NIST80053R5Checks(log_ignores=True))
         Aspects.of(self).add(PCIDSS321Checks(log_ignores=True))
         Aspects.of(self).add(HIPAASecurityChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-1.9.0/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-1.9.1/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-1.9.0/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-1.9.1/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

