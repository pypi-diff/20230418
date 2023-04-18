# Comparing `tmp/cdktf-cdktf-provider-salesforce-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-salesforce-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-salesforce-3.0.0.tar", last modified: Tue Jan 17 14:55:41 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-salesforce-4.0.0.tar", last modified: Tue Apr 18 21:25:50 2023, max compression
```

## Comparing `cdktf-cdktf-provider-salesforce-3.0.0.tar` & `cdktf-cdktf-provider-salesforce-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.880329 cdktf-cdktf-provider-salesforce-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51440 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/profile/
--rw-r--r--   0 runner    (1001) docker     (123)    23541 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user/
--rw-r--r--   0 runner    (1001) docker     (123)    43170 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user_role/
--rw-r--r--   0 runner    (1001) docker     (123)    20652 2023-01-17 14:55:24.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:41.884329 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-01-17 14:55:41.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-01-17 14:55:41.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:55:41.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:55:41.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-17 14:55:41.000000 cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.279949 cdktf-cdktf-provider-salesforce-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128443 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    44505 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-04-18 21:25:38.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:50.283949 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-18 21:25:50.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-18 21:25:50.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:25:50.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 21:25:50.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 21:25:50.000000 cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/LICENSE` & `cdktf-cdktf-provider-salesforce-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-salesforce-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-salesforce
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt salesforce Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-salesforce.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-salesforce.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-salesforce-go`](https://github.com/cdktf/cdktf-provider-salesforce-go) package.
 
 `go get github.com/cdktf/cdktf-provider-salesforce-go/salesforce`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-salesforce).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform salesforce Provider version 1:1. In fact, it always tracks `latest` of `~> 0.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/README.md` & `cdktf-cdktf-provider-salesforce-4.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-salesforce-go`](https://github.com/cdktf/cdktf-provider-salesforce-go) package.
 
 `go get github.com/cdktf/cdktf-provider-salesforce-go/salesforce`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-salesforce).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform salesforce Provider version 1:1. In fact, it always tracks `latest` of `~> 0.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/setup.py` & `cdktf-cdktf-provider-salesforce-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-salesforce",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt salesforce Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-salesforce.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -28,37 +28,38 @@
         "cdktf_cdktf_provider_salesforce.profile",
         "cdktf_cdktf_provider_salesforce.provider",
         "cdktf_cdktf_provider_salesforce.user",
         "cdktf_cdktf_provider_salesforce.user_role"
     ],
     "package_data": {
         "cdktf_cdktf_provider_salesforce._jsii": [
-            "provider-salesforce@3.0.0.jsii.tgz"
+            "provider-salesforce@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_salesforce": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-salesforce-go`](https://github.com/cdktf/cdktf-provider-salesforce-go) package.
 
 `go get github.com/cdktf/cdktf-provider-salesforce-go/salesforce`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-salesforce).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform salesforce Provider version 1:1. In fact, it always tracks `latest` of `~> 0.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_salesforce_profile`
 
-Refer to the Terraform Registory for docs: [`data_salesforce_profile`](https://www.terraform.io/docs/providers/salesforce/d/profile).
+Refer to the Terraform Registory for docs: [`data_salesforce_profile`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataSalesforceProfile(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.dataSalesforceProfile.DataSalesforceProfile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce/d/profile salesforce_profile}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile salesforce_profile}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce/d/profile salesforce_profile} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile salesforce_profile} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/profile#name DataSalesforceProfile#name}
+        :param name: The name of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile#name DataSalesforceProfile#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -119,15 +119,15 @@
     },
 )
 class DataSalesforceProfileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: builtins.str,
     ) -> None:
@@ -135,15 +135,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/profile#name DataSalesforceProfile#name}
+        :param name: The name of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile#name DataSalesforceProfile#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cc708bd5e9e4da887df32964dc6b9359fced4ab92883187fe279ffb936d21f93)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -178,20 +178,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -233,15 +235,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the profile.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/profile#name DataSalesforceProfile#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/profile#name DataSalesforceProfile#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -264,15 +266,15 @@
 
 def _typecheckingstub__0119ba93d09de991c5ea5250ce9f94dce1b157788408ee950d0631fb5e80155f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     name: builtins.str,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -283,15 +285,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__cc708bd5e9e4da887df32964dc6b9359fced4ab92883187fe279ffb936d21f93(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_salesforce_user_license`
 
-Refer to the Terraform Registory for docs: [`data_salesforce_user_license`](https://www.terraform.io/docs/providers/salesforce/d/user_license).
+Refer to the Terraform Registory for docs: [`data_salesforce_user_license`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataSalesforceUserLicense(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.dataSalesforceUserLicense.DataSalesforceUserLicense",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce/d/user_license salesforce_user_license}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license salesforce_user_license}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         license_definition_key: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce/d/user_license salesforce_user_license} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license salesforce_user_license} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param license_definition_key: A string that uniquely identifies a particular user license. Valid options vary depending on organization type and configuration. For a complete list see https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_objects_userlicense.htm Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
+        :param license_definition_key: A string that uniquely identifies a particular user license. Valid options vary depending on organization type and configuration. For a complete list see https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_objects_userlicense.htm Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -119,15 +119,15 @@
     },
 )
 class DataSalesforceUserLicenseConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         license_definition_key: builtins.str,
     ) -> None:
@@ -135,15 +135,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param license_definition_key: A string that uniquely identifies a particular user license. Valid options vary depending on organization type and configuration. For a complete list see https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_objects_userlicense.htm Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
+        :param license_definition_key: A string that uniquely identifies a particular user license. Valid options vary depending on organization type and configuration. For a complete list see https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_objects_userlicense.htm Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dac9f6659f9fe6adc3579b97924e717b3135a334e9e388704578564c00a5eb71)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -178,20 +178,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -235,15 +237,15 @@
 
     @builtins.property
     def license_definition_key(self) -> builtins.str:
         '''A string that uniquely identifies a particular user license.
 
         Valid options vary depending on organization type and configuration. For a complete list see https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_objects_userlicense.htm
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/d/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/data-sources/user_license#license_definition_key DataSalesforceUserLicense#license_definition_key}
         '''
         result = self._values.get("license_definition_key")
         assert result is not None, "Required property 'license_definition_key' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -266,15 +268,15 @@
 
 def _typecheckingstub__0dfd33d2287e638186ba1ab54c4768422437d0257a3995a94611d1547419c92f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     license_definition_key: builtins.str,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -285,15 +287,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__dac9f6659f9fe6adc3579b97924e717b3135a334e9e388704578564c00a5eb71(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     license_definition_key: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `salesforce_profile`
 
-Refer to the Terraform Registory for docs: [`salesforce_profile`](https://www.terraform.io/docs/providers/salesforce/r/profile).
+Refer to the Terraform Registory for docs: [`salesforce_profile`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class Profile(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.profile.Profile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce/r/profile salesforce_profile}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile salesforce_profile}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         user_license_id: builtins.str,
         description: typing.Optional[builtins.str] = None,
         permissions: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce/r/profile salesforce_profile} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile salesforce_profile} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#name Profile#name}
-        :param user_license_id: ID of the UserLicense associated with this profile. Forces replacement if updated. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#user_license_id Profile#user_license_id}
-        :param description: Description of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#description Profile#description}
-        :param permissions: Map of permissions for the profile. At this time specific permissions can only be set, the comprehensive list will not be read from Salesforce. The keys should follow Salesforce 'SnakeCase' format however the 'Permissions' prefix should be omitted. Permissions will not import to state due to a technical limitation, you will need to run a subsequent apply if you have permissions set in config during import. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#permissions Profile#permissions}
+        :param name: The name of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#name Profile#name}
+        :param user_license_id: ID of the UserLicense associated with this profile. Forces replacement if updated. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#user_license_id Profile#user_license_id}
+        :param description: Description of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#description Profile#description}
+        :param permissions: Map of permissions for the profile. At this time specific permissions can only be set, the comprehensive list will not be read from Salesforce. The keys should follow Salesforce 'SnakeCase' format however the 'Permissions' prefix should be omitted. Permissions will not import to state due to a technical limitation, you will need to run a subsequent apply if you have permissions set in config during import. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#permissions Profile#permissions}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -197,15 +197,15 @@
     },
 )
 class ProfileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: builtins.str,
         user_license_id: builtins.str,
@@ -216,18 +216,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#name Profile#name}
-        :param user_license_id: ID of the UserLicense associated with this profile. Forces replacement if updated. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#user_license_id Profile#user_license_id}
-        :param description: Description of the profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#description Profile#description}
-        :param permissions: Map of permissions for the profile. At this time specific permissions can only be set, the comprehensive list will not be read from Salesforce. The keys should follow Salesforce 'SnakeCase' format however the 'Permissions' prefix should be omitted. Permissions will not import to state due to a technical limitation, you will need to run a subsequent apply if you have permissions set in config during import. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#permissions Profile#permissions}
+        :param name: The name of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#name Profile#name}
+        :param user_license_id: ID of the UserLicense associated with this profile. Forces replacement if updated. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#user_license_id Profile#user_license_id}
+        :param description: Description of the profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#description Profile#description}
+        :param permissions: Map of permissions for the profile. At this time specific permissions can only be set, the comprehensive list will not be read from Salesforce. The keys should follow Salesforce 'SnakeCase' format however the 'Permissions' prefix should be omitted. Permissions will not import to state due to a technical limitation, you will need to run a subsequent apply if you have permissions set in config during import. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#permissions Profile#permissions}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__95c130f2f2ba11559e3cba356a329e6c22941ea40405fecbc329590a1c91e43b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -270,20 +270,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -325,48 +327,48 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the profile.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#name Profile#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#name Profile#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def user_license_id(self) -> builtins.str:
         '''ID of the UserLicense associated with this profile. Forces replacement if updated.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#user_license_id Profile#user_license_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#user_license_id Profile#user_license_id}
         '''
         result = self._values.get("user_license_id")
         assert result is not None, "Required property 'user_license_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the profile.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#description Profile#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#description Profile#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def permissions(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]]:
         '''Map of permissions for the profile.
 
         At this time specific permissions can only be set, the comprehensive list will not be read from Salesforce. The keys should follow Salesforce 'SnakeCase' format however the 'Permissions' prefix should be omitted. Permissions will not import to state due to a technical limitation, you will need to run a subsequent apply if you have permissions set in config during import.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/profile#permissions Profile#permissions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/profile#permissions Profile#permissions}
         '''
         result = self._values.get("permissions")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -391,15 +393,15 @@
     id: builtins.str,
     *,
     name: builtins.str,
     user_license_id: builtins.str,
     description: typing.Optional[builtins.str] = None,
     permissions: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -428,15 +430,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__95c130f2f2ba11559e3cba356a329e6c22941ea40405fecbc329590a1c91e43b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
     user_license_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`salesforce`](https://www.terraform.io/docs/providers/salesforce).
+Refer to the Terraform Registory for docs: [`salesforce`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,38 +22,38 @@
 
 
 class SalesforceProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.provider.SalesforceProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce salesforce}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs salesforce}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         api_version: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         login_url: typing.Optional[builtins.str] = None,
         private_key: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce salesforce} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs salesforce} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#alias SalesforceProvider#alias}
-        :param api_version: API version of the salesforce org in the format in the format: MAJOR.MINOR (please omit any leading 'v'). The provider requires at least version 53.0. Can be specified with the environment variable SALESFORCE_API_VERSION. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#api_version SalesforceProvider#api_version}
-        :param client_id: Client ID of the connected app. Corresponds to Consumer Key in the user interface. Can be specified with the environment variable SALESFORCE_CLIENT_ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#client_id SalesforceProvider#client_id}
-        :param login_url: Directs the authentication request, defaults to the production endpoint https://login.salesforce.com, should be set to https://test.salesforce.com for sandbox organizations. Can be specified with the environment variable SALESFORCE_LOGIN_URL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#login_url SalesforceProvider#login_url}
-        :param private_key: Private Key associated to the public certificate that was uploaded to the connected app. This may point to a file location or be set directly. This should not be confused with the Consumer Secret in the user interface. Can be specified with the environment variable SALESFORCE_PRIVATE_KEY. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#private_key SalesforceProvider#private_key}
-        :param username: Salesforce Username of a System Administrator like user for the provider to authenticate as. Can be specified with the environment variable SALESFORCE_USERNAME. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#username SalesforceProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#alias SalesforceProvider#alias}
+        :param api_version: API version of the salesforce org in the format in the format: MAJOR.MINOR (please omit any leading 'v'). The provider requires at least version 53.0. Can be specified with the environment variable SALESFORCE_API_VERSION. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#api_version SalesforceProvider#api_version}
+        :param client_id: Client ID of the connected app. Corresponds to Consumer Key in the user interface. Can be specified with the environment variable SALESFORCE_CLIENT_ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#client_id SalesforceProvider#client_id}
+        :param login_url: Directs the authentication request, defaults to the production endpoint https://login.salesforce.com, should be set to https://test.salesforce.com for sandbox organizations. Can be specified with the environment variable SALESFORCE_LOGIN_URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#login_url SalesforceProvider#login_url}
+        :param private_key: Private Key associated to the public certificate that was uploaded to the connected app. This may point to a file location or be set directly. This should not be confused with the Consumer Secret in the user interface. Can be specified with the environment variable SALESFORCE_PRIVATE_KEY. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#private_key SalesforceProvider#private_key}
+        :param username: Salesforce Username of a System Administrator like user for the provider to authenticate as. Can be specified with the environment variable SALESFORCE_USERNAME. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#username SalesforceProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9a6435db0c50ddf76c4bce67d0322dfda080f6bcc1f0cabb9a44cc080d4ad548)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = SalesforceProviderConfig(
             alias=alias,
@@ -222,20 +222,20 @@
         api_version: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         login_url: typing.Optional[builtins.str] = None,
         private_key: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#alias SalesforceProvider#alias}
-        :param api_version: API version of the salesforce org in the format in the format: MAJOR.MINOR (please omit any leading 'v'). The provider requires at least version 53.0. Can be specified with the environment variable SALESFORCE_API_VERSION. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#api_version SalesforceProvider#api_version}
-        :param client_id: Client ID of the connected app. Corresponds to Consumer Key in the user interface. Can be specified with the environment variable SALESFORCE_CLIENT_ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#client_id SalesforceProvider#client_id}
-        :param login_url: Directs the authentication request, defaults to the production endpoint https://login.salesforce.com, should be set to https://test.salesforce.com for sandbox organizations. Can be specified with the environment variable SALESFORCE_LOGIN_URL. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#login_url SalesforceProvider#login_url}
-        :param private_key: Private Key associated to the public certificate that was uploaded to the connected app. This may point to a file location or be set directly. This should not be confused with the Consumer Secret in the user interface. Can be specified with the environment variable SALESFORCE_PRIVATE_KEY. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#private_key SalesforceProvider#private_key}
-        :param username: Salesforce Username of a System Administrator like user for the provider to authenticate as. Can be specified with the environment variable SALESFORCE_USERNAME. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#username SalesforceProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#alias SalesforceProvider#alias}
+        :param api_version: API version of the salesforce org in the format in the format: MAJOR.MINOR (please omit any leading 'v'). The provider requires at least version 53.0. Can be specified with the environment variable SALESFORCE_API_VERSION. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#api_version SalesforceProvider#api_version}
+        :param client_id: Client ID of the connected app. Corresponds to Consumer Key in the user interface. Can be specified with the environment variable SALESFORCE_CLIENT_ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#client_id SalesforceProvider#client_id}
+        :param login_url: Directs the authentication request, defaults to the production endpoint https://login.salesforce.com, should be set to https://test.salesforce.com for sandbox organizations. Can be specified with the environment variable SALESFORCE_LOGIN_URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#login_url SalesforceProvider#login_url}
+        :param private_key: Private Key associated to the public certificate that was uploaded to the connected app. This may point to a file location or be set directly. This should not be confused with the Consumer Secret in the user interface. Can be specified with the environment variable SALESFORCE_PRIVATE_KEY. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#private_key SalesforceProvider#private_key}
+        :param username: Salesforce Username of a System Administrator like user for the provider to authenticate as. Can be specified with the environment variable SALESFORCE_USERNAME. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#username SalesforceProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6cccb7e72f3dacefeb9dfd2e21c25145b46807a24109c64dbbf0c080fa8caeff)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument api_version", value=api_version, expected_type=type_hints["api_version"])
             check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
             check_type(argname="argument login_url", value=login_url, expected_type=type_hints["login_url"])
@@ -255,66 +255,66 @@
         if username is not None:
             self._values["username"] = username
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#alias SalesforceProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#alias SalesforceProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def api_version(self) -> typing.Optional[builtins.str]:
         '''API version of the salesforce org in the format in the format: MAJOR.MINOR (please omit any leading 'v'). The provider requires at least version 53.0. Can be specified with the environment variable SALESFORCE_API_VERSION.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#api_version SalesforceProvider#api_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#api_version SalesforceProvider#api_version}
         '''
         result = self._values.get("api_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_id(self) -> typing.Optional[builtins.str]:
         '''Client ID of the connected app.
 
         Corresponds to Consumer Key in the user interface. Can be specified with the environment variable SALESFORCE_CLIENT_ID.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#client_id SalesforceProvider#client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#client_id SalesforceProvider#client_id}
         '''
         result = self._values.get("client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_url(self) -> typing.Optional[builtins.str]:
         '''Directs the authentication request, defaults to the production endpoint https://login.salesforce.com, should be set to https://test.salesforce.com for sandbox organizations. Can be specified with the environment variable SALESFORCE_LOGIN_URL.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#login_url SalesforceProvider#login_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#login_url SalesforceProvider#login_url}
         '''
         result = self._values.get("login_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def private_key(self) -> typing.Optional[builtins.str]:
         '''Private Key associated to the public certificate that was uploaded to the connected app.
 
         This may point to a file location or be set directly. This should not be confused with the Consumer Secret in the user interface. Can be specified with the environment variable SALESFORCE_PRIVATE_KEY.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#private_key SalesforceProvider#private_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#private_key SalesforceProvider#private_key}
         '''
         result = self._values.get("private_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''Salesforce Username of a System Administrator like user for the provider to authenticate as.
 
         Can be specified with the environment variable SALESFORCE_USERNAME.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce#username SalesforceProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs#username SalesforceProvider#username}
         '''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `salesforce_user`
 
-Refer to the Terraform Registory for docs: [`salesforce_user`](https://www.terraform.io/docs/providers/salesforce/r/user).
+Refer to the Terraform Registory for docs: [`salesforce_user`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class User(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.user.User",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce/r/user salesforce_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user salesforce_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: builtins.str,
@@ -41,36 +41,36 @@
         email_encoding_key: typing.Optional[builtins.str] = None,
         language_locale_key: typing.Optional[builtins.str] = None,
         locale_sid_key: typing.Optional[builtins.str] = None,
         reset_password: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         time_zone_sid_key: typing.Optional[builtins.str] = None,
         user_role_id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce/r/user salesforce_user} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user salesforce_user} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: The user’s alias. For example, jsmith. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#alias User#alias}
-        :param email: The user’s email address. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email User#email}
-        :param last_name: The user’s last name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#last_name User#last_name}
-        :param profile_id: ID of the user’s Profile. Use this value to cache metadata based on profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#profile_id User#profile_id}
-        :param username: Contains the name that a user enters to log in to the API or the user interface. The value for this field must be in the form of an email address, using all lowercase characters. It must also be unique across all organizations. If you try to create or update a User with a duplicate value for this field, the operation is rejected. Each inserted User also counts as a license. Every organization has a maximum number of licenses. If you attempt to exceed the maximum number of licenses by inserting User records, the create request is rejected. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#username User#username}
-        :param email_encoding_key: The email encoding for the user, such as ISO-8859-1 or UTF-8. Defaults to UTF-8. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email_encoding_key User#email_encoding_key}
-        :param language_locale_key: The user’s language. Defaults to en_US. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#language_locale_key User#language_locale_key}
-        :param locale_sid_key: The value of the field affects formatting and parsing of values, especially numeric values, in the user interface. It doesn’t affect the API. The field values are named according to the language, and the country if necessary, using two-letter ISO codes. The set of names is based on the ISO standard. You can also manually set a user’s locale in the user interface, and then use that value for inserting or updating other users via the API. Defaults to en_US. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#locale_sid_key User#locale_sid_key}
-        :param reset_password: Reset password and send an email to the user. No reset is performed if this field is omitted, is false, or was true and remained true on subsequent apply. Please set to false and then true in subsequent applies, or have it set to true on create to trigger the reset. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#reset_password User#reset_password}
-        :param time_zone_sid_key: A User time zone affects the offset used when displaying or entering times in the user interface. But the API doesn’t use a User time zone when querying or setting values. Values for this field are named using region and key city, according to ISO standards. You can also manually set one User time zone in the user interface, and then use that value for creating or updating other User records via the API. Defaults to America/New_York. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#time_zone_sid_key User#time_zone_sid_key}
-        :param user_role_id: ID of the user’s UserRole. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#user_role_id User#user_role_id}
+        :param alias: The user’s alias. For example, jsmith. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#alias User#alias}
+        :param email: The user’s email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email User#email}
+        :param last_name: The user’s last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#last_name User#last_name}
+        :param profile_id: ID of the user’s Profile. Use this value to cache metadata based on profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#profile_id User#profile_id}
+        :param username: Contains the name that a user enters to log in to the API or the user interface. The value for this field must be in the form of an email address, using all lowercase characters. It must also be unique across all organizations. If you try to create or update a User with a duplicate value for this field, the operation is rejected. Each inserted User also counts as a license. Every organization has a maximum number of licenses. If you attempt to exceed the maximum number of licenses by inserting User records, the create request is rejected. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#username User#username}
+        :param email_encoding_key: The email encoding for the user, such as ISO-8859-1 or UTF-8. Defaults to UTF-8. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email_encoding_key User#email_encoding_key}
+        :param language_locale_key: The user’s language. Defaults to en_US. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#language_locale_key User#language_locale_key}
+        :param locale_sid_key: The value of the field affects formatting and parsing of values, especially numeric values, in the user interface. It doesn’t affect the API. The field values are named according to the language, and the country if necessary, using two-letter ISO codes. The set of names is based on the ISO standard. You can also manually set a user’s locale in the user interface, and then use that value for inserting or updating other users via the API. Defaults to en_US. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#locale_sid_key User#locale_sid_key}
+        :param reset_password: Reset password and send an email to the user. No reset is performed if this field is omitted, is false, or was true and remained true on subsequent apply. Please set to false and then true in subsequent applies, or have it set to true on create to trigger the reset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#reset_password User#reset_password}
+        :param time_zone_sid_key: A User time zone affects the offset used when displaying or entering times in the user interface. But the API doesn’t use a User time zone when querying or setting values. Values for this field are named using region and key city, according to ISO standards. You can also manually set one User time zone in the user interface, and then use that value for creating or updating other User records via the API. Defaults to America/New_York. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#time_zone_sid_key User#time_zone_sid_key}
+        :param user_role_id: ID of the user’s UserRole. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#user_role_id User#user_role_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -360,15 +360,15 @@
     },
 )
 class UserConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         alias: builtins.str,
         email: builtins.str,
@@ -386,25 +386,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param alias: The user’s alias. For example, jsmith. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#alias User#alias}
-        :param email: The user’s email address. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email User#email}
-        :param last_name: The user’s last name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#last_name User#last_name}
-        :param profile_id: ID of the user’s Profile. Use this value to cache metadata based on profile. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#profile_id User#profile_id}
-        :param username: Contains the name that a user enters to log in to the API or the user interface. The value for this field must be in the form of an email address, using all lowercase characters. It must also be unique across all organizations. If you try to create or update a User with a duplicate value for this field, the operation is rejected. Each inserted User also counts as a license. Every organization has a maximum number of licenses. If you attempt to exceed the maximum number of licenses by inserting User records, the create request is rejected. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#username User#username}
-        :param email_encoding_key: The email encoding for the user, such as ISO-8859-1 or UTF-8. Defaults to UTF-8. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email_encoding_key User#email_encoding_key}
-        :param language_locale_key: The user’s language. Defaults to en_US. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#language_locale_key User#language_locale_key}
-        :param locale_sid_key: The value of the field affects formatting and parsing of values, especially numeric values, in the user interface. It doesn’t affect the API. The field values are named according to the language, and the country if necessary, using two-letter ISO codes. The set of names is based on the ISO standard. You can also manually set a user’s locale in the user interface, and then use that value for inserting or updating other users via the API. Defaults to en_US. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#locale_sid_key User#locale_sid_key}
-        :param reset_password: Reset password and send an email to the user. No reset is performed if this field is omitted, is false, or was true and remained true on subsequent apply. Please set to false and then true in subsequent applies, or have it set to true on create to trigger the reset. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#reset_password User#reset_password}
-        :param time_zone_sid_key: A User time zone affects the offset used when displaying or entering times in the user interface. But the API doesn’t use a User time zone when querying or setting values. Values for this field are named using region and key city, according to ISO standards. You can also manually set one User time zone in the user interface, and then use that value for creating or updating other User records via the API. Defaults to America/New_York. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#time_zone_sid_key User#time_zone_sid_key}
-        :param user_role_id: ID of the user’s UserRole. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#user_role_id User#user_role_id}
+        :param alias: The user’s alias. For example, jsmith. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#alias User#alias}
+        :param email: The user’s email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email User#email}
+        :param last_name: The user’s last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#last_name User#last_name}
+        :param profile_id: ID of the user’s Profile. Use this value to cache metadata based on profile. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#profile_id User#profile_id}
+        :param username: Contains the name that a user enters to log in to the API or the user interface. The value for this field must be in the form of an email address, using all lowercase characters. It must also be unique across all organizations. If you try to create or update a User with a duplicate value for this field, the operation is rejected. Each inserted User also counts as a license. Every organization has a maximum number of licenses. If you attempt to exceed the maximum number of licenses by inserting User records, the create request is rejected. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#username User#username}
+        :param email_encoding_key: The email encoding for the user, such as ISO-8859-1 or UTF-8. Defaults to UTF-8. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email_encoding_key User#email_encoding_key}
+        :param language_locale_key: The user’s language. Defaults to en_US. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#language_locale_key User#language_locale_key}
+        :param locale_sid_key: The value of the field affects formatting and parsing of values, especially numeric values, in the user interface. It doesn’t affect the API. The field values are named according to the language, and the country if necessary, using two-letter ISO codes. The set of names is based on the ISO standard. You can also manually set a user’s locale in the user interface, and then use that value for inserting or updating other users via the API. Defaults to en_US. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#locale_sid_key User#locale_sid_key}
+        :param reset_password: Reset password and send an email to the user. No reset is performed if this field is omitted, is false, or was true and remained true on subsequent apply. Please set to false and then true in subsequent applies, or have it set to true on create to trigger the reset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#reset_password User#reset_password}
+        :param time_zone_sid_key: A User time zone affects the offset used when displaying or entering times in the user interface. But the API doesn’t use a User time zone when querying or setting values. Values for this field are named using region and key city, according to ISO standards. You can also manually set one User time zone in the user interface, and then use that value for creating or updating other User records via the API. Defaults to America/New_York. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#time_zone_sid_key User#time_zone_sid_key}
+        :param user_role_id: ID of the user’s UserRole. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#user_role_id User#user_role_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__258da2adb5f434d4c71fb0b2646bf9976b10dd70457167daa77d33c15d4a9f52)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -465,20 +465,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -520,120 +522,120 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def alias(self) -> builtins.str:
         '''The user’s alias. For example, jsmith.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#alias User#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#alias User#alias}
         '''
         result = self._values.get("alias")
         assert result is not None, "Required property 'alias' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def email(self) -> builtins.str:
         '''The user’s email address.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email User#email}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email User#email}
         '''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def last_name(self) -> builtins.str:
         '''The user’s last name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#last_name User#last_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#last_name User#last_name}
         '''
         result = self._values.get("last_name")
         assert result is not None, "Required property 'last_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def profile_id(self) -> builtins.str:
         '''ID of the user’s Profile. Use this value to cache metadata based on profile.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#profile_id User#profile_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#profile_id User#profile_id}
         '''
         result = self._values.get("profile_id")
         assert result is not None, "Required property 'profile_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''Contains the name that a user enters to log in to the API or the user interface.
 
         The value for this field must be in the form of an email address, using all lowercase characters. It must also be unique across all organizations. If you try to create or update a User with a duplicate value for this field, the operation is rejected. Each inserted User also counts as a license. Every organization has a maximum number of licenses. If you attempt to exceed the maximum number of licenses by inserting User records, the create request is rejected.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#username User#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#username User#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def email_encoding_key(self) -> typing.Optional[builtins.str]:
         '''The email encoding for the user, such as ISO-8859-1 or UTF-8. Defaults to UTF-8.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#email_encoding_key User#email_encoding_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#email_encoding_key User#email_encoding_key}
         '''
         result = self._values.get("email_encoding_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def language_locale_key(self) -> typing.Optional[builtins.str]:
         '''The user’s language. Defaults to en_US.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#language_locale_key User#language_locale_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#language_locale_key User#language_locale_key}
         '''
         result = self._values.get("language_locale_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def locale_sid_key(self) -> typing.Optional[builtins.str]:
         '''The value of the field affects formatting and parsing of values, especially numeric values, in the user interface.
 
         It doesn’t affect the API. The field values are named according to the language, and the country if necessary, using two-letter ISO codes. The set of names is based on the ISO standard. You can also manually set a user’s locale in the user interface, and then use that value for inserting or updating other users via the API. Defaults to en_US.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#locale_sid_key User#locale_sid_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#locale_sid_key User#locale_sid_key}
         '''
         result = self._values.get("locale_sid_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def reset_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Reset password and send an email to the user.
 
         No reset is performed if this field is omitted, is false, or was true and remained true on subsequent apply. Please set to false and then true in subsequent applies, or have it set to true on create to trigger the reset.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#reset_password User#reset_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#reset_password User#reset_password}
         '''
         result = self._values.get("reset_password")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def time_zone_sid_key(self) -> typing.Optional[builtins.str]:
         '''A User time zone affects the offset used when displaying or entering times in the user interface.
 
         But the API doesn’t use a User time zone when querying or setting values. Values for this field are named using region and key city, according to ISO standards. You can also manually set one User time zone in the user interface, and then use that value for creating or updating other User records via the API. Defaults to America/New_York.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#time_zone_sid_key User#time_zone_sid_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#time_zone_sid_key User#time_zone_sid_key}
         '''
         result = self._values.get("time_zone_sid_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_role_id(self) -> typing.Optional[builtins.str]:
         '''ID of the user’s UserRole.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user#user_role_id User#user_role_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user#user_role_id User#user_role_id}
         '''
         result = self._values.get("user_role_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -665,15 +667,15 @@
     email_encoding_key: typing.Optional[builtins.str] = None,
     language_locale_key: typing.Optional[builtins.str] = None,
     locale_sid_key: typing.Optional[builtins.str] = None,
     reset_password: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     time_zone_sid_key: typing.Optional[builtins.str] = None,
     user_role_id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -744,15 +746,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__258da2adb5f434d4c71fb0b2646bf9976b10dd70457167daa77d33c15d4a9f52(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     alias: builtins.str,
     email: builtins.str,
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `salesforce_user_role`
 
-Refer to the Terraform Registory for docs: [`salesforce_user_role`](https://www.terraform.io/docs/providers/salesforce/r/user_role).
+Refer to the Terraform Registory for docs: [`salesforce_user_role`](https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class UserRole(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-salesforce.userRole.UserRole",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/salesforce/r/user_role salesforce_user_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role salesforce_user_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         developer_name: builtins.str,
         name: builtins.str,
         parent_role_id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/salesforce/r/user_role salesforce_user_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role salesforce_user_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param developer_name: The unique name of the object in the API. This name can contain only underscores and alphanumeric characters, and must be unique in your org. It must begin with a letter, not include spaces, not end with an underscore, and not contain two consecutive underscores. In managed packages, this field prevents naming conflicts on package installations. With this field, a developer can change the object’s name in a managed package and the changes are reflected in a subscriber’s organization. Corresponds to Role Name in the user interface. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#developer_name UserRole#developer_name}
-        :param name: Name of the role. Corresponds to Label on the user interface. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#name UserRole#name}
-        :param parent_role_id: The ID of the parent role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#parent_role_id UserRole#parent_role_id}
+        :param developer_name: The unique name of the object in the API. This name can contain only underscores and alphanumeric characters, and must be unique in your org. It must begin with a letter, not include spaces, not end with an underscore, and not contain two consecutive underscores. In managed packages, this field prevents naming conflicts on package installations. With this field, a developer can change the object’s name in a managed package and the changes are reflected in a subscriber’s organization. Corresponds to Role Name in the user interface. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#developer_name UserRole#developer_name}
+        :param name: Name of the role. Corresponds to Label on the user interface. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#name UserRole#name}
+        :param parent_role_id: The ID of the parent role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#parent_role_id UserRole#parent_role_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -165,15 +165,15 @@
     },
 )
 class UserRoleConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         developer_name: builtins.str,
         name: builtins.str,
@@ -183,17 +183,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param developer_name: The unique name of the object in the API. This name can contain only underscores and alphanumeric characters, and must be unique in your org. It must begin with a letter, not include spaces, not end with an underscore, and not contain two consecutive underscores. In managed packages, this field prevents naming conflicts on package installations. With this field, a developer can change the object’s name in a managed package and the changes are reflected in a subscriber’s organization. Corresponds to Role Name in the user interface. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#developer_name UserRole#developer_name}
-        :param name: Name of the role. Corresponds to Label on the user interface. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#name UserRole#name}
-        :param parent_role_id: The ID of the parent role. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#parent_role_id UserRole#parent_role_id}
+        :param developer_name: The unique name of the object in the API. This name can contain only underscores and alphanumeric characters, and must be unique in your org. It must begin with a letter, not include spaces, not end with an underscore, and not contain two consecutive underscores. In managed packages, this field prevents naming conflicts on package installations. With this field, a developer can change the object’s name in a managed package and the changes are reflected in a subscriber’s organization. Corresponds to Role Name in the user interface. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#developer_name UserRole#developer_name}
+        :param name: Name of the role. Corresponds to Label on the user interface. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#name UserRole#name}
+        :param parent_role_id: The ID of the parent role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#parent_role_id UserRole#parent_role_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__640d6b51a6b191bdb5834309c2bf01899a30a4f5186e65f1373c664fa13f4307)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -233,20 +233,22 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("connection")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
+    def count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]]:
         '''
         :stability: experimental
         '''
         result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]], result)
 
     @builtins.property
     def depends_on(
         self,
     ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
         '''
         :stability: experimental
@@ -290,35 +292,35 @@
 
     @builtins.property
     def developer_name(self) -> builtins.str:
         '''The unique name of the object in the API.
 
         This name can contain only underscores and alphanumeric characters, and must be unique in your org. It must begin with a letter, not include spaces, not end with an underscore, and not contain two consecutive underscores. In managed packages, this field prevents naming conflicts on package installations. With this field, a developer can change the object’s name in a managed package and the changes are reflected in a subscriber’s organization. Corresponds to Role Name in the user interface.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#developer_name UserRole#developer_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#developer_name UserRole#developer_name}
         '''
         result = self._values.get("developer_name")
         assert result is not None, "Required property 'developer_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Name of the role. Corresponds to Label on the user interface.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#name UserRole#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#name UserRole#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def parent_role_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the parent role.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/salesforce/r/user_role#parent_role_id UserRole#parent_role_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/salesforce/0.1.0/docs/resources/user_role#parent_role_id UserRole#parent_role_id}
         '''
         result = self._values.get("parent_role_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -342,15 +344,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     developer_name: builtins.str,
     name: builtins.str,
     parent_role_id: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -373,15 +375,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__640d6b51a6b191bdb5834309c2bf01899a30a4f5186e65f1373c664fa13f4307(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     developer_name: builtins.str,
     name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-salesforce
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt salesforce Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-salesforce.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-salesforce.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-salesforce-go`](https://github.com/cdktf/cdktf-provider-salesforce-go) package.
 
 `go get github.com/cdktf/cdktf-provider-salesforce-go/salesforce`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-salesforce).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform salesforce Provider version 1:1. In fact, it always tracks `latest` of `~> 0.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-salesforce-3.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-salesforce-4.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdktf_cdktf_provider_salesforce/py.typed
 src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
 src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
-src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
 src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
 src/cdktf_cdktf_provider_salesforce/profile/__init__.py
 src/cdktf_cdktf_provider_salesforce/provider/__init__.py
 src/cdktf_cdktf_provider_salesforce/user/__init__.py
 src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
```

