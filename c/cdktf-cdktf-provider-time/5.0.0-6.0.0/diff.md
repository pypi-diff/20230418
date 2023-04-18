# Comparing `tmp/cdktf-cdktf-provider-time-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-time-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-time-5.0.0.tar", last modified: Tue Jan 17 14:49:27 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-time-6.0.0.tar", last modified: Tue Apr 18 20:54:26 2023, max compression
```

## Comparing `cdktf-cdktf-provider-time-5.0.0.tar` & `cdktf-cdktf-provider-time-6.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.199423 cdktf-cdktf-provider-time-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:49:27.199423 cdktf-cdktf-provider-time-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/_jsii/provider-time@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/offset/
--rw-r--r--   0 runner    (1001) docker     (123)    35489 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/rotating/
--rw-r--r--   0 runner    (1001) docker     (123)    38581 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/sleep/
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/static_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-01-17 14:49:13.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:49:27.195423 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:49:26.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-17 14:49:27.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:49:26.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:49:27.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-17 14:49:27.000000 cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:54:14.000000 cdktf-cdktf-provider-time-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.946295 cdktf-cdktf-provider-time-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.946295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.946295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118811 2023-04-18 20:54:14.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/_jsii/provider-time@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.946295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/offset/
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/rotating/
+-rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/sleep/
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.950295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/static_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-04-18 20:54:15.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:54:26.946295 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:54:26.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 20:54:26.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:54:26.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:54:26.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:54:26.000000 cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/LICENSE` & `cdktf-cdktf-provider-time-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-time-6.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-time-go`](https://github.com/cdktf/cdktf-provider-time-go) package.
 
 `go get github.com/cdktf/cdktf-provider-time-go/time`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-time).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/README.md` & `cdktf-cdktf-provider-time-6.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-time-go`](https://github.com/cdktf/cdktf-provider-time-go) package.
 
 `go get github.com/cdktf/cdktf-provider-time-go/time`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-time).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/setup.py` & `cdktf-cdktf-provider-time-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-time",
-    "version": "5.0.0",
+    "version": "6.0.0",
     "description": "Prebuilt time Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-time.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,37 +27,38 @@
         "cdktf_cdktf_provider_time.provider",
         "cdktf_cdktf_provider_time.rotating",
         "cdktf_cdktf_provider_time.sleep",
         "cdktf_cdktf_provider_time.static_resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_time._jsii": [
-            "provider-time@5.0.0.jsii.tgz"
+            "provider-time@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_time": [
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

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-time-go`](https://github.com/cdktf/cdktf-provider-time-go) package.
 
 `go get github.com/cdktf/cdktf-provider-time-go/time`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-time).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_offset`
 
-Refer to the Terraform Registory for docs: [`time_offset`](https://www.terraform.io/docs/providers/time/r/offset).
+Refer to the Terraform Registory for docs: [`time_offset`](https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Offset(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.offset.Offset",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/time/r/offset time_offset}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset time_offset}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         base_rfc3339: typing.Optional[builtins.str] = None,
@@ -38,33 +38,33 @@
         offset_hours: typing.Optional[jsii.Number] = None,
         offset_minutes: typing.Optional[jsii.Number] = None,
         offset_months: typing.Optional[jsii.Number] = None,
         offset_seconds: typing.Optional[jsii.Number] = None,
         offset_years: typing.Optional[jsii.Number] = None,
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/time/r/offset time_offset} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset time_offset} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#base_rfc3339 Offset#base_rfc3339}
-        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_days Offset#offset_days}
-        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_hours Offset#offset_hours}
-        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_minutes Offset#offset_minutes}
-        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_months Offset#offset_months}
-        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_seconds Offset#offset_seconds}
-        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_years Offset#offset_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#triggers Offset#triggers}
+        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
+        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_days Offset#offset_days}
+        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_hours Offset#offset_hours}
+        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_minutes Offset#offset_minutes}
+        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_months Offset#offset_months}
+        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_seconds Offset#offset_seconds}
+        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_years Offset#offset_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#triggers Offset#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -340,15 +340,15 @@
     },
 )
 class OffsetConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         base_rfc3339: typing.Optional[builtins.str] = None,
         offset_days: typing.Optional[jsii.Number] = None,
@@ -363,22 +363,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#base_rfc3339 Offset#base_rfc3339}
-        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_days Offset#offset_days}
-        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_hours Offset#offset_hours}
-        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_minutes Offset#offset_minutes}
-        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_months Offset#offset_months}
-        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_seconds Offset#offset_seconds}
-        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_years Offset#offset_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#triggers Offset#triggers}
+        :param base_rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
+        :param offset_days: Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_days Offset#offset_days}
+        :param offset_hours: Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_hours Offset#offset_hours}
+        :param offset_minutes: Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_minutes Offset#offset_minutes}
+        :param offset_months: Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_months Offset#offset_months}
+        :param offset_seconds: Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_seconds Offset#offset_seconds}
+        :param offset_years: Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_years Offset#offset_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#triggers Offset#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__129647c305336dbf1cae2ce70d04cb6a6fee40863714fac62a4bfe71187fa828)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -434,20 +434,22 @@
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
@@ -489,80 +491,80 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def base_rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#base_rfc3339 Offset#base_rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#base_rfc3339 Offset#base_rfc3339}
         '''
         result = self._values.get("base_rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def offset_days(self) -> typing.Optional[jsii.Number]:
         '''Number of days to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_days Offset#offset_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_days Offset#offset_days}
         '''
         result = self._values.get("offset_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_hours(self) -> typing.Optional[jsii.Number]:
         '''Number of hours to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_hours Offset#offset_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_hours Offset#offset_hours}
         '''
         result = self._values.get("offset_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_minutes(self) -> typing.Optional[jsii.Number]:
         '''Number of minutes to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_minutes Offset#offset_minutes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_minutes Offset#offset_minutes}
         '''
         result = self._values.get("offset_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_months(self) -> typing.Optional[jsii.Number]:
         '''Number of months to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_months Offset#offset_months}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_months Offset#offset_months}
         '''
         result = self._values.get("offset_months")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_seconds(self) -> typing.Optional[jsii.Number]:
         '''Number of seconds to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_seconds Offset#offset_seconds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_seconds Offset#offset_seconds}
         '''
         result = self._values.get("offset_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def offset_years(self) -> typing.Optional[jsii.Number]:
         '''Number of years to offset the base timestamp. At least one of the 'offset_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#offset_years Offset#offset_years}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#offset_years Offset#offset_years}
         '''
         result = self._values.get("offset_years")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/offset#triggers Offset#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/offset#triggers Offset#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -591,15 +593,15 @@
     offset_hours: typing.Optional[jsii.Number] = None,
     offset_minutes: typing.Optional[jsii.Number] = None,
     offset_months: typing.Optional[jsii.Number] = None,
     offset_seconds: typing.Optional[jsii.Number] = None,
     offset_years: typing.Optional[jsii.Number] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -652,15 +654,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__129647c305336dbf1cae2ce70d04cb6a6fee40863714fac62a4bfe71187fa828(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     base_rfc3339: typing.Optional[builtins.str] = None,
     offset_days: typing.Optional[jsii.Number] = None,
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`time`](https://www.terraform.io/docs/providers/time).
+Refer to the Terraform Registory for docs: [`time`](https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class TimeProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.provider.TimeProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/time time}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs time}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/time time} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs time} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time#alias TimeProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs#alias TimeProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c869539a3d05780607af068e02b355518195eadc27a829071227e5c37a3a6b69)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = TimeProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-time.provider.TimeProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class TimeProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time#alias TimeProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs#alias TimeProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__77704b117f84b4019cf445d89efdcfb386e41b68dfdf53448bbb9298a0e4435f)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time#alias TimeProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs#alias TimeProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_rotating`
 
-Refer to the Terraform Registory for docs: [`time_rotating`](https://www.terraform.io/docs/providers/time/r/rotating).
+Refer to the Terraform Registory for docs: [`time_rotating`](https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Rotating(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.rotating.Rotating",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/time/r/rotating time_rotating}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating time_rotating}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         rfc3339: typing.Optional[builtins.str] = None,
@@ -38,33 +38,33 @@
         rotation_hours: typing.Optional[jsii.Number] = None,
         rotation_minutes: typing.Optional[jsii.Number] = None,
         rotation_months: typing.Optional[jsii.Number] = None,
         rotation_rfc3339: typing.Optional[builtins.str] = None,
         rotation_years: typing.Optional[jsii.Number] = None,
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/time/r/rotating time_rotating} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating time_rotating} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rfc3339 Rotating#rfc3339}
-        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_days Rotating#rotation_days}
-        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_hours Rotating#rotation_hours}
-        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_minutes Rotating#rotation_minutes}
-        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_months Rotating#rotation_months}
-        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
-        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_years Rotating#rotation_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#triggers Rotating#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rfc3339 Rotating#rfc3339}
+        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_days Rotating#rotation_days}
+        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
+        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
+        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_months Rotating#rotation_months}
+        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_years Rotating#rotation_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#triggers Rotating#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -335,15 +335,15 @@
     },
 )
 class RotatingConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         rfc3339: typing.Optional[builtins.str] = None,
         rotation_days: typing.Optional[jsii.Number] = None,
@@ -358,22 +358,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rfc3339 Rotating#rfc3339}
-        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_days Rotating#rotation_days}
-        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_hours Rotating#rotation_hours}
-        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_minutes Rotating#rotation_minutes}
-        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_months Rotating#rotation_months}
-        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
-        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_years Rotating#rotation_years}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#triggers Rotating#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rfc3339 Rotating#rfc3339}
+        :param rotation_days: Number of days to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_days Rotating#rotation_days}
+        :param rotation_hours: Number of hours to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
+        :param rotation_minutes: Number of minutes to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
+        :param rotation_months: Number of months to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_months Rotating#rotation_months}
+        :param rotation_rfc3339: Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        :param rotation_years: Number of years to add to the base timestamp to configure the rotation timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_years Rotating#rotation_years}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#triggers Rotating#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9ff127dfa3aa123c42955f732770508fb130fcb2094145ead1fd7fbe2809aa7e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -429,20 +429,22 @@
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
@@ -484,90 +486,90 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rfc3339 Rotating#rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rfc3339 Rotating#rfc3339}
         '''
         result = self._values.get("rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rotation_days(self) -> typing.Optional[jsii.Number]:
         '''Number of days to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_days Rotating#rotation_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_days Rotating#rotation_days}
         '''
         result = self._values.get("rotation_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_hours(self) -> typing.Optional[jsii.Number]:
         '''Number of hours to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_hours Rotating#rotation_hours}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_hours Rotating#rotation_hours}
         '''
         result = self._values.get("rotation_hours")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_minutes(self) -> typing.Optional[jsii.Number]:
         '''Number of minutes to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_minutes Rotating#rotation_minutes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_minutes Rotating#rotation_minutes}
         '''
         result = self._values.get("rotation_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_months(self) -> typing.Optional[jsii.Number]:
         '''Number of months to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_months Rotating#rotation_months}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_months Rotating#rotation_months}
         '''
         result = self._values.get("rotation_months")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def rotation_rfc3339(self) -> typing.Optional[builtins.str]:
         '''Configure the rotation timestamp with an `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format of the offset timestamp. When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_rfc3339 Rotating#rotation_rfc3339}
         '''
         result = self._values.get("rotation_rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rotation_years(self) -> typing.Optional[jsii.Number]:
         '''Number of years to add to the base timestamp to configure the rotation timestamp.
 
         When the current time has passed the rotation timestamp, the resource will trigger recreation. At least one of the 'rotation_' arguments must be configured.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#rotation_years Rotating#rotation_years}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#rotation_years Rotating#rotation_years}
         '''
         result = self._values.get("rotation_years")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         These conditions recreate the resource in addition to other rotation arguments. See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/rotating#triggers Rotating#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/rotating#triggers Rotating#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -596,15 +598,15 @@
     rotation_hours: typing.Optional[jsii.Number] = None,
     rotation_minutes: typing.Optional[jsii.Number] = None,
     rotation_months: typing.Optional[jsii.Number] = None,
     rotation_rfc3339: typing.Optional[builtins.str] = None,
     rotation_years: typing.Optional[jsii.Number] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -657,15 +659,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9ff127dfa3aa123c42955f732770508fb130fcb2094145ead1fd7fbe2809aa7e(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     rfc3339: typing.Optional[builtins.str] = None,
     rotation_days: typing.Optional[jsii.Number] = None,
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_sleep`
 
-Refer to the Terraform Registory for docs: [`time_sleep`](https://www.terraform.io/docs/providers/time/r/sleep).
+Refer to the Terraform Registory for docs: [`time_sleep`](https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class Sleep(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.sleep.Sleep",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/time/r/sleep time_sleep}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep time_sleep}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         create_duration: typing.Optional[builtins.str] = None,
         destroy_duration: typing.Optional[builtins.str] = None,
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/time/r/sleep time_sleep} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep time_sleep} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#create_duration Sleep#create_duration}
-        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#destroy_duration Sleep#destroy_duration}
-        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#triggers Sleep#triggers}
+        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#create_duration Sleep#create_duration}
+        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
+        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#triggers Sleep#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -175,15 +175,15 @@
     },
 )
 class SleepConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         create_duration: typing.Optional[builtins.str] = None,
         destroy_duration: typing.Optional[builtins.str] = None,
@@ -193,17 +193,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#create_duration Sleep#create_duration}
-        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#destroy_duration Sleep#destroy_duration}
-        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#triggers Sleep#triggers}
+        :param create_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#create_duration Sleep#create_duration}
+        :param destroy_duration: `Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
+        :param triggers: (Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#triggers Sleep#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2a5326ad9173cd184a5987482265cc897932e1ea5d86f4294def627dc1a98c34)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -244,20 +244,22 @@
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
@@ -299,35 +301,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def create_duration(self) -> typing.Optional[builtins.str]:
         '''`Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource creation. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#create_duration Sleep#create_duration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#create_duration Sleep#create_duration}
         '''
         result = self._values.get("create_duration")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def destroy_duration(self) -> typing.Optional[builtins.str]:
         '''`Time duration <https://golang.org/pkg/time/#ParseDuration>`_ to delay resource destroy. For example, ``30s`` for 30 seconds or ``5m`` for 5 minutes. Updating this value by itself will not trigger a delay. This value or any updates to it must be successfully applied into the Terraform state before destroying this resource to take effect.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#destroy_duration Sleep#destroy_duration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#destroy_duration Sleep#destroy_duration}
         '''
         result = self._values.get("destroy_duration")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(Optional) Arbitrary map of values that, when changed, will run any creation or destroy delays again.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/sleep#triggers Sleep#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/sleep#triggers Sleep#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -351,15 +353,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     create_duration: typing.Optional[builtins.str] = None,
     destroy_duration: typing.Optional[builtins.str] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -382,15 +384,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2a5326ad9173cd184a5987482265cc897932e1ea5d86f4294def627dc1a98c34(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     create_duration: typing.Optional[builtins.str] = None,
     destroy_duration: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `time_static`
 
-Refer to the Terraform Registory for docs: [`time_static`](https://www.terraform.io/docs/providers/time/r/static).
+Refer to the Terraform Registory for docs: [`time_static`](https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class StaticResource(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-time.staticResource.StaticResource",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/time/r/static time_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static time_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         rfc3339: typing.Optional[builtins.str] = None,
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/time/r/static time_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static time_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#rfc3339 StaticResource#rfc3339}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#triggers StaticResource#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#rfc3339 StaticResource#rfc3339}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#triggers StaticResource#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -185,15 +185,15 @@
     },
 )
 class StaticResourceConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         rfc3339: typing.Optional[builtins.str] = None,
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
@@ -202,16 +202,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#rfc3339 StaticResource#rfc3339}
-        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#triggers StaticResource#triggers}
+        :param rfc3339: Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#rfc3339 StaticResource#rfc3339}
+        :param triggers: Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved. See `the main provider documentation <../index.md>`_ for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#triggers StaticResource#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4c379934e27cbed249355b819eba1f15c20fc2c2b6039e308a1ebfcb6edc88e6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -249,20 +249,22 @@
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
@@ -304,26 +306,26 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def rfc3339(self) -> typing.Optional[builtins.str]:
         '''Base timestamp in `RFC3339 <https://datatracker.ietf.org/doc/html/rfc3339#section-5.8>`_ format (see `RFC3339 time string <https://tools.ietf.org/html/rfc3339#section-5.8>`_ e.g., ``YYYY-MM-DDTHH:MM:SSZ``). Defaults to the current time.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#rfc3339 StaticResource#rfc3339}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#rfc3339 StaticResource#rfc3339}
         '''
         result = self._values.get("rfc3339")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Arbitrary map of values that, when changed, will trigger a new base timestamp value to be saved.
 
         See `the main provider documentation <../index.md>`_ for more information.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/time/r/static#triggers StaticResource#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/time/0.9.1/docs/resources/static#triggers StaticResource#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -346,15 +348,15 @@
 def _typecheckingstub__f061a57a3a7c557ef0911ddab138eb0f2059fdca2cc10c05eaa3f60f948e900f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     rfc3339: typing.Optional[builtins.str] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -371,15 +373,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4c379934e27cbed249355b819eba1f15c20fc2c2b6039e308a1ebfcb6edc88e6(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     rfc3339: typing.Optional[builtins.str] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-time-go`](https://github.com/cdktf/cdktf-provider-time-go) package.
 
 `go get github.com/cdktf/cdktf-provider-time-go/time`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-time).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform time Provider version 1:1. In fact, it always tracks `latest` of `~> 0.7` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-time-5.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-time-6.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_time/py.typed
 src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_time.egg-info/requires.txt
 src/cdktf_cdktf_provider_time.egg-info/top_level.txt
 src/cdktf_cdktf_provider_time/_jsii/__init__.py
-src/cdktf_cdktf_provider_time/_jsii/provider-time@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_time/_jsii/provider-time@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_time/offset/__init__.py
 src/cdktf_cdktf_provider_time/provider/__init__.py
 src/cdktf_cdktf_provider_time/rotating/__init__.py
 src/cdktf_cdktf_provider_time/sleep/__init__.py
 src/cdktf_cdktf_provider_time/static_resource/__init__.py
```

