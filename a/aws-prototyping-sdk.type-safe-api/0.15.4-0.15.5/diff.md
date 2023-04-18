# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.15.4.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.15.4.tar", last modified: Tue Apr 18 04:47:46 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.15.5.tar", last modified: Tue Apr 18 07:15:26 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.15.4.tar` & `aws_prototyping_sdk.type_safe_api-0.15.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.109696 aws_prototyping_sdk.type_safe_api-0.15.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-18 04:47:46.109696 aws_prototyping_sdk.type_safe_api-0.15.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53263 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:47:46.109696 aws_prototyping_sdk.type_safe_api-0.15.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.097696 aws_prototyping_sdk.type_safe_api-0.15.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.097696 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.101696 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   275121 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.101696 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   841240 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.15.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:47:29.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:47:46.101696 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-18 04:47:45.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 04:47:46.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:47:45.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 04:47:46.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 04:47:46.000000 aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.891071 aws_prototyping_sdk.type_safe_api-0.15.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-18 07:15:26.887071 aws_prototyping_sdk.type_safe_api-0.15.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53263 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:15:26.891071 aws_prototyping_sdk.type_safe_api-0.15.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.883071 aws_prototyping_sdk.type_safe_api-0.15.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.883071 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.887071 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   275121 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.887071 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   841515 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.15.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:15:10.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:15:26.887071 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-18 07:15:26.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 07:15:26.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:15:26.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 07:15:26.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 07:15:26.000000 aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.15.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.15.4
+Version: 0.15.5
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/README.md` & `aws_prototyping_sdk.type_safe_api-0.15.5/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/setup.py` & `aws_prototyping_sdk.type_safe_api-0.15.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.15.4",
+    "version": "0.15.5",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.15.4.jsii.tgz"
+            "type-safe-api@0.15.5.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.15.4
+Version: 0.15.5
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.15.4/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.15.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.15.4.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.15.5.jsii.tgz
```

