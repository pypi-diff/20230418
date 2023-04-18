# Comparing `tmp/cdktf-cdktf-provider-hashicups-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-hashicups-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hashicups-3.0.0.tar", last modified: Tue Jan 17 13:31:20 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hashicups-4.0.0.tar", last modified: Tue Apr 18 20:45:11 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hashicups-3.0.0.tar` & `cdktf-cdktf-provider-hashicups-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     4044 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3111 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-01-17 13:31:20.197253 cdktf-cdktf-provider-hashicups-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2116 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/
--rw-r--r--   0 runner    (1000) runner    (1000)     3702 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/
--rw-r--r--   0 runner    (1000) runner    (1000)      421 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54154 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/
--rw-r--r--   0 runner    (1000) runner    (1000)    34409 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/
--rw-r--r--   0 runner    (1000) runner    (1000)    27076 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    25018 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/order/
--rw-r--r--   0 runner    (1000) runner    (1000)    40009 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/provider/
--rw-r--r--   0 runner    (1000) runner    (1000)    12019 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-01-17 13:31:08.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-17 13:31:20.193253 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4044 2023-01-17 13:31:19.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      882 2023-01-17 13:31:20.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-01-17 13:31:19.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-01-17 13:31:20.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2023-01-17 13:31:20.000000 cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     4213 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3249 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2166 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3840 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   157027 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/
+-rw-r--r--   0 runner    (1000) runner    (1000)    34892 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/
+-rw-r--r--   0 runner    (1000) runner    (1000)    27655 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    25501 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    40851 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12334 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4213 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      882 2023-04-18 20:45:11.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/LICENSE` & `cdktf-cdktf-provider-hashicups-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-hashicups-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hashicups
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt hashicups Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hashicups.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hashicups.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hashicups-go`](https://github.com/cdktf/cdktf-provider-hashicups-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hashicups-go/hashicups`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hashicups).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/README.md` & `cdktf-cdktf-provider-hashicups-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hashicups-go`](https://github.com/cdktf/cdktf-provider-hashicups-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hashicups-go/hashicups`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hashicups).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/setup.py` & `cdktf-cdktf-provider-hashicups-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hashicups",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt hashicups Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hashicups.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,37 +27,38 @@
         "cdktf_cdktf_provider_hashicups.data_hashicups_ingredients",
         "cdktf_cdktf_provider_hashicups.data_hashicups_order",
         "cdktf_cdktf_provider_hashicups.order",
         "cdktf_cdktf_provider_hashicups.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hashicups._jsii": [
-            "provider-hashicups@3.0.0.jsii.tgz"
+            "provider-hashicups@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hashicups": [
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

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hashicups-go`](https://github.com/cdktf/cdktf-provider-hashicups-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hashicups-go/hashicups`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hashicups).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hashicups_coffees`
 
-Refer to the Terraform Registory for docs: [`data_hashicups_coffees`](https://www.terraform.io/docs/providers/hashicups/d/coffees).
+Refer to the Terraform Registory for docs: [`data_hashicups_coffees`](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataHashicupsCoffees(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hashicups.dataHashicupsCoffees.DataHashicupsCoffees",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hashicups/d/coffees hashicups_coffees}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees hashicups_coffees}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hashicups/d/coffees hashicups_coffees} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees hashicups_coffees} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/coffees#id DataHashicupsCoffees#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees#id DataHashicupsCoffees#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -438,15 +438,15 @@
     },
 )
 class DataHashicupsCoffeesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -454,15 +454,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/coffees#id DataHashicupsCoffees#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees#id DataHashicupsCoffees#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__712c68d87776404c41d755c59e5d939ad819ba6c045062d4020c0bec2ba3051b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -497,20 +497,22 @@
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
@@ -550,15 +552,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/coffees#id DataHashicupsCoffees#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/coffees#id DataHashicupsCoffees#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -589,15 +591,15 @@
 
 def _typecheckingstub__8528845cadc35681a7c56dbe16a7718efa9b03e501778128efc86bd447a0aed3(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
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
@@ -702,15 +704,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__712c68d87776404c41d755c59e5d939ad819ba6c045062d4020c0bec2ba3051b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hashicups_ingredients`
 
-Refer to the Terraform Registory for docs: [`data_hashicups_ingredients`](https://www.terraform.io/docs/providers/hashicups/d/ingredients).
+Refer to the Terraform Registory for docs: [`data_hashicups_ingredients`](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataHashicupsIngredients(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hashicups.dataHashicupsIngredients.DataHashicupsIngredients",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients hashicups_ingredients}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients hashicups_ingredients}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         coffee_id: jsii.Number,
         id: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients hashicups_ingredients} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients hashicups_ingredients} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param coffee_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#id DataHashicupsIngredients#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param coffee_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#id DataHashicupsIngredients#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -144,15 +144,15 @@
     },
 )
 class DataHashicupsIngredientsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         coffee_id: jsii.Number,
         id: typing.Optional[builtins.str] = None,
@@ -161,16 +161,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param coffee_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#id DataHashicupsIngredients#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param coffee_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#id DataHashicupsIngredients#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1b644fe69f04adf91bb10a9a2a830eed45d3f5bacc5f522364f8b8d4408920a5)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -208,20 +208,22 @@
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
@@ -261,22 +263,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def coffee_id(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#coffee_id DataHashicupsIngredients#coffee_id}.'''
         result = self._values.get("coffee_id")
         assert result is not None, "Required property 'coffee_id' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/ingredients#id DataHashicupsIngredients#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/ingredients#id DataHashicupsIngredients#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -464,15 +466,15 @@
 def _typecheckingstub__229395a87f54f984d95842c1bf98097cd912f2e31f2189424ae556ae027eaee5(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     coffee_id: jsii.Number,
     id: typing.Optional[builtins.str] = None,
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
@@ -489,15 +491,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1b644fe69f04adf91bb10a9a2a830eed45d3f5bacc5f522364f8b8d4408920a5(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     coffee_id: jsii.Number,
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hashicups_order`
 
-Refer to the Terraform Registory for docs: [`data_hashicups_order`](https://www.terraform.io/docs/providers/hashicups/d/order).
+Refer to the Terraform Registory for docs: [`data_hashicups_order`](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataHashicupsOrder(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hashicups.dataHashicupsOrder.DataHashicupsOrder",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hashicups/d/order hashicups_order}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order hashicups_order}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: jsii.Number,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hashicups/d/order hashicups_order} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order hashicups_order} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/order#id DataHashicupsOrder#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order#id DataHashicupsOrder#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
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
 class DataHashicupsOrderConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: jsii.Number,
     ) -> None:
@@ -135,15 +135,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/order#id DataHashicupsOrder#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order#id DataHashicupsOrder#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6050110ae59401b843c18b7c392baa1a41983ac666f37b58a7786a4557711335)
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
@@ -231,15 +233,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/d/order#id DataHashicupsOrder#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/data-sources/order#id DataHashicupsOrder#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(jsii.Number, result)
@@ -436,15 +438,15 @@
 
 def _typecheckingstub__d367674d7c1544971a002e54c59a4c3d6ef635bf08142a80ab3822fa34a1b51f(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: jsii.Number,
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
@@ -455,15 +457,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6050110ae59401b843c18b7c392baa1a41983ac666f37b58a7786a4557711335(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: jsii.Number,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hashicups_order`
 
-Refer to the Terraform Registory for docs: [`hashicups_order`](https://www.terraform.io/docs/providers/hashicups/r/order).
+Refer to the Terraform Registory for docs: [`hashicups_order`](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class Order(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hashicups.order.Order",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hashicups/r/order hashicups_order}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order hashicups_order}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         items: typing.Union[typing.Sequence[typing.Union["OrderItems", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
         id: typing.Optional[builtins.str] = None,
         last_updated: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hashicups/r/order hashicups_order} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order hashicups_order} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param items: items block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#items Order#items}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_updated: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#last_updated Order#last_updated}.
+        :param items: items block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#items Order#items}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_updated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#last_updated Order#last_updated}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -172,15 +172,15 @@
     },
 )
 class OrderConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         items: typing.Union[typing.Sequence[typing.Union["OrderItems", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
         id: typing.Optional[builtins.str] = None,
@@ -190,17 +190,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param items: items block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#items Order#items}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_updated: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#last_updated Order#last_updated}.
+        :param items: items block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#items Order#items}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_updated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#last_updated Order#last_updated}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__508754e3122383f854f4d8512bfbc631821c67977e6d2fa3c09b732d9441b140)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -241,20 +241,22 @@
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
@@ -298,33 +300,33 @@
 
     @builtins.property
     def items(
         self,
     ) -> typing.Union[typing.List["OrderItems"], _cdktf_9a9027ec.IResolvable]:
         '''items block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#items Order#items}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#items Order#items}
         '''
         result = self._values.get("items")
         assert result is not None, "Required property 'items' is missing"
         return typing.cast(typing.Union[typing.List["OrderItems"], _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def last_updated(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#last_updated Order#last_updated}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#last_updated Order#last_updated}.'''
         result = self._values.get("last_updated")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -345,16 +347,16 @@
     def __init__(
         self,
         *,
         coffee: typing.Union["OrderItemsCoffee", typing.Dict[builtins.str, typing.Any]],
         quantity: jsii.Number,
     ) -> None:
         '''
-        :param coffee: coffee block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#coffee Order#coffee}
-        :param quantity: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#quantity Order#quantity}.
+        :param coffee: coffee block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#coffee Order#coffee}
+        :param quantity: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#quantity Order#quantity}.
         '''
         if isinstance(coffee, dict):
             coffee = OrderItemsCoffee(**coffee)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1f004744e71417b2d7f1a3c6e6bd0bf65f1e2c947c1fa63be99afb6b20703338)
             check_type(argname="argument coffee", value=coffee, expected_type=type_hints["coffee"])
             check_type(argname="argument quantity", value=quantity, expected_type=type_hints["quantity"])
@@ -363,23 +365,23 @@
             "quantity": quantity,
         }
 
     @builtins.property
     def coffee(self) -> "OrderItemsCoffee":
         '''coffee block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#coffee Order#coffee}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#coffee Order#coffee}
         '''
         result = self._values.get("coffee")
         assert result is not None, "Required property 'coffee' is missing"
         return typing.cast("OrderItemsCoffee", result)
 
     @builtins.property
     def quantity(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#quantity Order#quantity}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#quantity Order#quantity}.'''
         result = self._values.get("quantity")
         assert result is not None, "Required property 'quantity' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -396,26 +398,26 @@
     jsii_type="@cdktf/provider-hashicups.order.OrderItemsCoffee",
     jsii_struct_bases=[],
     name_mapping={"id": "id"},
 )
 class OrderItemsCoffee:
     def __init__(self, *, id: jsii.Number) -> None:
         '''
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b1cb8596abd2c21dcab116d0a08df0b710a96059bbf5945b8f24b9ee89d2d431)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "id": id,
         }
 
     @builtins.property
     def id(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(jsii.Number, result)
@@ -622,15 +624,15 @@
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @jsii.member(jsii_name="putCoffee")
     def put_coffee(self, *, id: jsii.Number) -> None:
         '''
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups/r/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs/resources/order#id Order#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         value = OrderItemsCoffee(id=id)
 
         return typing.cast(None, jsii.invoke(self, "putCoffee", [value]))
 
     @builtins.property
     @jsii.member(jsii_name="coffee")
@@ -693,15 +695,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     items: typing.Union[typing.Sequence[typing.Union[OrderItems, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     id: typing.Optional[builtins.str] = None,
     last_updated: typing.Optional[builtins.str] = None,
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
@@ -724,15 +726,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__508754e3122383f854f4d8512bfbc631821c67977e6d2fa3c09b732d9441b140(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     items: typing.Union[typing.Sequence[typing.Union[OrderItems, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
     id: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`hashicups`](https://www.terraform.io/docs/providers/hashicups).
+Refer to the Terraform Registory for docs: [`hashicups`](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,34 +22,34 @@
 
 
 class HashicupsProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hashicups.provider.HashicupsProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hashicups hashicups}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs hashicups}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         host: typing.Optional[builtins.str] = None,
         password: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hashicups hashicups} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs hashicups} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#alias HashicupsProvider#alias}
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#host HashicupsProvider#host}.
-        :param password: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#password HashicupsProvider#password}.
-        :param username: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#username HashicupsProvider#username}.
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#alias HashicupsProvider#alias}
+        :param host: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#host HashicupsProvider#host}.
+        :param password: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#password HashicupsProvider#password}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#username HashicupsProvider#username}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0ac09006b5290e236227d37eaef067e2bd7fe85933f091a023598b2fd03e23fb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HashicupsProviderConfig(
             alias=alias, host=host, password=password, username=username
@@ -167,18 +167,18 @@
         *,
         alias: typing.Optional[builtins.str] = None,
         host: typing.Optional[builtins.str] = None,
         password: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#alias HashicupsProvider#alias}
-        :param host: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#host HashicupsProvider#host}.
-        :param password: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#password HashicupsProvider#password}.
-        :param username: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#username HashicupsProvider#username}.
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#alias HashicupsProvider#alias}
+        :param host: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#host HashicupsProvider#host}.
+        :param password: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#password HashicupsProvider#password}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#username HashicupsProvider#username}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1215b2927309adab7120a222f882fa7ad0685d1557e42737fc391243e6a4f2b5)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument host", value=host, expected_type=type_hints["host"])
             check_type(argname="argument password", value=password, expected_type=type_hints["password"])
             check_type(argname="argument username", value=username, expected_type=type_hints["username"])
@@ -192,34 +192,34 @@
         if username is not None:
             self._values["username"] = username
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#alias HashicupsProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#alias HashicupsProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#host HashicupsProvider#host}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#host HashicupsProvider#host}.'''
         result = self._values.get("host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#password HashicupsProvider#password}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#password HashicupsProvider#password}.'''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hashicups#username HashicupsProvider#username}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hashicups/0.3.1/docs#username HashicupsProvider#username}.'''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hashicups
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt hashicups Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hashicups.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hashicups.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hashicups-go`](https://github.com/cdktf/cdktf-provider-hashicups-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hashicups-go/hashicups`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hashicups).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-hashicups-3.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_hashicups/py.typed
 src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
-src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
 src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
 src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
 src/cdktf_cdktf_provider_hashicups/order/__init__.py
 src/cdktf_cdktf_provider_hashicups/provider/__init__.py
```

