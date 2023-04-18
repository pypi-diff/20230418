# Comparing `tmp/cdktf-cdktf-provider-tls-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-tls-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-tls-5.0.0.tar", last modified: Tue Jan 17 14:57:41 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-tls-6.0.0.tar", last modified: Tue Apr 18 20:54:49 2023, max compression
```

## Comparing `cdktf-cdktf-provider-tls-5.0.0.tar` & `cdktf-cdktf-provider-tls-6.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68635 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/_jsii/provider-tls@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/cert_request/
--rw-r--r--   0 runner    (1001) docker     (123)    50746 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    31947 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/
--rw-r--r--   0 runner    (1001) docker     (123)    39988 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/private_key/
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/
--rw-r--r--   0 runner    (1001) docker     (123)    74593 2023-01-17 14:57:28.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:57:41.203514 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-17 14:57:40.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-17 14:57:41.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:57:40.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:57:41.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 14:57:41.000000 cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.663172 cdktf-cdktf-provider-tls-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.663172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.663172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   225367 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/_jsii/provider-tls@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/cert_request/
+-rw-r--r--   0 runner    (1001) docker     (123)    52342 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)    41062 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/private_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.667172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)    76711 2023-04-18 20:54:38.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:49.663172 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:54:49.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-18 20:54:49.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:54:49.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:54:49.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:54:49.000000 cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/LICENSE` & `cdktf-cdktf-provider-tls-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-tls-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tls
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt tls Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tls.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tls.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-tls-go`](https://github.com/cdktf/cdktf-provider-tls-go) package.
 
 `go get github.com/cdktf/cdktf-provider-tls-go/tls`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-tls).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform tls Provider version 1:1. In fact, it always tracks `latest` of `~> 4.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/README.md` & `cdktf-cdktf-provider-tls-6.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-tls-go`](https://github.com/cdktf/cdktf-provider-tls-go) package.
 
 `go get github.com/cdktf/cdktf-provider-tls-go/tls`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-tls).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform tls Provider version 1:1. In fact, it always tracks `latest` of `~> 4.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/setup.py` & `cdktf-cdktf-provider-tls-6.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-tls",
-    "version": "5.0.0",
+    "version": "6.0.0",
     "description": "Prebuilt tls Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-tls.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -29,37 +29,38 @@
         "cdktf_cdktf_provider_tls.locally_signed_cert",
         "cdktf_cdktf_provider_tls.private_key",
         "cdktf_cdktf_provider_tls.provider",
         "cdktf_cdktf_provider_tls.self_signed_cert"
     ],
     "package_data": {
         "cdktf_cdktf_provider_tls._jsii": [
-            "provider-tls@5.0.0.jsii.tgz"
+            "provider-tls@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_tls": [
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

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-tls-go`](https://github.com/cdktf/cdktf-provider-tls-go) package.
 
 `go get github.com/cdktf/cdktf-provider-tls-go/tls`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-tls).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform tls Provider version 1:1. In fact, it always tracks `latest` of `~> 4.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tls_cert_request`
 
-Refer to the Terraform Registory for docs: [`tls_cert_request`](https://www.terraform.io/docs/providers/tls/r/cert_request).
+Refer to the Terraform Registory for docs: [`tls_cert_request`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class CertRequest(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.certRequest.CertRequest",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/r/cert_request tls_cert_request}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request tls_cert_request}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         private_key_pem: builtins.str,
         dns_names: typing.Optional[typing.Sequence[builtins.str]] = None,
         ip_addresses: typing.Optional[typing.Sequence[builtins.str]] = None,
         subject: typing.Optional[typing.Union["CertRequestSubject", typing.Dict[builtins.str, typing.Any]]] = None,
         uris: typing.Optional[typing.Sequence[builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/r/cert_request tls_cert_request} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request tls_cert_request} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#private_key_pem CertRequest#private_key_pem}
-        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#dns_names CertRequest#dns_names}
-        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#ip_addresses CertRequest#ip_addresses}
-        :param subject: subject block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#subject CertRequest#subject}
-        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#uris CertRequest#uris}
+        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#private_key_pem CertRequest#private_key_pem}
+        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#dns_names CertRequest#dns_names}
+        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#ip_addresses CertRequest#ip_addresses}
+        :param subject: subject block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#subject CertRequest#subject}
+        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#uris CertRequest#uris}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,23 +95,23 @@
         organizational_unit: typing.Optional[builtins.str] = None,
         postal_code: typing.Optional[builtins.str] = None,
         province: typing.Optional[builtins.str] = None,
         serial_number: typing.Optional[builtins.str] = None,
         street_address: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#common_name CertRequest#common_name}
-        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#country CertRequest#country}
-        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#locality CertRequest#locality}
-        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organization CertRequest#organization}
-        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organizational_unit CertRequest#organizational_unit}
-        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#postal_code CertRequest#postal_code}
-        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#province CertRequest#province}
-        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#serial_number CertRequest#serial_number}
-        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#street_address CertRequest#street_address}
+        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#common_name CertRequest#common_name}
+        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#country CertRequest#country}
+        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#locality CertRequest#locality}
+        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organization CertRequest#organization}
+        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organizational_unit CertRequest#organizational_unit}
+        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#postal_code CertRequest#postal_code}
+        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#province CertRequest#province}
+        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#serial_number CertRequest#serial_number}
+        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#street_address CertRequest#street_address}
         '''
         value = CertRequestSubject(
             common_name=common_name,
             country=country,
             locality=locality,
             organization=organization,
             organizational_unit=organizational_unit,
@@ -261,15 +261,15 @@
     },
 )
 class CertRequestConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         private_key_pem: builtins.str,
         dns_names: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -281,19 +281,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#private_key_pem CertRequest#private_key_pem}
-        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#dns_names CertRequest#dns_names}
-        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#ip_addresses CertRequest#ip_addresses}
-        :param subject: subject block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#subject CertRequest#subject}
-        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#uris CertRequest#uris}
+        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#private_key_pem CertRequest#private_key_pem}
+        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#dns_names CertRequest#dns_names}
+        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#ip_addresses CertRequest#ip_addresses}
+        :param subject: subject block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#subject CertRequest#subject}
+        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#uris CertRequest#uris}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(subject, dict):
             subject = CertRequestSubject(**subject)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8d8bb59ca00900d949baa74bfdb37389f671ebdea175593d860cd095bd87e0d6)
@@ -342,20 +342,22 @@
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
@@ -397,52 +399,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def private_key_pem(self) -> builtins.str:
         '''Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#private_key_pem CertRequest#private_key_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#private_key_pem CertRequest#private_key_pem}
         '''
         result = self._values.get("private_key_pem")
         assert result is not None, "Required property 'private_key_pem' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def dns_names(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of DNS names for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#dns_names CertRequest#dns_names}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#dns_names CertRequest#dns_names}
         '''
         result = self._values.get("dns_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def ip_addresses(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#ip_addresses CertRequest#ip_addresses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#ip_addresses CertRequest#ip_addresses}
         '''
         result = self._values.get("ip_addresses")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def subject(self) -> typing.Optional["CertRequestSubject"]:
         '''subject block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#subject CertRequest#subject}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#subject CertRequest#subject}
         '''
         result = self._values.get("subject")
         return typing.cast(typing.Optional["CertRequestSubject"], result)
 
     @builtins.property
     def uris(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of URIs for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#uris CertRequest#uris}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#uris CertRequest#uris}
         '''
         result = self._values.get("uris")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -481,23 +483,23 @@
         organizational_unit: typing.Optional[builtins.str] = None,
         postal_code: typing.Optional[builtins.str] = None,
         province: typing.Optional[builtins.str] = None,
         serial_number: typing.Optional[builtins.str] = None,
         street_address: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#common_name CertRequest#common_name}
-        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#country CertRequest#country}
-        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#locality CertRequest#locality}
-        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organization CertRequest#organization}
-        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organizational_unit CertRequest#organizational_unit}
-        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#postal_code CertRequest#postal_code}
-        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#province CertRequest#province}
-        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#serial_number CertRequest#serial_number}
-        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#street_address CertRequest#street_address}
+        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#common_name CertRequest#common_name}
+        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#country CertRequest#country}
+        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#locality CertRequest#locality}
+        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organization CertRequest#organization}
+        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organizational_unit CertRequest#organizational_unit}
+        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#postal_code CertRequest#postal_code}
+        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#province CertRequest#province}
+        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#serial_number CertRequest#serial_number}
+        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#street_address CertRequest#street_address}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e487a18f53276ee3cb541ef5a77df0e6dfe48c28dccc088cbddf339b9d47afea)
             check_type(argname="argument common_name", value=common_name, expected_type=type_hints["common_name"])
             check_type(argname="argument country", value=country, expected_type=type_hints["country"])
             check_type(argname="argument locality", value=locality, expected_type=type_hints["locality"])
             check_type(argname="argument organization", value=organization, expected_type=type_hints["organization"])
@@ -526,87 +528,87 @@
         if street_address is not None:
             self._values["street_address"] = street_address
 
     @builtins.property
     def common_name(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``CN``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#common_name CertRequest#common_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#common_name CertRequest#common_name}
         '''
         result = self._values.get("common_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def country(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``C``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#country CertRequest#country}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#country CertRequest#country}
         '''
         result = self._values.get("country")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def locality(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``L``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#locality CertRequest#locality}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#locality CertRequest#locality}
         '''
         result = self._values.get("locality")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``O``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organization CertRequest#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organization CertRequest#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organizational_unit(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``OU``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#organizational_unit CertRequest#organizational_unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#organizational_unit CertRequest#organizational_unit}
         '''
         result = self._values.get("organizational_unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def postal_code(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``PC``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#postal_code CertRequest#postal_code}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#postal_code CertRequest#postal_code}
         '''
         result = self._values.get("postal_code")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def province(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``ST``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#province CertRequest#province}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#province CertRequest#province}
         '''
         result = self._values.get("province")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def serial_number(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``SERIALNUMBER``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#serial_number CertRequest#serial_number}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#serial_number CertRequest#serial_number}
         '''
         result = self._values.get("serial_number")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def street_address(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Distinguished name: ``STREET``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/cert_request#street_address CertRequest#street_address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/cert_request#street_address CertRequest#street_address}
         '''
         result = self._values.get("street_address")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -856,15 +858,15 @@
     *,
     private_key_pem: builtins.str,
     dns_names: typing.Optional[typing.Sequence[builtins.str]] = None,
     ip_addresses: typing.Optional[typing.Sequence[builtins.str]] = None,
     subject: typing.Optional[typing.Union[CertRequestSubject, typing.Dict[builtins.str, typing.Any]]] = None,
     uris: typing.Optional[typing.Sequence[builtins.str]] = None,
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
@@ -893,15 +895,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8d8bb59ca00900d949baa74bfdb37389f671ebdea175593d860cd095bd87e0d6(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     private_key_pem: builtins.str,
     dns_names: typing.Optional[typing.Sequence[builtins.str]] = None,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tls_certificate`
 
-Refer to the Terraform Registory for docs: [`data_tls_certificate`](https://www.terraform.io/docs/providers/tls/d/certificate).
+Refer to the Terraform Registory for docs: [`data_tls_certificate`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataTlsCertificate(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.dataTlsCertificate.DataTlsCertificate",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/d/certificate tls_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate tls_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         content: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
         verify_chain: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/d/certificate tls_certificate} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate tls_certificate} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param content: The content of the certificate in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#content DataTlsCertificate#content}
-        :param url: URL of the endpoint to get the certificates from. Accepted schemes are: ``https``, ``tls``. For scheme ``https://`` it will use the HTTP protocol and apply the ``proxy`` configuration of the provider, if set. For scheme ``tls://`` it will instead use a secure TCP socket. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#url DataTlsCertificate#url}
-        :param verify_chain: Whether to verify the certificate chain while parsing it or not (default: ``true``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#verify_chain DataTlsCertificate#verify_chain}
+        :param content: The content of the certificate in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#content DataTlsCertificate#content}
+        :param url: URL of the endpoint to get the certificates from. Accepted schemes are: ``https``, ``tls``. For scheme ``https://`` it will use the HTTP protocol and apply the ``proxy`` configuration of the provider, if set. For scheme ``tls://`` it will instead use a secure TCP socket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#url DataTlsCertificate#url}
+        :param verify_chain: Whether to verify the certificate chain while parsing it or not (default: ``true``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#verify_chain DataTlsCertificate#verify_chain}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -377,15 +377,15 @@
     },
 )
 class DataTlsCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         content: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
@@ -395,17 +395,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param content: The content of the certificate in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#content DataTlsCertificate#content}
-        :param url: URL of the endpoint to get the certificates from. Accepted schemes are: ``https``, ``tls``. For scheme ``https://`` it will use the HTTP protocol and apply the ``proxy`` configuration of the provider, if set. For scheme ``tls://`` it will instead use a secure TCP socket. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#url DataTlsCertificate#url}
-        :param verify_chain: Whether to verify the certificate chain while parsing it or not (default: ``true``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#verify_chain DataTlsCertificate#verify_chain}
+        :param content: The content of the certificate in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#content DataTlsCertificate#content}
+        :param url: URL of the endpoint to get the certificates from. Accepted schemes are: ``https``, ``tls``. For scheme ``https://`` it will use the HTTP protocol and apply the ``proxy`` configuration of the provider, if set. For scheme ``tls://`` it will instead use a secure TCP socket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#url DataTlsCertificate#url}
+        :param verify_chain: Whether to verify the certificate chain while parsing it or not (default: ``true``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#verify_chain DataTlsCertificate#verify_chain}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__816f7f18f8d1013954e54c545c1f6f647e0627164f7a91863cced3641b00650d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -446,20 +446,22 @@
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
@@ -501,37 +503,37 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def content(self) -> typing.Optional[builtins.str]:
         '''The content of the certificate in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#content DataTlsCertificate#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#content DataTlsCertificate#content}
         '''
         result = self._values.get("content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
         '''URL of the endpoint to get the certificates from.
 
         Accepted schemes are: ``https``, ``tls``. For scheme ``https://`` it will use the HTTP protocol and apply the ``proxy`` configuration of the provider, if set. For scheme ``tls://`` it will instead use a secure TCP socket.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#url DataTlsCertificate#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#url DataTlsCertificate#url}
         '''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def verify_chain(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to verify the certificate chain while parsing it or not (default: ``true``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/certificate#verify_chain DataTlsCertificate#verify_chain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/certificate#verify_chain DataTlsCertificate#verify_chain}
         '''
         result = self._values.get("verify_chain")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -558,15 +560,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     content: typing.Optional[builtins.str] = None,
     url: typing.Optional[builtins.str] = None,
     verify_chain: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -636,15 +638,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__816f7f18f8d1013954e54c545c1f6f647e0627164f7a91863cced3641b00650d(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     content: typing.Optional[builtins.str] = None,
     url: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tls_public_key`
 
-Refer to the Terraform Registory for docs: [`data_tls_public_key`](https://www.terraform.io/docs/providers/tls/d/public_key).
+Refer to the Terraform Registory for docs: [`data_tls_public_key`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataTlsPublicKey(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.dataTlsPublicKey.DataTlsPublicKey",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/d/public_key tls_public_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key tls_public_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         private_key_openssh: typing.Optional[builtins.str] = None,
         private_key_pem: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/d/public_key tls_public_key} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key tls_public_key} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param private_key_openssh: The private key (in `OpenSSH PEM (RFC 4716) <https://datatracker.ietf.org/doc/html/rfc4716>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_pem``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
-        :param private_key_pem: The private key (in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_openssh``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
+        :param private_key_openssh: The private key (in `OpenSSH PEM (RFC 4716) <https://datatracker.ietf.org/doc/html/rfc4716>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_pem``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
+        :param private_key_pem: The private key (in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_openssh``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -173,15 +173,15 @@
     },
 )
 class DataTlsPublicKeyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         private_key_openssh: typing.Optional[builtins.str] = None,
         private_key_pem: typing.Optional[builtins.str] = None,
@@ -190,16 +190,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param private_key_openssh: The private key (in `OpenSSH PEM (RFC 4716) <https://datatracker.ietf.org/doc/html/rfc4716>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_pem``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
-        :param private_key_pem: The private key (in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_openssh``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
+        :param private_key_openssh: The private key (in `OpenSSH PEM (RFC 4716) <https://datatracker.ietf.org/doc/html/rfc4716>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_pem``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
+        :param private_key_pem: The private key (in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_openssh``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1c9faaa7ba175f16df922503437b83d563bdb02fc554f97683939c66b122a8f3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -237,20 +237,22 @@
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
@@ -292,24 +294,24 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def private_key_openssh(self) -> typing.Optional[builtins.str]:
         '''The private key (in  `OpenSSH PEM (RFC 4716) <https://datatracker.ietf.org/doc/html/rfc4716>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_pem``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_openssh DataTlsPublicKey#private_key_openssh}
         '''
         result = self._values.get("private_key_openssh")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def private_key_pem(self) -> typing.Optional[builtins.str]:
         '''The private key (in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format) to extract the public key from. This is *mutually exclusive* with ``private_key_openssh``. Currently-supported algorithms for keys are: ``RSA``, ``ECDSA``, ``ED25519``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/d/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/data-sources/public_key#private_key_pem DataTlsPublicKey#private_key_pem}
         '''
         result = self._values.get("private_key_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -332,15 +334,15 @@
 def _typecheckingstub__b173e24869d78d1a5679eabe044faf297e7a097e473d1e0227822e32bed28523(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     private_key_openssh: typing.Optional[builtins.str] = None,
     private_key_pem: typing.Optional[builtins.str] = None,
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
@@ -357,15 +359,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1c9faaa7ba175f16df922503437b83d563bdb02fc554f97683939c66b122a8f3(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     private_key_openssh: typing.Optional[builtins.str] = None,
     private_key_pem: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tls_locally_signed_cert`
 
-Refer to the Terraform Registory for docs: [`tls_locally_signed_cert`](https://www.terraform.io/docs/providers/tls/r/locally_signed_cert).
+Refer to the Terraform Registory for docs: [`tls_locally_signed_cert`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class LocallySignedCert(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.locallySignedCert.LocallySignedCert",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert tls_locally_signed_cert}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert tls_locally_signed_cert}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         allowed_uses: typing.Sequence[builtins.str],
@@ -38,33 +38,33 @@
         ca_private_key_pem: builtins.str,
         cert_request_pem: builtins.str,
         validity_period_hours: jsii.Number,
         early_renewal_hours: typing.Optional[jsii.Number] = None,
         is_ca_certificate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set_subject_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert tls_locally_signed_cert} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert tls_locally_signed_cert} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
-        :param ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
-        :param cert_request_pem: Certificate request data in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
-        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
-        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
-        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
-        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
+        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
+        :param ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
+        :param cert_request_pem: Certificate request data in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
+        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
+        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
+        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
+        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -317,15 +317,15 @@
     },
 )
 class LocallySignedCertConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         allowed_uses: typing.Sequence[builtins.str],
         ca_cert_pem: builtins.str,
@@ -340,22 +340,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
-        :param ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
-        :param cert_request_pem: Certificate request data in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
-        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
-        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
-        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
-        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
+        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
+        :param ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
+        :param cert_request_pem: Certificate request data in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
+        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
+        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
+        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
+        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__200b4de7e400455fc367e1409cc253c18f300f93dc244c931a386c8de109ba88)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -407,20 +407,22 @@
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
@@ -464,89 +466,89 @@
 
     @builtins.property
     def allowed_uses(self) -> typing.List[builtins.str]:
         '''List of key usages allowed for the issued certificate.
 
         Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#allowed_uses LocallySignedCert#allowed_uses}
         '''
         result = self._values.get("allowed_uses")
         assert result is not None, "Required property 'allowed_uses' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def ca_cert_pem(self) -> builtins.str:
         '''Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_cert_pem LocallySignedCert#ca_cert_pem}
         '''
         result = self._values.get("ca_cert_pem")
         assert result is not None, "Required property 'ca_cert_pem' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_private_key_pem(self) -> builtins.str:
         '''Private key of the Certificate Authority (CA) used to sign the certificate, in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#ca_private_key_pem LocallySignedCert#ca_private_key_pem}
         '''
         result = self._values.get("ca_private_key_pem")
         assert result is not None, "Required property 'ca_private_key_pem' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cert_request_pem(self) -> builtins.str:
         '''Certificate request data in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#cert_request_pem LocallySignedCert#cert_request_pem}
         '''
         result = self._values.get("cert_request_pem")
         assert result is not None, "Required property 'cert_request_pem' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def validity_period_hours(self) -> jsii.Number:
         '''Number of hours, after initial issuing, that the certificate will remain valid for.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#validity_period_hours LocallySignedCert#validity_period_hours}
         '''
         result = self._values.get("validity_period_hours")
         assert result is not None, "Required property 'validity_period_hours' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def early_renewal_hours(self) -> typing.Optional[jsii.Number]:
         '''The resource will consider the certificate to have expired the given number of hours before its actual expiry time.
 
         This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``)
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#early_renewal_hours LocallySignedCert#early_renewal_hours}
         '''
         result = self._values.get("early_renewal_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def is_ca_certificate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Is the generated certificate representing a Certificate Authority (CA) (default: ``false``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#is_ca_certificate LocallySignedCert#is_ca_certificate}
         '''
         result = self._values.get("is_ca_certificate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def set_subject_key_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/locally_signed_cert#set_subject_key_id LocallySignedCert#set_subject_key_id}
         '''
         result = self._values.get("set_subject_key_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -575,15 +577,15 @@
     ca_private_key_pem: builtins.str,
     cert_request_pem: builtins.str,
     validity_period_hours: jsii.Number,
     early_renewal_hours: typing.Optional[jsii.Number] = None,
     is_ca_certificate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set_subject_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
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
@@ -636,15 +638,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__200b4de7e400455fc367e1409cc253c18f300f93dc244c931a386c8de109ba88(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     allowed_uses: typing.Sequence[builtins.str],
     ca_cert_pem: builtins.str,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tls_private_key`
 
-Refer to the Terraform Registory for docs: [`tls_private_key`](https://www.terraform.io/docs/providers/tls/r/private_key).
+Refer to the Terraform Registory for docs: [`tls_private_key`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class PrivateKey(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.privateKey.PrivateKey",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/r/private_key tls_private_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key tls_private_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         algorithm: builtins.str,
         ecdsa_curve: typing.Optional[builtins.str] = None,
         rsa_bits: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/r/private_key tls_private_key} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key tls_private_key} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param algorithm: Name of the algorithm to use when generating the private key. Currently-supported values are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#algorithm PrivateKey#algorithm}
-        :param ecdsa_curve: When ``algorithm`` is ``ECDSA``, the name of the elliptic curve to use. Currently-supported values are: ``P224``, ``P256``, ``P384``, ``P521``. (default: ``P224``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
-        :param rsa_bits: When ``algorithm`` is ``RSA``, the size of the generated RSA key, in bits (default: ``2048``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#rsa_bits PrivateKey#rsa_bits}
+        :param algorithm: Name of the algorithm to use when generating the private key. Currently-supported values are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#algorithm PrivateKey#algorithm}
+        :param ecdsa_curve: When ``algorithm`` is ``ECDSA``, the name of the elliptic curve to use. Currently-supported values are: ``P224``, ``P256``, ``P384``, ``P521``. (default: ``P224``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
+        :param rsa_bits: When ``algorithm`` is ``RSA``, the size of the generated RSA key, in bits (default: ``2048``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#rsa_bits PrivateKey#rsa_bits}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -204,15 +204,15 @@
     },
 )
 class PrivateKeyConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         algorithm: builtins.str,
         ecdsa_curve: typing.Optional[builtins.str] = None,
@@ -222,17 +222,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param algorithm: Name of the algorithm to use when generating the private key. Currently-supported values are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#algorithm PrivateKey#algorithm}
-        :param ecdsa_curve: When ``algorithm`` is ``ECDSA``, the name of the elliptic curve to use. Currently-supported values are: ``P224``, ``P256``, ``P384``, ``P521``. (default: ``P224``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
-        :param rsa_bits: When ``algorithm`` is ``RSA``, the size of the generated RSA key, in bits (default: ``2048``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#rsa_bits PrivateKey#rsa_bits}
+        :param algorithm: Name of the algorithm to use when generating the private key. Currently-supported values are: ``RSA``, ``ECDSA``, ``ED25519``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#algorithm PrivateKey#algorithm}
+        :param ecdsa_curve: When ``algorithm`` is ``ECDSA``, the name of the elliptic curve to use. Currently-supported values are: ``P224``, ``P256``, ``P384``, ``P521``. (default: ``P224``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
+        :param rsa_bits: When ``algorithm`` is ``RSA``, the size of the generated RSA key, in bits (default: ``2048``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#rsa_bits PrivateKey#rsa_bits}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e821c6d8bb32bc18961d9d9c6dc20c962abe38ce632acd7bab05981406915273)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -273,20 +273,22 @@
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
@@ -328,36 +330,36 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def algorithm(self) -> builtins.str:
         '''Name of the algorithm to use when generating the private key. Currently-supported values are: ``RSA``, ``ECDSA``, ``ED25519``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#algorithm PrivateKey#algorithm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#algorithm PrivateKey#algorithm}
         '''
         result = self._values.get("algorithm")
         assert result is not None, "Required property 'algorithm' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ecdsa_curve(self) -> typing.Optional[builtins.str]:
         '''When ``algorithm`` is ``ECDSA``, the name of the elliptic curve to use.
 
         Currently-supported values are: ``P224``, ``P256``, ``P384``, ``P521``. (default: ``P224``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#ecdsa_curve PrivateKey#ecdsa_curve}
         '''
         result = self._values.get("ecdsa_curve")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rsa_bits(self) -> typing.Optional[jsii.Number]:
         '''When ``algorithm`` is ``RSA``, the size of the generated RSA key, in bits (default: ``2048``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/private_key#rsa_bits PrivateKey#rsa_bits}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/private_key#rsa_bits PrivateKey#rsa_bits}
         '''
         result = self._values.get("rsa_bits")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -381,15 +383,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     algorithm: builtins.str,
     ecdsa_curve: typing.Optional[builtins.str] = None,
     rsa_bits: typing.Optional[jsii.Number] = None,
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
@@ -412,15 +414,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e821c6d8bb32bc18961d9d9c6dc20c962abe38ce632acd7bab05981406915273(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     algorithm: builtins.str,
     ecdsa_curve: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tls_self_signed_cert`
 
-Refer to the Terraform Registory for docs: [`tls_self_signed_cert`](https://www.terraform.io/docs/providers/tls/r/self_signed_cert).
+Refer to the Terraform Registory for docs: [`tls_self_signed_cert`](https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class SelfSignedCert(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tls.selfSignedCert.SelfSignedCert",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert tls_self_signed_cert}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert tls_self_signed_cert}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         allowed_uses: typing.Sequence[builtins.str],
@@ -41,36 +41,36 @@
         ip_addresses: typing.Optional[typing.Sequence[builtins.str]] = None,
         is_ca_certificate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set_authority_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set_subject_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         subject: typing.Optional[typing.Union["SelfSignedCertSubject", typing.Dict[builtins.str, typing.Any]]] = None,
         uris: typing.Optional[typing.Sequence[builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert tls_self_signed_cert} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert tls_self_signed_cert} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
-        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
-        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
-        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#dns_names SelfSignedCert#dns_names}
-        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
-        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
-        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
-        :param set_authority_key_id: Should the generated certificate include an `authority key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1>`_: for self-signed certificates this is the same value as the `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
-        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
-        :param subject: subject block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#subject SelfSignedCert#subject}
-        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#uris SelfSignedCert#uris}
+        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
+        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
+        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
+        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#dns_names SelfSignedCert#dns_names}
+        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
+        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
+        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
+        :param set_authority_key_id: Should the generated certificate include an `authority key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1>`_: for self-signed certificates this is the same value as the `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
+        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
+        :param subject: subject block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#subject SelfSignedCert#subject}
+        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#uris SelfSignedCert#uris}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -113,23 +113,23 @@
         organizational_unit: typing.Optional[builtins.str] = None,
         postal_code: typing.Optional[builtins.str] = None,
         province: typing.Optional[builtins.str] = None,
         serial_number: typing.Optional[builtins.str] = None,
         street_address: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#common_name SelfSignedCert#common_name}
-        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#country SelfSignedCert#country}
-        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#locality SelfSignedCert#locality}
-        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organization SelfSignedCert#organization}
-        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
-        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#postal_code SelfSignedCert#postal_code}
-        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#province SelfSignedCert#province}
-        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#serial_number SelfSignedCert#serial_number}
-        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#street_address SelfSignedCert#street_address}
+        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#common_name SelfSignedCert#common_name}
+        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#country SelfSignedCert#country}
+        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#locality SelfSignedCert#locality}
+        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organization SelfSignedCert#organization}
+        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
+        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#postal_code SelfSignedCert#postal_code}
+        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#province SelfSignedCert#province}
+        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#serial_number SelfSignedCert#serial_number}
+        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#street_address SelfSignedCert#street_address}
         '''
         value = SelfSignedCertSubject(
             common_name=common_name,
             country=country,
             locality=locality,
             organization=organization,
             organizational_unit=organizational_unit,
@@ -439,15 +439,15 @@
     },
 )
 class SelfSignedCertConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         allowed_uses: typing.Sequence[builtins.str],
         private_key_pem: builtins.str,
@@ -465,25 +465,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
-        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
-        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
-        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#dns_names SelfSignedCert#dns_names}
-        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
-        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
-        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
-        :param set_authority_key_id: Should the generated certificate include an `authority key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1>`_: for self-signed certificates this is the same value as the `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
-        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
-        :param subject: subject block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#subject SelfSignedCert#subject}
-        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#uris SelfSignedCert#uris}
+        :param allowed_uses: List of key usages allowed for the issued certificate. Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
+        :param private_key_pem: Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
+        :param validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
+        :param dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#dns_names SelfSignedCert#dns_names}
+        :param early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
+        :param ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
+        :param is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
+        :param set_authority_key_id: Should the generated certificate include an `authority key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1>`_: for self-signed certificates this is the same value as the `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
+        :param set_subject_key_id: Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
+        :param subject: subject block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#subject SelfSignedCert#subject}
+        :param uris: List of URIs for which a certificate is being requested (i.e. certificate subjects). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#uris SelfSignedCert#uris}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(subject, dict):
             subject = SelfSignedCertSubject(**subject)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3c90b0ca48ac264c883ba6f6404b6bc1015ce6da51d1b57efc09b5d1e5a4b9aa)
@@ -548,20 +548,22 @@
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
@@ -605,116 +607,116 @@
 
     @builtins.property
     def allowed_uses(self) -> typing.List[builtins.str]:
         '''List of key usages allowed for the issued certificate.
 
         Values are defined in `RFC 5280 <https://datatracker.ietf.org/doc/html/rfc5280>`_ and combine flags defined by both `Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3>`_ and `Extended Key Usages <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12>`_. Accepted values: ``any_extended``, ``cert_signing``, ``client_auth``, ``code_signing``, ``content_commitment``, ``crl_signing``, ``data_encipherment``, ``decipher_only``, ``digital_signature``, ``email_protection``, ``encipher_only``, ``ipsec_end_system``, ``ipsec_tunnel``, ``ipsec_user``, ``key_agreement``, ``key_encipherment``, ``microsoft_commercial_code_signing``, ``microsoft_kernel_code_signing``, ``microsoft_server_gated_crypto``, ``netscape_server_gated_crypto``, ``ocsp_signing``, ``server_auth``, ``timestamping``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#allowed_uses SelfSignedCert#allowed_uses}
         '''
         result = self._values.get("allowed_uses")
         assert result is not None, "Required property 'allowed_uses' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def private_key_pem(self) -> builtins.str:
         '''Private key in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format, that the certificate will belong to. This can be read from a separate file using the ```file`` <https://www.terraform.io/language/functions/file>`_ interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#private_key_pem SelfSignedCert#private_key_pem}
         '''
         result = self._values.get("private_key_pem")
         assert result is not None, "Required property 'private_key_pem' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def validity_period_hours(self) -> jsii.Number:
         '''Number of hours, after initial issuing, that the certificate will remain valid for.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#validity_period_hours SelfSignedCert#validity_period_hours}
         '''
         result = self._values.get("validity_period_hours")
         assert result is not None, "Required property 'validity_period_hours' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def dns_names(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of DNS names for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#dns_names SelfSignedCert#dns_names}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#dns_names SelfSignedCert#dns_names}
         '''
         result = self._values.get("dns_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def early_renewal_hours(self) -> typing.Optional[jsii.Number]:
         '''The resource will consider the certificate to have expired the given number of hours before its actual expiry time.
 
         This can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the early renewal period. (default: ``0``)
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#early_renewal_hours SelfSignedCert#early_renewal_hours}
         '''
         result = self._values.get("early_renewal_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def ip_addresses(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#ip_addresses SelfSignedCert#ip_addresses}
         '''
         result = self._values.get("ip_addresses")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def is_ca_certificate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Is the generated certificate representing a Certificate Authority (CA) (default: ``false``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#is_ca_certificate SelfSignedCert#is_ca_certificate}
         '''
         result = self._values.get("is_ca_certificate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def set_authority_key_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Should the generated certificate include an `authority key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1>`_: for self-signed certificates this is the same value as the `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_authority_key_id SelfSignedCert#set_authority_key_id}
         '''
         result = self._values.get("set_authority_key_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def set_subject_key_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Should the generated certificate include a `subject key identifier <https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2>`_ (default: ``false``).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#set_subject_key_id SelfSignedCert#set_subject_key_id}
         '''
         result = self._values.get("set_subject_key_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def subject(self) -> typing.Optional["SelfSignedCertSubject"]:
         '''subject block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#subject SelfSignedCert#subject}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#subject SelfSignedCert#subject}
         '''
         result = self._values.get("subject")
         return typing.cast(typing.Optional["SelfSignedCertSubject"], result)
 
     @builtins.property
     def uris(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of URIs for which a certificate is being requested (i.e. certificate subjects).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#uris SelfSignedCert#uris}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#uris SelfSignedCert#uris}
         '''
         result = self._values.get("uris")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -753,23 +755,23 @@
         organizational_unit: typing.Optional[builtins.str] = None,
         postal_code: typing.Optional[builtins.str] = None,
         province: typing.Optional[builtins.str] = None,
         serial_number: typing.Optional[builtins.str] = None,
         street_address: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#common_name SelfSignedCert#common_name}
-        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#country SelfSignedCert#country}
-        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#locality SelfSignedCert#locality}
-        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organization SelfSignedCert#organization}
-        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
-        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#postal_code SelfSignedCert#postal_code}
-        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#province SelfSignedCert#province}
-        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#serial_number SelfSignedCert#serial_number}
-        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#street_address SelfSignedCert#street_address}
+        :param common_name: Distinguished name: ``CN``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#common_name SelfSignedCert#common_name}
+        :param country: Distinguished name: ``C``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#country SelfSignedCert#country}
+        :param locality: Distinguished name: ``L``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#locality SelfSignedCert#locality}
+        :param organization: Distinguished name: ``O``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organization SelfSignedCert#organization}
+        :param organizational_unit: Distinguished name: ``OU``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
+        :param postal_code: Distinguished name: ``PC``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#postal_code SelfSignedCert#postal_code}
+        :param province: Distinguished name: ``ST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#province SelfSignedCert#province}
+        :param serial_number: Distinguished name: ``SERIALNUMBER``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#serial_number SelfSignedCert#serial_number}
+        :param street_address: Distinguished name: ``STREET``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#street_address SelfSignedCert#street_address}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0ff2e19ab5c6a3a521c208f4eb5e753ac61cdcb3cf45e7901747ebacd18b4a74)
             check_type(argname="argument common_name", value=common_name, expected_type=type_hints["common_name"])
             check_type(argname="argument country", value=country, expected_type=type_hints["country"])
             check_type(argname="argument locality", value=locality, expected_type=type_hints["locality"])
             check_type(argname="argument organization", value=organization, expected_type=type_hints["organization"])
@@ -798,87 +800,87 @@
         if street_address is not None:
             self._values["street_address"] = street_address
 
     @builtins.property
     def common_name(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``CN``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#common_name SelfSignedCert#common_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#common_name SelfSignedCert#common_name}
         '''
         result = self._values.get("common_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def country(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``C``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#country SelfSignedCert#country}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#country SelfSignedCert#country}
         '''
         result = self._values.get("country")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def locality(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``L``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#locality SelfSignedCert#locality}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#locality SelfSignedCert#locality}
         '''
         result = self._values.get("locality")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``O``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organization SelfSignedCert#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organization SelfSignedCert#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organizational_unit(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``OU``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#organizational_unit SelfSignedCert#organizational_unit}
         '''
         result = self._values.get("organizational_unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def postal_code(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``PC``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#postal_code SelfSignedCert#postal_code}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#postal_code SelfSignedCert#postal_code}
         '''
         result = self._values.get("postal_code")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def province(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``ST``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#province SelfSignedCert#province}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#province SelfSignedCert#province}
         '''
         result = self._values.get("province")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def serial_number(self) -> typing.Optional[builtins.str]:
         '''Distinguished name: ``SERIALNUMBER``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#serial_number SelfSignedCert#serial_number}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#serial_number SelfSignedCert#serial_number}
         '''
         result = self._values.get("serial_number")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def street_address(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Distinguished name: ``STREET``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/tls/r/self_signed_cert#street_address SelfSignedCert#street_address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tls/4.0.4/docs/resources/self_signed_cert#street_address SelfSignedCert#street_address}
         '''
         result = self._values.get("street_address")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1134,15 +1136,15 @@
     ip_addresses: typing.Optional[typing.Sequence[builtins.str]] = None,
     is_ca_certificate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set_authority_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set_subject_key_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     subject: typing.Optional[typing.Union[SelfSignedCertSubject, typing.Dict[builtins.str, typing.Any]]] = None,
     uris: typing.Optional[typing.Sequence[builtins.str]] = None,
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
@@ -1207,15 +1209,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3c90b0ca48ac264c883ba6f6404b6bc1015ce6da51d1b57efc09b5d1e5a4b9aa(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     allowed_uses: typing.Sequence[builtins.str],
     private_key_pem: builtins.str,
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tls
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt tls Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tls.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tls.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-tls-go`](https://github.com/cdktf/cdktf-provider-tls-go) package.
 
 `go get github.com/cdktf/cdktf-provider-tls-go/tls`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-tls).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform tls Provider version 1:1. In fact, it always tracks `latest` of `~> 4.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-tls-5.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-tls-6.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_tls/py.typed
 src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_tls.egg-info/requires.txt
 src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
 src/cdktf_cdktf_provider_tls/_jsii/__init__.py
-src/cdktf_cdktf_provider_tls/_jsii/provider-tls@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_tls/_jsii/provider-tls@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_tls/cert_request/__init__.py
 src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
 src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
 src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
 src/cdktf_cdktf_provider_tls/private_key/__init__.py
 src/cdktf_cdktf_provider_tls/provider/__init__.py
 src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
```

