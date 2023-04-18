# Comparing `tmp/cdktf-cdktf-provider-null-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-null-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-null-5.0.0.tar", last modified: Tue Jan 17 14:54:40 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-null-6.0.0.tar", last modified: Tue Apr 18 20:47:41 2023, max compression
```

## Comparing `cdktf-cdktf-provider-null-5.0.0.tar` & `cdktf-cdktf-provider-null-6.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/_jsii/provider-null@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-01-17 14:54:27.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:54:40.836332 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:54:40.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-17 14:54:40.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:54:40.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:54:40.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-17 14:54:40.000000 cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48779 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/LICENSE` & `cdktf-cdktf-provider-null-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-null-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-null-go`](https://github.com/cdktf/cdktf-provider-null-go) package.
 
 `go get github.com/cdktf/cdktf-provider-null-go/null`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-null).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/README.md` & `cdktf-cdktf-provider-null-6.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-null-go`](https://github.com/cdktf/cdktf-provider-null-go) package.
 
 `go get github.com/cdktf/cdktf-provider-null-go/null`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-null).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/setup.py` & `cdktf-cdktf-provider-null-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-null",
-    "version": "5.0.0",
+    "version": "6.0.0",
     "description": "Prebuilt null Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-null.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,37 +25,38 @@
         "cdktf_cdktf_provider_null._jsii",
         "cdktf_cdktf_provider_null.data_null_data_source",
         "cdktf_cdktf_provider_null.provider",
         "cdktf_cdktf_provider_null.resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_null._jsii": [
-            "provider-null@5.0.0.jsii.tgz"
+            "provider-null@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_null": [
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

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/__init__.py` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-null-go`](https://github.com/cdktf/cdktf-provider-null-go) package.
 
 `go get github.com/cdktf/cdktf-provider-null-go/null`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-null).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_null_data_source`
 
-Refer to the Terraform Registory for docs: [`data_null_data_source`](https://www.terraform.io/docs/providers/null/d/data_source).
+Refer to the Terraform Registory for docs: [`data_null_data_source`](https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataNullDataSource(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-null.dataNullDataSource.DataNullDataSource",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/null/d/data_source null_data_source}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source null_data_source}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         has_computed_default: typing.Optional[builtins.str] = None,
         inputs: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/null/d/data_source null_data_source} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source null_data_source} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param has_computed_default: If set, its literal value will be stored and returned. If not, its value defaults to ``"default"``. This argument exists primarily for testing and has little practical use. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#has_computed_default DataNullDataSource#has_computed_default}
-        :param inputs: A map of arbitrary strings that is copied into the ``outputs`` attribute, and accessible directly for interpolation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#inputs DataNullDataSource#inputs}
+        :param has_computed_default: If set, its literal value will be stored and returned. If not, its value defaults to ``"default"``. This argument exists primarily for testing and has little practical use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#has_computed_default DataNullDataSource#has_computed_default}
+        :param inputs: A map of arbitrary strings that is copied into the ``outputs`` attribute, and accessible directly for interpolation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#inputs DataNullDataSource#inputs}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -160,15 +160,15 @@
     },
 )
 class DataNullDataSourceConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         has_computed_default: typing.Optional[builtins.str] = None,
         inputs: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
@@ -177,16 +177,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param has_computed_default: If set, its literal value will be stored and returned. If not, its value defaults to ``"default"``. This argument exists primarily for testing and has little practical use. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#has_computed_default DataNullDataSource#has_computed_default}
-        :param inputs: A map of arbitrary strings that is copied into the ``outputs`` attribute, and accessible directly for interpolation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#inputs DataNullDataSource#inputs}
+        :param has_computed_default: If set, its literal value will be stored and returned. If not, its value defaults to ``"default"``. This argument exists primarily for testing and has little practical use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#has_computed_default DataNullDataSource#has_computed_default}
+        :param inputs: A map of arbitrary strings that is copied into the ``outputs`` attribute, and accessible directly for interpolation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#inputs DataNullDataSource#inputs}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3f568bdc8bb6bdecd54349de76ea70485f40bb46ff3713de78791ae5af03e137)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -224,20 +224,22 @@
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
@@ -281,24 +283,24 @@
 
     @builtins.property
     def has_computed_default(self) -> typing.Optional[builtins.str]:
         '''If set, its literal value will be stored and returned.
 
         If not, its value defaults to ``"default"``. This argument exists primarily for testing and has little practical use.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#has_computed_default DataNullDataSource#has_computed_default}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#has_computed_default DataNullDataSource#has_computed_default}
         '''
         result = self._values.get("has_computed_default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def inputs(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of arbitrary strings that is copied into the ``outputs`` attribute, and accessible directly for interpolation.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/d/data_source#inputs DataNullDataSource#inputs}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/data-sources/data_source#inputs DataNullDataSource#inputs}
         '''
         result = self._values.get("inputs")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -321,15 +323,15 @@
 def _typecheckingstub__82870f086fbf4531c4484ed3edd4fb896b182475269d815fdb6c097c9e44da36(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     has_computed_default: typing.Optional[builtins.str] = None,
     inputs: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -346,15 +348,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3f568bdc8bb6bdecd54349de76ea70485f40bb46ff3713de78791ae5af03e137(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     has_computed_default: typing.Optional[builtins.str] = None,
     inputs: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`null`](https://www.terraform.io/docs/providers/null).
+Refer to the Terraform Registory for docs: [`null`](https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class NullProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-null.provider.NullProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/null null}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs null}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/null null} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs null} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null#alias NullProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs#alias NullProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6826303cd7fcf4d5f4d1627fdf9eb3c2fd60863476f6bb3072f57ac805f93238)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = NullProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-null.provider.NullProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class NullProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null#alias NullProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs#alias NullProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bdd958f653e70674d82d3f344415628311071ee1569cb7b2ca2cda66f3d816bf)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null#alias NullProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs#alias NullProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `null_resource`
 
-Refer to the Terraform Registory for docs: [`null_resource`](https://www.terraform.io/docs/providers/null/r/resource).
+Refer to the Terraform Registory for docs: [`null_resource`](https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class Resource(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-null.resource.Resource",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/null/r/resource null_resource}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource null_resource}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
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
-        '''Create a new {@link https://www.terraform.io/docs/providers/null/r/resource null_resource} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource null_resource} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param triggers: A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/r/resource#triggers Resource#triggers}
+        :param triggers: A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource#triggers Resource#triggers}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -125,15 +125,15 @@
     },
 )
 class ResourceConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
@@ -141,15 +141,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param triggers: A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/r/resource#triggers Resource#triggers}
+        :param triggers: A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource#triggers Resource#triggers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dab058c860434703ef191306865b79a888fcda939c0cbf3c2f1f93c22b1be4db)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -184,20 +184,22 @@
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
@@ -239,15 +241,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/null/r/resource#triggers Resource#triggers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/null/3.2.1/docs/resources/resource#triggers Resource#triggers}
         '''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -269,15 +271,15 @@
 
 def _typecheckingstub__bcca22b711b6a266a2fb9e0fd1d2a6b4c7819b841eb701f668ae37626b64c4bf(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
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
@@ -288,15 +290,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__dab058c860434703ef191306865b79a888fcda939c0cbf3c2f1f93c22b1be4db(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     triggers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-null-go`](https://github.com/cdktf/cdktf-provider-null-go) package.
 
 `go get github.com/cdktf/cdktf-provider-null-go/null`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-null).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-null-5.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_null/py.typed
 src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_null.egg-info/requires.txt
 src/cdktf_cdktf_provider_null.egg-info/top_level.txt
 src/cdktf_cdktf_provider_null/_jsii/__init__.py
-src/cdktf_cdktf_provider_null/_jsii/provider-null@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
 src/cdktf_cdktf_provider_null/provider/__init__.py
 src/cdktf_cdktf_provider_null/resource/__init__.py
```

