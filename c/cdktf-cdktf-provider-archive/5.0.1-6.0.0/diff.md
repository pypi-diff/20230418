# Comparing `tmp/cdktf-cdktf-provider-archive-5.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-archive-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-archive-5.0.1.tar", last modified: Thu Jan 19 11:45:32 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-archive-6.0.0.tar", last modified: Tue Apr 18 20:32:43 2023, max compression
```

## Comparing `cdktf-cdktf-provider-archive-5.0.1.tar` & `cdktf-cdktf-provider-archive-6.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.118809 cdktf-cdktf-provider-archive-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.118809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.118809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39953 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/_jsii/provider-archive@5.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    52364 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/file/
--rw-r--r--   0 runner    (1001) docker     (123)    51513 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.122809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 11:45:15.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:45:32.118809 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-19 11:45:31.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-19 11:45:32.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 11:45:31.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-19 11:45:31.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-19 11:45:31.000000 cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107697 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/data_archive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    53743 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    52790 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:32:32.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:43.831107 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-18 20:32:43.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 20:32:43.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:32:43.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:32:43.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 20:32:43.000000 cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/LICENSE` & `cdktf-cdktf-provider-archive-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-archive-5.0.1/PKG-INFO` & `cdktf-cdktf-provider-archive-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-archive
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt archive Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-archive.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-archive.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-archive-go`](https://github.com/cdktf/cdktf-provider-archive-go) package.
 
 `go get github.com/cdktf/cdktf-provider-archive-go/archive`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-archive).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform archive Provider version 1:1. In fact, it always tracks `latest` of `~> 2.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/README.md` & `cdktf-cdktf-provider-archive-6.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-archive-go`](https://github.com/cdktf/cdktf-provider-archive-go) package.
 
 `go get github.com/cdktf/cdktf-provider-archive-go/archive`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-archive).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform archive Provider version 1:1. In fact, it always tracks `latest` of `~> 2.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/setup.py` & `cdktf-cdktf-provider-archive-6.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-archive",
-    "version": "5.0.1",
+    "version": "6.0.0",
     "description": "Prebuilt archive Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-archive.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,37 +25,38 @@
         "cdktf_cdktf_provider_archive._jsii",
         "cdktf_cdktf_provider_archive.data_archive_file",
         "cdktf_cdktf_provider_archive.file",
         "cdktf_cdktf_provider_archive.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_archive._jsii": [
-            "provider-archive@5.0.1.jsii.tgz"
+            "provider-archive@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_archive": [
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

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/__init__.py` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-archive-go`](https://github.com/cdktf/cdktf-provider-archive-go) package.
 
 `go get github.com/cdktf/cdktf-provider-archive-go/archive`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-archive).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform archive Provider version 1:1. In fact, it always tracks `latest` of `~> 2.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_archive_file`
 
-Refer to the Terraform Registory for docs: [`data_archive_file`](https://www.terraform.io/docs/providers/archive/d/file).
+Refer to the Terraform Registory for docs: [`data_archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataArchiveFile(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.dataArchiveFile.DataArchiveFile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/archive/d/file archive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file archive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         output_path: builtins.str,
@@ -39,34 +39,34 @@
         output_file_mode: typing.Optional[builtins.str] = None,
         source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataArchiveFileSource", typing.Dict[builtins.str, typing.Any]]]]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/archive/d/file archive_file} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file archive_file} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_path DataArchiveFile#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#type DataArchiveFile#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#excludes DataArchiveFile#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_file_mode DataArchiveFile#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source DataArchiveFile#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content DataArchiveFile#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content_filename DataArchiveFile#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_dir DataArchiveFile#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_file DataArchiveFile#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -343,15 +343,15 @@
     },
 )
 class DataArchiveFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         output_path: builtins.str,
         type: builtins.str,
@@ -367,23 +367,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_path DataArchiveFile#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#type DataArchiveFile#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#excludes DataArchiveFile#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_file_mode DataArchiveFile#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source DataArchiveFile#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content DataArchiveFile#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content_filename DataArchiveFile#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_dir DataArchiveFile#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_file DataArchiveFile#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__395d6c956a8f6a157e1bf9db0b880a72f8d80755220480442d2acbff968ca74f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -441,20 +441,22 @@
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
@@ -496,101 +498,101 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def output_path(self) -> builtins.str:
         '''The output of the archive file.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_path DataArchiveFile#output_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
         '''
         result = self._values.get("output_path")
         assert result is not None, "Required property 'output_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of archive to generate. NOTE: ``zip`` is supported.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#type DataArchiveFile#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def excludes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Specify files to ignore when reading the ``source_dir``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#excludes DataArchiveFile#excludes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
         '''
         result = self._values.get("excludes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def output_file_mode(self) -> typing.Optional[builtins.str]:
         '''String that specifies the octal file mode for all archived files.
 
         For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#output_file_mode DataArchiveFile#output_file_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
         '''
         result = self._values.get("output_file_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataArchiveFileSource"]]]:
         '''source block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source DataArchiveFile#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
         '''
         result = self._values.get("source")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataArchiveFileSource"]]], result)
 
     @builtins.property
     def source_content(self) -> typing.Optional[builtins.str]:
         '''Add only this content to the archive with ``source_content_filename`` as the filename.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content DataArchiveFile#source_content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
         '''
         result = self._values.get("source_content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_content_filename(self) -> typing.Optional[builtins.str]:
         '''Set this as the filename when using ``source_content``.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_content_filename DataArchiveFile#source_content_filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
         '''
         result = self._values.get("source_content_filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_dir(self) -> typing.Optional[builtins.str]:
         '''Package entire contents of this directory into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_dir DataArchiveFile#source_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
         '''
         result = self._values.get("source_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_file(self) -> typing.Optional[builtins.str]:
         '''Package this file into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#source_file DataArchiveFile#source_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         '''
         result = self._values.get("source_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -607,41 +609,41 @@
     jsii_type="@cdktf/provider-archive.dataArchiveFile.DataArchiveFileSource",
     jsii_struct_bases=[],
     name_mapping={"content": "content", "filename": "filename"},
 )
 class DataArchiveFileSource:
     def __init__(self, *, content: builtins.str, filename: builtins.str) -> None:
         '''
-        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#content DataArchiveFile#content}
-        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#filename DataArchiveFile#filename}
+        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#content DataArchiveFile#content}
+        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#filename DataArchiveFile#filename}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5904c5461679cf6f1f619fb8bf2ab9cf44afa5adb738fa7a85022f5f3df3fa5b)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "content": content,
             "filename": filename,
         }
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Add this content to the archive with ``filename`` as the filename.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#content DataArchiveFile#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#content DataArchiveFile#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Set this as the filename when declaring a ``source``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/d/file#filename DataArchiveFile#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#filename DataArchiveFile#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -843,15 +845,15 @@
     output_file_mode: typing.Optional[builtins.str] = None,
     source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataArchiveFileSource, typing.Dict[builtins.str, typing.Any]]]]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
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
@@ -910,15 +912,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__395d6c956a8f6a157e1bf9db0b880a72f8d80755220480442d2acbff968ca74f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     output_path: builtins.str,
     type: builtins.str,
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/file/__init__.py` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/file/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `archive_file`
 
-Refer to the Terraform Registory for docs: [`archive_file`](https://www.terraform.io/docs/providers/archive/r/file).
+Refer to the Terraform Registory for docs: [`archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class File(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.file.File",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/archive/r/file archive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file archive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         output_path: builtins.str,
@@ -39,34 +39,34 @@
         output_file_mode: typing.Optional[builtins.str] = None,
         source: typing.Optional[typing.Union[typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/archive/r/file archive_file} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file archive_file} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_path File#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#type File#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#excludes File#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_file_mode File#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source File#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content File#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content_filename File#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_dir File#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_file File#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -343,15 +343,15 @@
     },
 )
 class FileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         output_path: builtins.str,
         type: builtins.str,
@@ -367,23 +367,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_path File#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#type File#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#excludes File#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_file_mode File#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source File#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content File#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content_filename File#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_dir File#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_file File#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4cf416deaa089a02b7fc630d948296d45144383aef1cde25d0742ca6c4454dd4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -441,20 +441,22 @@
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
@@ -496,101 +498,101 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def output_path(self) -> builtins.str:
         '''The output of the archive file.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_path File#output_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
         '''
         result = self._values.get("output_path")
         assert result is not None, "Required property 'output_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of archive to generate. NOTE: ``zip`` is supported.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#type File#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def excludes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Specify files to ignore when reading the ``source_dir``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#excludes File#excludes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
         '''
         result = self._values.get("excludes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def output_file_mode(self) -> typing.Optional[builtins.str]:
         '''String that specifies the octal file mode for all archived files.
 
         For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#output_file_mode File#output_file_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
         '''
         result = self._values.get("output_file_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(
         self,
     ) -> typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]]:
         '''source block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source File#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
         '''
         result = self._values.get("source")
         return typing.cast(typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def source_content(self) -> typing.Optional[builtins.str]:
         '''Add only this content to the archive with ``source_content_filename`` as the filename.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content File#source_content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
         '''
         result = self._values.get("source_content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_content_filename(self) -> typing.Optional[builtins.str]:
         '''Set this as the filename when using ``source_content``.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_content_filename File#source_content_filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
         '''
         result = self._values.get("source_content_filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_dir(self) -> typing.Optional[builtins.str]:
         '''Package entire contents of this directory into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_dir File#source_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
         '''
         result = self._values.get("source_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_file(self) -> typing.Optional[builtins.str]:
         '''Package this file into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#source_file File#source_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
         '''
         result = self._values.get("source_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -607,41 +609,41 @@
     jsii_type="@cdktf/provider-archive.file.FileSource",
     jsii_struct_bases=[],
     name_mapping={"content": "content", "filename": "filename"},
 )
 class FileSource:
     def __init__(self, *, content: builtins.str, filename: builtins.str) -> None:
         '''
-        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#content File#content}
-        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#filename File#filename}
+        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#content File#content}
+        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#filename File#filename}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b11194e55a06bbf9bdba900600d77ae8dc999b8147683c454f2452321f3945f3)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "content": content,
             "filename": filename,
         }
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Add this content to the archive with ``filename`` as the filename.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#content File#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#content File#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Set this as the filename when declaring a ``source``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive/r/file#filename File#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#filename File#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -843,15 +845,15 @@
     output_file_mode: typing.Optional[builtins.str] = None,
     source: typing.Optional[typing.Union[typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
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
@@ -910,15 +912,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4cf416deaa089a02b7fc630d948296d45144383aef1cde25d0742ca6c4454dd4(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     output_path: builtins.str,
     type: builtins.str,
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive/provider/__init__.py` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive/provider/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`archive`](https://www.terraform.io/docs/providers/archive).
+Refer to the Terraform Registory for docs: [`archive`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class ArchiveProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.provider.ArchiveProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/archive archive}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs archive}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/archive archive} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs archive} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive#alias ArchiveProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9334d8ee2bfd48a0b6bd3d2efceb54053666d2fefddaec92ffc4d091954d4b64)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = ArchiveProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-archive.provider.ArchiveProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class ArchiveProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive#alias ArchiveProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3c55b33d0d45082b5aaf9d9b53d8c0dbe974d4f669c09696067c98d7276df49b)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/archive#alias ArchiveProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-archive
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt archive Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-archive.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-archive.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-archive-go`](https://github.com/cdktf/cdktf-provider-archive-go) package.
 
 `go get github.com/cdktf/cdktf-provider-archive-go/archive`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-archive).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform archive Provider version 1:1. In fact, it always tracks `latest` of `~> 2.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-archive-5.0.1/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-archive-6.0.0/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_archive/py.typed
 src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_archive.egg-info/requires.txt
 src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
 src/cdktf_cdktf_provider_archive/_jsii/__init__.py
-src/cdktf_cdktf_provider_archive/_jsii/provider-archive@5.0.1.jsii.tgz
+src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
 src/cdktf_cdktf_provider_archive/file/__init__.py
 src/cdktf_cdktf_provider_archive/provider/__init__.py
```

